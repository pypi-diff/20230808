# Comparing `tmp/autosubmit-4.0.84.tar.gz` & `tmp/autosubmit-4.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosubmit-4.0.84.tar", last modified: Fri Jul 21 08:56:31 2023, max compression
+gzip compressed data, was "autosubmit-4.0.85.tar", last modified: Tue Aug  8 08:13:14 2023, max compression
```

## Comparing `autosubmit-4.0.84.tar` & `autosubmit-4.0.85.tar`

### file list

```diff
@@ -1,407 +1,412 @@
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.543668 autosubmit-4.0.84/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.gitlab-ci.yml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      937 2023-07-13 10:54:33.000000 autosubmit-4.0.84/.readthedocs.yaml
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/CHANGELOG
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-07-13 10:54:33.000000 autosubmit-4.0.84/CONTRIBUTING.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.84/LICENSE
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.84/MANIFEST.in
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-21 08:56:31.539668 autosubmit-4.0.84/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-07-13 10:54:33.000000 autosubmit-4.0.84/README.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-07-13 10:54:33.000000 autosubmit-4.0.84/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-07-21 08:56:14.000000 autosubmit-4.0.84/VERSION
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   324689 2023-07-20 14:05:47.000000 autosubmit-4.0.84/autosubmit/autosubmit.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/database/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/database/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/database/data/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/database/data/autosubmit.sql
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/database/db_structure.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/experiment/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/experiment/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/experiment/experiment_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/experiment/statistics.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/git/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/git/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/git/autosubmit_git.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit/helpers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/autosubmit/helpers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/autosubmit_helper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/data_transfer.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3304 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/parameters.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/helpers/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/data_classes/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/data_classes/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/data_classes/experiment_run.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/data_classes/job_data.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/database_managers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/database_managers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/database_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/database_models.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/experiment_history_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/database_managers/experiment_status_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/experiment_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/experiment_status.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/internal_logging.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/platform_monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/pending.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_utils.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor_item.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/history/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/job/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/job/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    99727 2023-07-20 07:01:43.000000 autosubmit-4.0.84/autosubmit/job/job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10907 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20136 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_dict.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   127858 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_list_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_package_persistence.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62148 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/job/job_packager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38254 2023-07-21 08:35:09.000000 autosubmit-4.0.84/autosubmit/job/job_packages.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/job/job_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/monitor/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/monitor/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10182 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/monitor/diagram.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    26910 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/monitor/monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/monitor/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.507669 autosubmit-4.0.84/autosubmit/notifications/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/notifications/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/notifications/mail_notifier.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/notifications/notifier.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/ecplatform.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/headers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/headers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ec_cca_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ec_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/local_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/lsf_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs10_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs11_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pbs12_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/pjm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/ps_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/sge_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8083 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/headers/slurm_header.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/locplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/lsfplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53819 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/paramiko_submitter.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/pbsplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/pjmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    27527 2023-07-20 06:53:28.000000 autosubmit-4.0.84/autosubmit/platforms/platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/psplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/sgeplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32072 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/slurmplatform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/platforms/submitter.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/platforms/wrappers/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38702 2023-07-21 08:11:30.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_builder.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9418 2023-07-21 08:13:50.000000 autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_factory.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/autosubmit/statistics/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.84/autosubmit/statistics/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/jobs_stat.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-06-28 10:21:26.000000 autosubmit-4.0.84/autosubmit/statistics/stats_summary.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-07-13 10:54:33.000000 autosubmit-4.0.84/autosubmit/statistics/utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.503669 autosubmit-4.0.84/autosubmit.egg-info/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3347 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/PKG-INFO
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13041 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/SOURCES.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/dependency_links.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      427 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/requires.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-07-21 08:56:31.000000 autosubmit-4.0.84/autosubmit.egg-info/top_level.txt
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/bin/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-07-13 10:54:33.000000 autosubmit-4.0.84/bin/autosubmit
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.511669 autosubmit-4.0.84/docs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/Makefile
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.84/docs/autosubmit.pdf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/experiment/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.515669 autosubmit-4.0.84/docs/source/agui/experiment/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/experiment/fig/fig_experiment.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/experiment/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig1_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig2_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig3_gui.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig4_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig5_gui.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_ev_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_tree_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/fig/fig_tree_2.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/graph/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/graph/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_3.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_4.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/graph/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/log/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/log/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/log/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/performance/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.519669 autosubmit-4.0.84/docs/source/agui/performance/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/performance/fig/fig_performance_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/performance/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/statistics/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/statistics/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_1.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/statistics/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/tree/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/agui/tree/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/agui/tree/fig/fig_tree_2.jpg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/agui/tree/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10217 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/conf.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/devguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/devguide/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2145 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/installation/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/installation/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.523669 autosubmit-4.0.84/docs/source/introduction/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig2.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/introduction/fig3.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/introduction/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/moduledoc/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/autosubmit.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/moduledoc/config.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/database.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/git.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/job.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/monitor.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/moduledoc/platforms.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/qstartguide/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/qstartguide/dummy.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/qstartguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/troubleshooting/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/changelog.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22857 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/error-codes.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/troubleshooting/fig/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/monarch-da.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_0.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_1.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/troubleshooting/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.527669 autosubmit-4.0.84/docs/source/unused_figs/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/group_chunk.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/horizontal-vertical.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper_expression.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/unused_figs/wrapper_hybrid.png
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/configure/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/configure/develop_a_project.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20564 2023-07-20 07:01:43.000000 autosubmit-4.0.84/docs/source/userguide/configure/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/create/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/create/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/manage/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/manage/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/run/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    16002 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/run/index.rst
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/wrappers/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/dasim.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/horizontal_remote.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/multiple_wrappers.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/rerun.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-horizontal.png
--rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-06-28 10:21:26.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-mixed.png
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-07-13 10:54:33.000000 autosubmit-4.0.84/docs/source/userguide/wrappers/index.rst
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      702 2023-07-13 10:54:33.000000 autosubmit-4.0.84/environment.yml
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/log/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.84/log/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-07-13 10:54:33.000000 autosubmit-4.0.84/log/fd_show.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-07-13 10:54:33.000000 autosubmit-4.0.84/log/log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      464 2023-07-20 07:01:43.000000 autosubmit-4.0.84/requeriments.txt
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-07-21 08:56:31.543668 autosubmit-4.0.84/setup.cfg
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3061 2023-07-13 10:54:33.000000 autosubmit-4.0.84/setup.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/test/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.531669 autosubmit-4.0.84/test/integration/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/integration/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/integration/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/integration/test_job.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/.gitignore
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/README
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/__init__.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/db/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/db/.gitignore
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/default_conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/default_conf/platforms.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/local_asparser_test.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.535668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.499669 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/src/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.84/test/regression/tests.conf
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/regression/tests_commands.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_runner.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/regression/tests_utils.py
-drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-07-21 08:56:31.539668 autosubmit-4.0.84/test/unit/
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/README_PIP.md
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.84/test/unit/__init__.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_basic_config.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_catlog.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.84/test/unit/test_chunk_date_lib.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_database_managers.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_db_manager.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9696 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_dependencies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_dic_jobs.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8327 2023-07-20 07:01:43.000000 autosubmit-4.0.84/test/unit/test_expid.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_history.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14748 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_job.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_common.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_graph.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_grouping.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12769 2023-07-20 06:53:28.000000 autosubmit-4.0.84/test/unit/test_job_list.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8531 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_job_package.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_log.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3846 2023-07-21 08:33:26.000000 autosubmit-4.0.84/test/unit/test_machinefiles_wrapper.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_paramiko_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5244 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_pjm.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_platform_monitor.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_setup.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2887 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_slurm_platform.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_statistics.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_strategies.py
--rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-07-13 10:54:33.000000 autosubmit-4.0.84/test/unit/test_wrappers.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.492303 autosubmit-4.0.85/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      226 2023-08-03 09:29:59.000000 autosubmit-4.0.85/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1361 2023-08-03 09:29:59.000000 autosubmit-4.0.85/.gitlab-ci.yml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      968 2023-08-08 07:34:49.000000 autosubmit-4.0.85/.readthedocs.yaml
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.85/CHANGELOG
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      722 2023-08-03 09:29:59.000000 autosubmit-4.0.85/CONTRIBUTING.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    35147 2021-10-05 14:18:20.000000 autosubmit-4.0.85/LICENSE
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      119 2021-10-05 14:18:20.000000 autosubmit-4.0.85/MANIFEST.in
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3348 2023-08-08 08:13:14.492303 autosubmit-4.0.85/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5651 2023-08-03 09:29:59.000000 autosubmit-4.0.85/README.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2287 2023-08-03 09:29:59.000000 autosubmit-4.0.85/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        7 2023-08-07 13:47:50.000000 autosubmit-4.0.85/VERSION
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   325314 2023-08-08 07:34:49.000000 autosubmit-4.0.85/autosubmit/autosubmit.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/database/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/database/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/database/data/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      258 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/database/data/autosubmit.sql
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19910 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/database/db_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7593 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/database/db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6065 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/database/db_structure.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/experiment/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/experiment/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5280 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/experiment/experiment_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8450 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/experiment/statistics.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/git/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/git/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13703 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/git/autosubmit_git.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/helpers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.85/autosubmit/helpers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5776 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/helpers/autosubmit_helper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      194 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/helpers/data_transfer.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3304 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/helpers/parameters.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1428 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/helpers/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/history/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/history/data_classes/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/data_classes/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2432 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/data_classes/experiment_run.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10305 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/data_classes/job_data.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/history/database_managers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/database_managers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5688 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/database_managers/database_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2409 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/database_managers/database_models.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19251 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/database_managers/experiment_history_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6456 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/database_managers/experiment_status_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18844 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/experiment_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2382 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/experiment_status.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1952 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/internal_logging.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit/history/platform_monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/pending.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      554 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper1.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      549 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper2.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6105 2022-11-21 08:34:36.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1025 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2298 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/platform_utils.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2475 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/slurm_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3454 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/platform_monitor/slurm_monitor_item.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10951 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/history/strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2784 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/history/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/job/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/job/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   100842 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/job/job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12553 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/job/job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20136 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/job/job_dict.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13797 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/job/job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   143199 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/job/job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4609 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/job/job_list_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3565 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/job/job_package_persistence.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    62148 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/job/job_packager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    40075 2023-08-07 13:03:22.000000 autosubmit-4.0.85/autosubmit/job/job_packages.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11580 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/job/job_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/monitor/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/monitor/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10806 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/monitor/diagram.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    29398 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/monitor/monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1414 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/monitor/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/notifications/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/notifications/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4049 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/notifications/mail_notifier.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1196 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/notifications/notifier.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/platforms/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/platforms/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13279 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/ecplatform.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/platforms/headers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/platforms/headers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5514 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/ec_cca_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4100 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/ec_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1826 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/local_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7391 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/lsf_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2972 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/pbs10_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3497 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/pbs11_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2963 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/pbs12_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5750 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/pjm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2214 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/ps_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/sge_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8083 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/headers/slurm_header.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10469 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/locplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5557 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/lsfplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53819 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11370 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/paramiko_submitter.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5224 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/pbsplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20846 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/pjmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    28797 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/platforms/platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4184 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/psplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4617 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/platforms/sgeplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32055 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/platforms/slurmplatform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1316 2023-08-03 09:29:59.000000 autosubmit-4.0.85/autosubmit/platforms/submitter.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/platforms/wrappers/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/autosubmit/platforms/wrappers/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    38702 2023-08-07 11:49:14.000000 autosubmit-4.0.85/autosubmit/platforms/wrappers/wrapper_builder.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9418 2023-08-07 11:49:14.000000 autosubmit-4.0.85/autosubmit/platforms/wrappers/wrapper_factory.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/profiler/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 07:34:49.000000 autosubmit-4.0.85/autosubmit/profiler/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4646 2023-08-08 07:34:49.000000 autosubmit-4.0.85/autosubmit/profiler/profiler.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/autosubmit/statistics/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2023-02-02 09:02:16.000000 autosubmit-4.0.85/autosubmit/statistics/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2869 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/statistics/jobs_stat.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7520 2023-08-07 13:30:59.000000 autosubmit-4.0.85/autosubmit/statistics/statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1818 2023-06-28 10:21:26.000000 autosubmit-4.0.85/autosubmit/statistics/stats_summary.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1830 2023-08-07 06:23:10.000000 autosubmit-4.0.85/autosubmit/statistics/utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/autosubmit.egg-info/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3348 2023-08-08 08:13:13.000000 autosubmit-4.0.85/autosubmit.egg-info/PKG-INFO
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13162 2023-08-08 08:13:14.000000 autosubmit-4.0.85/autosubmit.egg-info/SOURCES.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        1 2023-08-08 08:13:13.000000 autosubmit-4.0.85/autosubmit.egg-info/dependency_links.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      434 2023-08-08 08:13:13.000000 autosubmit-4.0.85/autosubmit.egg-info/requires.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       20 2023-08-08 08:13:14.000000 autosubmit-4.0.85/autosubmit.egg-info/top_level.txt
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/bin/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)     3086 2023-08-03 09:29:59.000000 autosubmit-4.0.85/bin/autosubmit
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.460304 autosubmit-4.0.85/docs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     7869 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/Makefile
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)  1513786 2021-10-05 14:18:20.000000 autosubmit-4.0.85/docs/autosubmit.pdf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.464304 autosubmit-4.0.85/docs/source/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.464304 autosubmit-4.0.85/docs/source/agui/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.464304 autosubmit-4.0.85/docs/source/agui/experiment/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.464304 autosubmit-4.0.85/docs/source/agui/experiment/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   112356 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/experiment/fig/fig_experiment.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1430 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/agui/experiment/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.464304 autosubmit-4.0.85/docs/source/agui/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25707 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig1_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   140255 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig2_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   184237 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig3_gui.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114416 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig4_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    44047 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig5_gui.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248267 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig_ev_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   248251 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig_tree_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   241752 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/fig/fig_tree_2.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/graph/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/graph/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   122929 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   123449 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   213843 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_3.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    57438 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_4.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6535 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/agui/graph/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4263 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/agui/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/log/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/log/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    25433 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/log/fig/fig_log_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   117240 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/log/fig/fig_log_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1125 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/log/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/performance/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/performance/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   174233 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/performance/fig/fig_performance_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      910 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/performance/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/statistics/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/statistics/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    56486 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/statistics/fig/fig_stat_1.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   101911 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/statistics/fig/fig_stat_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      988 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/statistics/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/tree/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/agui/tree/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   114354 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/agui/tree/fig/fig_tree_2.jpg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5756 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/agui/tree/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    10329 2023-08-08 07:34:49.000000 autosubmit-4.0.85/docs/source/conf.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.468304 autosubmit-4.0.85/docs/source/devguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2109 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/devguide/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2145 2023-08-07 11:49:14.000000 autosubmit-4.0.85/docs/source/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.472304 autosubmit-4.0.85/docs/source/installation/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12768 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/installation/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.472304 autosubmit-4.0.85/docs/source/introduction/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   769052 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/introduction/fig1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    93570 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/introduction/fig2.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    53843 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/introduction/fig3.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6099 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/introduction/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.472304 autosubmit-4.0.85/docs/source/moduledoc/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      130 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/autosubmit.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      445 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/moduledoc/config.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       99 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/database.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       89 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/git.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      128 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      185 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/job.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       94 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/monitor.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      547 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/moduledoc/platforms.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.472304 autosubmit-4.0.85/docs/source/qstartguide/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    50473 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/qstartguide/dummy.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     9400 2023-08-07 11:49:14.000000 autosubmit-4.0.85/docs/source/qstartguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/troubleshooting/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    18379 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/troubleshooting/changelog.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23329 2023-08-08 07:34:49.000000 autosubmit-4.0.85/docs/source/troubleshooting/error-codes.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/troubleshooting/fig/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    83094 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/troubleshooting/fig/monarch-da.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/troubleshooting/fig/new_dependencies_0.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    68077 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/troubleshooting/fig/new_dependencies_1.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2770 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/troubleshooting/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/unused_figs/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    49607 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/unused_figs/group_chunk.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    32622 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/unused_figs/horizontal-vertical.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   106298 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/unused_figs/wrapper.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   251472 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/unused_figs/wrapper_expression.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19009 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/unused_figs/wrapper_hybrid.png
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/configure/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    30910 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/userguide/configure/develop_a_project.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    20564 2023-08-07 11:49:14.000000 autosubmit-4.0.85/docs/source/userguide/configure/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/create/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6907 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/userguide/create/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1877 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/userguide/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/manage/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14283 2023-08-03 09:29:59.000000 autosubmit-4.0.85/docs/source/userguide/manage/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/run/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17471 2023-08-08 07:34:49.000000 autosubmit-4.0.85/docs/source/userguide/run/index.rst
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.476304 autosubmit-4.0.85/docs/source/userguide/wrappers/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)   198622 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/dasim.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    23826 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/horizontal_remote.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)   308786 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/multiple_wrappers.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    17531 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/rerun.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    33805 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/vertical-horizontal.png
+-rwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)    33140 2023-06-28 10:21:26.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/fig/vertical-mixed.png
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    11646 2023-08-03 10:23:37.000000 autosubmit-4.0.85/docs/source/userguide/wrappers/index.rst
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      713 2023-08-08 07:34:49.000000 autosubmit-4.0.85/environment.yml
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/log/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-11-21 08:34:36.000000 autosubmit-4.0.85/log/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      871 2023-08-03 09:29:59.000000 autosubmit-4.0.85/log/fd_show.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13696 2023-08-03 09:29:59.000000 autosubmit-4.0.85/log/log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      471 2023-08-08 07:34:49.000000 autosubmit-4.0.85/requeriments.txt
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       38 2023-08-08 08:13:14.492303 autosubmit-4.0.85/setup.cfg
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3070 2023-08-08 07:34:49.000000 autosubmit-4.0.85/setup.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/integration/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/integration/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1315 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/integration/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2874 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/integration/test_job.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       33 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/.gitignore
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2429 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/README
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/__init__.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/db/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       90 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/db/.gitignore
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/default_conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1368 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/default_conf/platforms.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2946 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/local_asparser_test.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.452304 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2459 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      577 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       97 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.452304 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.452304 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.480304 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      647 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      656 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      207 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      640 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      208 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.484304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      586 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2462 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      538 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2464 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      229 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2455 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      352 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2457 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/src/TEST_NOLEAP.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2456 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      353 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       88 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/src/TEST_NOLEAP.sh
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.456304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      587 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2458 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      218 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)       27 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/proj.conf
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.488304 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/src/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      104 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2775 2022-11-21 08:34:36.000000 autosubmit-4.0.85/test/regression/tests.conf
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1135 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/regression/tests_commands.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5968 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/tests_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5504 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/tests_runner.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3603 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/regression/tests_utils.py
+drwxrwxr-x   0 dbeltran  (1001) dbeltran  (1001)        0 2023-08-08 08:13:14.492303 autosubmit-4.0.85/test/unit/
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2039 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/README_PIP.md
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)        0 2022-12-20 13:25:07.000000 autosubmit-4.0.85/test/unit/__init__.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1104 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_basic_config.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4581 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_catlog.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8359 2023-08-07 13:30:59.000000 autosubmit-4.0.85/test/unit/test_checkpoints.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13253 2021-10-05 14:18:20.000000 autosubmit-4.0.85/test/unit/test_chunk_date_lib.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    13319 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_database_managers.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2490 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_db_manager.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    24110 2023-08-07 13:30:59.000000 autosubmit-4.0.85/test/unit/test_dependencies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    22969 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_dic_jobs.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8327 2023-08-07 11:49:14.000000 autosubmit-4.0.85/test/unit/test_expid.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    19073 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_history.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    14749 2023-08-07 13:30:59.000000 autosubmit-4.0.85/test/unit/test_job.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1015 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_job_common.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    47843 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_job_graph.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    59633 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_job_grouping.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    12754 2023-08-07 13:30:59.000000 autosubmit-4.0.85/test/unit/test_job_list.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     8424 2023-08-07 13:03:22.000000 autosubmit-4.0.85/test/unit/test_job_package.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      815 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_log.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3846 2023-08-07 11:49:14.000000 autosubmit-4.0.85/test/unit/test_machinefiles_wrapper.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4878 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_paramiko_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     5350 2023-08-07 11:49:14.000000 autosubmit-4.0.85/test/unit/test_pjm.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     4528 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_platform_monitor.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     1407 2023-08-08 07:34:49.000000 autosubmit-4.0.85/test/unit/test_profiler.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)      393 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_setup.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     2887 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_slurm_platform.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     3130 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_statistics.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)     6724 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_strategies.py
+-rw-rw-r--   0 dbeltran  (1001) dbeltran  (1001)    81739 2023-08-03 09:29:59.000000 autosubmit-4.0.85/test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.84/.gitlab-ci.yml` & `autosubmit-4.0.85/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/.readthedocs.yaml` & `autosubmit-4.0.85/.readthedocs.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 version: 2
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
     python: "3.9"
+  apt_packages:
+    - graphviz
   jobs:
     post_install:
       # ruamel.yaml.clib appears to cause the build to fail when
       # using new API in ruamel.yaml
       # refs:
       # - https://earth.bsc.es/gitlab/es/autosubmit/-/merge_requests/340/
       # - https://yaml.readthedocs.io/en/latest/api.html
```

### Comparing `autosubmit-4.0.84/CONTRIBUTING.md` & `autosubmit-4.0.85/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/LICENSE` & `autosubmit-4.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/PKG-INFO` & `autosubmit-4.0.85/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.84
+Version: 4.0.85
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
@@ -24,7 +24,8 @@
 These multi-scale workflows can contain from a few steps to thousands of steps, and from a single platform to multiple platforms. Platform is a concept in Autosubmit to abstract servers. A workflow configuration can include one or multiple platforms, allowing the workflow to run on any number of servers via password-less SSH without any external deployment.
 
 Due to its robustness it can handle different eventualities such as networking connectivity issues or I/O errors. The monitoring capabilities extend beyond the command-line application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI.
 
 It has contributed to various European research projects and runs different operational systems. It will support the Earth Digital Twins as the Digital Twin Ocean over the next years.
 
 It is currently used at the Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES, and others), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and for many other use cases. Autosubmit has been used to run workflows in different supercomputers at BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+
```

### Comparing `autosubmit-4.0.84/README.md` & `autosubmit-4.0.85/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/README_PIP.md` & `autosubmit-4.0.85/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/autosubmit.py` & `autosubmit-4.0.85/autosubmit/autosubmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from .job.job_grouping import JobGrouping
 from .job.job_list import JobList
 from .job.job_list_persistence import JobListPersistenceDb
 from .job.job_list_persistence import JobListPersistencePkl
 from .job.job_package_persistence import JobPackagePersistence
 from .job.job_packager import JobPackager
 from .job.job_utils import SubJob, SubJobManager
+from .profiler.profiler import Profiler
 from .monitor.monitor import Monitor
 from .notifications.mail_notifier import MailNotifier
 from .notifications.notifier import Notifier
 from .platforms.paramiko_submitter import ParamikoSubmitter
 from .platforms.platform import Platform
 
 dialog = None
@@ -186,14 +187,16 @@
                                    default=False, help='Update experiment version')
             subparser.add_argument('-st', '--start_time', required=False,
                                    help='Sets the starting time for this experiment')
             subparser.add_argument('-sa', '--start_after', required=False,
                                    help='Sets a experiment expid which completion will trigger the start of this experiment.')
             subparser.add_argument('-rom', '--run_only_members', required=False,
                                    help='Sets members allowed on this run.')
+            subparser.add_argument('-p', '--profile', action='store_true', default=False, required=False,
+                                   help='Prints performance parameters of the execution of this experiment.')
 
 
             # Expid
             subparser = subparsers.add_parser(
                 'expid', description="Creates a new experiment")
             group = subparser.add_mutually_exclusive_group()
             group.add_argument(
@@ -643,15 +646,15 @@
         expid = "None"
         if hasattr(args, 'expid'):
             expid = args.expid
         if args.command != "configure" and args.command != "install":
             Autosubmit._init_logs(args, args.logconsole, args.logfile, expid)
 
         if args.command == 'run':
-            return Autosubmit.run_experiment(args.expid, args.notransitive,args.start_time,args.start_after, args.run_only_members)
+            return Autosubmit.run_experiment(args.expid, args.notransitive,args.start_time,args.start_after, args.run_only_members, args.profile)
         elif args.command == 'expid':
             return Autosubmit.expid(args.description,args.HPC,args.copy, args.dummy,args.minimal_configuration,args.git_repo,args.git_branch,args.git_as_conf,args.operational,args.testcase,args.use_local_minimal) != ''
         elif args.command == 'delete':
             return Autosubmit.delete(args.expid, args.force)
         elif args.command == 'monitor':
             return Autosubmit.monitor(args.expid, args.output, args.list, args.filter_chunks, args.filter_status,
                                       args.filter_type, args.hide, args.text, args.group_by, args.expand,
@@ -1995,33 +1998,40 @@
                 len(job_list.get_failed()), time.strftime("%H:%M")))
         safetysleeptime = as_conf.get_safetysleeptime()
         default_retrials = as_conf.get_retrials()
         check_wrapper_jobs_sleeptime = as_conf.get_wrapper_check_time()
         Log.debug("Sleep: {0}", safetysleeptime)
         Log.debug("Number of retrials: {0}", default_retrials)
         return total_jobs, safetysleeptime, default_retrials, check_wrapper_jobs_sleeptime
+    
     @staticmethod
-    def run_experiment(expid, notransitive=False, start_time=None, start_after=None,run_only_members=None):
+    def run_experiment(expid, notransitive=False, start_time=None, start_after=None, run_only_members=None, profile=False):
         """
         Runs and experiment (submitting all the jobs properly and repeating its execution in case of failure).
         :param expid: the experiment id
         :param notransitive: if True, the transitive closure of the graph is not computed
         :param start_time: the time at which the experiment should start
         :param start_after: the expid after which the experiment should start
         :param run_only_members: the members to run
+        :param profile: if True, the whole experiment will be profiled
         :return: None
 
         """
         # Initialize common folders
         try:
             exp_path = os.path.join(BasicConfig.LOCAL_ROOT_DIR, expid)
             tmp_path = os.path.join(exp_path, BasicConfig.LOCAL_TMP_DIR)
         except BaseException as e:
             raise AutosubmitCritical("Failure during the loading of the experiment configuration, check file paths",
                                      7014, str(e))
+        
+        # If the profile flag has been used, activate the profiler and start taking measures
+        if profile:
+            profiler = Profiler(expid)
+            profiler.start()
 
         # checking if there is a lock file to avoid multiple running on the same expid
         try:
             # Portalocker is used to avoid multiple autosubmit running on the same experiment, we have to change this system in #806
             with portalocker.Lock(os.path.join(tmp_path, 'autosubmit.lock'), timeout=1):
                 try:
                     Log.debug("Preparing run")
