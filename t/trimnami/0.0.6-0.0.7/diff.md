# Comparing `tmp/trimnami-0.0.6.tar.gz` & `tmp/trimnami-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.0.6.tar", last modified: Thu Jul 13 02:12:45 2023, max compression
+gzip compressed data, was "trimnami-0.0.7.tar", last modified: Tue Aug  8 06:59:26 2023, max compression
```

## Comparing `trimnami-0.0.6.tar` & `trimnami-0.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.227274 trimnami-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-13 02:12:33.000000 trimnami-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-13 02:12:45.227274 trimnami-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-07-13 02:12:33.000000 trimnami-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 02:12:45.227274 trimnami-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-13 02:12:33.000000 trimnami-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.199270 trimnami-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 02:12:33.000000 trimnami-0.0.6/tests/test_skipHostRm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-13 02:12:33.000000 trimnami-0.0.6/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.203270 trimnami-0.0.6/trimnami/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.203270 trimnami-0.0.6/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.203270 trimnami-0.0.6/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/scripts/skipHostRm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.211271 trimnami-0.0.6/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.215272 trimnami-0.0.6/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.215272 trimnami-0.0.6/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.219272 trimnami-0.0.6/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.223273 trimnami-0.0.6/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/fastqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/multiqc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/envs/rasusa.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.223273 trimnami-0.0.6/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/fastqc.smk
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/nanopore.smk
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/notrim.smk
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/rasusa.smk
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-07-13 02:12:33.000000 trimnami-0.0.6/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 02:12:45.203270 trimnami-0.0.6/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 02:12:45.000000 trimnami-0.0.6/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.281526 trimnami-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-08 06:59:12.000000 trimnami-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-08-08 06:59:26.281526 trimnami-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-08-08 06:59:12.000000 trimnami-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 06:59:26.281526 trimnami-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 06:59:12.000000 trimnami-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.265527 trimnami-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 06:59:12.000000 trimnami-0.0.7/tests/test_skipHostRm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-08-08 06:59:12.000000 trimnami-0.0.7/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.265527 trimnami-0.0.7/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.265527 trimnami-0.0.7/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.265527 trimnami-0.0.7/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/scripts/skipHostRm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.273527 trimnami-0.0.7/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   950550 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1016766 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1018716 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1019116 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1418720 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.273527 trimnami-0.0.7/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (123)   350434 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   840483 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)  1942970 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.277526 trimnami-0.0.7/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.277526 trimnami-0.0.7/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (123)   911854 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.277526 trimnami-0.0.7/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/multiqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/envs/rasusa.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.281526 trimnami-0.0.7/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/fastqc.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/nanopore.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/rasusa.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-08-08 06:59:12.000000 trimnami-0.0.7/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 06:59:26.265527 trimnami-0.0.7/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 06:59:26.000000 trimnami-0.0.7/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.0.6/PKG-INFO` & `trimnami-0.0.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: trimnami
-Version: 0.0.6
-Summary: Trim lots of metagenomics samples all at once.
-Home-page: https://github.com/beardymcjohnface/Trimnami
-Author: Michael Roach
-Author-email: beardymcjohnface@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 ![](trimnami.png)
 
 [![](https://img.shields.io/static/v1?label=CLI&message=Snaketool&color=blueviolet)](https://github.com/beardymcjohnface/Snaketool)
 [![](https://img.shields.io/static/v1?label=Licence&message=MIT&color=black)](https://opensource.org/license/mit/)
 [![](https://img.shields.io/static/v1?label=Install%20with&message=PIP&color=success)](https://pypi.org/project/trimnami/)
 ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/beardymcjohnface/Trimnami/main)
 [![Unit tests](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml/badge.svg)](https://github.com/beardymcjohnface/Trimnami/actions/workflows/python-app.yml)
@@ -130,68 +120,82 @@
 ## Outputs
 
 Trimmed reads will be saved in various subfolders in the output directory.
 e.g. if trimming with Fastp or Prinseq++, 
 trimmed reads will be in `trimnami.out/fastp/` or `trimnami.out/prinseq/`.
 Paired reads will yield three files: 
 The R1 and R2 paired reads, and any singletons from trimming or host removal.
+Subsampling will produce extra files of subsampled trimmed reads.
+Multiqc-fastqc reports for any runs will be available in `trimnami.out/reports/`
 
-
+### Example outputs
 <details>
-    <summary><b>If you run all the tests you should get this</b></summary>
+    <summary>Click to expand</summary>
+
+prinseq
+
+```text
+trimnami.out/
+└── prinseq
+    ├── A13-04-182-06_TAGCTT.paired.R1.fastq.gz
+    ├── A13-04-182-06_TAGCTT.paired.R2.fastq.gz
+    ├── A13-04-182-06_TAGCTT.paired.S.fastq.gz
+    ├── A13-12-250-06_GGCTAC.paired.R1.fastq.gz
+    ├── A13-12-250-06_GGCTAC.paired.R2.fastq.gz
+    ├── A13-12-250-06_GGCTAC.paired.S.fastq.gz
+    └── A13-135-177-06_AGTTCC.single.fastq.gz
+```
+
+prinseq with fastqc reports
 
 ```text
 trimnami.out/
-├── fastp
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.R1.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.R2.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.S.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.paired.R1.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.paired.R2.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.paired.S.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.R1.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.R2.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.S.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.paired.R1.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.paired.R2.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.paired.S.fastq.gz
-│   ├── A13-135-177-06_AGTTCC.host_rm.single.fastq.gz
-│   └── A13-135-177-06_AGTTCC.single.fastq.gz
-├── nanopore
-│   ├── SRR7947171.host_rm.single.fastq.gz
-│   └── SRR7947176.host_rm.single.fastq.gz
 ├── prinseq
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.R1.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.R2.fastq.gz
-│   ├── A13-04-182-06_TAGCTT.host_rm.paired.S.fastq.gz
 │   ├── A13-04-182-06_TAGCTT.paired.R1.fastq.gz
 │   ├── A13-04-182-06_TAGCTT.paired.R2.fastq.gz
 │   ├── A13-04-182-06_TAGCTT.paired.S.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.R1.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.R2.fastq.gz
-│   ├── A13-12-250-06_GGCTAC.host_rm.paired.S.fastq.gz
 │   ├── A13-12-250-06_GGCTAC.paired.R1.fastq.gz
 │   ├── A13-12-250-06_GGCTAC.paired.R2.fastq.gz
 │   ├── A13-12-250-06_GGCTAC.paired.S.fastq.gz
-│   ├── A13-135-177-06_AGTTCC.host_rm.single.fastq.gz
 │   └── A13-135-177-06_AGTTCC.single.fastq.gz
-└── roundAB
+└── reports
+    ├── prinseq.fastqc.html
+    └── untrimmed.fastqc.html
+
+```
+
+prinseq with host removal
+
+```text
+trimnami.out/
+└── prinseq
     ├── A13-04-182-06_TAGCTT.host_rm.paired.R1.fastq.gz
     ├── A13-04-182-06_TAGCTT.host_rm.paired.R2.fastq.gz
     ├── A13-04-182-06_TAGCTT.host_rm.paired.S.fastq.gz
-    ├── A13-04-182-06_TAGCTT.paired.R1.fastq.gz
-    ├── A13-04-182-06_TAGCTT.paired.R2.fastq.gz
-    ├── A13-04-182-06_TAGCTT.paired.S.fastq.gz
     ├── A13-12-250-06_GGCTAC.host_rm.paired.R1.fastq.gz
     ├── A13-12-250-06_GGCTAC.host_rm.paired.R2.fastq.gz
     ├── A13-12-250-06_GGCTAC.host_rm.paired.S.fastq.gz
-    ├── A13-12-250-06_GGCTAC.paired.R1.fastq.gz
-    ├── A13-12-250-06_GGCTAC.paired.R2.fastq.gz
-    ├── A13-12-250-06_GGCTAC.paired.S.fastq.gz
-    ├── A13-135-177-06_AGTTCC.host_rm.single.fastq.gz
-    └── A13-135-177-06_AGTTCC.single.fastq.gz
-
+    └── A13-135-177-06_AGTTCC.host_rm.single.fastq.gz
 ```
 
-</details>
+prinseq with host removal and subsampling
 
+```text
+trimnami.out/
+└── prinseq
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.R1.fastq.gz
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.R1.subsampled.fastq.gz
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.R2.fastq.gz
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.R2.subsampled.fastq.gz
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.S.fastq.gz
+    ├── A13-04-182-06_TAGCTT.host_rm.paired.S.subsampled.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.R1.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.R1.subsampled.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.R2.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.R2.subsampled.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.S.fastq.gz
+    ├── A13-12-250-06_GGCTAC.host_rm.paired.S.subsampled.fastq.gz
+    ├── A13-135-177-06_AGTTCC.host_rm.single.fastq.gz
+    └── A13-135-177-06_AGTTCC.host_rm.single.subsampled.fastq.gz
+```
+</details>
```

### Comparing `trimnami-0.0.6/setup.py` & `trimnami-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,15 @@
     data_files=get_data_files(),
     py_modules=["trimnami"],
     install_requires=[
         "snaketool-utils>=0.0.3",
         "snakemake>=7.14.0",
         "pyyaml>=6.0",
         "Click>=8.1.3",
-        "metasnek>=0.0.4",
-        "attrmap>=0.0.7",
+        "metasnek>=0.0.5",
     ],
     entry_points={
         "console_scripts": [
             "trimnami=trimnami.__main__:main"
         ]
     },
     include_package_data=True,
```

### Comparing `trimnami-0.0.6/tests/test_skipHostRm.py` & `trimnami-0.0.7/tests/test_skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/tests/test_trimnami.py` & `trimnami-0.0.7/tests/test_trimnami.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/__main__.py` & `trimnami-0.0.7/trimnami/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,28 +149,28 @@
 Specify targets:    trimnami run ... all print_targets
 Available targets:
     fastp           Trim reads with fastp (default)
     prinseq         Trim reads with prinseq++
     roundAB         Trim round A/B viral metagenome reads
     nanopore        Trim nanopore reads
     notrim          Skip read trimming
-    print_targets   List available targets
+    print_trimmers  List available trimming modules
 """
 
 
 @click.command(
     epilog=help_msg_extra,
     context_settings=dict(
         help_option_names=["-h", "--help"], ignore_unknown_options=True
     ),
 )
 @click.option("--reads", help="Input file/directory", type=str, required=True)
 @click.option('--host', help='Host genome fasta for filtering', show_default=False, required=False)
 @click.option("--minimap", help="Minimap preset", default="sr", show_default=True,
-              type=click.Choice(["map-pb", "map-ont", "map-hifi", "sr"]))
+              type=click.Choice(["sr", "map-pb", "map-ont", "map-hifi"]))
 @common_options
 def run(**kwargs):
     """Run Trimnami"""
     # Config to add or update in configfile
     merge_config = {
         "trimnami": {
             "args": {
```

### Comparing `trimnami-0.0.6/trimnami/config/config.yaml` & `trimnami-0.0.7/trimnami/config/config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 resources:
     med:
         mem: 16000
         cpu: 8
-        time: 240
+        time: "04:00:00"
 trimnami:
     qc:
         compression:
             1
         minimapIndex:
             -I 8G
+        hostRemoveFlagstat:
+            -f 4
+            -F 3584
         fastp:
             --qualified_quality_phred 15
             --length_required 90
             --cut_tail 
             --cut_tail_window_size 25
             --cut_tail_mean_quality 15
             --dedup
@@ -31,10 +34,8 @@
             -trim_qual_type min 
             -trim_qual_left 30
             -trim_qual_right 30 
             -trim_qual_window 10
         nanopore:
             filtlong:
                 --min_length 1000
-                --keep_percent 95
-            rasusa:
-                --bases 10000000
+                --keep_percent 95
```

### Comparing `trimnami-0.0.6/trimnami/config/system_config.yaml` & `trimnami-0.0.7/trimnami/config/system_config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 trimnami:
+    trimmers:
+    - fastp
+    - prinseq
+    - roundAB
+    - nanopore
+    - notrim
     args:
         reads:
         output:
         host:
         minimap:
         fastqc:
         subsample:
```

### Comparing `trimnami-0.0.6/trimnami/scripts/skipHostRm.py` & `trimnami-0.0.7/trimnami/scripts/skipHostRm.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.0.7/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.0.7/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/test_data/ref.fna` & `trimnami-0.0.7/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/trimnami.LICENSE` & `trimnami-0.0.7/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.0.7/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/workflow/databases/primerB.fa` & `trimnami-0.0.7/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.0.7/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.0.7/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.0.6/trimnami/workflow/rules/fastp.smk` & `trimnami-0.0.7/trimnami/workflow/rules/fastp.smk`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,43 @@
+@target_rule
+rule fastp:
+    input:
+        targets["fastp"],
+        targets["reports"]
+
+
 rule fastp_paired_end:
     """Read trimming with fastp for paired reads"""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.fastq.gz"),
-        r2=os.path.join(dir.temp,"{file}.R2.fastq.gz"),
-        s=os.path.join(dir.temp,"{file}.S.fastq.gz"),
+        r1=os.path.join(dir["temp"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["temp"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["temp"],"{sample}_S{host}.fastq.gz"),
     output:
-        r1=os.path.join(dir.fastp,"{file}.R1.fastq.gz"),
-        r2=os.path.join(dir.fastp,"{file}.R2.fastq.gz"),
-        s=os.path.join(dir.fastp,"{file}.S.fastq.gz"),
-        s1=temp(os.path.join(dir.fastp,"{file}.S1.fastq.gz")),
-        s2=temp(os.path.join(dir.fastp,"{file}.S2.fastq.gz")),
-        stats=temp(os.path.join(dir.fastp,"{file}.stats.json")),
-        html=temp(os.path.join(dir.fastp,"{file}.stats.html"))
+        r1=os.path.join(dir["fastp"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["fastp"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["fastp"],"{sample}_S{host}.fastq.gz"),
+        s1=temp(os.path.join(dir["fastp"],"{sample}_S1{host}.fastq.gz")),
+        s2=temp(os.path.join(dir["fastp"],"{sample}_S2{host}.fastq.gz")),
+        stats=temp(os.path.join(dir["fastp"],"{sample}{host}.stats.json")),
+        html=temp(os.path.join(dir["fastp"],"{sample}{host}.stats.html"))
     benchmark:
-        os.path.join(dir.bench,"fastp.{file}.txt")
+        os.path.join(dir["bench"],"fastp.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"fastp.{file}.log")
+        os.path.join(dir["log"],"fastp.{sample}{host}.log")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     conda:
-        os.path.join(dir.env,"fastp.yaml")
+        os.path.join(dir["env"],"fastp.yaml")
     params:
-        fastp=config.fastp,
-        compression=config.qc.compression
+        fastp=config["qc"]["fastp"],
+        compression=config["qc"]["compression"]
     shell:
         """
         fastp \
             -i {input.r1} \
             -I {input.r2} \
             -o {output.r1} \
             -O {output.r2} \
@@ -58,33 +66,34 @@
         cat {output.s1} {output.s2} >> {output.s}
         """
 
 
 rule fastp_single_end:
     """Read trimming with fastp for single end reads"""
     input:
-        r1=os.path.join(dir.temp,"{file}.single.fastq.gz"),
+        r1=os.path.join(dir["temp"],"{sample}_single{host}.fastq.gz"),
     output:
-        r1=os.path.join(dir.fastp,"{file}.single.fastq.gz"),
-        stats=temp(os.path.join(dir.fastp,"{file}.stats.json")),
-        html=temp(os.path.join(dir.fastp,"{file}.stats.html"))
+        r1=os.path.join(dir["fastp"],"{sample}_single{host}.fastq.gz"),
+        stats=temp(os.path.join(dir["fastp"],"{sample}{host}.stats.json")),
+        html=temp(os.path.join(dir["fastp"],"{sample}{host}.stats.html"))
     benchmark:
-        os.path.join(dir.bench,"fastp.{file}.txt")
+        os.path.join(dir["bench"],"fastp.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"fastp.{file}.log")
+        os.path.join(dir["log"],"fastp.{sample}{host}.log")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     conda:
-        os.path.join(dir.env,"fastp.yaml")
+        os.path.join(dir["env"],"fastp.yaml")
     params:
-        fastp=config.fastp,
-        compression=config.qc.compression
+        fastp=config["qc"]["fastp"],
+        compression=config["qc"]["compression"]
     shell:
         """
         fastp \
             -i {input.r1} \
             -o {output.r1} \
             -z {params.compression} \
             -j {output.stats} \
```

### Comparing `trimnami-0.0.6/trimnami/workflow/rules/fastqc.smk` & `trimnami-0.0.7/trimnami/workflow/rules/fastqc.smk`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 rule fastqc_paired_untrimmed:
     input:
-        r1 = lambda wildcards: samples.reads[wildcards.sample]["R1"],
-        r2 = lambda wildcards: samples.reads[wildcards.sample]["R2"],
+        r1 = lambda wildcards: samples["reads"][wildcards.sample]["R1"],
+        r2 = lambda wildcards: samples["reads"][wildcards.sample]["R2"],
     output:
-        z1 = temp(os.path.join(dir.reports,"untrimmed","{sample}.paired.R1_fastqc.zip")),
-        z2 = temp(os.path.join(dir.reports,"untrimmed","{sample}.paired.R2_fastqc.zip")),
-        t=touch(temp(os.path.join(dir.temp,"{sample}.untrimmed.fastqc")))
+        z1 = temp(os.path.join(dir["reports"],"untrimmed","{sample}_R1_fastqc.zip")),
+        z2 = temp(os.path.join(dir["reports"],"untrimmed","{sample}_R2_fastqc.zip")),
+        t=touch(temp(os.path.join(dir["temp"],"{sample}.untrimmed.fastqc")))
     params:
-        dir = dir.temp,
-        r1 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R1"])) + "_fastqc.html"),
-        r2 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R2"])) + "_fastqc.html"),
-        z1 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R1"])) + "_fastqc.zip"),
-        z2 = lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R2"])) + "_fastqc.zip"),
+        dir = dir["temp"],
+        r1 = lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R1"])) + "_fastqc.html"),
+        r2 = lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R2"])) + "_fastqc.html"),
+        z1 = lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R1"])) + "_fastqc.zip"),
+        z2 = lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R2"])) + "_fastqc.zip"),
     conda:
-        os.path.join(dir.env, "fastqc.yaml")
+        os.path.join(dir["env"], "fastqc.yaml")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     log:
-        os.path.join(dir.log, "fastqc_paired_untrimmed.{sample}.log")
+        os.path.join(dir["log"], "fastqc_paired_untrimmed.{sample}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_paired_untrimmed.{sample}.txt")
+        os.path.join(dir["bench"],"fastqc_paired_untrimmed.{sample}.txt")
     shell:
         """
         fastqc {input} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
         
@@ -38,77 +39,77 @@
         mv {params.z2} {output.z2}
         rm {params.r1} {params.r2}
         """
 
 
 rule fastqc_unpaired_untrimmed:
     input:
-        r1=lambda wildcards: samples.reads[wildcards.sample]["R1"],
+        r1=lambda wildcards: samples["reads"][wildcards.sample]["R1"],
     output:
-        z1=temp(os.path.join(dir.reports,"untrimmed","{sample}.untrimmed.single_fastqc.zip")),
-        t=touch(temp(os.path.join(dir.temp,"{sample}.untrimmed.fastqc")))
+        z1=temp(os.path.join(dir["reports"],"untrimmed","{sample}.untrimmed_single_fastqc.zip")),
+        t=touch(temp(os.path.join(dir["temp"],"{sample}.untrimmed.fastqc")))
     params:
-        dir=dir.temp,
-        r1=lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R1"])) + "_fastqc.html"),
-        z1=lambda wildcards: os.path.join(dir.temp,re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
-            samples.reads[wildcards.sample]["R1"])) + "_fastqc.zip"),
+        dir=dir["temp"],
+        r1=lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R1"])) + "_fastqc.html"),
+        z1=lambda wildcards: os.path.join(dir["temp"],re.sub(r"\.(fasta|fastq)(\.gz)?$","",os.path.basename(
+            samples["reads"][wildcards.sample]["R1"])) + "_fastqc.zip"),
     conda:
-        os.path.join(dir.env,"fastqc.yaml")
+        os.path.join(dir["env"],"fastqc.yaml")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     log:
-        os.path.join(dir.log,"fastqc_unpaired_untrimmed.{sample}.log")
+        os.path.join(dir["log"],"fastqc_unpaired_untrimmed.{sample}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_unpaired_untrimmed.{sample}.txt")
+        os.path.join(dir["bench"],"fastqc_unpaired_untrimmed.{sample}.txt")
     shell:
         """
         fastqc {input} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
 
         mv {params.z1} {output.z1}
         rm {params.r1}
         """
 
 
 rule fastqc_paired_trimmed:
     input:
-        r1 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R1{subsampled}.fastq.gz"),
-        r2 = os.path.join(dir.out, "{trimmer}", "{sample}.paired.R2{subsampled}.fastq.gz"),
-        rs = os.path.join(dir.out, "{trimmer}", "{sample}.paired.S{subsampled}.fastq.gz"),
+        r1 = os.path.join(dir["out"], "{trimmer}", "{sample}_R1{hostSubsampled}.fastq.gz"),
+        r2 = os.path.join(dir["out"], "{trimmer}", "{sample}_R2{hostSubsampled}.fastq.gz"),
+        rs = os.path.join(dir["out"], "{trimmer}", "{sample}_S{hostSubsampled}.fastq.gz"),
     output:
-        r1 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.html")),
-        r2 = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.html")),
-        rs = temp(os.path.join(dir.temp,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.html")),
-        z1 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.zip")),
-        z2 = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.zip")),
-        zs = temp(os.path.join(dir.reports,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.zip")),
+        r1 = temp(os.path.join(dir["temp"],"{trimmer}","{sample}_R1{hostSubsampled}_fastqc.html")),
+        r2 = temp(os.path.join(dir["temp"],"{trimmer}","{sample}_R2{hostSubsampled}_fastqc.html")),
+        rs = temp(os.path.join(dir["temp"],"{trimmer}","{sample}_S{hostSubsampled}_fastqc.html")),
+        z1 = temp(os.path.join(dir["reports"],"{trimmer}","{sample}_R1{hostSubsampled}_fastqc.zip")),
+        z2 = temp(os.path.join(dir["reports"],"{trimmer}","{sample}_R2{hostSubsampled}_fastqc.zip")),
+        zs = temp(os.path.join(dir["reports"],"{trimmer}","{sample}_S{hostSubsampled}_fastqc.zip")),
     params:
-        dir = os.path.join(dir.temp,"{trimmer}"),
-        z1 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R1{subsampled}_fastqc.zip"),
-        z2 = os.path.join(dir.temp,"{trimmer}","{sample}.paired.R2{subsampled}_fastqc.zip"),
-        zs = os.path.join(dir.temp,"{trimmer}","{sample}.paired.S{subsampled}_fastqc.zip"),
-    wildcard_constraints:
-        subsampled = ".{0}|\.subsampled"
+        dir = os.path.join(dir["temp"],"{trimmer}"),
+        z1 = os.path.join(dir["temp"],"{trimmer}","{sample}_R1{hostSubsampled}_fastqc.zip"),
+        z2 = os.path.join(dir["temp"],"{trimmer}","{sample}_R2{hostSubsampled}_fastqc.zip"),
+        zs = os.path.join(dir["temp"],"{trimmer}","{sample}_S{hostSubsampled}_fastqc.zip"),
     conda:
-        os.path.join(dir.env, "fastqc.yaml")
+        os.path.join(dir["env"], "fastqc.yaml")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     log:
-        os.path.join(dir.log, "fastqc_paired_trimmed.{sample}.{trimmer}{subsampled}.log")
+        os.path.join(dir["log"], "fastqc_paired_trimmed.{sample}.{trimmer}{hostSubsampled}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_paired_trimmed.{sample}.{trimmer}{subsampled}.txt")
+        os.path.join(dir["bench"],"fastqc_paired_trimmed.{sample}.{trimmer}{hostSubsampled}.txt")
     shell:
         """
         fastqc {input.r1} {input.r2} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
         
@@ -126,55 +127,54 @@
         mv {params.z2} {output.z2}
         mv {params.zs} {output.zs}
         """
 
 
 rule fastqc_single_trimmed:
     input:
-        os.path.join(dir.out,"{trimmer}","{sample}.single{subsampled}.fastq.gz"),
+        os.path.join(dir["out"],"{trimmer}","{sample}_single{hostSubsampled}.fastq.gz"),
     output:
-        r=temp(os.path.join(dir.temp,"{trimmer}","{sample}.single{subsampled}_fastqc.html")),
-        z=temp(os.path.join(dir.reports,"{trimmer}","{sample}.single{subsampled}_fastqc.zip")),
+        r=temp(os.path.join(dir["temp"],"{trimmer}","{sample}_single{hostSubsampled}_fastqc.html")),
+        z=temp(os.path.join(dir["reports"],"{trimmer}","{sample}_single{hostSubsampled}_fastqc.zip")),
     params:
-        dir=os.path.join(dir.temp,"{trimmer}"),
-        z=os.path.join(dir.temp,"{trimmer}","{sample}.single{subsampled}_fastqc.zip"),
-    wildcard_constraints:
-        subsampled = ".{0}|\.subsampled"
+        dir=os.path.join(dir["temp"],"{trimmer}"),
+        z=os.path.join(dir["temp"],"{trimmer}","{sample}_single{hostSubsampled}_fastqc.zip"),
     conda:
-        os.path.join(dir.env,"fastqc.yaml")
+        os.path.join(dir["env"],"fastqc.yaml")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     log:
-        os.path.join(dir.log,"fastqc_single_trimmed.{sample}.{trimmer}{subsampled}.log")
+        os.path.join(dir["log"],"fastqc_single_trimmed.{sample}.{trimmer}{hostSubsampled}.log")
     benchmark:
-        os.path.join(dir.bench,"fastqc_single_trimmed.{sample}.{trimmer}{subsampled}.txt")
+        os.path.join(dir["bench"],"fastqc_single_trimmed.{sample}.{trimmer}{hostSubsampled}.txt")
     shell:
         """
         fastqc {input} \
             -t {threads} \
             --outdir {params.dir} \
             &> {log}
 
         mv {params.z} {output.z}
         """
 
 
 rule multiqc_fastqc:
     input:
-        lambda wildcards: targets.fastqc[wildcards.trimmer]
+        lambda wildcards: targets["fastqc"][wildcards.trimmer]
     output:
-        os.path.join(dir.reports, "{trimmer}.fastqc.html")
+        os.path.join(dir["reports"], "{trimmer}.fastqc.html")
     params:
-        dir=os.path.join(dir.reports, "{trimmer}")
+        dir=os.path.join(dir["reports"], "{trimmer}")
     conda:
-        os.path.join(dir.env,"multiqc.yaml")
+        os.path.join(dir["env"],"multiqc.yaml")
     log:
-        os.path.join(dir.log,"multiqc_fastqc.{trimmer}.log")
+        os.path.join(dir["log"],"multiqc_fastqc.{trimmer}.log")
     benchmark:
-        os.path.join(dir.bench,"multiqc_fastqc.{trimmer}.txt")
+        os.path.join(dir["bench"],"multiqc_fastqc.{trimmer}.txt")
     shell:
         """
         multiqc {params.dir} -n {output} --no-data-dir 2> {log}
         """
```

### Comparing `trimnami-0.0.6/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.0.7/trimnami/workflow/rules/hostRemoval.smk`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,130 @@
 rule index_host_genome:
     """Pre-index the host genome for mapping with minimap2"""
     input:
-        lambda wildcards: config.args.host if config.args.host else ""
+        lambda wildcards: config["args"]["host"] if config["args"]["host"] else ""
     output:
-        config.args.hostIndex
+        config["args"]["hostIndex"]
     params:
-        params = config.qc.minimapIndex
+        params = config["qc"]["minimapIndex"]
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     conda:
-        os.path.join(dir.env,"minimap2.yaml")
+        os.path.join(dir["env"],"minimap2.yaml")
     benchmark:
-        os.path.join(dir.bench,"index_host_genome.txt")
+        os.path.join(dir["bench"],"index_host_genome.txt")
     log:
-        os.path.join(dir.log,"index_host_genome.log")
+        os.path.join(dir["log"],"index_host_genome.log")
     shell:
         """minimap2 -t {threads} {params} -d {output} {input} &> {log}"""
 
 
 rule host_removal_mapping_paired:
     """Map reads to host and return unmapped reads"""
     input:
-        r1=lambda wildcards: samples.reads[wildcards.sample]["R1"],
-        r2=lambda wildcards: samples.reads[wildcards.sample]["R2"],
-        host=lambda wildcards: config.args.hostIndex if config.args.host else ""
+        r1=lambda wildcards: samples["reads"][wildcards.sample]["R1"],
+        r2=lambda wildcards: samples["reads"][wildcards.sample]["R2"],
+        host=lambda wildcards: config["args"]["hostIndex"] if config["args"]["host"] else ""
     output:
-        r1=temp(os.path.join(dir.temp,"{sample}.host_rm.paired.R1.fastq.gz")),
-        r2=temp(os.path.join(dir.temp,"{sample}.host_rm.paired.R2.fastq.gz")),
-        s=temp(os.path.join(dir.temp,"{sample}.host_rm.paired.S.fastq.gz")),
-        o=temp(os.path.join(dir.temp,"{sample}.host_rm.paired.O.fastq.gz")),
+        r1=temp(os.path.join(dir["temp"],"{sample}_R1.host_rm.fastq.gz")),
+        r2=temp(os.path.join(dir["temp"],"{sample}_R2.host_rm.fastq.gz")),
+        s=temp(os.path.join(dir["temp"],"{sample}_S.host_rm.fastq.gz")),
+        o=temp(os.path.join(dir["temp"],"{sample}_0.host_rm.fastq.gz")),
     params:
-        compression=config.qc.compression
+        compression=config["qc"]["compression"],
+        minimap_mode=config["args"]["minimap"],
+        flagFilt=config["qc"]["hostRemoveFlagstat"]
     benchmark:
-        os.path.join(dir.bench,"host_removal_mapping.{sample}.txt")
+        os.path.join(dir["bench"],"host_removal_mapping.{sample}.txt")
     log:
-        mm=os.path.join(dir.log,"host_removal_mapping.{sample}.minimap.log"),
-        sv=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsView.log"),
-        fq=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsFastq.log"),
+        mm=os.path.join(dir["log"],"host_removal_mapping.{sample}.minimap.log"),
+        sv=os.path.join(dir["log"],"host_removal_mapping.{sample}.samtoolsView.log"),
+        fq=os.path.join(dir["log"],"host_removal_mapping.{sample}.samtoolsFastq.log"),
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     conda:
-        os.path.join(dir.env,"minimap2.yaml")
+        os.path.join(dir["env"],"minimap2.yaml")
     shell:
         """
-        minimap2 -ax sr -t {threads} --secondary=no {input.host} {input.r1} {input.r2} 2> {log.mm} \
-            | samtools view -f 4 -h 2> {log.sv} \
-            | samtools fastq -NO -c {params.compression} -1 {output.r1} -2 {output.r2} -0 {output.o} -s {output.s} 2> {log.fq}
+        minimap2 -ax {params.minimap_mode} -t {threads} --secondary=no {input.host} {input.r1} {input.r2} 2> {log.mm} \
+            | samtools view -h {params.flagFilt} 2> {log.sv} \
+            | samtools fastq -N -O -c {params.compression} -1 {output.r1} -2 {output.r2} -0 {output.o} -s {output.s} 2> {log.fq}
         cat {output.o} >> {output.s}
         """
 
 
 rule host_removal_mapping_single:
     """Map reads to host and return unmapped reads"""
     input:
-        r1=lambda wildcards: samples.reads[wildcards.sample]["R1"],
-        host=lambda wildcards: config.args.hostIndex if config.args.host else ""
+        r1=lambda wildcards: samples["reads"][wildcards.sample]["R1"],
+        host=lambda wildcards: config["args"]["hostIndex"] if config["args"]["host"] else ""
     output:
-        r1=temp(os.path.join(dir.temp,"{sample}.host_rm.single.fastq.gz")),
-        s=temp(os.path.join(dir.temp,"{sample}.host_rm.single.S.fastq.gz")),
-        o=temp(os.path.join(dir.temp,"{sample}.host_rm.single.O.fastq.gz")),
+        r1=temp(os.path.join(dir["temp"],"{sample}_single.host_rm.fastq.gz")),
+        s=temp(os.path.join(dir["temp"],"{sample}_single.host_rm.S.fastq.gz")),
+        o=temp(os.path.join(dir["temp"],"{sample}_single.host_rm.O.fastq.gz")),
     params:
-        compression=config.qc.compression,
-        minimap_mode=config.args.minimap
+        compression=config["qc"]["compression"],
+        minimap_mode=config["args"]["minimap"],
+        flagFilt=config["qc"]["hostRemoveFlagstat"]
     benchmark:
-        os.path.join(dir.bench,"host_removal_mapping.{sample}.txt")
+        os.path.join(dir["bench"],"host_removal_mapping.{sample}.txt")
     log:
-        mm=os.path.join(dir.log,"host_removal_mapping.{sample}.minimap.log"),
-        sv=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsView.log"),
-        fq=os.path.join(dir.log,"host_removal_mapping.{sample}.samtoolsFastq.log")
+        mm=os.path.join(dir["log"],"host_removal_mapping.{sample}.minimap.log"),
+        sv=os.path.join(dir["log"],"host_removal_mapping.{sample}.samtoolsView.log"),
+        fq=os.path.join(dir["log"],"host_removal_mapping.{sample}.samtoolsFastq.log")
     resources:
-        mem_mb=resources.med.mem,
-        time=resources.med.time
+        mem_mb=resources["med"]["mem"],
+        mem=str(resources["med"]["mem"]) + "MB",
+        time=resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     conda:
-        os.path.join(dir.env,"minimap2.yaml")
+        os.path.join(dir["env"],"minimap2.yaml")
     shell:
         """
         minimap2 -ax {params.minimap_mode} -t {threads} --secondary=no {input.host} {input.r1} 2> {log.mm} \
-            | samtools view -f 4 -h 2> {log.sv} \
-            | samtools fastq -nO -c {params.compression} -o {output.r1} -0 {output.o} -s {output.s} 2> {log.fq}
+            | samtools view -h {params.flagFilt} 2> {log.sv} \
+            | samtools fastq -n -O -c {params.compression} -o {output.r1} -0 {output.o} -s {output.s} 2> {log.fq}
         cat {output.o} {output.s} >> {output.r1}
         """
 
 
 rule skip_host_rm_paired:
     """Skip host removal of paired reads"""
     input:
-        r1 = lambda wildcards: samples.reads[wildcards.sample]["R1"],
-        r2 = lambda wildcards: samples.reads[wildcards.sample]["R2"],
+        r1 = lambda wildcards: samples["reads"][wildcards.sample]["R1"],
+        r2 = lambda wildcards: samples["reads"][wildcards.sample]["R2"],
     output:
-        r1 = temp(os.path.join(dir.temp,"{sample}.paired.R1.fastq.gz")),
-        r2 = temp(os.path.join(dir.temp,"{sample}.paired.R2.fastq.gz")),
-        s = temp(os.path.join(dir.temp,"{sample}.paired.S.fastq.gz")),
+        r1 = temp(os.path.join(dir["temp"],"{sample}_R1.fastq.gz")),
+        r2 = temp(os.path.join(dir["temp"],"{sample}_R2.fastq.gz")),
+        s = temp(os.path.join(dir["temp"],"{sample}_S.fastq.gz")),
     params:
         is_paired = True
     localrule:
         True
     log:
-        stderr = os.path.join(dir.log, "skip_host_rm_pair.{sample}.err"),
-        stdout = os.path.join(dir.log, "skip_host_rm_pair.{sample}.out")
+        stderr = os.path.join(dir["log"], "skip_host_rm_pair.{sample}.err"),
+        stdout = os.path.join(dir["log"], "skip_host_rm_pair.{sample}.out")
     script:
-        os.path.join(dir.scripts, "skipHostRm.py")
+        os.path.join(dir["scripts"], "skipHostRm.py")
 
 
 rule skip_host_rm_single:
     """Skip host removal of paired reads"""
     input:
-        r1 = lambda wildcards: samples.reads[wildcards.sample]["R1"],
+        r1 = lambda wildcards: samples["reads"][wildcards.sample]["R1"],
     output:
-        r1 = temp(os.path.join(dir.temp,"{sample}.single.fastq.gz")),
+        r1 = temp(os.path.join(dir["temp"],"{sample}_single.fastq.gz")),
     params:
         is_paired = False
     localrule:
         True
     script:
-        os.path.join(dir.scripts, "skipHostRm.py")
+        os.path.join(dir["scripts"], "skipHostRm.py")
```

### Comparing `trimnami-0.0.6/trimnami/workflow/rules/notrim.smk` & `trimnami-0.0.7/trimnami/workflow/rules/notrim.smk`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,39 @@
+@target_rule
+rule notrim:
+    input:
+        targets["notrim"],
+        targets["reports"]
+
+
 rule notrim_paired_end:
     """Skip read trimming for paired reads"""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.fastq.gz"),
-        r2=os.path.join(dir.temp,"{file}.R2.fastq.gz"),
-        s=os.path.join(dir.temp,"{file}.S.fastq.gz"),
+        r1=os.path.join(dir["temp"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["temp"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["temp"],"{sample}_S{host}.fastq.gz"),
     output:
-        r1=os.path.join(dir.notrim,"{file}.R1.fastq.gz"),
-        r2=os.path.join(dir.notrim,"{file}.R2.fastq.gz"),
-        s=os.path.join(dir.notrim,"{file}.S.fastq.gz"),
+        r1=os.path.join(dir["notrim"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["notrim"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["notrim"],"{sample}_S{host}.fastq.gz"),
     localrule:
         True
     shell:
         """
         ln {input.r1} {output.r1}
         ln {input.r2} {output.r2}
         ln {input.s} {output.s}
         """
 
 
 rule notrim_single_end:
     """Skip read trimming for single end"""
     input:
-        r1=os.path.join(dir.temp,"{file}.single.fastq.gz"),
+        r1=os.path.join(dir["temp"],"{sample}_single{host}.fastq.gz"),
     output:
-        r1=os.path.join(dir.notrim,"{file}.single.fastq.gz"),
+        r1=os.path.join(dir["notrim"],"{sample}_single{host}.fastq.gz"),
     localrule:
         True
     shell:
         """
         ln {input.r1} {output.r1}
         """
```

### Comparing `trimnami-0.0.6/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.0.7/trimnami/workflow/rules/roundAB.smk`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,40 @@
+@target_rule
+rule roundAB:
+    input:
+        targets["roundAB"],
+        targets["reports"]
+
+
 rule remove_5prime_primer:
     """Round A/B step 01: Remove 5' primer."""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.fastq.gz"),
-        r2=os.path.join(dir.temp,"{file}.R2.fastq.gz"),
-        s=os.path.join(dir.temp,"{file}.S.fastq.gz"),
-        primers=os.path.join(dir.db,"primerB.fa")
+        r1=os.path.join(dir["temp"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["temp"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["temp"],"{sample}_S{host}.fastq.gz"),
+        primers=os.path.join(dir["db"],"primerB.fa")
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s1.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s1.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s1.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s1.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s1.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s1.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_5prime_primer.{file}.txt")
+        os.path.join(dir["bench"],"remove_5prime_primer.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_5prime_primer.{file}.log")
+        os.path.join(dir["log"],"remove_5prime_primer.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_5p
+        params = config["qc"]["bbduk"]["rm_5p"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -52,36 +60,37 @@
         fi
         """
 
 
 rule remove_3prime_contaminant:
     """Round A/B step 02: Remove 3' read through contaminant."""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.s1.fastq"),
-        r2=os.path.join(dir.temp,"{file}.R2.s1.fastq"),
-        s=os.path.join(dir.temp,"{file}.S.s1.fastq"),
-        primers=os.path.join(dir.db,"rc_primerB_ad6.fa")
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s1.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s1.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s1.fastq"),
+        primers=os.path.join(dir["db"],"rc_primerB_ad6.fa")
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s2.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s2.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s2.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s2.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s2.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s2.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_3prime_contaminant.{file}.txt")
+        os.path.join(dir["bench"],"remove_3prime_contaminant.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_3prime_contaminant.{file}.log")
+        os.path.join(dir["log"],"remove_3prime_contaminant.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_3rt
+        params = config["qc"]["bbduk"]["rm_3rt"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -107,36 +116,37 @@
         fi
         """
 
 
 rule remove_primer_free_adapter:
     """Round A/B step 03: Remove primer free adapter (both orientations)."""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.s2.fastq"),
-        r2=os.path.join(dir.temp,"{file}.R2.s2.fastq"),
-        s=os.path.join(dir.temp,"{file}.S.s2.fastq"),
-        primers=os.path.join(dir.db,"nebnext_adapters.fa")
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s2.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s2.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s2.fastq"),
+        primers=os.path.join(dir["db"],"nebnext_adapters.fa")
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s3.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s3.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s3.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s3.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s3.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s3.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_primer_free_adapter.{file}.txt")
+        os.path.join(dir["bench"],"remove_primer_free_adapter.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_primer_free_adapter.{file}.log")
+        os.path.join(dir["log"],"remove_primer_free_adapter.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.neb
+        params = config["qc"]["bbduk"]["neb"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -162,36 +172,37 @@
         fi
         """
 
 
 rule remove_adapter_free_primer:
     """Round A/B step 04: Remove adapter free primer (both orientations)."""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.s3.fastq"),
-        r2=os.path.join(dir.temp,"{file}.R2.s3.fastq"),
-        s=os.path.join(dir.temp,"{file}.S.s3.fastq"),
-        primers=os.path.join(dir.db,"rc_primerB_ad6.fa")
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s3.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s3.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s3.fastq"),
+        primers=os.path.join(dir["db"],"rc_primerB_ad6.fa")
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s4.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s4.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s4.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s4.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s4.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s4.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_adapter_free_primer.{file}.txt")
+        os.path.join(dir["bench"],"remove_adapter_free_primer.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_adapter_free_primer.{file}.log")
+        os.path.join(dir["log"],"remove_adapter_free_primer.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_afp
+        params = config["qc"]["bbduk"]["rm_afp"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -217,36 +228,37 @@
         fi
         """
 
 
 rule remove_vector_contamination:
     """Round A/B step 05: Vector contamination removal (PhiX + NCBI UniVecDB)"""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.s4.fastq"),
-        r2=os.path.join(dir.temp,"{file}.R2.s4.fastq"),
-        s=os.path.join(dir.temp,"{file}.S.s4.fastq"),
-        primers=os.path.join(dir.db,"vector_contaminants.fa")
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s4.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s4.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s4.fastq"),
+        primers=os.path.join(dir["db"],"vector_contaminants.fa")
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s5.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s5.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s5.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s5.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s5.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s5.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_vector_contamination.{file}.txt")
+        os.path.join(dir["bench"],"remove_vector_contamination.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_vector_contamination.{file}.log")
+        os.path.join(dir["log"],"remove_vector_contamination.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_vc
+        params = config["qc"]["bbduk"]["rm_vc"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -272,35 +284,36 @@
         fi
         """
 
 
 rule remove_low_quality:
     """Round A/B step 06: Remove remaining low-quality bases and short reads."""
     input:
-        r1=os.path.join(dir.temp,"{file}.R1.s5.fastq"),
-        r2=os.path.join(dir.temp,"{file}.R2.s5.fastq"),
-        s=os.path.join(dir.temp,"{file}.S.s5.fastq"),
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s5.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s5.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s5.fastq"),
     output:
-        r1=temp(os.path.join(dir.temp,"{file}.R1.s6.fastq")),
-        r2=temp(os.path.join(dir.temp,"{file}.R2.s6.fastq")),
-        s=temp(os.path.join(dir.temp,"{file}.S.s6.fastq")),
+        r1=temp(os.path.join(dir["temp"],"{sample}.R1{host}.s6.fastq")),
+        r2=temp(os.path.join(dir["temp"],"{sample}.R2{host}.s6.fastq")),
+        s=temp(os.path.join(dir["temp"],"{sample}.S{host}.s6.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_low_quality.{file}.txt")
+        os.path.join(dir["bench"],"remove_low_quality.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_low_quality.{file}.log")
+        os.path.join(dir["log"],"remove_low_quality.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_lq
+        params = config["qc"]["bbduk"]["rm_lq"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             in2={input.r2} \
@@ -324,67 +337,69 @@
         fi
         """
 
 
 rule zip_roundAB:
     """Zip the final trimmed reads for Round A/B"""
     input:
-        r1 = os.path.join(dir.temp,"{file}.R1.s6.fastq"),
-        r2 = os.path.join(dir.temp,"{file}.R2.s6.fastq"),
-        s = os.path.join(dir.temp,"{file}.S.s6.fastq"),
+        r1=os.path.join(dir["temp"],"{sample}.R1{host}.s6.fastq"),
+        r2=os.path.join(dir["temp"],"{sample}.R2{host}.s6.fastq"),
+        s=os.path.join(dir["temp"],"{sample}.S{host}.s6.fastq"),
     output:
-        r1 = os.path.join(dir.roundAB,"{file}.R1.fastq.gz"),
-        r2 = os.path.join(dir.roundAB,"{file}.R2.fastq.gz"),
-        s = os.path.join(dir.roundAB,"{file}.S.fastq.gz")
+        r1=os.path.join(dir["roundAB"],"{sample}_R1{host}.fastq.gz"),
+        r2=os.path.join(dir["roundAB"],"{sample}_R2{host}.fastq.gz"),
+        s=os.path.join(dir["roundAB"],"{sample}_S{host}.fastq.gz"),
     benchmark:
-        os.path.join(dir.bench,"zip_roundAB.{file}.txt")
+        os.path.join(dir["bench"],"zip_roundAB.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"zip_roundAB.{file}.log")
+        os.path.join(dir["log"],"zip_roundAB.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = "00:00:01"
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        compression = config.qc.compression
+        compression = config["qc"]["compression"]
     conda:
-        os.path.join(dir.env, "pigz.yaml")
+        os.path.join(dir["env"], "pigz.yaml")
     group:
         "roundAB"
     shell:
         """
         pigz -p {threads} -{params.compression} -c {input.r1} > {output.r1} 2> {log}
         pigz -p {threads} -{params.compression} -c {input.r2} > {output.r2} 2> {log}
         pigz -p {threads} -{params.compression} -c {input.s} > {output.s} 2> {log}
         """
 
 
 rule roundAB_single_end:
     """Round A/B for single end: This should not occur but this rule is here for testing purposes."""
     input:
-        r1=os.path.join(dir.temp,"{file}.single.fastq.gz"),
+        r1=os.path.join(dir["temp"],"{sample}_single{host}.fastq.gz"),
     output:
-        r1=os.path.join(dir.roundAB,"{file}.single.fastq.gz"),
-        tmp=temp(os.path.join(dir.roundAB,"{file}.single.fastq")),
+        r1=os.path.join(dir["roundAB"],"{sample}_single{host}.fastq.gz"),
+        tmp=temp(os.path.join(dir["temp"],"{sample}_single{host}.fastq")),
     benchmark:
-        os.path.join(dir.bench,"remove_low_quality.{file}.txt")
+        os.path.join(dir["bench"],"remove_low_quality.{sample}{host}.txt")
     log:
-        os.path.join(dir.log,"remove_low_quality.{file}.log")
+        os.path.join(dir["log"],"remove_low_quality.{sample}{host}.log")
     resources:
-        mem_mb = resources.med.mem,
-        javaAlloc = int(0.9 * resources.med.mem),
-        time = int(0.5 * resources.med.time)
+        mem_mb = resources["med"]["mem"],
+        mem = str(resources["med"]["mem"]) + "MB",
+        javaAlloc = int(0.9 * resources["med"]["mem"]),
+        time = resources["med"]["time"]
     threads:
-        resources.med.cpu
+        resources["med"]["cpu"]
     params:
-        params = config.qc.bbduk.rm_lq,
-        compression = config.qc.compression
+        params = config["qc"]["bbduk"]["rm_lq"],
+        compression = config["qc"]["compression"]
     conda:
-        os.path.join(dir.env, "bbmap.yaml")
+        os.path.join(dir["env"], "bbmap.yaml")
     group:
         "roundAB"
     shell:
         """
         bbduk.sh \
             in={input.r1} \
             out={output.tmp} \
```

### Comparing `trimnami-0.0.6/trimnami.egg-info/SOURCES.txt` & `trimnami-0.0.7/trimnami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