@@ -2246,14 +2256,17 @@
         except (portalocker.AlreadyLocked, portalocker.LockException) as e:
             message = "We have detected that there is another Autosubmit instance using the experiment\n. Stop other Autosubmit instances that are using the experiment or delete autosubmit.lock file located on tmp folder"
             raise AutosubmitCritical(message, 7000)
         except AutosubmitCritical as e:
             raise
         except BaseException as e:
             raise AutosubmitCritical("This seems like a bug in the code, please contact AS developers", 7070, str(e))
+        finally:
+            if profile:
+                profiler.stop()
 
     @staticmethod
     def restore_platforms(platform_to_test, mail_notify=False, as_conf=None, expid=None):
         Log.info("Checking the connection to all platforms in use")
         issues = ""
         platform_issues = ""
         ssh_config_issues = ""
```

### Comparing `autosubmit-4.0.84/autosubmit/database/db_common.py` & `autosubmit-4.0.85/autosubmit/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/database/db_manager.py` & `autosubmit-4.0.85/autosubmit/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/database/db_structure.py` & `autosubmit-4.0.85/autosubmit/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/experiment/experiment_common.py` & `autosubmit-4.0.85/autosubmit/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/experiment/statistics.py` & `autosubmit-4.0.85/autosubmit/experiment/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/git/autosubmit_git.py` & `autosubmit-4.0.85/autosubmit/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/helpers/autosubmit_helper.py` & `autosubmit-4.0.85/autosubmit/helpers/autosubmit_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/helpers/parameters.py` & `autosubmit-4.0.85/autosubmit/helpers/parameters.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/helpers/utils.py` & `autosubmit-4.0.85/autosubmit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/data_classes/experiment_run.py` & `autosubmit-4.0.85/autosubmit/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/data_classes/job_data.py` & `autosubmit-4.0.85/autosubmit/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/database_managers/database_manager.py` & `autosubmit-4.0.85/autosubmit/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/database_managers/database_models.py` & `autosubmit-4.0.85/autosubmit/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/database_managers/experiment_history_db_manager.py` & `autosubmit-4.0.85/autosubmit/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/database_managers/experiment_status_db_manager.py` & `autosubmit-4.0.85/autosubmit/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/experiment_history.py` & `autosubmit-4.0.85/autosubmit/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/experiment_status.py` & `autosubmit-4.0.85/autosubmit/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/internal_logging.py` & `autosubmit-4.0.85/autosubmit/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper1.txt` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper1.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper2.txt` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper2.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/output_examples/wrapper_big.txt`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_monitor.py` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/platform_utils.py` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor.py` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/platform_monitor/slurm_monitor_item.py` & `autosubmit-4.0.85/autosubmit/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/strategies.py` & `autosubmit-4.0.85/autosubmit/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/history/utils.py` & `autosubmit-4.0.85/autosubmit/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job.py` & `autosubmit-4.0.85/autosubmit/job/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,41 +17,41 @@
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 Main module for Autosubmit. Only contains an interface class to all functionality implemented on Autosubmit
 """
 
-import os
-import re
-import time
-import json
-import datetime
-import textwrap
 from collections import OrderedDict
-import copy
 
+import copy
+import datetime
+import json
 import locale
+import os
+import re
+import textwrap
+import time
+from bscearth.utils.date import date2str, parse_date, previous_day, chunk_end_date, chunk_start_date, Log, subs_dates
+from functools import reduce
+from threading import Thread
+from time import sleep
+from typing import List, Union
 
-from autosubmitconfigparser.config.configcommon import AutosubmitConfig
-from autosubmit.job.job_common import Status, Type, increase_wallclock_by_chunk
+from autosubmit.helpers.parameters import autosubmit_parameter, autosubmit_parameters
+from autosubmit.history.experiment_history import ExperimentHistory
 from autosubmit.job.job_common import StatisticsSnippetBash, StatisticsSnippetPython
 from autosubmit.job.job_common import StatisticsSnippetR, StatisticsSnippetEmpty
+from autosubmit.job.job_common import Status, Type, increase_wallclock_by_chunk
 from autosubmit.job.job_utils import get_job_package_code
-from autosubmitconfigparser.config.basicconfig import BasicConfig
-from autosubmit.history.experiment_history import ExperimentHistory
-from bscearth.utils.date import date2str, parse_date, previous_day, chunk_end_date, chunk_start_date, Log, subs_dates
-from time import sleep
-from threading import Thread
 from autosubmit.platforms.paramiko_submitter import ParamikoSubmitter
-from log.log import Log, AutosubmitCritical, AutosubmitError
-from typing import List, Union
-from functools import reduce
+from autosubmitconfigparser.config.basicconfig import BasicConfig
+from autosubmitconfigparser.config.configcommon import AutosubmitConfig
 from autosubmitconfigparser.config.yamlparser import YAMLParserFactory
-from autosubmit.helpers.parameters import autosubmit_parameter, autosubmit_parameters
+from log.log import Log, AutosubmitCritical, AutosubmitError
 
 Log.get_logger("Autosubmit")
 
 # A wrapper for encapsulate threads , TODO: Python 3+ to be replaced by the < from concurrent.futures >
 
 
 def threaded(fn):
@@ -217,14 +217,17 @@
         self._dependencies = []
         self.running = "once"
         self.start_time = None
         self.edge_info = dict()
         self.total_jobs = None
         self.max_waiting_jobs = None
         self.exclusive = ""
+        # internal
+        self.current_checkpoint_step = 0
+        self.max_checkpoint_step = 0
 
     @property
     @autosubmit_parameter(name='tasktype')
     def section(self):
         """Type of the job, as given on job configuration file."""
         return self._section
 
@@ -249,14 +252,31 @@
         return self._fail_count
 
     @fail_count.setter
     def fail_count(self, value):
         self._fail_count = value
 
     @property
+    @autosubmit_parameter(name='checkpoint')
+    def checkpoint(self):
+        '''Generates a checkpoint step for this job based on job.type.'''
+        if self.type == Type.PYTHON:
+            return "checkpoint()"
+        elif self.type == Type.R:
+            return "checkpoint()"
+        else:  # bash
+            return "as_checkpoint"
+
+    def get_checkpoint_files(self):
+        """
+        Check if there is a file on the remote host that contains the checkpoint
+        """
+        return self.platform.get_checkpoint_files(self)
+
+    @property
     @autosubmit_parameter(name='sdate')
     def sdate(self):
         """Current start date."""
         return date2str(self.date, self.date_format)
 
     @property
     @autosubmit_parameter(name='member')
@@ -566,14 +586,15 @@
         """
         Sets the partion to be used by the job.
 
         :param value: partion to set
         :type value: HPCPlatform
         """
         self._partition = value
+
     @property
     def children(self):
         """
         Returns a list containing all children of the job
 
         :return: child jobs
         :rtype: set
@@ -686,28 +707,28 @@
         Adds a new child to the job
 
         :param new_child: new child to add
         :type new_child: Job
         """
         self.children.add(new_child)
 
-    def add_edge_info(self,parent_name, special_variables):
+    def add_edge_info(self, parent, special_variables):
         """
         Adds edge information to the job
 
-        :param parent_name: parent name
-        :type parent_name: str
+        :param parent: parent job
+        :type parent: Job
         :param special_variables: special variables
         :type special_variables: dict
         """
-        if parent_name not in self.edge_info:
-            self.edge_info[parent_name] = special_variables
-        else:
-            self.edge_info[parent_name].update(special_variables)
-        pass
+        if special_variables["STATUS"] not in self.edge_info:
+            self.edge_info[special_variables["STATUS"]] = {}
+
+        self.edge_info[special_variables["STATUS"]][parent.name] = (parent,special_variables.get("FROM_STEP", 0))
+
     def delete_parent(self, parent):
         """
         Remove a parent from the job
 
         :param parent: parent to remove
         :type parent: Job
         """
@@ -1342,14 +1363,16 @@
             parameters[wrapper_section + "_JOBS"] = as_conf.get_wrapper_jobs(
                 as_conf.experiment_data["WRAPPERS"].get(wrapper_section))
             parameters[wrapper_section + "_EXTENSIBLE"] = int(
                 as_conf.get_extensible_wallclock(as_conf.experiment_data["WRAPPERS"].get(wrapper_section)))
         return parameters
 
     def update_job_parameters(self,as_conf, parameters):
+        if self.checkpoint: # To activate placeholder sustitution per <empty> in the template
+            parameters["AS_CHECKPOINT"] = self.checkpoint
         parameters['JOBNAME'] = self.name
         parameters['FAIL_COUNT'] = str(self.fail_count)
         parameters['SDATE'] = self.sdate
         parameters['MEMBER'] = self.member
         parameters['SPLIT'] = self.split
         parameters['SPLITS'] = self.splits
         parameters['DELAY'] = self.delay
@@ -1423,14 +1446,16 @@
                 parameters['CHUNK_LAST'] = 'FALSE'
         parameters['NUMMEMBERS'] = len(as_conf.get_member_list())
         parameters['DEPENDENCIES'] = str(as_conf.jobs_data[self.section].get("DEPENDENCIES",""))
         self.dependencies = parameters['DEPENDENCIES']
         parameters['EXPORT'] = self.export
         parameters['PROJECT_TYPE'] = as_conf.get_project_type()
         self.wchunkinc = as_conf.get_wchunkinc(self.section)
+        for key,value in as_conf.jobs_data[self.section].items():
+            parameters["CURRENT_"+key.upper()] = value
         return parameters
 
     def update_parameters(self, as_conf, parameters,
                           default_parameters={'d': '%d%', 'd_': '%d_%', 'Y': '%Y%', 'Y_': '%Y_%',
                                               'M': '%M%', 'M_': '%M_%', 'm': '%m%', 'm_': '%m_%'}):
         """
         Refresh parameters value
@@ -1609,16 +1634,18 @@
 
                 filename = os.path.basename(os.path.splitext(additional_file)[0])
                 full_path = os.path.join(self._tmp_path,filename ) + "_" + self.name[5:]
                 open(full_path, 'wb').write(additional_template_content.encode(lang))
             except:
                 pass
         for key, value in parameters.items():
+            # parameters[key] can have '\\' characters that are interpreted as escape characters
+            # by re.sub. To avoid this, we use re.escape
             template_content = re.sub(
-                '%(?<!%%)' + key + '%(?!%%)', str(parameters[key]), template_content,flags=re.I)
+                '%(?<!%%)' + key + '%(?!%%)', re.escape(str(parameters[key])), template_content,flags=re.I)
         for variable in self.undefined_variables:
             template_content = re.sub(
                 '%(?<!%%)' + variable + '%(?!%%)', '', template_content,flags=re.I)
         template_content = template_content.replace("%%", "%")
         script_name = '{0}.cmd'.format(self.name)
         self.script_name = '{0}.cmd'.format(self.name)
```

### Comparing `autosubmit-4.0.84/autosubmit/job/job_common.py` & `autosubmit-4.0.85/autosubmit/job/job_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # Autosubmit is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
-import textwrap
 import datetime
+import textwrap
 
 
 class Status:
     """
     Class to handle the status of a job
     """
     WAITING = 0
@@ -37,14 +36,15 @@
     DELAYED = 9
     UNKNOWN = -2
     SUSPENDED = -3
     #######
     # Note: any change on constants must be applied on the dict below!!!
     VALUE_TO_KEY = {-3: 'SUSPENDED', -2: 'UNKNOWN', -1: 'FAILED', 0: 'WAITING', 1: 'READY',
                     2: 'SUBMITTED', 3: 'QUEUING', 4: 'RUNNING', 5: 'COMPLETED', 6: 'HELD', 7: 'PREPARED', 8: 'SKIPPED', 9: 'DELAYED'}
+    LOGICAL_ORDER = ["WAITING", "DELAYED", "PREPARED", "READY", "SUBMITTED", "HELD", "QUEUING", "RUNNING", "SKIPPED", "FAILED", "UNKNOWN", "COMPLETED", "SUSPENDED"]
 
     def retval(self, value):
         return getattr(self, value)
 
 
 class bcolors:
     HEADER = '\033[95m'
@@ -124,14 +124,24 @@
                 fi 
             fi
             
             set -xuve
             job_name_ptrn='%CURRENT_LOGDIR%/%JOBNAME%'
             echo $(date +%s) > ${job_name_ptrn}_STAT
 
+            ################### 
+            # AS CHECKPOINT FUNCTION
+            ###################
+            # Creates a new checkpoint file upon call based on the current numbers of calls to the function
+            
+            AS_CHECKPOINT_CALLS=0
+            function as_checkpoint {
+                AS_CHECKPOINT_CALLS=$((AS_CHECKPOINT_CALLS+1))
+                touch ${job_name_ptrn}_CHECKPOINT_${AS_CHECKPOINT_CALLS}
+            }
             ###################
             # Autosubmit job
             ###################
 
             """)
 
     @staticmethod
@@ -186,19 +196,28 @@
                             locale.setlocale(locale.LC_ALL, 'es_ES')
             except Exception as e:
                 locale.setlocale(locale.LC_ALL, 'C')
             job_name_ptrn = '%CURRENT_LOGDIR%/%JOBNAME%'
             stat_file = open(job_name_ptrn + '_STAT', 'w')
             stat_file.write('{0:.0f}\\n'.format(time.time()))
             stat_file.close()
-
-
+            ###################
+            # Autosubmit Checkpoint
+            ###################
+            # Creates a new checkpoint file upton call based on the current numbers of calls to the function
+            AS_CHECKPOINT_CALLS = 0
+            def as_checkpoint():
+                global AS_CHECKPOINT_CALLS
+                global job_name_ptrn
+                AS_CHECKPOINT_CALLS = AS_CHECKPOINT_CALLS + 1
+                open(job_name_ptrn + '_CHECKPOINT_' + str(AS_CHECKPOINT_CALLS), 'w').close()                
             ###################
             # Autosubmit job
             ###################
+            
 
             """)
 
     # expand tailer to use python3
     def as_tailer(self):
         return textwrap.dedent("""\
 
@@ -250,15 +269,24 @@
                 }
             } 
             options( warn = oldw )
             job_name_ptrn = '%CURRENT_LOGDIR%/%JOBNAME%'
             fileConn<-file(paste(job_name_ptrn,"_STAT", sep = ''),"w")
             writeLines(toString(trunc(as.numeric(Sys.time()))), fileConn)
             close(fileConn)
-
+            ###################
+            # Autosubmit Checkpoint
+            ###################
+            # Creates a new checkpoint file upton call based on the current numbers of calls to the function
+            AS_CHECKPOINT_CALLS = 0
+            as_checkpoint <- function() {
+                AS_CHECKPOINT_CALLS <<- AS_CHECKPOINT_CALLS + 1
+                fileConn<-file(paste(job_name_ptrn,"_CHECKPOINT_",AS_CHECKPOINT_CALLS, sep = ''),"w")
+                close(fileConn)
+            }
             ###################
             # Autosubmit job
             ###################
 
             """)
 
     @staticmethod
```

### Comparing `autosubmit-4.0.84/autosubmit/job/job_dict.py` & `autosubmit-4.0.85/autosubmit/job/job_dict.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job_grouping.py` & `autosubmit-4.0.85/autosubmit/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job_list.py` & `autosubmit-4.0.85/autosubmit/job/job_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,71 +9,72 @@
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # Autosubmit is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
-
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
-import collections
 import copy
-import re
+import datetime
+import math
 import os
 import pickle
+import re
 import traceback
-import math
-import copy
-from time import localtime, strftime, mktime
+from bscearth.utils.date import date2str, parse_date
+from networkx import DiGraph
 from shutil import move
+from threading import Thread
+from time import localtime, strftime, mktime
+from typing import List, Dict
+
+import autosubmit.database.db_structure as DbStructure
+from autosubmit.helpers.data_transfer import JobRow
 from autosubmit.job.job import Job
-from autosubmit.job.job_package_persistence import JobPackagePersistence
+from autosubmit.job.job_common import Status, bcolors
 from autosubmit.job.job_dict import DicJobs
+from autosubmit.job.job_package_persistence import JobPackagePersistence
 from autosubmit.job.job_packages import JobPackageThread
 from autosubmit.job.job_utils import Dependency
-from autosubmit.job.job_common import Status, bcolors
-from bscearth.utils.date import date2str, parse_date
-import autosubmit.database.db_structure as DbStructure
-import datetime
-from networkx import DiGraph
 from autosubmit.job.job_utils import transitive_reduction
-from log.log import AutosubmitCritical, AutosubmitError, Log
-from threading import Thread
 from autosubmitconfigparser.config.basicconfig import BasicConfig
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
-from autosubmit.helpers.data_transfer import JobRow
-from typing import List, Dict
-import log.fd_show
+from log.log import AutosubmitCritical, AutosubmitError, Log
+
+
 # Log.get_logger("Log.Autosubmit")
 
 
 def threaded(fn):
     def wrapper(*args, **kwargs):
         thread = Thread(target=fn, args=args, kwargs=kwargs)
         thread.name = "data_processing"
         thread.start()
         return thread
+
     return wrapper
 
 
 class JobList(object):
     """
     Class to manage the list of jobs to be run by autosubmit
 
     """
 
-    def __init__(self, expid, config, parser_factory, job_list_persistence,as_conf):
+    def __init__(self, expid, config, parser_factory, job_list_persistence, as_conf):
         self._persistence_path = os.path.join(
             config.LOCAL_ROOT_DIR, expid, "pkl")
         self._update_file = "updated_list_" + expid + ".txt"
         self._failed_file = "failed_job_list_" + expid + ".pkl"
         self._persistence_file = "job_list_" + expid
         self._job_list = list()
         self._base_job_list = list()
+        self.jobs_edges = {}
         self._expid = expid
         self._config = config
         self.experiment_data = as_conf.experiment_data
         self._parser_factory = parser_factory
         self._stat_val = Status()
         self._parameters = []
         self._date_list = []
@@ -88,14 +89,15 @@
 
         self.packages_id = dict()
         self.job_package_map = dict()
         self.sections_checked = set()
         self._run_members = None
         self.jobs_to_run_first = list()
         self.rerun_job_list = list()
+
     @property
     def expid(self):
         """
         Returns the experiment identifier
 
         :return: experiment's identifier
         :rtype: str
@@ -122,54 +124,64 @@
 
     @property
     def run_members(self):
         return self._run_members
 
     @run_members.setter
     def run_members(self, value):
-        if value is not None and len(str(value)) > 0 :
+        if value is not None and len(str(value)) > 0:
             self._run_members = value
-            self._base_job_list = [job for job in self._job_list]            
+            self._base_job_list = [job for job in self._job_list]
             found_member = False
             processed_job_list = []
-            for job in self._job_list: # We are assuming that the jobs are sorted in topological order (which is the default)
-                if (job.member is None and found_member is False) or job.member in self._run_members or job.status not in [Status.WAITING, Status.READY]:
+            for job in self._job_list:  # We are assuming that the jobs are sorted in topological order (which is the default)
+                if (
+                        job.member is None and not found_member) or job.member in self._run_members or job.status not in [
+                    Status.WAITING, Status.READY]:
                     processed_job_list.append(job)
                 if job.member is not None and len(str(job.member)) > 0:
                     found_member = True
-            self._job_list = processed_job_list    
+            self._job_list = processed_job_list
             # Old implementation that also considered children of the members.        
             # self._job_list = [job for job in old_job_list if len(
             #     job.parents) == 0 or len(set(old_job_list_names).intersection(set([jobp.name for jobp in job.parents]))) == len(job.parents)]
 
-    def create_dictionary(self, date_list, member_list, num_chunks, chunk_ini, date_format, default_retrials, wrapper_jobs):
+    def create_dictionary(self, date_list, member_list, num_chunks, chunk_ini, date_format, default_retrials,
+                          wrapper_jobs):
         chunk_list = list(range(chunk_ini, num_chunks + 1))
 
         jobs_parser = self._get_jobs_parser()
         dic_jobs = DicJobs(self, date_list, member_list,
-                           chunk_list, date_format, default_retrials,jobs_data={},experiment_data=self.experiment_data)
+                           chunk_list, date_format, default_retrials, jobs_data={},
+                           experiment_data=self.experiment_data)
         self._dic_jobs = dic_jobs
         for wrapper_section in wrapper_jobs:
             if str(wrapper_jobs[wrapper_section]).lower() != 'none':
-                self._ordered_jobs_by_date_member[wrapper_section] = self._create_sorted_dict_jobs(wrapper_jobs[wrapper_section])
+                self._ordered_jobs_by_date_member[wrapper_section] = self._create_sorted_dict_jobs(
+                    wrapper_jobs[wrapper_section])
             else:
                 self._ordered_jobs_by_date_member[wrapper_section] = {}
         pass
+
     def _delete_edgeless_jobs(self):
         jobs_to_delete = []
         # indices to delete
         for i, job in enumerate(self._job_list):
             if job.dependencies is not None:
-                if ( ( len(job.dependencies) > 0 and not job.has_parents()) and not job.has_children()) and job.delete_when_edgeless in ["true",True,1]:
+                if ((
+                            len(job.dependencies) > 0 and not job.has_parents()) and not job.has_children()) and job.delete_when_edgeless in [
+                    "true", True, 1]:
                     jobs_to_delete.append(job)
         # delete jobs by indices
         for i in jobs_to_delete:
             self._job_list.remove(i)
+
     def generate(self, date_list, member_list, num_chunks, chunk_ini, parameters, date_format, default_retrials,
-                 default_job_type, wrapper_type=None, wrapper_jobs=dict(), new=True, notransitive=False, update_structure=False, run_only_members=[],show_log=True,jobs_data={},as_conf=""):
+                 default_job_type, wrapper_type=None, wrapper_jobs=dict(), new=True, notransitive=False,
+                 update_structure=False, run_only_members=[], show_log=True, jobs_data={}, as_conf=""):
         """
         Creates all jobs needed for the current workflow
 
         :param as_conf:
         :param jobs_data:
         :param show_log:
         :param run_only_members:
@@ -199,16 +211,16 @@
         """
         self._parameters = parameters
         self._date_list = date_list
         self._member_list = member_list
         chunk_list = list(range(chunk_ini, num_chunks + 1))
         self._chunk_list = chunk_list
 
-
-        dic_jobs = DicJobs(self,date_list, member_list,chunk_list, date_format, default_retrials,jobs_data,experiment_data=self.experiment_data)
+        dic_jobs = DicJobs(self, date_list, member_list, chunk_list, date_format, default_retrials, jobs_data,
+                           experiment_data=self.experiment_data)
         self._dic_jobs = dic_jobs
         priority = 0
         if show_log:
             Log.info("Creating jobs...")
         # jobs_data includes the name of the .our and .err files of the job in LOG_expid
         jobs_data = dict()
         if not new:
@@ -216,31 +228,31 @@
                 jobs_data = {row[0]: row for row in self.load()}
             except Exception as e:
                 try:
                     jobs_data = {row[0]: row for row in self.backup_load()}
                 except Exception as e:
                     pass
                     Log.info("Deleting previous pkl due being incompatible with current AS version")
-                    if os.path.exists(os.path.join(self._persistence_path, self._persistence_file+".pkl")):
-                        os.remove(os.path.join(self._persistence_path, self._persistence_file+".pkl"))
-                    if os.path.exists(os.path.join(self._persistence_path, self._persistence_file+"_backup.pkl")):
-                        os.remove(os.path.join(self._persistence_path, self._persistence_file+"_backup.pkl"))
+                    if os.path.exists(os.path.join(self._persistence_path, self._persistence_file + ".pkl")):
+                        os.remove(os.path.join(self._persistence_path, self._persistence_file + ".pkl"))
+                    if os.path.exists(os.path.join(self._persistence_path, self._persistence_file + "_backup.pkl")):
+                        os.remove(os.path.join(self._persistence_path, self._persistence_file + "_backup.pkl"))
 
-        self._create_jobs(dic_jobs, priority,default_job_type, jobs_data)
+        self._create_jobs(dic_jobs, priority, default_job_type, jobs_data)
         if show_log:
             Log.info("Adding dependencies...")
-        self._add_dependencies(date_list, member_list,chunk_list, dic_jobs, self.graph)
+        self._add_dependencies(date_list, member_list, chunk_list, dic_jobs, self.graph)
 
         if show_log:
             Log.info("Removing redundant dependencies...")
         self.update_genealogy(
             new, notransitive, update_structure=update_structure)
         for job in self._job_list:
             job.parameters = parameters
-            job_data = jobs_data.get(job.name,"none")
+            job_data = jobs_data.get(job.name, "none")
             try:
                 if job_data != "none":
                     job.wrapper_type = job_data[12]
                 else:
                     job.wrapper_type = "none"
             except BaseException as e:
                 job.wrapper_type = "none"
@@ -249,68 +261,70 @@
         if len(run_only_members) > 0:
             # Found
             if show_log:
                 Log.info("Considering only members {0}".format(
                     str(run_only_members)))
             old_job_list = [job for job in self._job_list]
             self._job_list = [
-                job for job in old_job_list if job.member is None or job.member in run_only_members or job.status not in [Status.WAITING, Status.READY]]
+                job for job in old_job_list if
+                job.member is None or job.member in run_only_members or job.status not in [Status.WAITING,
+                                                                                           Status.READY]]
             for job in self._job_list:
                 for jobp in job.parents:
                     if jobp in self._job_list:
                         job.parents.add(jobp)
                 for jobc in job.children:
                     if jobc in self._job_list:
                         job.children.add(jobc)
         if show_log:
             Log.info("Looking for edgeless jobs...")
         self._delete_edgeless_jobs()
         for wrapper_section in wrapper_jobs:
             try:
                 if wrapper_jobs[wrapper_section] is not None and len(str(wrapper_jobs[wrapper_section])) > 0:
-                    self._ordered_jobs_by_date_member[wrapper_section] = self._create_sorted_dict_jobs(wrapper_jobs[wrapper_section])
+                    self._ordered_jobs_by_date_member[wrapper_section] = self._create_sorted_dict_jobs(
+                        wrapper_jobs[wrapper_section])
                 else:
                     self._ordered_jobs_by_date_member[wrapper_section] = {}
             except BaseException as e:
-                raise AutosubmitCritical("Some section jobs of the wrapper:{0} are not in the current job_list defined in jobs.conf".format(wrapper_section),7014,str(e))
-
+                raise AutosubmitCritical(
+                    "Some section jobs of the wrapper:{0} are not in the current job_list defined in jobs.conf".format(
+                        wrapper_section), 7014, str(e))
 
-    @staticmethod
-    def _add_dependencies(date_list, member_list, chunk_list, dic_jobs, graph, option="DEPENDENCIES"):
-        jobs_data = dic_jobs._jobs_data.get("JOBS",{})
+    def _add_dependencies(self, date_list, member_list, chunk_list, dic_jobs, graph, option="DEPENDENCIES"):
+        jobs_data = dic_jobs._jobs_data.get("JOBS", {})
         for job_section in jobs_data.keys():
             Log.debug("Adding dependencies for {0} jobs".format(job_section))
             # If it does not have dependencies, do nothing
             if not (job_section, option):
                 continue
 
-            dependencies_keys = jobs_data[job_section].get(option,{})
+            dependencies_keys = jobs_data[job_section].get(option, {})
             if type(dependencies_keys) is str:
                 if "," in dependencies_keys:
                     dependencies_list = dependencies_keys.split(",")
                 else:
                     dependencies_list = dependencies_keys.split(" ")
                 dependencies_keys = {}
                 for dependency in dependencies_list:
                     dependencies_keys[dependency] = {}
             if dependencies_keys is None:
                 dependencies_keys = {}
-            dependencies = JobList._manage_dependencies(dependencies_keys, dic_jobs, job_section)
+            dependencies = self._manage_dependencies(dependencies_keys, dic_jobs, job_section)
 
             for job in dic_jobs.get_jobs(job_section):
                 num_jobs = 1
                 if isinstance(job, list):
                     num_jobs = len(job)
                 for i in range(num_jobs):
                     _job = job[i] if num_jobs > 1 else job
-                    JobList._manage_job_dependencies(dic_jobs, _job, date_list, member_list, chunk_list, dependencies_keys,
-                                                     dependencies, graph)
+                    self._manage_job_dependencies(dic_jobs, _job, date_list, member_list, chunk_list, dependencies_keys,
+                                                  dependencies, graph)
         pass
 
-
     @staticmethod
     def _manage_dependencies(dependencies_keys, dic_jobs, job_section):
         parameters = dic_jobs._jobs_data["JOBS"]
         dependencies = dict()
         for key in dependencies_keys:
             distance = None
             splits = None
@@ -330,31 +344,31 @@
                     elif '*' in key:
                         sign = '*'
                     key_split = key.split(sign)
                     section = key_split[0]
                     distance = int(key_split[1])
 
             if '[' in section:
-                #Todo check what is this because we never enter this
+                # Todo check what is this because we never enter this
                 try:
                     section_name = section[0:section.find("[")]
                     splits_section = int(
                         dic_jobs.experiment_data["JOBS"][section_name].get('SPLITS', -1))
                     splits = JobList._calculate_splits_dependencies(
                         section, splits_section)
                     section = section_name
                 except Exception as e:
                     pass
-            if parameters.get(section,None) is None:
-                Log.printlog("WARNING: SECTION {0} is not defined in jobs.conf".format(section))
+            if parameters.get(section, None) is None:
                 continue
-                #raise AutosubmitCritical("Section:{0} doesn't exists.".format(section),7014)
+                # raise AutosubmitCritical("Section:{0} doesn't exists.".format(section),7014)
             dependency_running_type = str(parameters[section].get('RUNNING', 'once')).lower()
             delay = int(parameters[section].get('DELAY', -1))
-            dependency = Dependency(section, distance, dependency_running_type, sign, delay, splits,relationships=dependencies_keys[key])
+            dependency = Dependency(section, distance, dependency_running_type, sign, delay, splits,
+                                    relationships=dependencies_keys[key])
             dependencies[key] = dependency
         return dependencies
 
     @staticmethod
     def _calculate_splits_dependencies(section, max_splits):
         splits_list = section[section.find("[") + 1:section.find("]")]
         splits = []
@@ -366,276 +380,452 @@
                 for count in range(int(numbers[0]), max_splits + 1):
                     splits.append(int(str(count).zfill(len(numbers[0]))))
             else:
                 if int(str_split) <= max_splits:
                     splits.append(int(str_split))
         return splits
 
+
     @staticmethod
-    def _apply_filter(parent_value,filter_value,associative_list,filter_type="dates"):
+    def _apply_filter(parent_value, filter_value, associative_list, level_to_check="DATES_FROM", child=None, parent=None):
         """
         Check if the current_job_value is included in the filter_value
         :param parent_value:
         :param filter_value: filter
-        :param associative_list: dates, members, chunks.
-        :param is_chunk: True if the filter_value is a chunk.
-        :return: boolean
-        """
-        to_filter = []
-        # strip special chars if any
-        filter_value = filter_value.strip("?")
-        if str(parent_value).lower().find("none") != -1:
+        :param associative_list: dates, members, chunks, splits.
+        :param filter_type: dates, members, chunks, splits .
+        :param level_to_check: Can be dates,members, chunks, splits.
+        :return:
+        """
+        if "NONE".casefold() in str(parent_value).casefold():
             return True
-        if filter_value.lower().find("all") != -1:
+        if parent and child and level_to_check.casefold() == "splits".casefold():
+            if not parent.splits:
+                parent_splits = -1
+            else:
+                parent_splits = parent.splits
+            if not child.splits:
+                child_splits = -1
+            else:
+                child_splits = child.splits
+            if parent_splits == child_splits:
+                to_look_at_lesser = associative_list
+                lesser_group = -1
+                lesser = str(parent_splits)
+                greater = str(child_splits)
+                lesser_value = "parent"
+            else:
+                if parent_splits > child_splits:
+                    lesser = str(child_splits)
+                    greater = str(parent_splits)
+                    lesser_value = "child"
+                else:
+                    lesser = str(parent_splits)
+                    greater = str(child_splits)
+                    lesser_value = "parent"
+                to_look_at_lesser = [associative_list[i:i + 1] for i in range(0, int(lesser), 1)]
+                for lesser_group in range(len(to_look_at_lesser)):
+                    if lesser_value == "parent":
+                        if str(parent_value) in to_look_at_lesser[lesser_group]:
+                            break
+                    else:
+                        if str(child.split) in to_look_at_lesser[lesser_group]:
+                            break
+        else:
+            to_look_at_lesser = associative_list
+            lesser_group = -1
+        if "?" in filter_value:
+            # replace all ? for ""
+            filter_value = filter_value.replace("?", "")
+        if "*" in filter_value:
+            aux_filter = filter_value
+            filter_value = ""
+            for filter_ in aux_filter.split(","):
+                if "*" in filter_:
+                    filter_,split_info = filter_.split("*")
+                    if "\\" in split_info:
+                        split_info = int(split_info.split("\\")[-1])
+                    else:
+                        split_info = 1
+                    # split_info: if a value is 1, it means that the filter is 1-to-1, if it is 2, it means that the filter is 1-to-2, etc.
+                    if child and parent:
+                        if (split_info == 1 or level_to_check.casefold() != "splits".casefold()) and str(parent_value).casefold() == str(filter_).casefold():
+                            if child.split == parent_value:
+                                return True
+                        elif split_info > 1 and level_to_check.casefold() == "splits".casefold():
+                            # 1-to-X filter
+                            to_look_at_greater = [associative_list[i:i + split_info] for i in
+                                                range(0, int(greater), split_info)]
+                            if lesser_value == "parent":
+                                if str(child.split) in to_look_at_greater[lesser_group]:
+                                    return True
+                            else:
+                                if str(parent_value) in to_look_at_greater[lesser_group]:
+                                    return True
+                    else:
+                        filter_value += filter_ + ","
+                else:
+                    filter_value += filter_ + ","
+            filter_value = filter_value[:-1]
+        to_filter = JobList._parse_filters_to_check(filter_value,associative_list,level_to_check)
+        if to_filter is None:
+            return False
+        elif len(to_filter) == 0:
+            return False
+        elif "ALL".casefold() == str(to_filter[0]).casefold():
             return True
-        elif filter_value.lower().find("natural") != -1:
+        elif "NATURAL".casefold() == str(to_filter[0]).casefold():
             if parent_value is None or parent_value in associative_list:
                 return True
-        elif filter_value.lower().find("none") != -1:
+        elif "NONE".casefold() == str(to_filter[0]).casefold():
             return False
-        elif filter_value.find(",") != -1:
-            aux_filter = filter_value.split(",")
-            if filter_type not in ["chunks", "splits"]:
-                for value in aux_filter:
-                    if str(value).isdigit():
-                        to_filter.append(associative_list[int(value)])
-                    else:
-                        to_filter.append(value)
-            else:
-                to_filter = aux_filter
-            del aux_filter
-        elif filter_value.find(":") != -1:
-            start_end = filter_value.split(":")
-            start = start_end[0].strip("[]")
-            end = start_end[1].strip("[]")
-            del start_end
-            if filter_type not in ["chunks", "splits"]: # chunk directly
-                for value in range(int(start), int(end) + 1):
-                    to_filter.append(value)
-            else: # index
-                for value in range(int(start+1), int(end) + 1):
-                    to_filter.append(value)
-        else:
-            to_filter.append(filter_value)
-
-        if str(parent_value).upper() in str(to_filter).upper():
+        elif len( [ filter_ for filter_ in to_filter if str(parent_value).casefold() == str(filter_).casefold() ] )>0:
             return True
         else:
             return False
 
 
+
+    @staticmethod
+    def _parse_filters_to_check(list_of_values_to_check,value_list=[],level_to_check="DATES_FROM"):
+        final_values = []
+        list_of_values_to_check = str(list_of_values_to_check).upper()
+        if list_of_values_to_check is None:
+            return None
+        elif list_of_values_to_check.casefold() == "ALL".casefold() :
+            return ["ALL"]
+        elif list_of_values_to_check.casefold() == "NONE".casefold():
+            return ["NONE"]
+        elif list_of_values_to_check.casefold() == "NATURAL".casefold():
+            return ["NATURAL"]
+        elif "," in list_of_values_to_check:
+            for value_to_check in list_of_values_to_check.split(","):
+                final_values.extend(JobList._parse_filter_to_check(value_to_check,value_list,level_to_check))
+        else:
+            final_values = JobList._parse_filter_to_check(list_of_values_to_check,value_list,level_to_check)
+        return final_values
+
+
     @staticmethod
-    def _check_relationship(relationships,level_to_check,value_to_check):
+    def _parse_filter_to_check(value_to_check,value_list=[],level_to_check="DATES_FROM"):
+        """
+        Parse the filter to check and return the value to check.
+        Selection process:
+        value_to_check can be:
+        a range: [0:], [:N], [0:N], [:-1], [0:N:M] ...
+        a value: N.
+        a range with step: [0::M], [::2], [0::3], [::3] ...
+        :param value_to_check: value to check.
+        :param value_list: list of values to check. Dates, members, chunks or splits.
+        :return: parsed value to check.
+        """
+        step = 1
+        if value_to_check.count(":") == 1:
+            # range
+            if value_to_check[1] == ":":
+                # [:N]
+                # Find N index in the list
+                start = None
+                end = value_to_check.split(":")[1].strip("[]")
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    end = int(end)
+            elif value_to_check[-2] == ":":
+                # [N:]
+                # Find N index in the list
+                start = value_to_check.split(":")[0].strip("[]")
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    start = int(start)
+                end = None
+            else:
+                # [N:M]
+                # Find N index in the list
+                start = value_to_check.split(":")[0].strip("[]")
+                end = value_to_check.split(":")[1].strip("[]")
+                step = 1
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    start = int(start)
+                    end = int(end)
+        elif value_to_check.count(":") == 2:
+            # range with step
+            if value_to_check[-2] == ":" and value_to_check[-3] == ":":  # [N::]
+                # Find N index in the list
+                start = value_to_check.split(":")[0].strip("[]")
+                end = None
+                step = 1
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    start = int(start)
+            elif value_to_check[1] == ":" and value_to_check[2] == ":":  # [::S]
+                # Find N index in the list
+                start = None
+                end = None
+                step = value_to_check.split(":")[-1].strip("[]")
+                # get index in the value_list
+                step = int(step)
+            elif value_to_check[1] == ":" and value_to_check[-2] == ":": # [:M:]
+                # Find N index in the list
+                start = None
+                end = value_to_check.split(":")[1].strip("[]")
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    end = int(end)
+                step = 1
+            else: # [N:M:S]
+                # Find N index in the list
+                start = value_to_check.split(":")[0].strip("[]")
+                end = value_to_check.split(":")[1].strip("[]")
+                step = value_to_check.split(":")[2].strip("[]")
+                step = int(step)
+                if level_to_check in ["CHUNKS_FROM","SPLITS_FROM"]:
+                    start = int(start)
+                    end = int(end)
+        else:
+            # value
+            return [value_to_check]
+        ## values to return
+        if len(value_list) > 0:
+            if start is None:
+                start = value_list[0]
+            if end is None:
+                end = value_list[-1]
+            try:
+                if level_to_check == "CHUNKS_TO":
+                    start = int(start)
+                    end = int(end)
+                return value_list[slice(value_list.index(start), value_list.index(end)+1, int(step))]
+            except ValueError:
+                return value_list[slice(0,len(value_list)-1,int(step))]
+        else:
+            if not start:
+                start = 0
+            if end is None:
+                return []
+            return [number_gen for number_gen in range(int(start), int(end)+1, int(step))]
+
+    def _check_relationship(self, relationships, level_to_check, value_to_check):
         """
         Check if the current_job_value is included in the filter_value
-        :param relationship: current filter level to check.
-        :param level_to_check: can be a date, member, chunk or split.
+        :param relationships: current filter level to check.
+        :param level_to_check: Can be dates_from, members_from, chunks_from, splits_from.
         :param value_to_check: Can be None, a date, a member, a chunk or a split.
         :return:
         """
         filters = []
-        for filter_range,filter_data in relationships.get(level_to_check,{}).items():
-            if not value_to_check or str(filter_range).upper() in "ALL" or str(value_to_check).upper() in str(filter_range).upper():
-                if filter_data:
-                    if "?" in filter_range:
-                        filter_data["OPTIONAL"] = True
-                    else:
-                        filter_data["OPTIONAL"] = relationships["OPTIONAL"]
+        if level_to_check == "DATES_FROM":
+            try:
+                value_to_check = date2str(value_to_check, "%Y%m%d") # need to convert in some cases
+            except:
+                pass
+            try:
+                values_list = [date2str(date_, "%Y%m%d") for date_ in self._date_list] # need to convert in some cases
+            except:
+                values_list = self._date_list
+        elif level_to_check == "MEMBERS_FROM":
+            values_list = self._member_list # Str list
+        elif level_to_check == "CHUNKS_FROM":
+            values_list = self._chunk_list # int list
+        else:
+            values_list = [] # splits, int list ( artificially generated later )
+
+        relationship = relationships.get(level_to_check, {})
+        status = relationship.pop("STATUS", relationships.get("STATUS", None))
+        from_step = relationship.pop("FROM_STEP", relationships.get("FROM_STEP", None))
+        for filter_range, filter_data in relationship.items():
+            if filter_range.casefold() in ["ALL".casefold(),"NATURAL".casefold()] or ( not value_to_check or str(value_to_check).upper() in str(
+                    JobList._parse_filters_to_check(filter_range,values_list,level_to_check)).upper()):
+                if not filter_data.get("STATUS", None):
+                    filter_data["STATUS"] = status
+                if not filter_data.get("FROM_STEP", None):
+                    filter_data["FROM_STEP"] = from_step
                 filters.append(filter_data)
         # Normalize the filter return
         if len(filters) == 0:
             filters = [{}]
         return filters
 
-    @staticmethod
-    def _check_dates(relationships, current_job):
+
+    def _check_dates(self, relationships, current_job):
         """
         Check if the current_job_value is included in the filter_from and retrieve filter_to value
         :param relationships: Remaining filters to apply.
         :param current_job: Current job to check.
         :return:  filters_to_apply
         """
-        optional = False
-        filters_to_apply = JobList._check_relationship(relationships, "DATES_FROM", date2str(current_job.date))
-        # there could be multiple filters that apply... per example
-        # Current task date is 20020201, and member is fc2
-        # Dummy example, not specially usefull in a real case
-        #DATES_FROM:
-            #all:
-                #MEMBERS_FROM:
-                    #ALL: ...
-                #CHUNKS_FROM:
-                    #ALL: ...
-            #20020201:
-                #MEMBERS_FROM:
-                    #fc2:
-                        #DATES_TO: "20020201"
-                        #MEMBERS_TO: "fc2"
-                        #CHUNKS_TO: "ALL"
-                #SPLITS_FROM:
-                    #ALL:
-                        #SPLITS_TO: "1"
-        # this "for" iterates for ALL and fc2 as current task is selected in both filters
-        # The dict in this step is:
-        # [{MEMBERS_FROM{..},CHUNKS_FROM{...}},{MEMBERS_FROM{..},SPLITS_FROM{...}}]
-        for i,filter in enumerate(filters_to_apply):
-            # {MEMBERS_FROM{..},CHUNKS_FROM{...}} I want too look ALL filters not only one, but I want to go recursivily until get the  _TO filter
-            optional = filter.pop("OPTIONAL", False)
-            # This is not an if_else, because the current level ( dates ) could have two different filters.
-            # Second case commented: ( date_from 20020201 )
-            # Will enter, go recursivily to the similar methods and in the end it will do:
-            # Will enter members_from, and obtain [{DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", CHUNKS_FROM{...}]
+        # Check the test_dependencies.py to see how to use this function
+        filters_to_apply = self._check_relationship(relationships, "DATES_FROM", date2str(current_job.date))
+        for i, filter in enumerate(filters_to_apply):
             if "MEMBERS_FROM" in filter:
-                filters_to_apply_m = JobList._check_members({"MEMBERS_FROM": (filter.pop("MEMBERS_FROM")),"OPTIONAL":optional}, current_job)
+                filters_to_apply_m = self._check_members({"MEMBERS_FROM": (filter.pop("MEMBERS_FROM"))}, current_job)
                 if len(filters_to_apply_m) > 0:
                     filters_to_apply[i].update(filters_to_apply_m)
             # Will enter chunks_from, and obtain [{DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", SPLITS_TO: "2"]
             if "CHUNKS_FROM" in filter:
-                filters_to_apply_c = JobList._check_chunks({"CHUNKS_FROM": (filter.pop("CHUNKS_FROM")),"OPTIONAL":optional}, current_job)
+                filters_to_apply_c = self._check_chunks({"CHUNKS_FROM": (filter.pop("CHUNKS_FROM"))}, current_job)
                 if len(filters_to_apply_c) > 0 and len(filters_to_apply_c[0]) > 0:
                     filters_to_apply[i].update(filters_to_apply_c)
-            #IGNORED
+            # IGNORED
             if "SPLITS_FROM" in filter:
-                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+                filters_to_apply_s = self._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM"))}, current_job)
                 if len(filters_to_apply_s) > 0:
                     filters_to_apply[i].update(filters_to_apply_s)
         # Unify filters from all filters_from where the current job is included to have a single SET of filters_to
-        if optional:
-            for i,filter in enumerate(filters_to_apply):
-                filters_to_apply[i]["OPTIONAL"] = True
-        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        filters_to_apply = self._unify_to_filters(filters_to_apply)
         # {DATES_TO: "20020201", MEMBERS_TO: "fc2", CHUNKS_TO: "ALL", SPLITS_TO: "2"}
         return filters_to_apply
 
-    @staticmethod
-    def _check_members(relationships, current_job):
+
+    def _check_members(self,relationships, current_job):
         """
         Check if the current_job_value is included in the filter_from and retrieve filter_to value
         :param relationships: Remaining filters to apply.
         :param current_job: Current job to check.
         :return: filters_to_apply
         """
-        filters_to_apply = JobList._check_relationship(relationships, "MEMBERS_FROM", current_job.member)
-        optional = False
-        for i,filter in enumerate(filters_to_apply):
-            optional = filter.pop("OPTIONAL", False)
-            if "CHUNKS_FROM" in filter:
-                filters_to_apply_c = JobList._check_chunks({"CHUNKS_FROM": (filter.pop("CHUNKS_FROM")),"OPTIONAL":optional}, current_job)
+        filters_to_apply = self._check_relationship(relationships, "MEMBERS_FROM", current_job.member)
+        for i, filter_ in enumerate(filters_to_apply):
+            if "CHUNKS_FROM" in filter_:
+                filters_to_apply_c = self._check_chunks({"CHUNKS_FROM": (filter_.pop("CHUNKS_FROM"))}, current_job)
                 if len(filters_to_apply_c) > 0:
                     filters_to_apply[i].update(filters_to_apply_c)
-
-            if "SPLITS_FROM" in filter:
-                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+            if "SPLITS_FROM" in filter_:
+                filters_to_apply_s = self._check_splits({"SPLITS_FROM": (filter_.pop("SPLITS_FROM"))}, current_job)
                 if len(filters_to_apply_s) > 0:
                     filters_to_apply[i].update(filters_to_apply_s)
-        if optional:
-            for i,filter in enumerate(filters_to_apply):
-                filters_to_apply[i]["OPTIONAL"] = True
-        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        filters_to_apply = self._unify_to_filters(filters_to_apply)
         return filters_to_apply
 
-    @staticmethod
-    def _check_chunks(relationships, current_job):
+    def _check_chunks(self,relationships, current_job):
         """
         Check if the current_job_value is included in the filter_from and retrieve filter_to value
         :param relationships: Remaining filters to apply.
         :param current_job: Current job to check.
         :return: filters_to_apply
         """
-        optional = False
-        filters_to_apply = JobList._check_relationship(relationships, "CHUNKS_FROM", current_job.chunk)
-        for i,filter in enumerate(filters_to_apply):
-            optional = filter.pop("OPTIONAL", False)
+
+        filters_to_apply = self._check_relationship(relationships, "CHUNKS_FROM", current_job.chunk)
+        for i, filter in enumerate(filters_to_apply):
             if "SPLITS_FROM" in filter:
-                filters_to_apply_s = JobList._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM")),"OPTIONAL":optional}, current_job)
+                filters_to_apply_s = self._check_splits({"SPLITS_FROM": (filter.pop("SPLITS_FROM"))}, current_job)
                 if len(filters_to_apply_s) > 0:
                     filters_to_apply[i].update(filters_to_apply_s)
-        if optional:
-            for i,filter in enumerate(filters_to_apply):
-                filters_to_apply[i]["OPTIONAL"] = True
-        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        filters_to_apply = self._unify_to_filters(filters_to_apply)
         return filters_to_apply
 
-    @staticmethod
-    def _check_splits(relationships, current_job):
+    def _check_splits(self,relationships, current_job):
         """
         Check if the current_job_value is included in the filter_from and retrieve filter_to value
         :param relationships: Remaining filters to apply.
         :param current_job: Current job to check.
         :return: filters_to_apply
         """
 
-        filters_to_apply = JobList._check_relationship(relationships, "SPLITS_FROM", current_job.split)
+        filters_to_apply = self._check_relationship(relationships, "SPLITS_FROM", current_job.split)
         # No more FROM sections to check, unify _to FILTERS and return
-        filters_to_apply = JobList._unify_to_filters(filters_to_apply)
+        filters_to_apply = self._unify_to_filters(filters_to_apply)
         return filters_to_apply
 
-    @staticmethod
-    def _unify_to_filter(unified_filter,filter_to,filter_type):
+    def _unify_to_filter(self,unified_filter, filter_to, filter_type):
         """
         Unify filter_to filters into a single dictionary
         :param unified_filter: Single dictionary with all filters_to
         :param filter_to: Current dictionary that contains the filters_to
         :param filter_type: "DATES_TO", "MEMBERS_TO", "CHUNKS_TO", "SPLITS_TO"
         :return: unified_filter
         """
-        if "all" not in unified_filter[filter_type]:
+        if len(unified_filter[filter_type]) > 0 and unified_filter[filter_type][-1] != ",":
+            unified_filter[filter_type] += ","
+        if filter_type == "DATES_TO":
+            value_list = self._date_list
+            level_to_check = "DATES_FROM"
+        elif filter_type == "MEMBERS_TO":
+            value_list = self._member_list
+            level_to_check = "MEMBERS_FROM"
+        elif filter_type == "CHUNKS_TO":
+            value_list = self._chunk_list
+            level_to_check = "CHUNKS_FROM"
+        elif filter_type == "SPLITS_TO":
+            value_list = []
+            level_to_check = "SPLITS_FROM"
+        if "all".casefold() not in unified_filter[filter_type].casefold():
             aux = filter_to.pop(filter_type, None)
             if aux:
                 aux = aux.split(",")
                 for element in aux:
-                    if element.lower().strip("?") in ["natural","none"] and len(unified_filter[filter_type]) > 0:
+                    if element == "":
+                        continue
+                    # Get only the first alphanumeric part and [:] chars
+                    parsed_element = re.findall(r"([\[:\]a-zA-Z0-9]+)", element)[0].lower()
+                    extra_data = element[len(parsed_element):]
+                    parsed_element = JobList._parse_filter_to_check(parsed_element, value_list = value_list, level_to_check = filter_type)
+                    # convert list to str
+                    skip = False
+                    if isinstance(parsed_element, list):
+                        # check if any element is natural or none
+                        for ele in parsed_element:
+                            if type(ele) is str and ele.lower() in ["natural", "none"]:
+                                skip = True
+                    else:
+                        if type(parsed_element) is str and parsed_element.lower() in ["natural", "none"]:
+                            skip = True
+                    if skip and len(unified_filter[filter_type]) > 0:
                         continue
                     else:
-                        if filter_to.get("OPTIONAL",False) and element[-1] != "?":
-                            element += "?"
-                        unified_filter[filter_type].add(element)
+                        for ele in parsed_element:
+                            if extra_data:
+                                check_whole_string = str(ele)+extra_data+","
+                            else:
+                                check_whole_string = str(ele)+","
+                            if str(check_whole_string) not in unified_filter[filter_type]:
+                                unified_filter[filter_type] += check_whole_string
+        return unified_filter
+
     @staticmethod
-    def _normalize_to_filters(filter_to,filter_type):
+    def _normalize_to_filters(filter_to, filter_type):
         """
         Normalize filter_to filters to a single string or "all"
         :param filter_to: Unified filter_to dictionary
         :param filter_type: "DATES_TO", "MEMBERS_TO", "CHUNKS_TO", "SPLITS_TO"
         :return:
         """
-        if len(filter_to[filter_type]) == 0:
+        if len(filter_to[filter_type]) == 0 or ("," in filter_to[filter_type] and len(filter_to[filter_type]) == 1):
             filter_to.pop(filter_type, None)
-        elif "all" in filter_to[filter_type]:
+        elif "all".casefold() in filter_to[filter_type]:
             filter_to[filter_type] = "all"
         else:
-            # transform to str separated by commas if multiple elements
-            filter_to[filter_type] = ",".join(filter_to[filter_type])
+            # delete last comma
+            if "," in filter_to[filter_type][-1]:
+                filter_to[filter_type] = filter_to[filter_type][:-1]
+            # delete first comma
+            if "," in filter_to[filter_type][0]:
+                filter_to[filter_type] = filter_to[filter_type][1:]
 
-    @staticmethod
-    def _unify_to_filters(filter_to_apply):
+    def _unify_to_filters(self,filter_to_apply):
         """
         Unify all filter_to filters into a single dictionary ( of current selection )
         :param filter_to_apply: Filters to apply
         :return: Single dictionary with all filters_to
         """
-        unified_filter = {"DATES_TO": set(), "MEMBERS_TO": set(), "CHUNKS_TO": set(), "SPLITS_TO": set()}
+        unified_filter = {"DATES_TO": "", "MEMBERS_TO": "", "CHUNKS_TO": "", "SPLITS_TO": ""}
         for filter_to in filter_to_apply:
+            if "STATUS" not in unified_filter and filter_to.get("STATUS", None):
+                unified_filter["STATUS"] = filter_to["STATUS"]
+            if "FROM_STEP" not in unified_filter and filter_to.get("FROM_STEP", None):
+                unified_filter["FROM_STEP"] = filter_to["FROM_STEP"]
             if len(filter_to) > 0:
-                JobList._unify_to_filter(unified_filter,filter_to,"DATES_TO")
-                JobList._unify_to_filter(unified_filter,filter_to,"MEMBERS_TO")
-                JobList._unify_to_filter(unified_filter,filter_to,"CHUNKS_TO")
-                JobList._unify_to_filter(unified_filter,filter_to,"SPLITS_TO")
-                filter_to.pop("OPTIONAL", None)
-
-        JobList._normalize_to_filters(unified_filter,"DATES_TO")
-        JobList._normalize_to_filters(unified_filter,"MEMBERS_TO")
-        JobList._normalize_to_filters(unified_filter,"CHUNKS_TO")
-        JobList._normalize_to_filters(unified_filter,"SPLITS_TO")
-
+                self._unify_to_filter(unified_filter, filter_to, "DATES_TO")
+                self._unify_to_filter(unified_filter, filter_to, "MEMBERS_TO")
+                self._unify_to_filter(unified_filter, filter_to, "CHUNKS_TO")
+                self._unify_to_filter(unified_filter, filter_to, "SPLITS_TO")
+
+        JobList._normalize_to_filters(unified_filter, "DATES_TO")
+        JobList._normalize_to_filters(unified_filter, "MEMBERS_TO")
+        JobList._normalize_to_filters(unified_filter, "CHUNKS_TO")
+        JobList._normalize_to_filters(unified_filter, "SPLITS_TO")
         return unified_filter
 
-    @staticmethod
-    def _filter_current_job(current_job,relationships):
-        '''
-        This function will filter the current job based on the relationships given
+    def _filter_current_job(self,current_job, relationships):
+        ''' This function will filter the current job based on the relationships given
         :param current_job: Current job to filter
         :param relationships: Relationships to apply
         :return: dict() with the filters to apply, or empty dict() if no filters to apply
         '''
 
         # This function will look if the given relationship is set for the given job DATEs,MEMBER,CHUNK,SPLIT ( _from filters )
         # And if it is, it will return the dependencies that need to be activated (_TO filters)
@@ -651,93 +841,108 @@
         # 2. NONE: no dependencies will be activated of the given filter type (dates, members, chunks or/and splits)
         # 3. NATURAL: this is the normal behavior, represents a way of letting the job to be activated if they would normally be activated.
         # 4. ? : this is a weak dependency activation flag, The dependency will be activated but the job can fail without affecting the workflow.
 
         filters_to_apply = {}
         # Check if filter_from-filter_to relationship is set
         if relationships is not None and len(relationships) > 0:
-            if "OPTIONAL" not in relationships:
-                relationships["OPTIONAL"] = False
             # Look for a starting point, this can be if else becasue they're exclusive as a DATE_FROM can't be in a MEMBER_FROM and so on
             if "DATES_FROM" in relationships:
-                filters_to_apply = JobList._check_dates(relationships, current_job)
+                filters_to_apply = self._check_dates(relationships, current_job)
             elif "MEMBERS_FROM" in relationships:
-                filters_to_apply = JobList._check_members(relationships, current_job)
+                filters_to_apply = self._check_members(relationships, current_job)
             elif "CHUNKS_FROM" in relationships:
-                filters_to_apply = JobList._check_chunks(relationships, current_job)
+                filters_to_apply = self._check_chunks(relationships, current_job)
             elif "SPLITS_FROM" in relationships:
-                filters_to_apply = JobList._check_splits(relationships, current_job)
+                filters_to_apply = self._check_splits(relationships, current_job)
             else:
-                relationships.pop("OPTIONAL", None)
                 relationships.pop("CHUNKS_FROM", None)
                 relationships.pop("MEMBERS_FROM", None)
                 relationships.pop("DATES_FROM", None)
                 relationships.pop("SPLITS_FROM", None)
                 filters_to_apply = relationships
         return filters_to_apply
 
-
-
     @staticmethod
-    def _valid_parent(parent,member_list,date_list,chunk_list,is_a_natural_relation,filter_):
+    def _valid_parent(parent, member_list, date_list, chunk_list, is_a_natural_relation, filter_,child):
         '''
         Check if the parent is valid for the current job
         :param parent: job to check
         :param member_list: list of members
         :param date_list: list of dates
         :param chunk_list: list of chunks
         :param is_a_natural_relation: if the relation is natural or not
-        :param filters_to_apply: filters to apply
         :return: True if the parent is valid, False otherwise
         '''
-        #check if current_parent is listed on dependency.relationships
+        # check if current_parent is listed on dependency.relationships
         associative_list = {}
         associative_list["dates"] = date_list
         associative_list["members"] = member_list
         associative_list["chunks"] = chunk_list
 
-        if parent.splits is not None:
-            associative_list["splits"] = [ str(split) for split in range(1,int(parent.splits)+1) ]
+        if not child.splits:
+            child_splits = 0
+        else:
+            child_splits = int(child.splits)
+        if not parent.splits:
+            parent_splits = 0
+        else:
+            parent_splits = int(parent.splits)
+        splits = max(child_splits, parent_splits)
+        if splits > 0:
+            associative_list["splits"] = [str(split) for split in range(1, int(splits) + 1)]
         else:
             associative_list["splits"] = None
         dates_to = str(filter_.get("DATES_TO", "natural")).lower()
         members_to = str(filter_.get("MEMBERS_TO", "natural")).lower()
         chunks_to = str(filter_.get("CHUNKS_TO", "natural")).lower()
         splits_to = str(filter_.get("SPLITS_TO", "natural")).lower()
+        
         if not is_a_natural_relation:
             if dates_to == "natural":
                 dates_to = "none"
             if members_to == "natural":
                 members_to = "none"
             if chunks_to == "natural":
                 chunks_to = "none"
             if splits_to == "natural":
                 splits_to = "none"
-        if dates_to == "natural":
+        if "natural" in dates_to:
             associative_list["dates"] = [date2str(parent.date)] if parent.date is not None else date_list
-        if members_to == "natural":
+        if "natural" in members_to:
             associative_list["members"] = [parent.member] if parent.member is not None else member_list
-        if chunks_to == "natural":
+        if "natural" in chunks_to:
             associative_list["chunks"] = [parent.chunk] if parent.chunk is not None else chunk_list
-        if splits_to == "natural":
+        if "natural" in splits_to:
             associative_list["splits"] = [parent.split] if parent.split is not None else parent.splits
         parsed_parent_date = date2str(parent.date) if parent.date is not None else None
-        # Apply all filters to look if this parent is an appropriated candidate for the current_job
-        valid_dates   = JobList._apply_filter(parsed_parent_date, dates_to, associative_list["dates"], "dates")
+        valid_dates = JobList._apply_filter(parsed_parent_date, dates_to, associative_list["dates"], "dates")
         valid_members = JobList._apply_filter(parent.member, members_to, associative_list["members"], "members")
-        valid_chunks  = JobList._apply_filter(parent.chunk, chunks_to, associative_list["chunks"], "chunks")
-        valid_splits  = JobList._apply_filter(parent.split, splits_to, associative_list["splits"], "splits")
+        valid_chunks = JobList._apply_filter(parent.chunk, chunks_to, associative_list["chunks"], "chunks")
+        valid_splits = JobList._apply_filter(parent.split, splits_to, associative_list["splits"], "splits", child, parent)
         if valid_dates and valid_members and valid_chunks and valid_splits:
-            for value in [dates_to, members_to, chunks_to, splits_to]:
-                if "?" in value:
-                    return True, True
-            return True, False
-        return False,False
-    @staticmethod
-    def _manage_job_dependencies(dic_jobs, job, date_list, member_list, chunk_list, dependencies_keys, dependencies,
+            return True
+        return False
+
+    def _add_edge_info(self, job, special_status):
+        """
+        Special relations to be check in the update_list method
+        :param job: Current job
+        :param parent: parent jobs to check
+        :return:
+        """
+        if special_status not in self.jobs_edges:
+            self.jobs_edges[special_status] = set()
+        self.jobs_edges[special_status].add(job)
+        if "ALL" not in self.jobs_edges:
+            self.jobs_edges["ALL"] = set()
+        self.jobs_edges["ALL"].add(job)
+
+    def _manage_job_dependencies(self, dic_jobs, job, date_list, member_list, chunk_list, dependencies_keys,
+                                 dependencies,
                                  graph):
         '''
         Manage the dependencies of a job
         :param dic_jobs:
         :param job:
         :param date_list:
         :param member_list:
@@ -746,50 +951,76 @@
         :param dependencies:
         :param graph:
         :return:
         '''
         parsed_date_list = []
         for dat in date_list:
             parsed_date_list.append(date2str(dat))
+        special_conditions = dict()
         for key in dependencies_keys:
-            dependency = dependencies.get(key,None)
+            dependency = dependencies.get(key, None)
             if dependency is None:
-                Log.printlog("WARNING: SECTION {0} is not defined in jobs.conf. Dependency skipped".format(key),Log.WARNING)
+                Log.printlog("WARNING: SECTION {0} is not defined in jobs.conf. Dependency skipped".format(key),
+                             Log.WARNING)
                 continue
             skip, (chunk, member, date) = JobList._calculate_dependency_metadata(job.chunk, chunk_list,
                                                                                  job.member, member_list,
                                                                                  job.date, date_list,
                                                                                  dependency)
             if skip:
                 continue
 
             other_parents = dic_jobs.get_jobs(dependency.section, None, None, None)
             parents_jobs = dic_jobs.get_jobs(dependency.section, date, member, chunk)
             natural_jobs = dic_jobs.get_jobs(dependency.section, date, member, chunk)
             all_parents = list(set(other_parents + parents_jobs))
             # Get dates_to, members_to, chunks_to of the deepest level of the relationship.
-            filters_to_apply = JobList._filter_current_job(job,copy.deepcopy(dependency.relationships))
+            filters_to_apply = self._filter_current_job(job, copy.deepcopy(dependency.relationships))
+            if "?" in filters_to_apply.get("SPLITS_TO", "") or "?" in filters_to_apply.get("DATES_TO","") or "?" in filters_to_apply.get("MEMBERS_TO", "") or "?" in filters_to_apply.get("CHUNKS_TO", ""):
+                only_marked_status = True
+            else:
+                only_marked_status = False
+            special_conditions["STATUS"] = filters_to_apply.pop("STATUS", None)
+            special_conditions["FROM_STEP"] = filters_to_apply.pop("FROM_STEP", None)
             for parent in all_parents:
                 # If splits is not None, the job is a list of jobs
                 if parent.name == job.name:
                     continue
                 # Check if it is a natural relation. The only difference is that a chunk can depend on a chunks <= than the current chunk
-                if parent in natural_jobs and (job.chunk is None or parent.chunk is None or parent.chunk <= job.chunk ):
+                if parent in natural_jobs and (job.chunk is None or parent.chunk is None or parent.chunk <= job.chunk):
                     natural_relationship = True
                 else:
                     natural_relationship = False
                 # Check if the current parent is a valid parent based on the dependencies set on expdef.conf
-                valid,optional = JobList._valid_parent(parent, member_list, parsed_date_list, chunk_list, natural_relationship,filters_to_apply)
                 # If the parent is valid, add it to the graph
-                if valid:
+
+                if JobList._valid_parent(parent, member_list, parsed_date_list, chunk_list, natural_relationship,
+                                         filters_to_apply,job):
                     job.add_parent(parent)
-                    JobList._add_edge(graph, job, parent)
+                    self._add_edge(graph, job, parent)
                     # Could be more variables in the future
-                    if optional:
-                        job.add_edge_info(parent.name,special_variables={"optional":True})
+                    # Do parse checkpoint
+                    if special_conditions.get("STATUS", None):
+                        if only_marked_status:
+                            if str(job.split) + "?" in filters_to_apply.get("SPLITS_TO", "") or str(
+                                    job.chunk) + "?" in filters_to_apply.get("CHUNKS_TO", "") or str(
+                                    job.member) + "?" in filters_to_apply.get("MEMBERS_TO", "") or str(
+                                    job.date) + "?" in filters_to_apply.get("DATES_TO", ""):
+                                selected = True
+                            else:
+                                selected = False
+                        else:
+                            selected = True
+                        if selected:
+                            if special_conditions.get("FROM_STEP", None):
+                                job.max_checkpoint_step = int(special_conditions.get("FROM_STEP", 0)) if int(
+                                    special_conditions.get("FROM_STEP",
+                                                           0)) > job.max_checkpoint_step else job.max_checkpoint_step
+                            self._add_edge_info(job, special_conditions["STATUS"])
+                            job.add_edge_info(parent, special_conditions)
             JobList.handle_frequency_interval_dependencies(chunk, chunk_list, date, date_list, dic_jobs, job, member,
                                                            member_list, dependency.section, graph, other_parents)
 
     @staticmethod
     def _calculate_dependency_metadata(chunk, chunk_list, member, member_list, date, date_list, dependency):
         skip = False
         if dependency.sign == '-':
@@ -837,15 +1068,15 @@
                     date = date_list[date_index - dependency.distance]
                 else:
                     skip = True
         return skip, (chunk, member, date)
 
     @staticmethod
     def handle_frequency_interval_dependencies(chunk, chunk_list, date, date_list, dic_jobs, job, member, member_list,
-                                               section_name, graph,visited_parents):
+                                               section_name, graph, visited_parents):
         if job.wait and job.frequency > 1:
             if job.chunk is not None and len(str(job.chunk)) > 0:
                 max_distance = (chunk_list.index(chunk) + 1) % job.frequency
                 if max_distance == 0:
                     max_distance = job.frequency
                 for distance in range(1, max_distance):
                     for parent in dic_jobs.get_jobs(section_name, date, member, chunk - distance):
@@ -880,17 +1111,18 @@
         num_parents = 1
         if isinstance(parents, list):
             num_parents = len(parents)
         for i in range(num_parents):
             parent = parents[i] if isinstance(parents, list) else parents
             graph.add_edge(parent.name, job.name)
             pass
+
     @staticmethod
     def _create_jobs(dic_jobs, priority, default_job_type, jobs_data=dict()):
-        for section in dic_jobs._jobs_data.get("JOBS",{}).keys():
+        for section in dic_jobs._jobs_data.get("JOBS", {}).keys():
             Log.debug("Creating {0} jobs".format(section))
             dic_jobs.read_section(section, priority, default_job_type, jobs_data)
             priority += 1
 
     def _create_sorted_dict_jobs(self, wrapper_jobs):
         """
         Creates a sorting of the jobs whose job.section is in wrapper_jobs, according to the following filters in order of importance:
@@ -899,39 +1131,40 @@
         If the job does not have a chunk number, the total number of chunks configured for the experiment is used.
 
         :param wrapper_jobs: User defined job types in autosubmit_,conf [wrapper] section to be wrapped. \n
         :type wrapper_jobs: String \n
         :return: Sorted Dictionary of List that represents the jobs included in the wrapping process. \n
         :rtype: Dictionary Key: date, Value: (Dictionary Key: Member, Value: List of jobs that belong to the date, member, and are ordered by chunk number if it is a chunk job otherwise num_chunks from JOB TYPE (section)
         """
+
         # Dictionary Key: date, Value: (Dictionary Key: Member, Value: List)
+        job = None
+
         dict_jobs = dict()
         for date in self._date_list:
             dict_jobs[date] = dict()
             for member in self._member_list:
                 dict_jobs[date][member] = list()
         num_chunks = len(self._chunk_list)
 
-
         sections_running_type_map = dict()
         if wrapper_jobs is not None and len(str(wrapper_jobs)) > 0:
             if type(wrapper_jobs) is not list:
                 if "&" in wrapper_jobs:
                     char = "&"
                 else:
                     char = " "
                 wrapper_jobs = wrapper_jobs.split(char)
 
-
             for section in wrapper_jobs:
                 # RUNNING = once, as default. This value comes from jobs_.yml
                 try:
                     sections_running_type_map[section] = str(self.jobs_data[section].get("RUNNING", 'once'))
                 except BaseException as e:
-                    raise AutosubmitCritical("Key {0} doesn't exists.".format(section),7014,str(e))
+                    raise AutosubmitCritical("Key {0} doesn't exists.".format(section), 7014, str(e))
 
             # Select only relevant jobs, those belonging to the sections defined in the wrapper
 
         sections_to_filter = ""
         for section in sections_running_type_map:
             sections_to_filter += section
 
@@ -941,61 +1174,62 @@
             filtered_jobs_list)
 
         for date in self._date_list:
             str_date = self._get_date(date)
             for member in self._member_list:
                 # Filter list of fake jobs according to date and member, result not sorted at this point
                 sorted_jobs_list = list(filter(lambda job: job.name.split("_")[1] == str_date and
-                                          job.name.split("_")[2] == member, filtered_jobs_fake_date_member))
-                #sorted_jobs_list = [job for job in filtered_jobs_fake_date_member if job.name.split("_")[1] == str_date and
+                                                           job.name.split("_")[2] == member,
+                                               filtered_jobs_fake_date_member))
+                # sorted_jobs_list = [job for job in filtered_jobs_fake_date_member if job.name.split("_")[1] == str_date and
                 #                          job.name.split("_")[2] == member]
 
-                #There can be no jobs for this member when select chunk/member is enabled
+                # There can be no jobs for this member when select chunk/member is enabled
                 if not sorted_jobs_list or len(sorted_jobs_list) == 0:
                     continue
 
-
                 previous_job = sorted_jobs_list[0]
 
                 # get RUNNING for this section
                 section_running_type = sections_running_type_map[previous_job.section]
-
                 jobs_to_sort = [previous_job]
                 previous_section_running_type = None
                 # Index starts at 1 because 0 has been taken in a previous step
                 for index in range(1, len(sorted_jobs_list) + 1):
                     # If not last item
                     if index < len(sorted_jobs_list):
                         job = sorted_jobs_list[index]
                         # Test if section has changed. e.g. from INI to SIM
                         if previous_job.section != job.section:
                             previous_section_running_type = section_running_type
                             section_running_type = sections_running_type_map[job.section]
                     # Test if RUNNING is different between sections, or if we have reached the last item in sorted_jobs_list
-                    if (previous_section_running_type is not None and previous_section_running_type != section_running_type) \
+                    if (
+                            previous_section_running_type is not None and previous_section_running_type != section_running_type) \
                             or index == len(sorted_jobs_list):
 
                         # Sorting by date, member, chunk number if it is a chunk job otherwise num_chunks from JOB TYPE (section)
                         # Important to note that the only differentiating factor would be chunk OR num_chunks
                         jobs_to_sort = sorted(jobs_to_sort, key=lambda k: (k.name.split('_')[1], (k.name.split('_')[2]),
                                                                            (int(k.name.split('_')[3])
-                                                                            if len(k.name.split('_')) == 5 else num_chunks + 1)))
+                                                                            if len(k.name.split(
+                                                                               '_')) == 5 else num_chunks + 1)))
 
                         # Bringing back original job if identified
                         for idx in range(0, len(jobs_to_sort)):
                             # Test if it is a fake job
                             if jobs_to_sort[idx] in fake_original_job_map:
                                 fake_job = jobs_to_sort[idx]
                                 # Get original
                                 jobs_to_sort[idx] = fake_original_job_map[fake_job]
                         # Add to result, and reset jobs_to_sort
                         # By adding to the result at this step, only those with the same RUNNING have been added.
                         dict_jobs[date][member] += jobs_to_sort
                         jobs_to_sort = []
-                    if len(sorted_jobs_list) > 1 :
+                    if len(sorted_jobs_list) > 1:
                         jobs_to_sort.append(job)
                         previous_job = job
 
         return dict_jobs
 
     def _create_fake_dates_members(self, filtered_jobs_list):
         """
@@ -1019,15 +1253,15 @@
             if job.date is None and job.member is None:
                 # Declare None values as if they were the last items in corresponding list
                 date = self._date_list[-1]
                 member = self._member_list[-1]
                 fake_job = copy.deepcopy(job)
                 # Use previous values to modify name of fake job
                 fake_job.name = fake_job.name.split('_', 1)[0] + "_" + self._get_date(date) + "_" \
-                    + member + "_" + fake_job.name.split("_", 1)[1]
+                                + member + "_" + fake_job.name.split("_", 1)[1]
                 # Filling list of fake jobs, only difference is the name
                 filtered_jobs_fake_date_member.append(fake_job)
                 # Mapping fake jobs to original ones
                 fake_original_job_map[fake_job] = job
             # running date or synchronize member
             elif job.member is None:
                 # Declare None values as if it were the last items in corresponding list
@@ -1109,15 +1343,16 @@
                 date_format = 'H'
             if date.minute > 1:
                 date_format = 'M'
         return date_format
 
     def copy_ordered_jobs_by_date_member(self):
         pass
-    def get_ordered_jobs_by_date_member(self,section):
+
+    def get_ordered_jobs_by_date_member(self, section):
         """
         Get the dictionary of jobs ordered according to wrapper's expression divided by date and member
 
         :return: jobs ordered divided by date and member
         :rtype: dict
         """
         if len(self._ordered_jobs_by_date_member) > 0:
@@ -1148,15 +1383,16 @@
 
         :param wrapper:
         :param platform: job platform
         :type platform: HPCPlatform
         :return: completed jobs
         :rtype: list
         """
-        uncompleted_jobs = [job for job in self._job_list if (platform is None or job.platform.name == platform.name) and
+        uncompleted_jobs = [job for job in self._job_list if
+                            (platform is None or job.platform.name == platform.name) and
                             job.status != Status.COMPLETED]
 
         if wrapper:
             return [job for job in uncompleted_jobs if job.packed is False]
         else:
             return uncompleted_jobs
 
@@ -1260,15 +1496,16 @@
         :param wrapper:
         :param platform: job platform
         :type platform: HPCPlatform
         :return: all jobs
         :rtype: list
         """
         unsubmitted = [job for job in self._job_list if (platform is None or job.platform.name == platform.name) and
-                       (job.status != Status.SUBMITTED and job.status != Status.QUEUING and job.status == Status.RUNNING and job.status == Status.COMPLETED)]
+                       (
+                                   job.status != Status.SUBMITTED and job.status != Status.QUEUING and job.status == Status.RUNNING and job.status == Status.COMPLETED)]
 
         if wrapper:
             return [job for job in unsubmitted if job.packed is False]
         else:
             return unsubmitted
 
     def get_all(self, platform=None, wrapper=False):
@@ -1284,15 +1521,15 @@
         all_jobs = [job for job in self._job_list]
 
         if wrapper:
             return [job for job in all_jobs if job.packed is False]
         else:
             return all_jobs
 
-    def get_job_names(self,lower_case=False):
+    def get_job_names(self, lower_case=False):
         """
         Returns a list of all job names
         :param: lower_case: if true, returns lower case job names
         :type: lower_case: bool
 
 
         :return: all job names
@@ -1305,29 +1542,32 @@
             all_jobs = [job.name for job in self._job_list]
 
         return all_jobs
 
     def update_two_step_jobs(self):
         prev_jobs_to_run_first = self.jobs_to_run_first
         if len(self.jobs_to_run_first) > 0:
-            self.jobs_to_run_first  = [ job for job in self.jobs_to_run_first if job.status != Status.COMPLETED ]
+            self.jobs_to_run_first = [job for job in self.jobs_to_run_first if job.status != Status.COMPLETED]
             keep_running = False
             for job in self.jobs_to_run_first:
-                running_parents = [parent for parent in job.parents if parent.status != Status.WAITING and parent.status != Status.FAILED ] #job is parent of itself
+                running_parents = [parent for parent in job.parents if
+                                   parent.status != Status.WAITING and parent.status != Status.FAILED]  # job is parent of itself
                 if len(running_parents) == len(job.parents):
                     keep_running = True
             if len(self.jobs_to_run_first) > 0 and keep_running is False:
-                raise AutosubmitCritical("No more jobs to run first, there were still pending jobs but they're unable to run without their parents or there are failed jobs.",7014)
+                raise AutosubmitCritical(
+                    "No more jobs to run first, there were still pending jobs but they're unable to run without their parents or there are failed jobs.",
+                    7014)
 
-    def parse_jobs_by_filter(self, unparsed_jobs,two_step_start = True):
+    def parse_jobs_by_filter(self, unparsed_jobs, two_step_start=True):
         jobs_to_run_first = list()
-        select_jobs_by_name = "" #job_name
-        select_all_jobs_by_section = "" #  all
+        select_jobs_by_name = ""  # job_name
+        select_all_jobs_by_section = ""  # all
         filter_jobs_by_section = ""  # Select, chunk / member
-        if "&" in unparsed_jobs: # If there are explicit jobs add them
+        if "&" in unparsed_jobs:  # If there are explicit jobs add them
             jobs_to_check = unparsed_jobs.split("&")
             select_jobs_by_name = jobs_to_check[0]
             unparsed_jobs = jobs_to_check[1]
         if not ";" in unparsed_jobs:
             if '[':
                 select_all_jobs_by_section = unparsed_jobs
                 filter_jobs_by_section = ""
@@ -1336,60 +1576,70 @@
                 filter_jobs_by_section = unparsed_jbos
         else:
             aux = unparsed_jobs.split(';')
             select_all_jobs_by_section = aux[0]
             filter_jobs_by_section = aux[1]
         if two_step_start:
             try:
-                self.jobs_to_run_first = self.get_job_related(select_jobs_by_name=select_jobs_by_name,select_all_jobs_by_section=select_all_jobs_by_section,filter_jobs_by_section=filter_jobs_by_section)
+                self.jobs_to_run_first = self.get_job_related(select_jobs_by_name=select_jobs_by_name,
+                                                              select_all_jobs_by_section=select_all_jobs_by_section,
+                                                              filter_jobs_by_section=filter_jobs_by_section)
             except Exception as e:
-                raise AutosubmitCritical("Check the {0} format.\nFirst filter is optional ends with '&'.\nSecond filter ends with ';'.\nThird filter must contain '['. ".format(unparsed_jobs))
+                raise AutosubmitCritical(
+                    "Check the {0} format.\nFirst filter is optional ends with '&'.\nSecond filter ends with ';'.\nThird filter must contain '['. ".format(
+                        unparsed_jobs))
         else:
             try:
                 self.rerun_job_list = self.get_job_related(select_jobs_by_name=select_jobs_by_name,
-                                                              select_all_jobs_by_section=select_all_jobs_by_section,
-                                                              filter_jobs_by_section=filter_jobs_by_section,two_step_start=two_step_start)
+                                                           select_all_jobs_by_section=select_all_jobs_by_section,
+                                                           filter_jobs_by_section=filter_jobs_by_section,
+                                                           two_step_start=two_step_start)
             except Exception as e:
                 raise AutosubmitCritical(
                     "Check the {0} format.\nFirst filter is optional ends with '&'.\nSecond filter ends with ';'.\nThird filter must contain '['. ".format(
                         unparsed_jobs))
 
-    def get_job_related(self, select_jobs_by_name="",select_all_jobs_by_section="",filter_jobs_by_section="",two_step_start=True):
+    def get_job_related(self, select_jobs_by_name="", select_all_jobs_by_section="", filter_jobs_by_section="",
+                        two_step_start=True):
         """
         :param two_step_start:
         :param select_jobs_by_name: job name
         :param select_all_jobs_by_section: section name
         :param filter_jobs_by_section: section, date , member? , chunk?
         :return: jobs_list names
         :rtype: list
         """
         ultimate_jobs_list = []
         jobs_filtered = []
         jobs_date = []
         # First Filter {select job by name}
         if select_jobs_by_name != "":
-            jobs_by_name = [ job for job in self._job_list if re.search("(^|[^0-9a-z_])"+job.name.lower()+"([^a-z0-9_]|$)",select_jobs_by_name.lower()) is not None  ]
-            jobs_by_name_no_expid = [job for job in self._job_list if
-                            re.search("(^|[^0-9a-z_])" + job.name.lower()[5:] + "([^a-z0-9_]|$)",
+            jobs_by_name = [job for job in self._job_list if
+                            re.search("(^|[^0-9a-z_])" + job.name.lower() + "([^a-z0-9_]|$)",
                                       select_jobs_by_name.lower()) is not None]
+            jobs_by_name_no_expid = [job for job in self._job_list if
+                                     re.search("(^|[^0-9a-z_])" + job.name.lower()[5:] + "([^a-z0-9_]|$)",
+                                               select_jobs_by_name.lower()) is not None]
             ultimate_jobs_list.extend(jobs_by_name)
             ultimate_jobs_list.extend(jobs_by_name_no_expid)
 
         # Second Filter { select all }
         if select_all_jobs_by_section != "":
-            all_jobs_by_section = [ job for job in self._job_list if re.search("(^|[^0-9a-z_])"+job.section.upper()+"([^a-z0-9_]|$)",select_all_jobs_by_section.upper()) is not None ]
+            all_jobs_by_section = [job for job in self._job_list if
+                                   re.search("(^|[^0-9a-z_])" + job.section.upper() + "([^a-z0-9_]|$)",
+                                             select_all_jobs_by_section.upper()) is not None]
             ultimate_jobs_list.extend(all_jobs_by_section)
         # Third Filter N section { date , member? , chunk?}
         # Section[date[member][chunk]]
         # filter_jobs_by_section="SIM[20[C:000][M:1]],DA[20 21[M:000 001][C:1]]"
         if filter_jobs_by_section != "":
-            section_name=""
-            section_dates=""
-            section_chunks=""
-            section_members=""
+            section_name = ""
+            section_dates = ""
+            section_chunks = ""
+            section_members = ""
             jobs_final = list()
             for complete_filter_by_section in filter_jobs_by_section.split(','):
                 section_list = complete_filter_by_section.split('[')
                 section_name = section_list[0].strip('[]')
                 section_dates = section_list[1].strip('[]')
                 if 'c' in section_list[2].lower():
                     section_chunks = section_list[2].strip('cC:[]')
@@ -1397,28 +1647,35 @@
                     section_members = section_list[2].strip('Mm:[]')
                 if len(section_list) > 3:
                     if 'c' in section_list[3].lower():
                         section_chunks = section_list[3].strip('Cc:[]')
                     elif 'm' in section_list[3].lower():
                         section_members = section_list[3].strip('mM:[]')
 
-
                 if section_name != "":
                     jobs_filtered = [job for job in self._job_list if
-                                           re.search("(^|[^0-9a-z_])" + job.section.upper() + "([^a-z0-9_]|$)",
-                                                     section_name.upper()) is not None]
+                                     re.search("(^|[^0-9a-z_])" + job.section.upper() + "([^a-z0-9_]|$)",
+                                               section_name.upper()) is not None]
                 if section_dates != "":
-                    jobs_date = [ job for job in jobs_filtered if re.search("(^|[^0-9a-z_])" + date2str(job.date, job.date_format) + "([^a-z0-9_]|$)", section_dates.lower()) is not None or job.date is None  ]
+                    jobs_date = [job for job in jobs_filtered if
+                                 re.search("(^|[^0-9a-z_])" + date2str(job.date, job.date_format) + "([^a-z0-9_]|$)",
+                                           section_dates.lower()) is not None or job.date is None]
 
                 if section_chunks != "" or section_members != "":
-                    jobs_final = [job for job in jobs_date if ( section_chunks == "" or re.search("(^|[^0-9a-z_])" + str(job.chunk) + "([^a-z0-9_]|$)",section_chunks)  is not None ) and ( section_members == "" or re.search("(^|[^0-9a-z_])" + str(job.member) + "([^a-z0-9_]|$)",section_members.lower()) is not None  )  ]
+                    jobs_final = [job for job in jobs_date if (
+                                section_chunks == "" or re.search("(^|[^0-9a-z_])" + str(job.chunk) + "([^a-z0-9_]|$)",
+                                                                  section_chunks) is not None) and (
+                                              section_members == "" or re.search(
+                                          "(^|[^0-9a-z_])" + str(job.member) + "([^a-z0-9_]|$)",
+                                          section_members.lower()) is not None)]
                 ultimate_jobs_list.extend(jobs_final)
         # Duplicates out
         ultimate_jobs_list = list(set(ultimate_jobs_list))
-        Log.debug("List of jobs filtered by TWO_STEP_START parameter:\n{0}".format([job.name for job in ultimate_jobs_list]))
+        Log.debug(
+            "List of jobs filtered by TWO_STEP_START parameter:\n{0}".format([job.name for job in ultimate_jobs_list]))
         return ultimate_jobs_list
 
     def get_logs(self):
         """
         Returns a dict of logs by jobs_name jobs
 
         :return: logs
@@ -1448,15 +1705,16 @@
         :param wrapper:
         :param hold:
         :param platform: job platform
         :type platform: HPCPlatform
         :return: ready jobs
         :rtype: list
         """
-        ready = [job for job in self._job_list if ( platform is None or platform == "" or job.platform.name == platform.name )  and
+        ready = [job for job in self._job_list if
+                 (platform is None or platform == "" or job.platform.name == platform.name) and
                  job.status == Status.READY and job.hold is hold]
 
         if wrapper:
             return [job for job in ready if job.packed is False]
         else:
             return ready
 
@@ -1468,26 +1726,28 @@
         :type platform: HPCPlatform
         :return: prepared jobs
         :rtype: list
         """
         prepared = [job for job in self._job_list if (platform is None or job.platform.name == platform.name) and
                     job.status == Status.PREPARED]
         return prepared
+
     def get_delayed(self, platform=None):
         """
         Returns a list of delayed jobs
 
         :param platform: job platform
         :type platform: HPCPlatform
         :return: delayed jobs
         :rtype: list
         """
         delayed = [job for job in self._job_list if (platform is None or job.platform.name == platform.name) and
-                    job.status == Status.DELAYED]
+                   job.status == Status.DELAYED]
         return delayed
+
     def get_skipped(self, platform=None):
         """
         Returns a list of skipped jobs
 
         :param platform: job platform
         :type platform: HPCPlatform
         :return: skipped jobs
@@ -1520,15 +1780,15 @@
         :param platform_type: platform type
         :type platform_type: str
         :return: waiting jobs
         :rtype: list
 
         """
         waiting_jobs = [job for job in self._job_list if (
-            job.platform.type == platform_type and job.status == Status.WAITING)]
+                job.platform.type == platform_type and job.status == Status.WAITING)]
         return waiting_jobs
 
     def get_held_jobs(self, platform=None):
         """
         Returns a list of jobs in the platforms (Held)
 
         :param platform: job platform
@@ -1632,21 +1892,23 @@
         :param platform: job platform
         :type platform: HPCPlatform
         :return: active jobs
         :rtype: list
         """
 
         active = self.get_in_queue(platform) + self.get_ready(
-            platform=platform, hold=True) + self.get_ready(platform=platform, hold=False) + self.get_delayed(platform=platform)
+            platform=platform, hold=True) + self.get_ready(platform=platform, hold=False) + self.get_delayed(
+            platform=platform)
         tmp = [job for job in active if job.hold and not (job.status ==
-               Status.SUBMITTED or job.status == Status.READY or job.status == Status.DELAYED) ]
+                                                          Status.SUBMITTED or job.status == Status.READY or job.status == Status.DELAYED)]
         if len(tmp) == len(active):  # IF only held jobs left without dependencies satisfied
             if len(tmp) != 0 and len(active) != 0:
                 raise AutosubmitCritical(
-                    "Only Held Jobs active. Exiting Autosubmit (TIP: This can happen if suspended or/and Failed jobs are found on the workflow)", 7066)
+                    "Only Held Jobs active. Exiting Autosubmit (TIP: This can happen if suspended or/and Failed jobs are found on the workflow)",
+                    7066)
             active = []
         return active
 
     def get_job_by_name(self, name):
         """
         Returns the job that its name matches parameter name
 
@@ -1654,14 +1916,15 @@
         :type name: str
         :return: found job
         :rtype: job
         """
         for job in self._job_list:
             if job.name == name:
                 return job
+
     def get_jobs_by_section(self, section_list):
         """
         Returns the job that its name matches parameter section
         :parameter section_list: list of sections to look for
         :type section_list: list
         :return: found job
         :rtype: job
@@ -1684,15 +1947,15 @@
             if len(jobs_by_id[job_id]) == 1:
                 jobs_by_id[job_id] = jobs_by_id[job_id][0]
         return jobs_by_id
 
     def get_in_ready_grouped_id(self, platform):
         jobs = []
         [jobs.append(job) for job in jobs if (
-            platform is None or job.platform.name is platform.name)]
+                platform is None or job.platform.name is platform.name)]
 
         jobs_by_id = dict()
         for job in jobs:
             if job.id not in jobs_by_id:
                 jobs_by_id[job.id] = list()
             jobs_by_id[job.id].append(job)
         return jobs_by_id
@@ -1787,46 +2050,46 @@
                 for job in self._base_job_list:
                     if job.name not in job_names:
                         job_list.append(job)
             self.update_status_log()
 
             try:
                 self._persistence.save(self._persistence_path,
-                                       self._persistence_file, self._job_list if self.run_members is None or job_list is None else job_list)
+                                       self._persistence_file,
+                                       self._job_list if self.run_members is None or job_list is None else job_list)
                 pass
             except BaseException as e:
-                raise AutosubmitError(str(e),6040,"Failure while saving the job_list")
+                raise AutosubmitError(str(e), 6040, "Failure while saving the job_list")
         except AutosubmitError as e:
             raise
         except BaseException as e:
-            raise AutosubmitError(str(e),6040,"Unknown failure while saving the job_list")
-
+            raise AutosubmitError(str(e), 6040, "Unknown failure while saving the job_list")
 
     def backup_save(self):
         """
         Persists the job list
         """
         self._persistence.save(self._persistence_path,
                                self._persistence_file + "_backup", self._job_list)
 
     def update_status_log(self):
 
         exp_path = os.path.join(BasicConfig.LOCAL_ROOT_DIR, self.expid)
         tmp_path = os.path.join(exp_path, BasicConfig.LOCAL_TMP_DIR)
         aslogs_path = os.path.join(tmp_path, BasicConfig.LOCAL_ASLOG_DIR)
-        Log.reset_status_file(os.path.join(aslogs_path,"jobs_active_status.log"),"status")
-        Log.reset_status_file(os.path.join(aslogs_path,"jobs_failed_status.log"),"status_failed")
+        Log.reset_status_file(os.path.join(aslogs_path, "jobs_active_status.log"), "status")
+        Log.reset_status_file(os.path.join(aslogs_path, "jobs_failed_status.log"), "status_failed")
         job_list = self.get_completed()[-5:] + self.get_in_queue()
         failed_job_list = self.get_failed()
         if len(job_list) > 0:
             Log.status("\n{0:<35}{1:<15}{2:<15}{3:<20}{4:<15}", "Job Name",
                        "Job Id", "Job Status", "Job Platform", "Job Queue")
         if len(failed_job_list) > 0:
             Log.status_failed("\n{0:<35}{1:<15}{2:<15}{3:<20}{4:<15}", "Job Name",
-                       "Job Id", "Job Status", "Job Platform", "Job Queue")
+                              "Job Id", "Job Status", "Job Platform", "Job Queue")
         for job in job_list:
             if len(job.queue) > 0 and str(job.platform.queue).lower() != "none":
                 queue = job.queue
             elif len(job.platform.queue) > 0 and str(job.platform.queue).lower() != "none":
                 queue = job.platform.queue
             else:
                 queue = job.queue
@@ -1859,16 +2122,18 @@
             output_date = strftime("%Y%m%d_%H%M", now)
             if store_change:
                 move(os.path.join(self._persistence_path, self._update_file),
                      os.path.join(self._persistence_path, self._update_file +
                                   "_" + output_date))
 
     def get_skippable_jobs(self, jobs_in_wrapper):
-        job_list_skip = [job for job in self.get_job_list() if job.skippable == "true" and (job.status == Status.QUEUING or job.status ==
-                                                                                          Status.RUNNING or job.status == Status.COMPLETED or job.status == Status.READY) and jobs_in_wrapper.find(job.section) == -1]
+        job_list_skip = [job for job in self.get_job_list() if
+                         job.skippable == "true" and (job.status == Status.QUEUING or job.status ==
+                                                      Status.RUNNING or job.status == Status.COMPLETED or job.status == Status.READY) and jobs_in_wrapper.find(
+                             job.section) == -1]
         skip_by_section = dict()
         for job in job_list_skip:
             if job.section not in skip_by_section:
                 skip_by_section[job.section] = [job]
             else:
                 skip_by_section[job.section].append(job)
         return skip_by_section
@@ -1882,14 +2147,48 @@
         """
         return self._parameters
 
     @parameters.setter
     def parameters(self, value):
         self._parameters = value
 
+    def check_checkpoint(self, job, parent):
+        """ Check if a checkpoint step exists for this edge"""
+        return job.get_checkpoint_files(parent.name)
+
+    def check_special_status(self):
+        """
+        Check if all parents of a job have the correct status for checkpointing
+        :return: jobs that fullfill the special conditions """
+        jobs_to_check = []
+        for status, sorted_job_list in self.jobs_edges.items():
+            if status == "ALL":
+                continue
+            for job in sorted_job_list:
+                if job.status != Status.WAITING:
+                    continue
+                if status in ["RUNNING", "FAILED"]:
+                    # check checkpoint if any
+                    if job.platform.connected:  # This will be true only when used under setstatus/run
+                        job.get_checkpoint_files()
+                non_completed_parents_current = 0
+                completed_parents = len([parent for parent in job.parents if parent.status == Status.COMPLETED])
+                for parent in job.edge_info[status].values():
+                    if status in ["RUNNING", "FAILED"] and parent[1] and int(parent[1]) >= job.current_checkpoint_step:
+                        continue
+                    else:
+                        status_str = Status.VALUE_TO_KEY[parent[0].status]
+                        if Status.LOGICAL_ORDER.index(status_str) >= Status.LOGICAL_ORDER.index(status):
+                            non_completed_parents_current += 1
+                if ( non_completed_parents_current + completed_parents ) == len(job.parents):
+                    jobs_to_check.append(job)
+
+        return jobs_to_check
+
+
     def update_list(self, as_conf, store_change=True, fromSetStatus=False, submitter=None, first_time=False):
         # type: (AutosubmitConfig, bool, bool, object, bool) -> bool
         """
         Updates job list, resetting failed jobs and changing to READY all WAITING jobs with all parents COMPLETED
 
         :param first_time:
         :param submitter:
@@ -1904,37 +2203,37 @@
         save = False
         if self.update_from_file(store_change):
             save = store_change
         Log.debug('Updating FAILED jobs')
         write_log_status = False
         if not first_time:
             for job in self.get_failed():
-                if self.jobs_data[job.section].get("RETRIALS",None) is None:
+                if self.jobs_data[job.section].get("RETRIALS", None) is None:
                     retrials = int(as_conf.get_retrials())
                 else:
                     retrials = int(job.retrials)
                 if job.fail_count < retrials:
                     job.inc_fail_count()
                     tmp = [
                         parent for parent in job.parents if parent.status == Status.COMPLETED]
                     if len(tmp) == len(job.parents):
                         if "+" == str(job.delay_retrials)[0] or "*" == str(job.delay_retrials)[0]:
                             aux_job_delay = int(job.delay_retrials[1:])
                         else:
                             aux_job_delay = int(job.delay_retrials)
 
-                        if self.jobs_data[job.section].get("DELAY_RETRY_TIME",None) or aux_job_delay <= 0:
+                        if self.jobs_data[job.section].get("DELAY_RETRY_TIME", None) or aux_job_delay <= 0:
                             delay_retry_time = str(as_conf.get_delay_retry_time())
                         else:
                             delay_retry_time = job.retry_delay
                         if "+" in delay_retry_time:
                             retry_delay = job.fail_count * int(delay_retry_time[:-1]) + int(delay_retry_time[:-1])
                         elif "*" in delay_retry_time:
                             retry_delay = int(delay_retry_time[1:])
-                            for retrial_amount in range(0,job.fail_count):
+                            for retrial_amount in range(0, job.fail_count):
                                 retry_delay += retry_delay * 10
                         else:
                             retry_delay = int(delay_retry_time)
                         if retry_delay > 0:
                             job.status = Status.DELAYED
                             job.delay_end = datetime.datetime.now() + datetime.timedelta(seconds=retry_delay)
                             Log.debug(
@@ -1953,14 +2252,22 @@
                         job.packed = False
                         Log.debug(
                             "Resetting job: {0} status to: WAITING for parents completion...".format(job.name))
                 else:
                     job.status = Status.FAILED
                     job.packed = False
                     save = True
+        # Check checkpoint jobs, the status can be Any
+        for job in self.check_special_status():
+            job.status = Status.READY
+            job.id = None
+            job.packed = False
+            job.wrapper_type = None
+            save = True
+            Log.debug(f"Special condition fullfilled for job {job.name}")
         # if waiting jobs has all parents completed change its State to READY
         for job in self.get_completed():
             if job.synchronize is not None and len(str(job.synchronize)) > 0:
                 tmp = [parent for parent in job.parents if parent.status == Status.COMPLETED]
                 if len(tmp) != len(job.parents):
                     tmp2 = [parent for parent in job.parents if
                             parent.status == Status.COMPLETED or parent.status == Status.SKIPPED or parent.status == Status.FAILED]
@@ -1975,26 +2282,27 @@
                                 break
                     else:
                         job.status = Status.WAITING
                         save = True
                         Log.debug(
                             "Resetting sync job: {0} status to: WAITING for parents completion...".format(
                                 job.name))
-
-
         Log.debug('Updating WAITING jobs')
         if not fromSetStatus:
             all_parents_completed = []
             for job in self.get_delayed():
                 if datetime.datetime.now() >= job.delay_end:
                     job.status = Status.READY
             for job in self.get_waiting():
-                tmp = [parent for parent in job.parents if parent.status == Status.COMPLETED or parent.status == Status.SKIPPED]
-                tmp2 = [parent for parent in job.parents if parent.status == Status.COMPLETED or parent.status == Status.SKIPPED or parent.status == Status.FAILED]
-                tmp3 = [parent for parent in job.parents if parent.status == Status.SKIPPED or parent.status == Status.FAILED]
+                tmp = [parent for parent in job.parents if
+                       parent.status == Status.COMPLETED or parent.status == Status.SKIPPED]
+                tmp2 = [parent for parent in job.parents if
+                        parent.status == Status.COMPLETED or parent.status == Status.SKIPPED or parent.status == Status.FAILED]
+                tmp3 = [parent for parent in job.parents if
+                        parent.status == Status.SKIPPED or parent.status == Status.FAILED]
                 failed_ones = [parent for parent in job.parents if parent.status == Status.FAILED]
                 if job.parents is None or len(tmp) == len(job.parents):
                     job.status = Status.READY
                     job.hold = False
                     Log.debug(
                         "Setting job: {0} status to: READY (all parents completed)...".format(job.name))
                     if as_conf.get_remote_dependencies() == "true":
@@ -2004,22 +2312,23 @@
                         if len(tmp2) == len(job.parents):
                             strong_dependencies_failure = False
                             weak_dependencies_failure = False
                             for parent in failed_ones:
                                 if parent.name in job.edge_info and job.edge_info[parent.name].get('optional', False):
                                     weak_dependencies_failure = True
                                 elif parent.section in job.dependencies:
-                                    if parent.status not in [Status.COMPLETED,Status.SKIPPED]:
+                                    if parent.status not in [Status.COMPLETED, Status.SKIPPED]:
                                         strong_dependencies_failure = True
                                     break
                             if not strong_dependencies_failure and weak_dependencies_failure:
                                 job.status = Status.READY
                                 job.hold = False
                                 Log.debug(
-                                    "Setting job: {0} status to: READY (conditional jobs are completed/failed)...".format(job.name))
+                                    "Setting job: {0} status to: READY (conditional jobs are completed/failed)...".format(
+                                        job.name))
                                 break
                             if as_conf.get_remote_dependencies() == "true":
                                 all_parents_completed.append(job.name)
                     else:
                         if len(tmp3) == 1 and len(job.parents) == 1:
                             for parent in job.parents:
                                 if parent.name in job.edge_info and job.edge_info[parent.name].get('optional', False):
@@ -2039,31 +2348,34 @@
                             parent.status == Status.SKIPPED or parent.status == Status.FAILED]
                     if len(tmp2) == len(job.parents) and len(tmp3) != len(job.parents):
                         job.status = Status.READY
                         job.packed = False
                         job.hold = False
                         save = True
                         Log.debug(
-                            "A job in prepared status has all parent completed, job: {0} status set to: READY ...".format(job.name))
+                            "A job in prepared status has all parent completed, job: {0} status set to: READY ...".format(
+                                job.name))
                 Log.debug('Updating WAITING jobs eligible for be prepared')
                 # Setup job name should be a variable
                 for job in self.get_waiting_remote_dependencies('slurm'):
                     if job.name not in all_parents_completed:
                         tmp = [parent for parent in job.parents if (
-                            (parent.status == Status.SKIPPED or parent.status == Status.COMPLETED or parent.status == Status.QUEUING or parent.status == Status.RUNNING) and "setup" not in parent.name.lower())]
+                                (
+                                            parent.status == Status.SKIPPED or parent.status == Status.COMPLETED or parent.status == Status.QUEUING or parent.status == Status.RUNNING) and "setup" not in parent.name.lower())]
                         if len(tmp) == len(job.parents):
                             job.status = Status.PREPARED
                             job.hold = True
                             Log.debug(
-                                "Setting job: {0} status to: Prepared for be held (all parents queuing, running or completed)...".format(job.name))
+                                "Setting job: {0} status to: Prepared for be held (all parents queuing, running or completed)...".format(
+                                    job.name))
 
                 Log.debug('Updating Held jobs')
                 if self.job_package_map:
                     held_jobs = [job for job in self.get_held_jobs() if (
-                        job.id not in list(self.job_package_map.keys()))]
+                            job.id not in list(self.job_package_map.keys()))]
                     held_jobs += [wrapper_job for wrapper_job in list(self.job_package_map.values())
                                   if wrapper_job.status == Status.HELD]
                 else:
                     held_jobs = self.get_held_jobs()
 
                 for job in held_jobs:
                     if self.job_package_map and job.id in list(self.job_package_map.keys()):  # Wrappers and inner jobs
@@ -2074,23 +2386,23 @@
                             tmp = [
                                 parent for parent in valid_parents if parent.status == Status.COMPLETED]
                             if len(tmp) < len(valid_parents):
                                 hold_wrapper = True
                         job.hold = hold_wrapper
                         if not job.hold:
                             for inner_job in job.job_list:
-                                inner_job.hold = False                                                               
+                                inner_job.hold = False
                             Log.debug(
                                 "Setting job: {0} status to: Queuing (all parents completed)...".format(
                                     job.name))
                     else:  # Non-wrapped jobs
                         tmp = [
                             parent for parent in job.parents if parent.status == Status.COMPLETED]
                         if len(tmp) == len(job.parents):
-                            job.hold = False                                                    
+                            job.hold = False
                             Log.debug(
                                 "Setting job: {0} status to: Queuing (all parents completed)...".format(
                                     job.name))
                         else:
                             job.hold = True
             jobs_to_skip = self.get_skippable_jobs(
                 as_conf.get_wrapper_jobs())  # Get A Dict with all jobs that are listed as skippable
@@ -2114,24 +2426,24 @@
                                     job.status = Status.SKIPPED
                                     save = True
                         elif job.running == 'member':
                             members = as_conf.get_member_list()
                             for related_job in jobs_to_skip[section]:
                                 if members.index(job.member) < members.index(
                                         related_job.member) and job.chunk == related_job.chunk and jobdate == date2str(
-                                        related_job.date, related_job.date_format):
+                                    related_job.date, related_job.date_format):
                                     try:
                                         if job.status == Status.QUEUING:
                                             job.platform.send_command(job.platform.cancel_cmd + " " + str(job.id),
                                                                       ignore_log=True)
                                     except Exception as e:
                                         pass  # job_id finished already
                                     job.status = Status.SKIPPED
                                     save = True
-            #save = True
+            # save = True
         self.update_two_step_jobs()
         Log.debug('Update finished')
         return save
 
     def update_genealogy(self, new=True, notransitive=False, update_structure=False):
         """
         When we have created the job list, every type of job is created.
@@ -2172,15 +2484,16 @@
             if (current_structure) and (len(self._job_list) == len(current_structure)) and update_structure is False:
                 structure_valid = True
                 # Further validation
                 # Structure exists and is valid, use it as a source of dependencies
                 if m_time_job_conf:
                     if m_time_job_conf > m_time_db:
                         Log.info(
-                            "File jobs_{0}.yml has been modified since the last time the structure persistence was saved.".format(self.expid))
+                            "File jobs_{0}.yml has been modified since the last time the structure persistence was saved.".format(
+                                self.expid))
                         structure_valid = False
                 else:
                     Log.info(
                         "File jobs_{0}.yml was not found.".format(self.expid))
 
                 if structure_valid is True:
                     for job in self._job_list:
@@ -2195,15 +2508,15 @@
                             child for child in job.children if child.name not in current_structure[job.name]]
                         for child in children_to_remove:
                             job.children.remove(child)
                             child.parents.remove(job)
             if structure_valid is False:
                 # Structure does not exist, or it is not be updated, attempt to create it.
                 Log.info("Updating structure persistence...")
-                self.graph = transitive_reduction(self.graph) # add threads for large experiments? todo
+                self.graph = transitive_reduction(self.graph)  # add threads for large experiments? todo
                 if self.graph:
                     for job in self._job_list:
                         children_to_remove = [
                             child for child in job.children if child.name not in self.graph.neighbors(job.name)]
                         for child in children_to_remove:
                             job.children.remove(child)
                             child.parents.remove(job)
@@ -2231,29 +2544,31 @@
         out = True
         for job in self._job_list:
             show_logs = job.check_warnings
             if not job.check_script(as_conf, self.parameters, show_logs):
                 out = False
         return out
 
-    def save_wrappers(self,packages_to_save,failed_packages,as_conf,packages_persistence,hold=False,inspect=False):
+    def save_wrappers(self, packages_to_save, failed_packages, as_conf, packages_persistence, hold=False,
+                      inspect=False):
         for package in packages_to_save:
             if package.jobs[0].id not in failed_packages:
                 if hasattr(package, "name"):
                     self.packages_dict[package.name] = package.jobs
                     from ..job.job import WrapperJob
                     wrapper_job = WrapperJob(package.name, package.jobs[0].id, Status.SUBMITTED, 0,
                                              package.jobs,
                                              package._wallclock, package._num_processors,
                                              package.platform, as_conf, hold)
                     self.job_package_map[package.jobs[0].id] = wrapper_job
                     if isinstance(package, JobPackageThread):
                         # Saving only when it is a real multi job package
                         packages_persistence.save(
                             package.name, package.jobs, package._expid, inspect)
+
     def check_scripts(self, as_conf):
         """
         When we have created the scripts, all parameters should have been substituted.
         %PARAMETER% handlers not allowed
 
         :param as_conf: experiment configuration
         :type as_conf: AutosubmitConfig
@@ -2303,26 +2618,26 @@
             child.delete_parent(job)
 
         for parent in job.parents:
             parent.children.remove(job)
 
         self._job_list.remove(job)
 
-    def rerun(self, job_list_unparsed,as_conf, monitor=False):
+    def rerun(self, job_list_unparsed, as_conf, monitor=False):
         """
         Updates job list to rerun the jobs specified by a job list
         :param job_list_unparsed: list of jobs to rerun
         :type job_list_unparsed: str
         :param as_conf: experiment configuration
         :type as_conf: AutosubmitConfig
         :param monitor: if True, the job list will be monitored
         :type monitor: bool
 
         """
-        self.parse_jobs_by_filter(job_list_unparsed,two_step_start=False)
+        self.parse_jobs_by_filter(job_list_unparsed, two_step_start=False)
         member_list = set()
         chunk_list = set()
         date_list = set()
         job_sections = set()
         for job in self.get_all():
             if not monitor:
                 job.status = Status.COMPLETED
@@ -2343,29 +2658,34 @@
         self._date_list = list(date_list)
         Log.info("Adding dependencies...")
         dependencies = dict()
 
         for job_section in job_sections:
             Log.debug(
                 "Reading rerun dependencies for {0} jobs".format(job_section))
-            if as_conf.jobs_data[job_section].get('DEPENDENCIES',None) is not None:
-                dependencies_keys = as_conf.jobs_data[job_section].get('DEPENDENCIES',{})
+            if as_conf.jobs_data[job_section].get('DEPENDENCIES', None) is not None:
+                dependencies_keys = as_conf.jobs_data[job_section].get('DEPENDENCIES', {})
                 if type(dependencies_keys) is str:
                     dependencies_keys = dependencies_keys.upper().split()
                 if dependencies_keys is None:
                     dependencies_keys = []
                 dependencies = JobList._manage_dependencies(dependencies_keys, self._dic_jobs, job_section)
                 for job in self.get_jobs_by_section(job_section):
                     for key in dependencies_keys:
                         dependency = dependencies[key]
-                        skip, (chunk, member, date) = JobList._calculate_dependency_metadata(job.chunk, self._chunk_list, job.member, self._member_list, job.date, self._date_list, dependency)
+                        skip, (chunk, member, date) = JobList._calculate_dependency_metadata(job.chunk,
+                                                                                             self._chunk_list,
+                                                                                             job.member,
+                                                                                             self._member_list,
+                                                                                             job.date, self._date_list,
+                                                                                             dependency)
                         if skip:
                             continue
                         section_name = dependencies[key].section
-                        for parent in self._dic_jobs.get_jobs(section_name, job.date, job.member,job.chunk):
+                        for parent in self._dic_jobs.get_jobs(section_name, job.date, job.member, job.chunk):
                             if not monitor:
                                 parent.status = Status.WAITING
                             Log.debug("Parent: " + parent.name)
 
     def _get_jobs_parser(self):
         jobs_parser = self._parser_factory.create_parser()
         jobs_parser.optionxform = str
@@ -2401,29 +2721,30 @@
         :return: String representation
         :rtype: String
         """
         # nocolor = True
         allJobs = self.get_all() if existingList is None else existingList
         # Header
         result = (bcolors.BOLD if nocolor is False else '') + \
-            "## String representation of Job List [" + str(len(allJobs)) + "] "
+                 "## String representation of Job List [" + str(len(allJobs)) + "] "
         if statusChange is not None and len(str(statusChange)) > 0:
             result += "with " + (bcolors.OKGREEN if nocolor is False else '') + str(len(list(statusChange.keys()))
-                                                                                    ) + " Change(s) ##" + (bcolors.ENDC + bcolors.ENDC if nocolor is False else '')
+                                                                                    ) + " Change(s) ##" + (
+                          bcolors.ENDC + bcolors.ENDC if nocolor is False else '')
         else:
             result += " ## "
 
         # Find root
         root = None
         roots = []
         for job in allJobs:
             if len(job.parents) == 0:
                 roots.append(job)
         visited = list()
-        #print(root)
+        # print(root)
         # root exists
         for root in roots:
             if root is not None and len(str(root)) > 0:
                 result += self._recursion_print(root, 0, visited,
                                                 statusChange=statusChange, nocolor=nocolor)
             else:
                 result += "\nCannot find root."
@@ -2476,25 +2797,25 @@
         if job.name not in visited:
             visited.append(job.name)
             prefix = ""
             for i in range(level):
                 prefix += "|  "
             # Prefix + Job Name
             result = "\n" + prefix + \
-                (bcolors.BOLD + bcolors.CODE_TO_COLOR[job.status] if nocolor is False else '') + \
-                job.name + \
-                (bcolors.ENDC + bcolors.ENDC if nocolor is False else '')
+                     (bcolors.BOLD + bcolors.CODE_TO_COLOR[job.status] if nocolor is False else '') + \
+                     job.name + \
+                     (bcolors.ENDC + bcolors.ENDC if nocolor is False else '')
             if len(job._children) > 0:
                 level += 1
                 children = job._children
                 total_children = len(job._children)
                 # Writes children number and status if color are not being showed
                 result += " ~ [" + str(total_children) + (" children] " if total_children > 1 else " child] ") + \
-                    ("[" + Status.VALUE_TO_KEY[job.status] +
-                     "] " if nocolor is True else "")
+                          ("[" + Status.VALUE_TO_KEY[job.status] +
+                           "] " if nocolor is True else "")
                 if statusChange is not None and len(str(statusChange)) > 0:
                     # Writes change if performed
                     result += (bcolors.BOLD +
                                bcolors.OKGREEN if nocolor is False else '')
                     result += (statusChange[job.name]
                                if job.name in statusChange else "")
                     result += (bcolors.ENDC +
@@ -2505,15 +2826,15 @@
                     result += self._recursion_print(
                         child, level, visited, statusChange=statusChange, nocolor=nocolor)
             else:
                 result += (" [" + Status.VALUE_TO_KEY[job.status] +
                            "] " if nocolor is True else "")
 
         return result
-    
+
     @staticmethod
     def retrieve_packages(BasicConfig, expid, current_jobs=None):
         """
         Retrieves dictionaries that map the collection of packages in the experiment
 
         :param BasicConfig: Basic configuration 
         :type BasicConfig: Configuration Object
@@ -2570,15 +2891,16 @@
                         package_to_symbol[list_packages[i]] = 'hexagon'
             except Exception as ex:
                 print((traceback.format_exc()))
 
         return job_to_package, package_to_jobs, package_to_package_id, package_to_symbol
 
     @staticmethod
-    def retrieve_times(status_code, name, tmp_path, make_exception=False, job_times=None, seconds=False, job_data_collection=None):
+    def retrieve_times(status_code, name, tmp_path, make_exception=False, job_times=None, seconds=False,
+                       job_data_collection=None):
         """
         Retrieve job timestamps from database.  
         :param job_data_collection:
         :param seconds:
         :param status_code: Code of the Status of the job
         :type status_code: Integer  
         :param name: Name of the job  
@@ -2631,31 +2953,34 @@
                         else:
                             queue_time = job_data.queuing_time()
                             running_time = job_data.running_time()
 
                         if status_code in [Status.SUSPENDED]:
                             t_submit = t_start = t_finish = 0
 
-                        return JobRow(job_data.job_name, int(queue_time), int(running_time), status, energy, JobList.ts_to_datetime(t_submit), JobList.ts_to_datetime(t_start), JobList.ts_to_datetime(t_finish), job_data.ncpus, job_data.run_id)
+                        return JobRow(job_data.job_name, int(queue_time), int(running_time), status, energy,
+                                      JobList.ts_to_datetime(t_submit), JobList.ts_to_datetime(t_start),
+                                      JobList.ts_to_datetime(t_finish), job_data.ncpus, job_data.run_id)
 
             # Using standard procedure
-            if status_code in [Status.RUNNING, Status.SUBMITTED, Status.QUEUING, Status.FAILED] or make_exception is True:
+            if status_code in [Status.RUNNING, Status.SUBMITTED, Status.QUEUING,
+                               Status.FAILED] or make_exception is True:
                 # COMPLETED adds too much overhead so these values are now stored in a database and retrieved separately
                 submit_time, start_time, finish_time, status = JobList._job_running_check(
                     status_code, name, tmp_path)
                 if status_code in [Status.RUNNING, Status.FAILED]:
                     running_for_min = (finish_time - start_time)
                     queuing_for_min = (start_time - submit_time)
                     submit_time = mktime(submit_time.timetuple())
                     start_time = mktime(start_time.timetuple())
                     finish_time = mktime(finish_time.timetuple()) if status_code in [
                         Status.FAILED] else 0
                 else:
                     queuing_for_min = (
-                        datetime.datetime.now() - submit_time)
+                            datetime.datetime.now() - submit_time)
                     running_for_min = datetime.datetime.now() - datetime.datetime.now()
                     submit_time = mktime(submit_time.timetuple())
                     start_time = 0
                     finish_time = 0
 
                 submit_time = int(submit_time)
                 start_time = int(start_time)
@@ -2681,37 +3006,37 @@
                     finish_time = 0
 
         except Exception as exp:
             print((traceback.format_exc()))
             return
 
         seconds_queued = seconds_queued * \
-            (-1) if seconds_queued < 0 else seconds_queued
+                         (-1) if seconds_queued < 0 else seconds_queued
         seconds_running = seconds_running * \
-            (-1) if seconds_running < 0 else seconds_running
+                          (-1) if seconds_running < 0 else seconds_running
         if seconds is False:
             queue_time = math.ceil(
                 seconds_queued / 60) if seconds_queued > 0 else 0
             running_time = math.ceil(
                 seconds_running / 60) if seconds_running > 0 else 0
         else:
             queue_time = seconds_queued
             running_time = seconds_running
 
-        return JobRow(name, 
-                    int(queue_time), 
-                    int(running_time), 
-                    status, 
-                    energy, 
-                    JobList.ts_to_datetime(submit_time), 
-                    JobList.ts_to_datetime(start_time), 
-                    JobList.ts_to_datetime(finish_time), 
-                    0,
-                    0)
-    
+        return JobRow(name,
+                      int(queue_time),
+                      int(running_time),
+                      status,
+                      energy,
+                      JobList.ts_to_datetime(submit_time),
+                      JobList.ts_to_datetime(start_time),
+                      JobList.ts_to_datetime(finish_time),
+                      0,
+                      0)
+
     @staticmethod
     def _job_running_check(status_code, name, tmp_path):
         """
         Receives job data and returns the data from its TOTAL_STATS file in an ordered way.  
         :param status_code: Status of job  
         :type status_code: Integer  
         :param name: Name of job  
@@ -2774,16 +3099,16 @@
 
         current_status = values[3] if (len(values) > 3 and len(
             values[3]) != 14) else status_from_job
         # TOTAL_STATS last line has more than 3 items, status is different from pkl, and status is not "NA"
         if len(values) > 3 and current_status != status_from_job and current_status != "NA":
             current_status = "SUSPICIOUS"
         return submit_time, start_time, finish_time, current_status
-    
+
     @staticmethod
     def ts_to_datetime(timestamp):
         if timestamp and timestamp > 0:
             # print(datetime.datetime.utcfromtimestamp(
             #     timestamp).strftime('%Y-%m-%d %H:%M:%S'))
             return datetime.datetime.fromtimestamp(timestamp).strftime('%Y-%m-%d %H:%M:%S')
         else:
-            return None
+            return None
```

### Comparing `autosubmit-4.0.84/autosubmit/job/job_list_persistence.py` & `autosubmit-4.0.85/autosubmit/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job_package_persistence.py` & `autosubmit-4.0.85/autosubmit/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job_packager.py` & `autosubmit-4.0.85/autosubmit/job/job_packager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/job/job_packages.py` & `autosubmit-4.0.85/autosubmit/job/job_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
 
-
+import json
 import os
 import random
 import time
 from datetime import timedelta
 
 from autosubmit.job.job_common import Status
 from log.log import Log, AutosubmitCritical
@@ -389,16 +389,21 @@
         if not hasattr(self,"_num_processors"):
             self._num_processors = '0'
         self._jobs_resources = jobs_resources
         self._wrapper_factory = self.platform.wrapper
         self.current_wrapper_section = wrapper_section
         self.inner_retrials = 0
         if configuration is not None:
-            self.inner_retrials = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("INNER_RETRIALS",configuration.get_retrials())
-
+            self.inner_retrials = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,
+                                                                                {}).get("RETRIALS",
+                                                                                        configuration.get_retrials())
+            if self.inner_retrials == 0:
+                self.inner_retrials = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,
+                                                                                    {}).get("INNER_RETRIALS",
+                                                                                            configuration.get_retrials())
             self.export = configuration.get_wrapper_export(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
             if self.export.lower() != "none" and len(self.export) > 0:
                 for job in self.jobs:
                     if job.export.lower() != "none" and len(job.export) > 0:
                         self.export = job.export
                         break
             wr_queue = configuration.get_wrapper_queue(configuration.experiment_data["WRAPPERS"][self.current_wrapper_section])
@@ -413,14 +418,34 @@
                 self.partition = jobs[0].partition
             wr_exclusive = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXCLUSIVE",None)
             if wr_exclusive is not None:
                 self.exclusive = wr_exclusive
             else:
                 self.exclusive = jobs[0].exclusive
             wr_custom_directives = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("CUSTOM_DIRECTIVES",[])
+            # parse custom_directives
+            if type(wr_custom_directives) is list:
+                wr_custom_directives = json.dumps(wr_custom_directives)
+            wr_custom_directives = wr_custom_directives.replace("\'", "\"").strip("[]").strip(", ")
+            if wr_custom_directives == '':
+                if jobs[0].custom_directives is None:
+                    jobs[0].custom_directives = ''
+                wr_custom_directives = jobs[0].custom_directives
+                if type(wr_custom_directives) is list:
+                    wr_custom_directives = json.dumps(wr_custom_directives)
+                wr_custom_directives = wr_custom_directives.replace("\'", "\"").strip("[]").strip(", ")
+            if wr_custom_directives != '':
+                if wr_custom_directives[0] != "\"":
+                    wr_custom_directives = "\""+wr_custom_directives
+                if wr_custom_directives[-1] != "\"":
+                    wr_custom_directives = wr_custom_directives+"\""
+                wr_custom_directives = "[" + wr_custom_directives + "]"
+                wr_custom_directives = json.loads(wr_custom_directives)
+            else:
+                wr_custom_directives = []
             if len(str(wr_custom_directives)) > 0:
                 self.custom_directives = wr_custom_directives
             else:
                 self.custom_directives = jobs[0].custom_directives
             wr_executable = configuration.experiment_data["WRAPPERS"].get(self.current_wrapper_section,{}).get("EXECUTABLE",None)
             if wr_executable:
                 self.executable = wr_executable
@@ -448,14 +473,15 @@
             self.tasks = jobs[0].tasks
             self.threads = jobs[0].threads
         self.method = method
         self._wrapper_data = configuration.experiment_data["WRAPPERS"][self.current_wrapper_section]
         self._wrapper_data["TYPE"] = self.wrapper_type
         self._wrapper_data["WRAPPER_POLICY"] = self.wrapper_policy
         self._wrapper_data["INNER_RETRIALS"] = self.inner_retrials
+        self._wrapper_data["RETRIALS"] = self.inner_retrials
         self._wrapper_data["EXTEND_WALLCLOCK"] = self.extensible_wallclock
         self._wrapper_data["METHOD"] = self.wrapper_method
         self._wrapper_data["EXPORT"] = self.export
         self._wrapper_data["QUEUE"] = self.queue
         self._wrapper_data["NODES"] = self.nodes
         self._wrapper_data["TASKS"] = self.tasks
         self._wrapper_data["THREADS"] = self.threads
```

### Comparing `autosubmit-4.0.84/autosubmit/job/job_utils.py` & `autosubmit-4.0.85/autosubmit/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/monitor/diagram.py` & `autosubmit-4.0.85/autosubmit/monitor/diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 
-import traceback
-import numpy as np
 import matplotlib as mtp
+import numpy as np
+import traceback
 
 mtp.use('Agg')
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 import matplotlib.patches as mpatches
 # from autosubmit.experiment.statistics import ExperimentStats
 from autosubmit.statistics.statistics import Statistics
 from autosubmit.job.job import Job
 from log.log import Log, AutosubmitCritical
 from datetime import datetime
-from typing import Dict, List
+from typing import List
 
 Log.get_logger("Autosubmit")
 
 # Autosubmit stats constants
 RATIO = 4
 MAX_JOBS_PER_PLOT = 12.0
 MAX_NUM_PLOTS = 40
 
 
+
 def create_bar_diagram(experiment_id, jobs_list, general_stats, output_file, period_ini=None, period_fi=None,
                        queue_time_fixes=None):
     # type: (str, List[Job], List[str], str, datetime, datetime, Dict[str, int]) -> None
     """
     Creates a bar diagram of the statistics.
 
     :param queue_time_fixes:
@@ -82,126 +83,131 @@
 
     # Plotting
     total_plots_count = normal_plots_count + failed_jobs_plots_count
     # num_plots = norma 
     # ind = np.arrange(int(MAX_JOBS_PER_PLOT))
     width = 0.16
     # Creating stats figure + sanity check
+    plot = True
+    err_message = "The results are too large to be shown, try narrowing your query.\nUse a filter like -ft where you supply a list of job types, e.g. INI, SIM or use the flag -fp where you supply an integer that represents the number of hours into the past that should be queried:\nSuppose it is noon, if you supply -fp 5 the query will consider changes starting from 7:00 am. If you really wish to query the whole experiment, refer to Autosubmit GUI."
     if total_plots_count > MAX_NUM_PLOTS:
-        message = "The results are too large to be shown, try narrowing your query. \n Use a filter like -ft where you supply a list of job types, e.g. INI, SIM; \
-        or -fp where you supply an integer that represents the number of hours into the past that should be queried: \
-        suppose it is noon, if you supply -fp 5 the query will consider changes starting from 7:00 am. If you really wish to query the whole experiment, refer to Autosubmit GUI."
-        Log.info(message)
-        raise AutosubmitCritical("Stats query out of bounds", 7061, message)
-
-    fig = plt.figure(figsize=(RATIO * 4, 3 * RATIO * total_plots_count))
-
-    fig.suptitle('STATS - ' + experiment_id, fontsize=24, fontweight='bold')
-    # Variables initialization
-    ax, ax2 = [], []
-    rects = [None] * 5
-    # print("Normal plots: {}".format(normal_plots_count))
-    # print("Failed jobs plots: {}".format(failed_jobs_plots_count))
-    # print("Total plots: {}".format(total_plots_count))
-    grid_spec = gridspec.GridSpec(RATIO * total_plots_count + 2, 1)
-    i_plot = 0
-    for plot in range(1, normal_plots_count + 1):
-        try:
-            # Calculating jobs inside the given plot
-            l1 = int((plot - 1) * MAX_JOBS_PER_PLOT)
-            l2 = min(int(plot * MAX_JOBS_PER_PLOT), len(exp_stats.jobs_stat))
-            if l2 - l1 <= 0:
-                continue
-            ind = np.arange(l2 - l1)
-            # Building plot axis
-            ax.append(fig.add_subplot(grid_spec[RATIO * plot - RATIO + 2:RATIO * plot + 1]))
-            ax[plot - 1].set_ylabel('hours')
-            ax[plot - 1].set_xticks(ind + width)
-            ax[plot - 1].set_xticklabels(
-                [job.name for job in jobs_list[l1:l2]], rotation='vertical')
-            ax[plot - 1].set_title(experiment_id, fontsize=20)
-            upper_limit = round(1.10 * exp_stats.max_time, 4)
-            ax[plot - 1].set_yticks(np.arange(0, upper_limit, round(upper_limit / 10, 4)))
-            ax[plot - 1].set_ylim(0, float(1.10 * exp_stats.max_time))
-            # Building reacts
-            rects[0] = ax[plot - 1].bar(ind, exp_stats.queued[l1:l2], width, color='lightpink')
-            rects[1] = ax[plot - 1].bar(ind + width, exp_stats.run[l1:l2], width, color='green')
-            rects[2] = ax[plot - 1].bar(ind + width * 3, exp_stats.fail_queued[l1:l2], width, color='lightsalmon')
-            rects[3] = ax[plot - 1].bar(ind + width * 4, exp_stats.fail_run[l1:l2], width, color='salmon')
-            rects[4] = ax[plot - 1].plot([0., width * 6 * MAX_JOBS_PER_PLOT],
-                                         [exp_stats.threshold, exp_stats.threshold], "k--", label='wallclock sim')
-            i_plot = plot
-        except Exception as exp:
-            print((traceback.format_exc()))
-            print(exp)
+        Log.info(err_message)
+        plot = False
+    else:
+        fig = plt.figure(figsize=(RATIO * 4, 3 * RATIO * total_plots_count))
+        fig.suptitle('STATS - ' + experiment_id, fontsize=24, fontweight='bold')
+        # Variables initialization
+        ax, ax2 = [], []
+        rects = [None] * 5
+        # print("Normal plots: {}".format(normal_plots_count))
+        # print("Failed jobs plots: {}".format(failed_jobs_plots_count))
+        # print("Total plots: {}".format(total_plots_count))
+        grid_spec = gridspec.GridSpec(RATIO * total_plots_count + 2, 1)
+        i_plot = 0
+        for plot in range(1, normal_plots_count + 1):
+            try:
+                # Calculating jobs inside the given plot
+                l1 = int((plot - 1) * MAX_JOBS_PER_PLOT)
+                l2 = min(int(plot * MAX_JOBS_PER_PLOT), len(exp_stats.jobs_stat))
+                if l2 - l1 <= 0:
+                    continue
+                ind = np.arange(l2 - l1)
+                # Building plot axis
+                ax.append(fig.add_subplot(grid_spec[RATIO * plot - RATIO + 2:RATIO * plot + 1]))
+                ax[plot - 1].set_ylabel('hours')
+                ax[plot - 1].set_xticks(ind + width)
+                ax[plot - 1].set_xticklabels(
+                    [job.name for job in jobs_list[l1:l2]], rotation='vertical')
+                ax[plot - 1].set_title(experiment_id, fontsize=20)
+                upper_limit = round(1.10 * exp_stats.max_time, 4)
+                ax[plot - 1].set_yticks(np.arange(0, upper_limit, round(upper_limit / 10, 4)))
+                ax[plot - 1].set_ylim(0, float(1.10 * exp_stats.max_time))
+                # Building reacts
+                rects[0] = ax[plot - 1].bar(ind, exp_stats.queued[l1:l2], width, color='lightpink')
+                rects[1] = ax[plot - 1].bar(ind + width, exp_stats.run[l1:l2], width, color='green')
+                rects[2] = ax[plot - 1].bar(ind + width * 3, exp_stats.fail_queued[l1:l2], width, color='lightsalmon')
+                rects[3] = ax[plot - 1].bar(ind + width * 4, exp_stats.fail_run[l1:l2], width, color='salmon')
+                rects[4] = ax[plot - 1].plot([0., width * 6 * MAX_JOBS_PER_PLOT],
+                                             [exp_stats.threshold, exp_stats.threshold], "k--", label='wallclock sim')
+                # Building legend
+                i_plot = plot
+            except Exception as exp:
+                print((traceback.format_exc()))
+                print(exp)
+
+        job_names_in_failed = [name for name in exp_stats.failed_jobs_dict]
+        failed_jobs_rects = [None]
+        for j_plot in range(1, failed_jobs_plots_count + 1):
+            try:
+                l1 = int((j_plot - 1) * MAX_JOBS_PER_PLOT)
+                l2 = min(int(j_plot * MAX_JOBS_PER_PLOT), len(job_names_in_failed))
+                if l2 - l1 <= 0:
+                    continue
+                ind = np.arange(l2 - l1)
+                plot = i_plot + j_plot
+                ax.append(fig.add_subplot(grid_spec[RATIO * plot - RATIO + 2:RATIO * plot + 1]))
+                ax[plot - 1].set_ylabel('# failed attempts')
+                ax[plot - 1].set_xticks(ind + width)
+                ax[plot - 1].set_xticklabels([name for name in job_names_in_failed[l1:l2]], rotation='vertical')
+                ax[plot - 1].set_title(experiment_id, fontsize=20)
+                ax[plot - 1].set_ylim(0, float(1.10 * exp_stats.max_fail))
+                ax[plot - 1].set_yticks(range(0, exp_stats.max_fail + 2))
+                failed_jobs_rects[0] = ax[plot - 1].bar(ind + width * 2, [exp_stats.failed_jobs_dict[name] for name in
+                                                                          job_names_in_failed[l1:l2]], width, color='red')
+            except Exception as exp:
+                print((traceback.format_exc()))
+                print(exp)
+
+        # Building legends subplot
+        legends_plot = fig.add_subplot(grid_spec[0, 0])
+        legends_plot.set_frame_on(False)
+        legends_plot.axes.get_xaxis().set_visible(False)
+        legends_plot.axes.get_yaxis().set_visible(False)
 
-    job_names_in_failed = [name for name in exp_stats.failed_jobs_dict]
-    failed_jobs_rects = [None]
-    for j_plot in range(1, failed_jobs_plots_count + 1):
         try:
-            l1 = int((j_plot - 1) * MAX_JOBS_PER_PLOT)
-            l2 = min(int(j_plot * MAX_JOBS_PER_PLOT), len(job_names_in_failed))
-            if l2 - l1 <= 0:
-                continue
-            ind = np.arange(l2 - l1)
-            plot = i_plot + j_plot
-            ax.append(fig.add_subplot(grid_spec[RATIO * plot - RATIO + 2:RATIO * plot + 1]))
-            ax[plot - 1].set_ylabel('# failed attempts')
-            ax[plot - 1].set_xticks(ind + width)
-            ax[plot - 1].set_xticklabels([name for name in job_names_in_failed[l1:l2]], rotation='vertical')
-            ax[plot - 1].set_title(experiment_id, fontsize=20)
-            ax[plot - 1].set_ylim(0, float(1.10 * exp_stats.max_fail))
-            ax[plot - 1].set_yticks(range(0, exp_stats.max_fail + 2))
-            failed_jobs_rects[0] = ax[plot - 1].bar(ind + width * 2, [exp_stats.failed_jobs_dict[name] for name in
-                                                                      job_names_in_failed[l1:l2]], width, color='red')
+            # Building legends
+            # print("Legends")
+            build_legends(legends_plot, rects, exp_stats, general_stats)
+            # Saving output figure
+            grid_spec.tight_layout(fig, rect=[0, 0.03, 1, 0.97])
+            plt.savefig(output_file)
         except Exception as exp:
-            print((traceback.format_exc()))
             print(exp)
-
-    # Building legends subplot
-    legends_plot = fig.add_subplot(grid_spec[0, 0])
-    legends_plot.set_frame_on(False)
-    legends_plot.axes.get_xaxis().set_visible(False)
-    legends_plot.axes.get_yaxis().set_visible(False)
-
+            print((traceback.format_exc()))
     try:
-        # Building legends
-        # print("Legends")
-        build_legends(legends_plot, rects, exp_stats, general_stats)
-
-        # Saving output figure
-        grid_spec.tight_layout(fig, rect=[0, 0.03, 1, 0.97])
-        plt.savefig(output_file)
-
         create_csv_stats(exp_stats, jobs_list, output_file)
     except Exception as exp:
-        print(exp)
-        print((traceback.format_exc()))
+        Log.info(f'Error while creating csv stats:\n{err_message}')
+    return plot
 
 
 def create_csv_stats(exp_stats, jobs_list, output_file):
     job_names = [job.name for job in exp_stats.jobs_stat]
     start_times = exp_stats.start_times
     end_times = exp_stats.end_times
     queuing_times = exp_stats.queued
     running_times = exp_stats.run
 
     output_file = output_file.replace('pdf', 'csv')
     with open(output_file, 'w') as file:
         file.write(
             "Job,Started,Ended,Queuing time (hours),Running time (hours)\n")
-        for i in range(len(jobs_list)):
+        # In the other function, job_names,start_times... etc is only filled if the job has completed retrials
+        # So I'll change this one to do the same
+        for i in range(len([ job for job in jobs_list if job.get_last_retrials() ])):
             file.write("{0},{1},{2},{3},{4}\n".format(
                 job_names[i], start_times[i], end_times[i], queuing_times[i], running_times[i]))
 
 
 def build_legends(plot, rects, experiment_stats, general_stats):
     # type: (plt.figure, List[plt.bar], Statistics, List[str]) -> None
     # Main legend with colourful rectangles
+
     legend_rects = [[rect[0] for rect in rects]]
+
     legend_titles = [
         ['Queued (h)', 'Run (h)', 'Fail Queued (h)', 'Fail Run (h)', 'Max wallclock (h)']
     ]
     legend_locs = ["upper right"]
     legend_handlelengths = [None]
 
     # General stats legends, if exists
```

### Comparing `autosubmit-4.0.84/autosubmit/monitor/monitor.py` & `autosubmit-4.0.85/autosubmit/monitor/monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -229,36 +229,87 @@
 
         for package, cluster in packages_subgraphs_dict.items():
             graph.add_subgraph(cluster)
 
         Log.debug('Graph definition finalized')
         return graph
 
+    def _check_final_status(self, job, child):
+        # order of self._table
+        # the dictionary is composed by:
+        label = None
+        if len(child.edge_info) > 0:
+            if job.name in child.edge_info.get("FAILED",{}):
+                color = self._table.get(Status.FAILED,None)
+                label = child.edge_info["FAILED"].get(job.name,0)[1]
+            elif job.name in child.edge_info.get("RUNNING",{}):
+                color =  self._table.get(Status.RUNNING,None)
+                label = child.edge_info["RUNNING"].get(job.name,0)[1]
+            elif job.name in child.edge_info.get("QUEUING",{}):
+                color =  self._table.get(Status.QUEUING,None)
+            elif job.name in child.edge_info.get("HELD",{}):
+                color =  self._table.get(Status.HELD,None)
+            elif job.name in child.edge_info.get("DELAYED",{}):
+                color =  self._table.get(Status.DELAYED,None)
+            elif job.name in child.edge_info.get("UNKNOWN",{}):
+                color =  self._table.get(Status.UNKNOWN,None)
+            elif job.name in child.edge_info.get("SUSPENDED",{}):
+                color =  self._table.get(Status.SUSPENDED,None)
+            elif job.name in child.edge_info.get("SKIPPED",{}):
+                color =  self._table.get(Status.SKIPPED,None)
+            elif job.name in child.edge_info.get("WAITING",{}):
+                color =  self._table.get(Status.WAITING,None)
+            elif job.name in child.edge_info.get("READY",{}):
+                color =  self._table.get(Status.READY,None)
+            elif job.name in child.edge_info.get("SUBMITTED",{}):
+                color =  self._table.get(Status.SUBMITTED,None)
+            else:
+                return None, None
+            if label and label == 0:
+                label = None
+            return color,label
+        else:
+            return None, None
+
+
+
+
+
+
     def _add_children(self, job, exp, node_job, groups, hide_groups):
         if job in self.nodes_plotted:
             return
         self.nodes_plotted.add(job)
         if job.has_children() != 0:
             for child in sorted(job.children, key=lambda k: k.name):
                 node_child, skip = self._check_node_exists(
                     exp, child, groups, hide_groups)
+                color, label = self._check_final_status(job, child)
                 if len(node_child) == 0 and not skip:
                     node_child = self._create_node(child, groups, hide_groups)
                     if node_child:
                         exp.add_node(node_child)
-                        if job.name in child.edge_info and child.edge_info[job.name].get('optional', False):
-                            exp.add_edge(pydotplus.Edge(node_job, node_child,style="dashed"))
+                        if color:
+                            # label = None doesn't disable label, instead it sets it to nothing and complain about invalid syntax
+                            if label:
+                                exp.add_edge(pydotplus.Edge(node_job, node_child,style="dashed",color=color,label=label))
+                            else:
+                                exp.add_edge(pydotplus.Edge(node_job, node_child,style="dashed",color=color))
                         else:
                             exp.add_edge(pydotplus.Edge(node_job, node_child))
                     else:
                         skip = True
                 elif not skip:
                     node_child = node_child[0]
-                    if job.name in child.edge_info and child.edge_info[job.name].get('optional', False):
-                        exp.add_edge(pydotplus.Edge(node_job, node_child,style="dashed"))
+                    if color:
+                        # label = None doesn't disable label, instead it sets it to nothing and complain about invalid syntax
+                        if label:
+                            exp.add_edge(pydotplus.Edge(node_job, node_child, style="dashed", color=color, label=label))
+                        else:
+                            exp.add_edge(pydotplus.Edge(node_job, node_child, style="dashed", color=color))
                     else:
                         exp.add_edge(pydotplus.Edge(node_job, node_child))
                     skip = True
                 if not skip:
                     self._add_children(
                         child, exp, node_child, groups, hide_groups)
 
@@ -477,15 +528,15 @@
             elif os.path.exists(os.path.join(BasicConfig.LOCAL_ROOT_DIR, expid, BasicConfig.LOCAL_TMP_DIR)) and os.access(os.path.join(BasicConfig.LOCAL_ROOT_DIR, expid, BasicConfig.LOCAL_TMP_DIR), os.W_OK):
                     output_complete_path = os.path.join(BasicConfig.LOCAL_ROOT_DIR, expid, BasicConfig.LOCAL_TMP_DIR, output_filename)
                     is_default_path = False
         if is_default_path:
             Log.info("You don't have enough permissions to the experiment's ({}) folder. The output file will be created in the default location: {}".format(expid, BasicConfig.DEFAULT_OUTPUT_DIR))
             HUtils.create_path_if_not_exists_group_permission(BasicConfig.DEFAULT_OUTPUT_DIR)                
 
-        create_bar_diagram(expid, joblist, self.get_general_stats(expid), output_complete_path, period_ini, period_fi, queue_time_fixes)
+        show = create_bar_diagram(expid, joblist, self.get_general_stats(expid), output_complete_path, period_ini, period_fi, queue_time_fixes)
         Log.result('Stats created at {0}', output_complete_path)
         if show:
             try:
                 if sys.platform != "linux":
                     try:
                         subprocess.check_output(["open", output_complete_path])
                     except Exception as e:
```

### Comparing `autosubmit-4.0.84/autosubmit/monitor/utils.py` & `autosubmit-4.0.85/autosubmit/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/notifications/mail_notifier.py` & `autosubmit-4.0.85/autosubmit/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/notifications/notifier.py` & `autosubmit-4.0.85/autosubmit/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/ecplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/ec_cca_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/ec_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/local_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/lsf_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/pbs10_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/pbs11_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/pbs12_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/pjm_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/pjm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/ps_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/sge_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/headers/slurm_header.py` & `autosubmit-4.0.85/autosubmit/platforms/headers/slurm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/locplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/lsfplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/paramiko_platform.py` & `autosubmit-4.0.85/autosubmit/platforms/paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/paramiko_submitter.py` & `autosubmit-4.0.85/autosubmit/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/pbsplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/pjmplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/pjmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/platform.py` & `autosubmit-4.0.85/autosubmit/platforms/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import locale
 import os
+from pathlib import Path
 
 import traceback
 from autosubmit.job.job_common import Status
 from typing import List, Union
 
 from autosubmit.helpers.parameters import autosubmit_parameter
 from log.log import AutosubmitCritical, AutosubmitError, Log
@@ -508,14 +509,30 @@
         :type exp_id: str
         :param remote_logs: names of the log files
         :type remote_logs: (str, str)
         """
         (job_out_filename, job_err_filename) = remote_logs
         self.get_files([job_out_filename, job_err_filename], False, 'LOG_{0}'.format(exp_id))
 
+    def get_checkpoint_files(self, job):
+        """
+        Get all the checkpoint files of a job
+        :param job: Get the checkpoint files
+        :type job: Job
+        :param max_step: max step possible
+        :type max_step: int
+        """
+
+        if job.current_checkpoint_step < job.max_checkpoint_step:
+            remote_checkpoint_path = f'{self.get_files_path()}/CHECKPOINT_'
+            self.get_file(f'{remote_checkpoint_path}{str(job.current_checkpoint_step)}', False, ignore_log=True)
+            while self.check_file_exists(f'{remote_checkpoint_path}{str(job.current_checkpoint_step)}') and job.current_checkpoint_step < job.max_checkpoint_step:
+                self.remove_checkpoint_file(f'{remote_checkpoint_path}{str(job.current_checkpoint_step)}')
+                job.current_checkpoint_step += 1
+                self.get_file(f'{remote_checkpoint_path}{str(job.current_checkpoint_step)}', False, ignore_log=True)
     def get_completed_files(self, job_name, retries=0, recovery=False, wrapper_failed=False):
         """
         Get the COMPLETED file of the given job
 
 
         :param wrapper_failed:
         :param recovery:
@@ -578,14 +595,23 @@
         :rtype: bool
         """
         filename = job_name + '_COMPLETED'
         if self.delete_file(filename):
             Log.debug('{0} been removed', filename)
             return True
         return False
+    def remove_checkpoint_file(self, filename):
+        """
+        Removes *CHECKPOINT* files from remote
+
+        :param job_name: name of job to check
+        :return: True if successful, False otherwise
+        """
+        if self.check_file_exists(filename):
+            self.delete_file(filename)
 
     def check_file_exists(self, src, wrapper_failed=False):
         return True
 
     def get_stat_file(self, job_name, retries=0):
         """
         Copies *STAT* files from remote to local
```

### Comparing `autosubmit-4.0.84/autosubmit/platforms/psplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/sgeplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/slurmplatform.py` & `autosubmit-4.0.85/autosubmit/platforms/slurmplatform.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with Autosubmit.  If not, see <http://www.gnu.org/licenses/>.
 import locale
 import os
-from contextlib import suppress
-from time import sleep
+from datetime import datetime
 from time import mktime
+from time import sleep
 from time import time
-from datetime import datetime
 from typing import List, Union
-
 from xml.dom.minidom import parseString
 
 from autosubmit.job.job_common import Status, parse_output_number
-from autosubmit.platforms.paramiko_platform import ParamikoPlatform
 from autosubmit.platforms.headers.slurm_header import SlurmHeader
+from autosubmit.platforms.paramiko_platform import ParamikoPlatform
 from autosubmit.platforms.wrappers.wrapper_factory import SlurmWrapperFactory
 from log.log import AutosubmitCritical, AutosubmitError, Log
 
 
 class SlurmPlatform(ParamikoPlatform):
     """
     Class to manage jobs to host using SLURM scheduler
@@ -84,16 +82,16 @@
         try:
             valid_packages_to_submit = [ package for package in valid_packages_to_submit if package.x11 != True]
             if len(valid_packages_to_submit) > 0:
                 package = valid_packages_to_submit[0]
                 try:
                     jobs_id = self.submit_Script(hold=hold)
                 except AutosubmitError as e:
-                    Log.error(f'TRACE:{e.trace}\n{e.message}')
                     jobnames = [job.name for job in valid_packages_to_submit[0].jobs]
+                    Log.error(f'TRACE:{e.trace}\n{e.message} JOBS:{jobnames}')
                     for jobname in jobnames:
                         jobid = self.get_jobid_by_jobname(jobname)
                         #cancel bad submitted job if jobid is encountered
                         for id_ in jobid:
                             self.cancel_job(id_)
                     jobs_id = None
                     self.connected = False
```

### Comparing `autosubmit-4.0.84/autosubmit/platforms/submitter.py` & `autosubmit-4.0.85/autosubmit/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_builder.py` & `autosubmit-4.0.85/autosubmit/platforms/wrappers/wrapper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/platforms/wrappers/wrapper_factory.py` & `autosubmit-4.0.85/autosubmit/platforms/wrappers/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/statistics/jobs_stat.py` & `autosubmit-4.0.85/autosubmit/statistics/jobs_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/statistics/statistics.py` & `autosubmit-4.0.85/autosubmit/statistics/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,154 @@
 #!/bin/env/python
 
 from datetime import datetime, timedelta
+from typing import List, Union, Dict
+
 from autosubmit.job.job import Job
 from .jobs_stat import JobStat
 from .stats_summary import StatsSummary
 from .utils import timedelta2hours, parse_number_processors
-from typing import List, Union, Dict
+
 # from collections import namedtuple
 
 _COMPLETED_RETRIAL = 1
 _FAILED_RETRIAL = 0
 
+
 class Statistics(object):
 
     def __init__(self, jobs, start, end, queue_time_fix):
         # type: (List[Job], datetime, datetime, Dict[str, int]) -> None
         """
         """
-        self._jobs = jobs 
+        self._jobs = jobs
         self._start = start
         self._end = end
         self._queue_time_fixes = queue_time_fix
-        self._name_to_jobstat_dict = dict() # type: Dict[str, JobStat]
-        self.jobs_stat = [] # type: List[JobStat]
+        self._name_to_jobstat_dict = dict()  # type: Dict[str, JobStat]
+        self.jobs_stat = []  # type: List[JobStat]
         # Old format
-        self.max_time = 0.0 # type: float
-        self.max_fail = 0 # type: int
-        self.start_times = [] # type: List[Union[datetime, None]]
-        self.end_times = [] # type: List[Union[datetime, None]]
-        self.queued = [] # type: List[timedelta]
-        self.run = [] # type: List[timedelta]
-        self.failed_jobs = [] # type: List[int]
-        self.fail_queued = [] # type: List[timedelta]
-        self.fail_run = [] # type: List[timedelta]
-        self.wallclocks = [] # type: List[float]
-        self.threshold = 0.0 # type: float
-        self.failed_jobs_dict = {} # type: Dict[str, int]
+        self.max_time = 0.0  # type: float
+        self.max_fail = 0  # type: int
+        self.start_times = []  # type: List[Union[datetime, None]]
+        self.end_times = []  # type: List[Union[datetime, None]]
+        self.queued = []  # type: List[timedelta]
+        self.run = []  # type: List[timedelta]
+        self.failed_jobs = []  # type: List[int]
+        self.fail_queued = []  # type: List[timedelta]
+        self.fail_run = []  # type: List[timedelta]
+        self.wallclocks = []  # type: List[float]
+        self.threshold = 0.0  # type: float
+        self.failed_jobs_dict = {}  # type: Dict[str, int]
         self.summary = StatsSummary()
         self.totals = [" Description text \n", "Line 1"]
-            
+
     def calculate_statistics(self):
-      # type: () -> List[JobStat]
-      for index, job in enumerate(self._jobs):
-          retrials = job.get_last_retrials()          
-          for retrial in retrials:
-              # print(retrial)
-              job_stat = self._name_to_jobstat_dict.setdefault(job.name, JobStat(job.name, parse_number_processors(job.processors), job.total_wallclock, job.section, job.date, job.member, job.chunk))
-              job_stat.inc_retrial_count()
-              if Job.is_a_completed_retrial(retrial):
-                  job_stat.inc_completed_retrial_count()
-                  job_stat.submit_time = retrial[0] 
-                  job_stat.start_time = retrial[1] 
-                  job_stat.finish_time = retrial[2] 
-                  adjusted_queue = max(job_stat.start_time - job_stat.submit_time, timedelta()) - timedelta(seconds=self._queue_time_fixes.get(job.name, 0))
-                  job_stat.completed_queue_time += max(adjusted_queue, timedelta())
-                  job_stat.completed_run_time += max(job_stat.finish_time - job_stat.start_time, timedelta())
-              else:
-                  job_stat.inc_failed_retrial_count()
-                  job_stat.submit_time = retrial[0] if len(retrial) >= 1 and type(retrial[0]) == datetime else None
-                  job_stat.start_time = retrial[1] if len(retrial) >= 2 and type(retrial[1]) == datetime else None
-                  job_stat.finish_time = retrial[2] if len(retrial) >= 3 and type(retrial[2]) == datetime else None
-                  if job_stat.finish_time and job_stat.start_time:
-                      job_stat.failed_run_time += max(job_stat.finish_time - job_stat.start_time, timedelta())
-                  if job_stat.start_time and job_stat.submit_time:
-                    adjusted_failed_queue = max(job_stat.start_time - job_stat.submit_time, timedelta()) - timedelta(seconds=self._queue_time_fixes.get(job.name, 0))
-                    job_stat.failed_queue_time += max(adjusted_failed_queue, timedelta())
-      self.jobs_stat =sorted(list(self._name_to_jobstat_dict.values()), key=lambda x: (x.date if x.date else datetime.now(), x.member if x.member else "", x.section if x.section else "", x.chunk))
-      return self.jobs_stat
-    
+        # type: () -> List[JobStat]
+        for index, job in enumerate(self._jobs):
+            retrials = job.get_last_retrials()
+            for retrial in retrials:
+                print(retrial)
+                job_stat = self._name_to_jobstat_dict.setdefault(job.name, JobStat(job.name, parse_number_processors(
+                    job.processors), job.total_wallclock, job.section, job.date, job.member, job.chunk))
+                job_stat.inc_retrial_count()
+                if Job.is_a_completed_retrial(retrial):
+                    job_stat.inc_completed_retrial_count()
+                    job_stat.submit_time = retrial[0]
+                    job_stat.start_time = retrial[1]
+                    job_stat.finish_time = retrial[2]
+                    adjusted_queue = max(job_stat.start_time - job_stat.submit_time, timedelta()) - timedelta(
+                        seconds=self._queue_time_fixes.get(job.name, 0))
+                    job_stat.completed_queue_time += max(adjusted_queue, timedelta())
+                    job_stat.completed_run_time += max(job_stat.finish_time - job_stat.start_time, timedelta())
+                else:
+                    job_stat.inc_failed_retrial_count()
+                    job_stat.submit_time = retrial[0] if len(retrial) >= 1 and type(retrial[0]) == datetime else None
+                    job_stat.start_time = retrial[1] if len(retrial) >= 2 and type(retrial[1]) == datetime else None
+                    job_stat.finish_time = retrial[2] if len(retrial) >= 3 and type(retrial[2]) == datetime else None
+                    if job_stat.finish_time and job_stat.start_time:
+                        job_stat.failed_run_time += max(job_stat.finish_time - job_stat.start_time, timedelta())
+                    if job_stat.start_time and job_stat.submit_time:
+                        adjusted_failed_queue = max(job_stat.start_time - job_stat.submit_time,
+                                                    timedelta()) - timedelta(
+                            seconds=self._queue_time_fixes.get(job.name, 0))
+                        job_stat.failed_queue_time += max(adjusted_failed_queue, timedelta())
+        self.jobs_stat = sorted(list(self._name_to_jobstat_dict.values()), key=lambda x: (
+        x.date if x.date else datetime.now(), x.member if x.member else "", x.section if x.section else "", x.chunk))
+        return self.jobs_stat
+
     def calculate_summary(self):
-      # type: () -> StatsSummary
-      stat_summary = StatsSummary()
-      for job in self.jobs_stat:
-        # print("{} -> {}".format(job._name, job.expected_real_consumption))
-        job_stat_dict = job.get_as_dict()
-        # Counter
-        stat_summary.submitted_count += job_stat_dict["submittedCount"]
-        stat_summary.run_count += job_stat_dict["retrialCount"]
-        stat_summary.completed_count += job_stat_dict["completedCount"]
-        stat_summary.failed_count += job_stat_dict["failedCount"]
-        # Consumption
-        stat_summary.expected_consumption += job_stat_dict["expectedConsumption"]
-        stat_summary.real_consumption += job_stat_dict["realConsumption"]
-        stat_summary.failed_real_consumption += job_stat_dict["failedRealConsumption"]
-        # CPU Consumption
-        stat_summary.expected_cpu_consumption += job_stat_dict["expectedCpuConsumption"] 
-        stat_summary.cpu_consumption += job_stat_dict["cpuConsumption"]
-        stat_summary.failed_cpu_consumption += job_stat_dict["failedCpuConsumption"]
-        stat_summary.total_queue_time += job_stat_dict["completedQueueTime"] + job_stat_dict["failedQueueTime"]
-      stat_summary.calculate_consumption_percentage()
-      self.summary = stat_summary
+        # type: () -> StatsSummary
+        stat_summary = StatsSummary()
+        for job in self.jobs_stat:
+            # print("{} -> {}".format(job._name, job.expected_real_consumption))
+            job_stat_dict = job.get_as_dict()
+            # Counter
+            stat_summary.submitted_count += job_stat_dict["submittedCount"]
+            stat_summary.run_count += job_stat_dict["retrialCount"]
+            stat_summary.completed_count += job_stat_dict["completedCount"]
+            stat_summary.failed_count += job_stat_dict["failedCount"]
+            # Consumption
+            stat_summary.expected_consumption += job_stat_dict["expectedConsumption"]
+            stat_summary.real_consumption += job_stat_dict["realConsumption"]
+            stat_summary.failed_real_consumption += job_stat_dict["failedRealConsumption"]
+            # CPU Consumption
+            stat_summary.expected_cpu_consumption += job_stat_dict["expectedCpuConsumption"]
+            stat_summary.cpu_consumption += job_stat_dict["cpuConsumption"]
+            stat_summary.failed_cpu_consumption += job_stat_dict["failedCpuConsumption"]
+            stat_summary.total_queue_time += job_stat_dict["completedQueueTime"] + job_stat_dict["failedQueueTime"]
+        stat_summary.calculate_consumption_percentage()
+        self.summary = stat_summary
 
     def get_summary_as_list(self):
-      return self.summary.get_as_list()
+        return self.summary.get_as_list()
 
     def get_statistics(self):
         job_stat_list = self.calculate_statistics()
         return {
             "Period": {"From": str(self._start), "To": str(self._end)},
             "JobStatistics": [job.get_as_dict() for job in job_stat_list]
         }
-    
+
     def make_old_format(self):
-      # type: () -> None
-      """ Makes old format """
-      self.start_times = [job.start_time for job in self.jobs_stat]
-      self.end_times = [job.finish_time for job in self.jobs_stat]
-      self.queued = [timedelta2hours(job.completed_queue_time) for job in self.jobs_stat]
-      self.run = [timedelta2hours(job.completed_run_time) for job in self.jobs_stat]
-      self.failed_jobs = [job.failed_retrial_count for job in self.jobs_stat]
-      self.max_fail = max(self.failed_jobs)
-      self.fail_run = [timedelta2hours(job.failed_run_time) for job in self.jobs_stat]
-      self.fail_queued = [timedelta2hours(job.failed_queue_time) for job in self.jobs_stat]
-      self.wallclocks = [job.expected_real_consumption for job in self.jobs_stat]
-      self.threshold = max(self.wallclocks)
-      max_queue = max(self.queued)
-      max_run = max(self.run)
-      max_fail_queue = max(self.fail_queued)
-      max_fail_run = max(self.fail_run)
-      self.max_time = max(max_queue, max_run, max_fail_queue, max_fail_run, self.threshold)
+        # type: () -> None
+        """ Makes old format """
+        self.start_times = [job.start_time for job in self.jobs_stat]
+        self.end_times = [job.finish_time for job in self.jobs_stat]
+        self.queued = [timedelta2hours(job.completed_queue_time) for job in self.jobs_stat]
+        self.run = [timedelta2hours(job.completed_run_time) for job in self.jobs_stat]
+        self.failed_jobs = [job.failed_retrial_count for job in self.jobs_stat]
+        if len(self.failed_jobs) == 0:
+            self.max_fail = 0
+        else:
+            self.max_fail = max(self.failed_jobs)
+        self.fail_run = [timedelta2hours(job.failed_run_time) for job in self.jobs_stat]
+        self.fail_queued = [timedelta2hours(job.failed_queue_time) for job in self.jobs_stat]
+        self.wallclocks = [job.expected_real_consumption for job in self.jobs_stat]
+        if len(self.wallclocks) == 0:
+            self.threshold = 0.0
+        else:
+            self.threshold = max(self.wallclocks)
+        if len(self.queued) == 0:
+            max_queue = 0.0
+        else:
+            max_queue = max(self.queued)
+        if len(self.run) == 0:
+            max_run = 0.0
+        else:
+            max_run = max(self.run)
+        if len(self.fail_queued) == 0:
+            max_fail_queue = 0.0
+        else:
+            max_fail_queue = max(self.fail_queued)
+        if len(self.fail_run) == 0:
+            max_fail_run = 0.0
+        else:
+            max_fail_run = max(self.fail_run)
+        self.max_time = max(max_queue, max_run, max_fail_queue, max_fail_run, self.threshold)
 
     def build_failed_jobs_only_list(self):
-      # type: () -> Dict[str, int]
-      for i, job in enumerate(self.jobs_stat):
-        if self.failed_jobs[i] > 0:
-          self.failed_jobs_dict[job._name] = self.failed_jobs[i]
-      return self.failed_jobs_dict
-
-    
-    
+        # type: () -> Dict[str, int]
+        for i, job in enumerate(self.jobs_stat):
+            if self.failed_jobs[i] > 0:
+                self.failed_jobs_dict[job._name] = self.failed_jobs[i]
+        return self.failed_jobs_dict
```

### Comparing `autosubmit-4.0.84/autosubmit/statistics/stats_summary.py` & `autosubmit-4.0.85/autosubmit/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit/statistics/utils.py` & `autosubmit-4.0.85/autosubmit/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/autosubmit.egg-info/PKG-INFO` & `autosubmit-4.0.85/autosubmit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit
-Version: 4.0.84
+Version: 4.0.85
 Summary: Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.
 Home-page: http://www.bsc.es/projects/earthscience/autosubmit/
 Download-URL: https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit
 Author: Daniel Beltran Mora
 Author-email: daniel.beltran@bsc.es
 License: GNU GPL v3
 Keywords: climate,weather,workflow,HPC
@@ -24,7 +24,8 @@
 These multi-scale workflows can contain from a few steps to thousands of steps, and from a single platform to multiple platforms. Platform is a concept in Autosubmit to abstract servers. A workflow configuration can include one or multiple platforms, allowing the workflow to run on any number of servers via password-less SSH without any external deployment.
 
 Due to its robustness it can handle different eventualities such as networking connectivity issues or I/O errors. The monitoring capabilities extend beyond the command-line application through a REST API that allows communication with workflow monitoring tools such as the Autosubmit web GUI.
 
 It has contributed to various European research projects and runs different operational systems. It will support the Earth Digital Twins as the Digital Twin Ocean over the next years.
 
 It is currently used at the Barcelona Supercomputing Centre (BSC) to run models (EC-Earth, MONARCH, NEMO, CALIOPE, HERMES, and others), operational toolchains (S2S4E), data-download workflows (ECMWF MARS), and for many other use cases. Autosubmit has been used to run workflows in different supercomputers at BSC, ECMWF, IC3, CESGA, EPCC, PDC, and OLCF.
+
```

### Comparing `autosubmit-4.0.84/autosubmit.egg-info/SOURCES.txt` & `autosubmit-4.0.85/autosubmit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 autosubmit/platforms/headers/pjm_header.py
 autosubmit/platforms/headers/ps_header.py
 autosubmit/platforms/headers/sge_header.py
 autosubmit/platforms/headers/slurm_header.py
 autosubmit/platforms/wrappers/__init__.py
 autosubmit/platforms/wrappers/wrapper_builder.py
 autosubmit/platforms/wrappers/wrapper_factory.py
+autosubmit/profiler/__init__.py
+autosubmit/profiler/profiler.py
 autosubmit/statistics/__init__.py
 autosubmit/statistics/jobs_stat.py
 autosubmit/statistics/statistics.py
 autosubmit/statistics/stats_summary.py
 autosubmit/statistics/utils.py
 bin/autosubmit
 docs/Makefile
@@ -272,14 +274,15 @@
 test/regression/test_sedema_with_paramiko_python/conf/jobs.conf
 test/regression/test_sedema_with_paramiko_python/conf/proj.conf
 test/regression/test_sedema_with_paramiko_python/src/TEST_NOLEAP.py
 test/unit/README_PIP.md
 test/unit/__init__.py
 test/unit/test_basic_config.py
 test/unit/test_catlog.py
+test/unit/test_checkpoints.py
 test/unit/test_chunk_date_lib.py
 test/unit/test_database_managers.py
 test/unit/test_db_manager.py
 test/unit/test_dependencies.py
 test/unit/test_dic_jobs.py
 test/unit/test_expid.py
 test/unit/test_history.py
@@ -290,12 +293,13 @@
 test/unit/test_job_list.py
 test/unit/test_job_package.py
 test/unit/test_log.py
 test/unit/test_machinefiles_wrapper.py
 test/unit/test_paramiko_platform.py
 test/unit/test_pjm.py
 test/unit/test_platform_monitor.py
+test/unit/test_profiler.py
 test/unit/test_setup.py
 test/unit/test_slurm_platform.py
 test/unit/test_statistics.py
 test/unit/test_strategies.py
 test/unit/test_wrappers.py
```

### Comparing `autosubmit-4.0.84/bin/autosubmit` & `autosubmit-4.0.85/bin/autosubmit`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/Makefile` & `autosubmit-4.0.85/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/autosubmit.pdf` & `autosubmit-4.0.85/docs/autosubmit.pdf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/experiment/fig/fig_experiment.jpg` & `autosubmit-4.0.85/docs/source/agui/experiment/fig/fig_experiment.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/experiment/index.rst` & `autosubmit-4.0.85/docs/source/agui/experiment/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig1_gui.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig1_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig2_gui.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig2_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig3_gui.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig3_gui.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig4_gui.jpg` & `autosubmit-4.0.85/docs/source/agui/fig/fig4_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig5_gui.jpg` & `autosubmit-4.0.85/docs/source/agui/fig/fig5_gui.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig_ev_1.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig_ev_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig_tree_1.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig_tree_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/fig/fig_tree_2.png` & `autosubmit-4.0.85/docs/source/agui/fig/fig_tree_2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_1.jpg` & `autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_2.jpg` & `autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_3.jpg` & `autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_3.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/graph/fig/fig_graph_4.jpg` & `autosubmit-4.0.85/docs/source/agui/graph/fig/fig_graph_4.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/graph/index.rst` & `autosubmit-4.0.85/docs/source/agui/graph/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/index.rst` & `autosubmit-4.0.85/docs/source/agui/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_1.jpg` & `autosubmit-4.0.85/docs/source/agui/log/fig/fig_log_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/log/fig/fig_log_2.jpg` & `autosubmit-4.0.85/docs/source/agui/log/fig/fig_log_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/log/index.rst` & `autosubmit-4.0.85/docs/source/agui/log/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/performance/fig/fig_performance_1.jpg` & `autosubmit-4.0.85/docs/source/agui/performance/fig/fig_performance_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/performance/index.rst` & `autosubmit-4.0.85/docs/source/agui/performance/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_1.jpg` & `autosubmit-4.0.85/docs/source/agui/statistics/fig/fig_stat_1.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/statistics/fig/fig_stat_2.jpg` & `autosubmit-4.0.85/docs/source/agui/statistics/fig/fig_stat_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/statistics/index.rst` & `autosubmit-4.0.85/docs/source/agui/statistics/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/tree/fig/fig_tree_2.jpg` & `autosubmit-4.0.85/docs/source/agui/tree/fig/fig_tree_2.jpg`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/agui/tree/index.rst` & `autosubmit-4.0.85/docs/source/agui/tree/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/conf.py` & `autosubmit-4.0.85/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,21 @@
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.imgmath',
     'sphinx.ext.autosectionlabel',
     'sphinx_rtd_theme',
     'sphinx_reredirects',
-    'autosubmit_variables'
+    'autosubmit_variables',
+    'sphinx.ext.graphviz'
 ]
 
+# Set .svg output fot the graphs generated by GraphViz
+graphviz_output_format='svg'
+
 autosectionlabel_prefix_document = True
 
 numfig = True
 numfig_format = {'figure': '%s', 'table': '%s', 'code-block': '%s'}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
```

### Comparing `autosubmit-4.0.84/docs/source/devguide/index.rst` & `autosubmit-4.0.85/docs/source/devguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/index.rst` & `autosubmit-4.0.85/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/installation/index.rst` & `autosubmit-4.0.85/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/introduction/fig1.png` & `autosubmit-4.0.85/docs/source/introduction/fig1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/introduction/fig2.png` & `autosubmit-4.0.85/docs/source/introduction/fig2.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/introduction/fig3.png` & `autosubmit-4.0.85/docs/source/introduction/fig3.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/introduction/index.rst` & `autosubmit-4.0.85/docs/source/introduction/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/moduledoc/platforms.rst` & `autosubmit-4.0.85/docs/source/moduledoc/platforms.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/qstartguide/dummy.png` & `autosubmit-4.0.85/docs/source/qstartguide/dummy.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/qstartguide/index.rst` & `autosubmit-4.0.85/docs/source/qstartguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/changelog.rst` & `autosubmit-4.0.85/docs/source/troubleshooting/changelog.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/error-codes.rst` & `autosubmit-4.0.85/docs/source/troubleshooting/error-codes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,16 @@
 +------+-----------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | 7072 | Basic configuration not found                 | Administrator: run `autosubmit configure --advanced` or create a common file in /etc/autosubmitrc.                                                                               |
 |      |                                               | User: run `autosubmit configure` or create a $HOME/.autosubmitrc. Following the skeleton of installation page                                                                    |
 +------+-----------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 | 7073 | Private key is encrypted                      | Each Session: Add your key into the ssh agent. ex. ssh-add $HOME/.ssh/id_rsa, then launch autosubmit.                                                                            |
 |      |                                               | Alternative: You can use a non-encrypted key, just make sure that nobody except you has access to the file.                                                                      |
 +------+-----------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
+| 7074 | Profiling process failed                      | You can find descriptive explanations in the log, as well as hints to solve the problem.                                                                                         |
++------+-----------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
 
 **Default Solution**
 
 Check autosubmit log for detailed information, there will be additional error codes.
 
 ----
```

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/fig/monarch-da.png` & `autosubmit-4.0.85/docs/source/troubleshooting/fig/monarch-da.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_0.png` & `autosubmit-4.0.85/docs/source/troubleshooting/fig/new_dependencies_0.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/fig/new_dependencies_1.png` & `autosubmit-4.0.85/docs/source/troubleshooting/fig/new_dependencies_1.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/troubleshooting/index.rst` & `autosubmit-4.0.85/docs/source/troubleshooting/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/unused_figs/group_chunk.png` & `autosubmit-4.0.85/docs/source/unused_figs/group_chunk.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/unused_figs/horizontal-vertical.png` & `autosubmit-4.0.85/docs/source/unused_figs/horizontal-vertical.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/unused_figs/wrapper.png` & `autosubmit-4.0.85/docs/source/unused_figs/wrapper.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/unused_figs/wrapper_expression.png` & `autosubmit-4.0.85/docs/source/unused_figs/wrapper_expression.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/unused_figs/wrapper_hybrid.png` & `autosubmit-4.0.85/docs/source/unused_figs/wrapper_hybrid.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/configure/develop_a_project.rst` & `autosubmit-4.0.85/docs/source/userguide/configure/develop_a_project.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/configure/index.rst` & `autosubmit-4.0.85/docs/source/userguide/configure/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/create/index.rst` & `autosubmit-4.0.85/docs/source/userguide/create/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/index.rst` & `autosubmit-4.0.85/docs/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/manage/index.rst` & `autosubmit-4.0.85/docs/source/userguide/manage/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/run/index.rst` & `autosubmit-4.0.85/docs/source/userguide/run/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -183,14 +183,50 @@
 
 Then, your terminal will show the current status of the experiment you are waiting for. The status format is `COMPLETED/QUEUING/RUNNING/SUSPENDED/FAILED`.
 
 This functionality can be used together with other options supplied by the `run` command.
 
 The `-sa` command has a long version `--start_after`.
 
+.. _basic_profiling:
+
+
+How to profile Autosubmit while running an experiment
+-----------------------------------------------------
+
+Autosubmit offers the possibility to profile an experiment execution. To enable the profiler, just 
+add the ``--profile`` (or ``-p``) flag to your ``autosubmit run`` command, as in the following example:
+
+.. code-block:: bash
+
+    autosubmit run --profile EXPID
+
+.. note:: Remember that the purpose of this profiler is to measure the performance of Autosubmit, 
+  not the jobs it runs.
+
+This profiler uses Python's ``cProfile`` and ``psutil`` modules to generate a report with simple CPU and 
+memory metrics for the experiment execution. These metrics will be displayed in your console after 
+the experiment finishes, as in the example below:
+
+.. figure:: profiler_output.png
+   :name: profiler_head_output
+   :align: center
+   :alt: Screenshot of the header of the profiler's output
+
+The profiler output is also saved in ``<EXPID>/tmp/profile``. There you will find two files, the 
+report in plain text format and a ``.prof`` binary which contains the CPU metrics. We highly recommend 
+using `SnakeViz <https://jiffyclub.github.io/snakeviz/>`_ to visualize this file, as follows:
+
+.. figure:: profiler_snakeviz.png
+   :name: profiler_snakeviz
+   :align: center
+   :alt: The .prof file represented by the graphical library SnakeViz
+
+For more detailed documentation about the profiler, please visit this :ref:`page<advanced_profiling>`.
+
 .. _run_modes:
 
 How to prepare an experiment to run in two independent job_list. (Priority jobs, Two-step-run) (OLD METHOD)
 -----------------------------------------------------------------------------------------------------------
 
 This feature allows to run an experiment in two separated steps without the need of do anything manually.
```

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/dasim.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/dasim.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/horizontal_remote.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/horizontal_remote.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/multiple_wrappers.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/multiple_wrappers.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/rerun.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/rerun.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-horizontal.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/vertical-horizontal.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/fig/vertical-mixed.png` & `autosubmit-4.0.85/docs/source/userguide/wrappers/fig/vertical-mixed.png`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/docs/source/userguide/wrappers/index.rst` & `autosubmit-4.0.85/docs/source/userguide/wrappers/index.rst`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/environment.yml` & `autosubmit-4.0.85/environment.yml`

 * *Files 16% similar despite different names*

```diff
@@ -40,8 +40,9 @@
   - ruamel.yaml
   - pythondialog
   - pytest
   - nose
   - coverage
   - requests
   - configobj
+  - psutil
```

### Comparing `autosubmit-4.0.84/log/fd_show.py` & `autosubmit-4.0.85/log/fd_show.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/log/log.py` & `autosubmit-4.0.85/log/log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/setup.py` & `autosubmit-4.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description='Autosubmit is a Python-based workflow manager to create, manage and monitor complex tasks involving different substeps, such as scientific computational experiments. These workflows may involve multiple computing systems for their completion, from HPCs to post-processing clusters or workstations. Autosubmit can orchestrate all the tasks integrating the workflow by managing their dependencies, interfacing with all the platforms involved, and handling eventual errors.',
     long_description=open('README_PIP.md').read(),
     author='Daniel Beltran Mora',
     author_email='daniel.beltran@bsc.es',
     url='http://www.bsc.es/projects/earthscience/autosubmit/',
     download_url='https://earth.bsc.es/wiki/doku.php?id=tools:autosubmit',
     keywords=['climate', 'weather', 'workflow', 'HPC'],
-    install_requires=['ruamel.yaml==0.17.21','cython','autosubmitconfigparser','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments'],
+    install_requires=['ruamel.yaml==0.17.21','cython','autosubmitconfigparser','bcrypt>=3.2','packaging>19','six>=1.10.0','configobj>=5.0.6','argparse>=1.4.0','python-dateutil>=2.8.2','matplotlib<3.6','numpy<1.22','py3dotplus>=1.1.0','pyparsing>=3.0.7','paramiko>=2.9.2','mock>=4.0.3','portalocker>=2.3.2','networkx==2.6.3','requests>=2.27.1','bscearth.utils>=0.5.2','cryptography>=36.0.1','setuptools>=60.8.2','xlib>=0.21','pip>=22.0.3','pythondialog','pytest','nose','coverage','PyNaCl>=1.4.0','Pygments','psutil'],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: POSIX :: Linux",
     ],
     packages=find_packages(),
```

### Comparing `autosubmit-4.0.84/test/integration/test_db_manager.py` & `autosubmit-4.0.85/test/integration/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/integration/test_job.py` & `autosubmit-4.0.85/test/integration/test_job.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/README` & `autosubmit-4.0.85/test/regression/README`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/default_conf/platforms.conf` & `autosubmit-4.0.85/test/regression/default_conf/platforms.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/local_asparser_test.py` & `autosubmit-4.0.85/test/regression/local_asparser_test.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.85/test/regression/test_ecmwf_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_large_experiment_on_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mistral_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mistral_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.85/test/regression/test_mn3_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn3_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_horizontal_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_vertical_horizontal_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_vertical_wrapper_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko/conf/jobs.conf` & `autosubmit-4.0.85/test/regression/test_mn4_with_paramiko/conf/jobs.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_mn4_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_moore_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_moore_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_moore_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_moore_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_sedema_with_paramiko/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf` & `autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/autosubmit.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf` & `autosubmit-4.0.85/test/regression/test_sedema_with_paramiko_python/conf/expdef.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/tests.conf` & `autosubmit-4.0.85/test/regression/tests.conf`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/tests_commands.py` & `autosubmit-4.0.85/test/regression/tests_commands.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/tests_log.py` & `autosubmit-4.0.85/test/regression/tests_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/tests_runner.py` & `autosubmit-4.0.85/test/regression/tests_runner.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/regression/tests_utils.py` & `autosubmit-4.0.85/test/regression/tests_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/README_PIP.md` & `autosubmit-4.0.85/test/unit/README_PIP.md`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_basic_config.py` & `autosubmit-4.0.85/test/unit/test_basic_config.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_catlog.py` & `autosubmit-4.0.85/test/unit/test_catlog.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_chunk_date_lib.py` & `autosubmit-4.0.85/test/unit/test_chunk_date_lib.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_database_managers.py` & `autosubmit-4.0.85/test/unit/test_database_managers.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_db_manager.py` & `autosubmit-4.0.85/test/unit/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_dic_jobs.py` & `autosubmit-4.0.85/test/unit/test_dic_jobs.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_expid.py` & `autosubmit-4.0.85/test/unit/test_expid.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_history.py` & `autosubmit-4.0.85/test/unit/test_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_job.py` & `autosubmit-4.0.85/test/unit/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from unittest import TestCase
+
+import datetime
+import inspect
 import os
 import sys
-from autosubmitconfigparser.config.configcommon import AutosubmitConfig
-from autosubmit.job.job_common import Status
-from autosubmit.job.job import Job
-from autosubmit.platforms.platform import Platform
 from mock import Mock, MagicMock
 from mock import patch
-import datetime
-
 # compatibility with both versions (2 & 3)
 from sys import version_info
 
+from autosubmit.job.job import Job
+from autosubmit.job.job_common import Status
+from autosubmit.platforms.platform import Platform
+from autosubmitconfigparser.config.configcommon import AutosubmitConfig
+
 if version_info.major == 2:
     import builtins as builtins
 else:
     import builtins
 
 
 class TestJob(TestCase):
@@ -358,15 +360,14 @@
             [datetime.datetime(1975, 5, 25, 22, 30, 0, 0, datetime.timezone.utc), 'S', '19750525223000'],
             [datetime.datetime(1975, 5, 25, 22, 30, 0, 0, datetime.timezone.utc), None, '19750525']
         ]:
             self.job.date = test[0]
             self.job.date_format = test[1]
             self.assertEquals(test[2], self.job.sdate)
 
-import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
     def props(self):
         pr = {}
         for name in dir(self):
             value = getattr(self, name)
```

### Comparing `autosubmit-4.0.84/test/unit/test_job_common.py` & `autosubmit-4.0.85/test/unit/test_job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_job_graph.py` & `autosubmit-4.0.85/test/unit/test_job_graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_job_grouping.py` & `autosubmit-4.0.85/test/unit/test_job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_job_list.py` & `autosubmit-4.0.85/test/unit/test_job_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,14 @@
     def _createDummyJobWithStatus(self, status):
         job_name = str(randrange(999999, 999999999))
         job_id = randrange(1, 999)
         job = Job(job_name, job_id, status, 0)
         job.type = randrange(0, 2)
         return job
 
-import inspect
 class FakeBasicConfig:
     def __init__(self):
         pass
     def props(self):
         pr = {}
         for name in dir(self):
             value = getattr(self, name)
```

### Comparing `autosubmit-4.0.84/test/unit/test_job_package.py` & `autosubmit-4.0.85/test/unit/test_job_package.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 from unittest import TestCase
 
 import os
+from pathlib import Path
 import inspect
-from copy import deepcopy
-from mock import Mock,MagicMock, mock_open , call
+import tempfile
+from mock import MagicMock
 from mock import patch
 
-from autosubmit.job.job_packages import JobPackageSimple, JobPackageVertical
 from autosubmit.job.job import Job
 from autosubmit.job.job_common import Status
-
-import shutil
-import tempfile
-
-from unittest import TestCase
-from mock import MagicMock
-from autosubmit.job.job_packager import JobPackager
 from autosubmit.job.job_list import JobList
-from autosubmit.job.job_dict import DicJobs
-from autosubmit.job.job_utils import Dependency
-from autosubmitconfigparser.config.yamlparser import YAMLParserFactory
 from autosubmit.job.job_list_persistence import JobListPersistenceDb
-from random import randrange
-from collections import OrderedDict
+from autosubmit.job.job_packages import JobPackageSimple, JobPackageVertical
 from autosubmitconfigparser.config.configcommon import AutosubmitConfig
+from autosubmitconfigparser.config.yamlparser import YAMLParserFactory
+
+
 class FakeBasicConfig:
     def __init__(self):
         pass
     def props(self):
         pr = {}
         for name in dir(self):
             value = getattr(self, name)
@@ -52,16 +44,17 @@
         self.experiment_id = 'random-id'
         self._wrapper_factory = MagicMock()
 
         self.config = FakeBasicConfig
         self.config.read = MagicMock()
 
 
-
-        self.as_conf = AutosubmitConfig(self.experiment_id, self.config, YAMLParserFactory())
+        with patch.object(Path, 'exists') as mock_exists:
+            mock_exists.return_value = True
+            self.as_conf = AutosubmitConfig(self.experiment_id, self.config, YAMLParserFactory())
         self.as_conf.experiment_data = dict()
         self.as_conf.experiment_data["JOBS"] = dict()
         self.as_conf.experiment_data["PLATFORMS"] = dict()
         self.as_conf.experiment_data["WRAPPERS"] = dict()
         self.temp_directory = tempfile.mkdtemp()
         self.job_list = JobList(self.experiment_id, self.config, YAMLParserFactory(),
                                 JobListPersistenceDb(self.temp_directory, 'db'), self.as_conf)
@@ -76,24 +69,26 @@
         self.jobs[0].tasks = "1"
         self.jobs[0].exclusive = True
         self.jobs[0].queue = "debug"
         self.jobs[0].partition = "debug"
         self.jobs[0].custom_directives = "dummy_directives"
         self.jobs[0].processors = "9"
         self.jobs[0]._processors = "9"
+        self.jobs[0]._platform = self.platform
         self.jobs[0].retrials = 0
         self.jobs[1].wallclock = "00:00"
         self.jobs[1].threads = ""
         self.jobs[1].tasks = ""
         self.jobs[1].exclusive = True
         self.jobs[1].queue = "debug2"
         self.jobs[1].partition = "debug2"
         self.jobs[1].custom_directives = "dummy_directives2"
         self.jobs[1].processors = "9"
         self.jobs[1]._processors = "9"
+        self.jobs[1]._platform = self.platform
 
 
         self.wrapper_type = options.get('TYPE', 'vertical')
         self.wrapper_policy = options.get('POLICY', 'flexible')
         self.wrapper_method = options.get('METHOD', 'ASThread')
         self.jobs_in_wrapper = options.get('JOBS_IN_WRAPPER', 'None')
         self.extensible_wallclock = options.get('EXTEND_WALLCLOCK', 0)
@@ -149,15 +144,15 @@
         self.setUpWrappers(options_slurm)
         self.assertEqual(self.job_package_wrapper._wrapper_data["EXCLUSIVE"], False)
         self.assertEqual(self.job_package_wrapper._wrapper_data["INNER_RETRIALS"], 30)
         self.assertEqual(self.job_package_wrapper._wrapper_data["QUEUE"], "bsc32")
         self.assertEqual(self.job_package_wrapper._wrapper_data["PARTITION"], "bsc32")
         self.assertEqual(self.job_package_wrapper._wrapper_data["THREADS"], "30")
         self.assertEqual(self.job_package_wrapper._wrapper_data["TASKS"], "40")
-        self.assertEqual(self.job_package_wrapper._wrapper_data["CUSTOM_DIRECTIVES"], "['#SBATCH --mem=1000']")
+        self.assertEqual(self.job_package_wrapper._wrapper_data["CUSTOM_DIRECTIVES"], ['#SBATCH --mem=1000'])
 
 
 
     def test_job_package_default_init(self):
         with self.assertRaises(Exception):
             JobPackageSimple([])
```

### Comparing `autosubmit-4.0.84/test/unit/test_log.py` & `autosubmit-4.0.85/test/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_machinefiles_wrapper.py` & `autosubmit-4.0.85/test/unit/test_machinefiles_wrapper.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_paramiko_platform.py` & `autosubmit-4.0.85/test/unit/test_paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_pjm.py` & `autosubmit-4.0.85/test/unit/test_pjm.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     def read():
         return
 class TestPJM(TestCase):
 
     def setUp(self) -> None:
         self.exp_id = 'a000'
         self.as_conf = MagicMock()
-        self.as_conf = AutosubmitConfig(self.exp_id, FakeBasicConfig, YAMLParserFactory())
+        with patch.object(Path, 'exists') as mock_exists:
+            mock_exists.return_value = True
+            self.as_conf = AutosubmitConfig(self.exp_id, FakeBasicConfig, YAMLParserFactory())
         self.as_conf.experiment_data = dict()
         self.as_conf.experiment_data["DEFAULT"] = dict()
         self.as_conf.experiment_data["DEFAULT"]["HPCARCH"] = "ARM"
         yml_file = Path(__file__).resolve().parent / "files/fake-jobs.yml"
         factory = YAMLParserFactory()
         parser = factory.create_parser()
         parser.data = parser.load(yml_file)
```

### Comparing `autosubmit-4.0.84/test/unit/test_platform_monitor.py` & `autosubmit-4.0.85/test/unit/test_platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_slurm_platform.py` & `autosubmit-4.0.85/test/unit/test_slurm_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_statistics.py` & `autosubmit-4.0.85/test/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_strategies.py` & `autosubmit-4.0.85/test/unit/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit-4.0.84/test/unit/test_wrappers.py` & `autosubmit-4.0.85/test/unit/test_wrappers.py`

 * *Files identical despite different names*

