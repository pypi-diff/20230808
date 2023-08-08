# Comparing `tmp/microcat-0.2.6rc0.tar.gz` & `tmp/microcat-0.2.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.2.6rc0.tar", last modified: Tue Jul 25 12:48:54 2023, max compression
+gzip compressed data, was "microcat-0.2.7b0.tar", last modified: Tue Aug  8 15:03:47 2023, max compression
```

## Comparing `microcat-0.2.6rc0.tar` & `microcat-0.2.7b0.tar`

### file list

```diff
@@ -1,85 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.6rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 03:24:51.000000 microcat-0.2.6rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.6rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       74 2023-07-25 12:48:48.000000 microcat-0.2.6rc0/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 12:02:38.000000 microcat-0.2.6rc0/microcat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/bulk_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/bulk_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3575 2023-07-23 14:44:49.000000 microcat-0.2.6rc0/microcat/bulk_wf/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/bulk_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.6rc0/microcat/bulk_wf/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.6rc0/microcat/chemistry_defs.json
--rw-r--r--   0 root         (0) root         (0)    43169 2023-07-25 12:48:27.000000 microcat-0.2.6rc0/microcat/cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9780 2023-07-25 03:11:48.000000 microcat-0.2.6rc0/microcat/configer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/multi_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat/multi_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:34.000000 microcat-0.2.6rc0/microcat/multi_wf/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     5099 2023-07-24 15:17:06.000000 microcat-0.2.6rc0/microcat/prepare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/profiles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/profiles/generic/
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/cluster_config.yaml
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-25 12:46:50.000000 microcat-0.2.6rc0/microcat/profiles/generic/config.yaml
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/key_mapping.yaml
--rwxr-xr-x   0 root         (0) root         (0)      430 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/lsf_status.py
--rwxr-xr-x   0 root         (0) root         (0)      747 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/pbs_status.py
--rwxr-xr-x   0 root         (0) root         (0)      869 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/pbspro_status.py
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/queues.tsv.example
--rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/scheduler.py
--rwxr-xr-x   0 root         (0) root         (0)     1755 2023-07-25 08:32:33.000000 microcat-0.2.6rc0/microcat/profiles/generic/slurm_status.py
--rwxr-xr-x   0 root         (0) root         (0)    12352 2023-07-23 12:47:45.000000 microcat-0.2.6rc0/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/single_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3587 2023-07-24 03:12:53.000000 microcat-0.2.6rc0/microcat/single_wf/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 01:32:51.000000 microcat-0.2.6rc0/microcat/single_wf/envs/trimming.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.005124 microcat-0.2.6rc0/microcat/single_wf/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    41025 2023-07-24 05:41:37.000000 microcat-0.2.6rc0/microcat/single_wf/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-07-21 01:32:43.000000 microcat-0.2.6rc0/microcat/single_wf/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    39092 2023-07-24 05:43:54.000000 microcat-0.2.6rc0/microcat/single_wf/rules/host.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/single_wf/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3776 2023-07-18 02:36:09.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1112 2023-07-17 14:48:20.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4624 2023-07-17 14:25:46.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15592 2023-07-17 14:25:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
--rw-r--r--   0 root         (0) root         (0)    13281 2023-07-18 02:03:42.000000 microcat-0.2.6rc0/microcat/single_wf/scripts/starsolo_tenX_auto.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/single_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-23 14:36:38.000000 microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_simulate.smk
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-23 14:44:14.000000 microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.981124 microcat-0.2.6rc0/microcat/spatial_wf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.009124 microcat-0.2.6rc0/microcat/spatial_wf/config/
--rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:46.000000 microcat-0.2.6rc0/microcat/spatial_wf/config/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/microcat/spatial_wf/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.6rc0/microcat/spatial_wf/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 12:48:53.985124 microcat-0.2.6rc0/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-25 12:48:53.000000 microcat-0.2.6rc0/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-23 14:40:32.000000 microcat-0.2.6rc0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 12:48:54.013124 microcat-0.2.6rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3134 2023-07-24 07:33:39.000000 microcat-0.2.6rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.553365 microcat-0.2.7b0/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.7b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 03:24:51.000000 microcat-0.2.7b0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-08-08 15:03:47.553365 microcat-0.2.7b0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.7b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.225368 microcat-0.2.7b0/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       74 2023-08-08 15:03:16.000000 microcat-0.2.7b0/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 12:02:38.000000 microcat-0.2.7b0/microcat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.165369 microcat-0.2.7b0/microcat/bulk_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.225368 microcat-0.2.7b0/microcat/bulk_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3575 2023-07-23 14:44:49.000000 microcat-0.2.7b0/microcat/bulk_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.245368 microcat-0.2.7b0/microcat/bulk_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.7b0/microcat/bulk_wf/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.7b0/microcat/chemistry_defs.json
+-rwxrwxrwx   0 root         (0) root         (0)    43898 2023-08-08 14:59:47.000000 microcat-0.2.7b0/microcat/cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9780 2023-07-25 03:11:48.000000 microcat-0.2.7b0/microcat/configer.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-08-08 15:02:58.000000 microcat-0.2.7b0/microcat/download_celline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.165369 microcat-0.2.7b0/microcat/multi_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.245368 microcat-0.2.7b0/microcat/multi_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:34.000000 microcat-0.2.7b0/microcat/multi_wf/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5099 2023-07-24 15:17:06.000000 microcat-0.2.7b0/microcat/prepare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.165369 microcat-0.2.7b0/microcat/profiles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.309367 microcat-0.2.7b0/microcat/profiles/generic/
+-rw-r--r--   0 root         (0) root         (0)      493 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/cluster_config.yaml
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-25 12:46:50.000000 microcat-0.2.7b0/microcat/profiles/generic/config.yaml
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/key_mapping.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      430 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/lsf_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      747 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/pbs_status.py
+-rwxr-xr-x   0 root         (0) root         (0)      869 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/pbspro_status.py
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/queues.tsv.example
+-rwxr-xr-x   0 root         (0) root         (0)     4928 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/scheduler.py
+-rwxr-xr-x   0 root         (0) root         (0)     1755 2023-07-25 08:32:33.000000 microcat-0.2.7b0/microcat/profiles/generic/slurm_status.py
+-rwxr-xr-x   0 root         (0) root         (0)    12352 2023-07-23 12:47:45.000000 microcat-0.2.7b0/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.165369 microcat-0.2.7b0/microcat/single_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.309367 microcat-0.2.7b0/microcat/single_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-08-07 02:22:32.000000 microcat-0.2.7b0/microcat/single_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.373367 microcat-0.2.7b0/microcat/single_wf/envs/
+-rw-r--r--   0 root         (0) root         (0)      140 2023-08-06 01:31:55.000000 microcat-0.2.7b0/microcat/single_wf/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 01:32:51.000000 microcat-0.2.7b0/microcat/single_wf/envs/trimming.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.385367 microcat-0.2.7b0/microcat/single_wf/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-21 01:32:43.000000 microcat-0.2.7b0/microcat/single_wf/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-07-21 01:32:43.000000 microcat-0.2.7b0/microcat/single_wf/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    43104 2023-08-08 13:03:17.000000 microcat-0.2.7b0/microcat/single_wf/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-07-21 01:32:43.000000 microcat-0.2.7b0/microcat/single_wf/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    39981 2023-08-08 11:50:40.000000 microcat-0.2.7b0/microcat/single_wf/rules/host.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.493366 microcat-0.2.7b0/microcat/single_wf/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.7b0/microcat/single_wf/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.7b0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.7b0/microcat/single_wf/scripts/create_hdf5.py
+-rw-r--r--   0 root         (0) root         (0)     4874 2023-08-07 13:27:04.000000 microcat-0.2.7b0/microcat/single_wf/scripts/extract_kraken_output.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.7b0/microcat/single_wf/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3776 2023-07-18 02:36:09.000000 microcat-0.2.7b0/microcat/single_wf/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-08-07 13:40:49.000000 microcat-0.2.7b0/microcat/single_wf/scripts/extrat_test.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.7b0/microcat/single_wf/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.7b0/microcat/single_wf/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1112 2023-07-17 14:48:20.000000 microcat-0.2.7b0/microcat/single_wf/scripts/krak2_output_denosing.R
+-rw-r--r--   0 root         (0) root         (0)     1693 2023-08-08 11:24:39.000000 microcat-0.2.7b0/microcat/single_wf/scripts/krak2_output_denosing.py
+-rw-r--r--   0 root         (0) root         (0)    25094 2023-08-06 02:39:05.000000 microcat-0.2.7b0/microcat/single_wf/scripts/krak_cell_denosing copy.py
+-rw-r--r--   0 root         (0) root         (0)    28785 2023-08-08 14:29:45.000000 microcat-0.2.7b0/microcat/single_wf/scripts/krak_sample_denosing.py
+-rw-r--r--   0 root         (0) root         (0)    12356 2023-08-08 13:06:03.000000 microcat-0.2.7b0/microcat/single_wf/scripts/krak_study_denosing.py
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-08-02 08:33:45.000000 microcat-0.2.7b0/microcat/single_wf/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14491 2023-08-08 11:39:32.000000 microcat-0.2.7b0/microcat/single_wf/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.7b0/microcat/single_wf/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4624 2023-07-17 14:25:46.000000 microcat-0.2.7b0/microcat/single_wf/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15592 2023-07-17 14:25:42.000000 microcat-0.2.7b0/microcat/single_wf/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.7b0/microcat/single_wf/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.7b0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
+-rw-r--r--   0 root         (0) root         (0)    13343 2023-08-07 10:37:36.000000 microcat-0.2.7b0/microcat/single_wf/scripts/starsolo_tenX_auto.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.521365 microcat-0.2.7b0/microcat/single_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-23 14:36:38.000000 microcat-0.2.7b0/microcat/single_wf/snakefiles/single_simulate.smk
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-23 14:44:14.000000 microcat-0.2.7b0/microcat/single_wf/snakefiles/single_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.165369 microcat-0.2.7b0/microcat/spatial_wf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.537365 microcat-0.2.7b0/microcat/spatial_wf/config/
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-07-25 08:58:46.000000 microcat-0.2.7b0/microcat/spatial_wf/config/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.553365 microcat-0.2.7b0/microcat/spatial_wf/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.7b0/microcat/spatial_wf/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:03:47.225368 microcat-0.2.7b0/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2685 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-08 15:03:46.000000 microcat-0.2.7b0/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-23 14:40:32.000000 microcat-0.2.7b0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 15:03:47.553365 microcat-0.2.7b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-07-24 07:33:39.000000 microcat-0.2.7b0/setup.py
```

### Comparing `microcat-0.2.6rc0/LICENSE` & `microcat-0.2.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/PKG-INFO` & `microcat-0.2.7b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.6rc0
+Version: 0.2.7b0
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.6rc0/microcat/__init__.py` & `microcat-0.2.7b0/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/bulk_wf/config/config.yaml` & `microcat-0.2.7b0/microcat/bulk_wf/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/chemistry_defs.json` & `microcat-0.2.7b0/microcat/chemistry_defs.json`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/cli.py` & `microcat-0.2.7b0/microcat/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     click.echo(versions_string)
     ctx.exit()
 
 def abort_if_false(ctx, param, value):
     if not value:
         ctx.abort()
 
+
 # ##############################################################################
 # Microcat Main function Init
 
 @click.group("microcat",cls=HelpColorsGroup,
             context_settings=CONTEXT_SETTINGS,
             help_headers_color='yellow',
             help_options_color='green')
@@ -116,24 +117,52 @@
             ██║ ╚═╝ ██║██║╚██████╗██║  ██║╚██████╔╝╚██████╗██║  ██║   ██║   
             ╚═╝     ╚═╝╚═╝ ╚═════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝╚═╝  ╚═╝   ╚═╝   
     Microbiome Identification upon Cell Resolution from Omics-Computational Analysis Toolbox
     """
     pass
 
 
+
+
+@microcat.command("path")
+def path():
+    """
+    Print out microcat install path
+    """
+    import microcat
+    MICROCAT_DIR = microcat.__path__[0]
+    click.echo(MICROCAT_DIR)
+
 # ##############################################################################
 # Utils module
 
 @microcat.group("download")
 def download():
     """
     Download necessary files for running microcat
     """
     pass
 
+@download.command("cellline")
+def download_celline():
+    """
+    Download cell line per million microbiome reads (rpmm) percentile data for single analysis pipeline
+    """
+
+    script_path = os.path.join(os.path.dirname(__file__),"download_celline.py")  
+    command = ["python", script_path]
+
+    try:
+        subprocess.check_call(command)
+    except subprocess.CalledProcessError as e:
+        click.secho(f"Error: Failed to run download_celline.py ({e})",fg="red")
+
+
+
+
 
 @download.command("whitelist")
 def download_barcode():
     """
     Download barcode whitelist for single analysis pipeline
     """
     script_path = os.path.join(os.path.dirname(__file__),"prepare.py")  
@@ -587,18 +616,18 @@
     generic_profile,
     edit):
     """
     Quickly adjust microcat's default configurations
     """
 
     microcat_dir = os.path.dirname(os.path.abspath(__file__))
-    bulk_config_file = os.path.join(microcat_dir,"bulk_wf","config", "config.yaml")
-    multi_config_file = os.path.join(microcat_dir,"multi_wf","config", "config.yaml")
+    # bulk_config_file = os.path.join(microcat_dir,"bulk_wf","config", "config.yaml")
+    # multi_config_file = os.path.join(microcat_dir,"multi_wf","config", "config.yaml")
     single_config_file = os.path.join(microcat_dir,"single_wf","config", "config.yaml")
-    spatial_config_file = os.path.join(microcat_dir,"spatial_wf","config", "config.yaml")
+    # spatial_config_file = os.path.join(microcat_dir,"spatial_wf","config", "config.yaml")
 
     edited = False  # Flag to check if the user has edited any config file
 
     if edit:
         if edit == "single":
             if os.path.exists(single_config_file):
                 click.edit(filename=single_config_file)
@@ -634,48 +663,48 @@
         click.echo(f"Cellranger Refernce location updated as '{cellranger_ref}' path.")
     if starsolo_ref is not None and not edited:
         # Spatial and single both have starsolo refernence 
         single_config = parse_yaml(single_config_file)
         single_config["params"]["host"]["starsolo"]["reference"] = starsolo_ref
         update_config(single_config_file, single_config_file, single_config)
 
-        spatial_config = parse_yaml(spatial_config_file)
-        spatial_config["host"]["starsolo"]["reference"] = starsolo_ref
-        update_config(spatial_config_file, spatial_config_file, spatial_config)
+        # spatial_config = parse_yaml(spatial_config_file)
+        # spatial_config["host"]["starsolo"]["reference"] = starsolo_ref
+        # update_config(spatial_config_file, spatial_config_file, spatial_config)
 
         click.echo(f"Starsolo Refernce location updated as '{starsolo_ref}' path.")
     if krak2_ref is not None and not edited:
         # Spatial and single both have starsolo refernence 
         single_config = parse_yaml(single_config_file)
         single_config["params"]["classifier"]["kraken2uniq"]["kraken2_database"] = krak2_ref
         update_config(single_config_file, single_config_file, single_config)
 
-        spatial_config = parse_yaml(spatial_config_file)
-        spatial_config["params"]["classifier"]["kraken2uniq"]["kraken2_database"] = krak2_ref
-        update_config(spatial_config_file, spatial_config_file, spatial_config)
-
-        bulk_config = parse_yaml(bulk_config_file)
-        bulk_config["params"]["classifier"]["kraken2uniq"]["kraken2_database"] = krak2_ref
-        update_config(bulk_config_file, bulk_config_file, bulk_config)
+        # spatial_config = parse_yaml(spatial_config_file)
+        # spatial_config["params"]["classifier"]["kraken2uniq"]["kraken2_database"] = krak2_ref
+        # update_config(spatial_config_file, spatial_config_file, spatial_config)
+
+        # bulk_config = parse_yaml(bulk_config_file)
+        # bulk_config["params"]["classifier"]["kraken2uniq"]["kraken2_database"] = krak2_ref
+        # update_config(bulk_config_file, bulk_config_file, bulk_config)
 
         click.echo(f"Krake2nuniq Refernce location updated as '{krak2_ref}' path.")
 
     if krakuniq_ref is not None and not edited:
         # Spatial and single both have starsolo refernence 
         single_config = parse_yaml(single_config_file)
         single_config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"] = krakuniq_ref
         update_config(single_config_file, single_config_file, single_config)
 
-        spatial_config = parse_yaml(spatial_config_file)
-        spatial_config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"] = krakuniq_ref
-        update_config(spatial_config_file, spatial_config_file, spatial_config)
-
-        bulk_config = parse_yaml(bulk_config_file)
-        bulk_config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"] = krakuniq_ref
-        update_config(bulk_config_file, bulk_config_file, bulk_config)
+        # spatial_config = parse_yaml(spatial_config_file)
+        # spatial_config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"] = krakuniq_ref
+        # update_config(spatial_config_file, spatial_config_file, spatial_config)
+
+        # bulk_config = parse_yaml(bulk_config_file)
+        # bulk_config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"] = krakuniq_ref
+        # update_config(bulk_config_file, bulk_config_file, bulk_config)
 
         click.echo(f"Krakenuniq Refernce location updated as '{krakuniq_ref}' path.")
     if generic_profile is not None :
         profile_path = os.path.join(microcat_dir,"profiles", "generic")
         profile_conf_file = os.path.join(profile_path, "config.yaml")
         submmit_conf_file = os.path.join(profile_path, "key_mapping.yaml")
 
@@ -978,15 +1007,15 @@
     proc.communicate()
 
     # Print the actual executed command
     click.echo(f'''\nReal running cmd:\n{cmd_str}''')
 
 
 
-@microcat.command("run-remote")
+@microcat.command("run-remote", context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--jobs",
     type=int,
     default=30,
     help="Cluster job numbers, available on '--run-remote'",
 )
 @click.option(
```

### Comparing `microcat-0.2.6rc0/microcat/configer.py` & `microcat-0.2.7b0/microcat/configer.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/multi_wf/config/config.yaml` & `microcat-0.2.7b0/microcat/multi_wf/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/prepare.py` & `microcat-0.2.7b0/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/profiles/generic/key_mapping.yaml` & `microcat-0.2.7b0/microcat/profiles/generic/key_mapping.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/profiles/generic/pbs_status.py` & `microcat-0.2.7b0/microcat/profiles/generic/pbs_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/profiles/generic/pbspro_status.py` & `microcat-0.2.7b0/microcat/profiles/generic/pbspro_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/profiles/generic/scheduler.py` & `microcat-0.2.7b0/microcat/profiles/generic/scheduler.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/profiles/generic/slurm_status.py` & `microcat-0.2.7b0/microcat/profiles/generic/slurm_status.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/sample.py` & `microcat-0.2.7b0/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/config/config.yaml` & `microcat-0.2.7b0/microcat/spatial_wf/config/config.yaml`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/rules/ERCC.smk` & `microcat-0.2.7b0/microcat/single_wf/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/rules/build.smk` & `microcat-0.2.7b0/microcat/single_wf/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/rules/classfier.smk` & `microcat-0.2.7b0/microcat/single_wf/rules/classfier.smk`

 * *Files 3% similar despite different names*

```diff
@@ -158,207 +158,235 @@
             {input.unmapped_fastq} \
             --use-names \
             --memory-mapping \
             2>&1 | tee {log};\
             cut -f 1-3,6-8 {output.krak2_report} > {output.krak2_std_report};\
             python {params.kraken2mpa_script} -r {output.krak2_std_report} -o {output.krak2_mpa_report};
             '''
-    rule extract_kraken2_reads:
-        input:
-            krak2_classified_output_fq = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_classified_output/{sample}/{sample}_kraken2_classified.fq"),
-            krak2_output = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_kraken2_output/{sample}/{sample}_kraken2_output.txt"),
-            krak2_report = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_kraken2_report/custom/{sample}/{sample}_kraken2_report.txt"),
-        output:
-            krak2_extracted_output_fq = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified.fq"),
-        log:
-            os.path.join(config["logs"]["classifier"],
-                        "rmhost_kraken2uniq_extracted/{sample}_kraken2uniq_classifier_extracted.log")
-        benchmark:
-            os.path.join(config["benchmarks"]["classifier"],
-                            "rmhost_kraken2uniq/{sample}_kraken2uniq_classifier_extracted_benchmark.log")
-        params:
-            extract_kraken_reads_script = config["scripts"]["extract_kraken_reads"]
-        conda:
-            config["envs"]["kmer_qc"]
-        priority: 
-            13
-        shell:
-            '''
-            python {params.extract_kraken_reads_script} \
-            -k {input.krak2_output} \
-            -s1 {input.krak2_classified_output_fq} \
-            --report {input.krak2_report}\
-            -o {output.krak2_extracted_output_fq} \
-            --taxid 9606 \
-            --exclude \
-            --include-parents \
-            2>&1 | tee {log};
-            '''
+    # rule extract_kraken2_reads:
+    #     input:
+    #         krak2_classified_output_fq = os.path.join(
+    #             config["output"]["classifier"],
+    #             "rmhost_classified_output/{sample}/{sample}_kraken2_classified.fq"),
+    #         krak2_output = os.path.join(
+    #             config["output"]["classifier"],
+    #             "rmhost_kraken2_output/{sample}/{sample}_kraken2_output.txt"),
+    #         krak2_report = os.path.join(
+    #             config["output"]["classifier"],
+    #             "rmhost_kraken2_report/custom/{sample}/{sample}_kraken2_report.txt"),
+    #     output:
+    #         krak2_extracted_output_fq = os.path.join(
+    #             config["output"]["classifier"],
+    #             "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified.fq"),
+    #     log:
+    #         os.path.join(config["logs"]["classifier"],
+    #                     "rmhost_kraken2uniq_extracted/{sample}_kraken2uniq_classifier_extracted.log")
+    #     benchmark:
+    #         os.path.join(config["benchmarks"]["classifier"],
+    #                         "rmhost_kraken2uniq/{sample}_kraken2uniq_classifier_extracted_benchmark.log")
+    #     params:
+    #         extract_kraken_reads_script = config["scripts"]["extract_kraken_reads"]
+    #     conda:
+    #         config["envs"]["kmer_python"]
+    #     priority: 
+    #         13
+    #     shell:
+    #         '''
+    #         python {params.extract_kraken_reads_script} \
+    #         -k {input.krak2_output} \
+    #         -s1 {input.krak2_classified_output_fq} \
+    #         --report {input.krak2_report}\
+    #         -o {output.krak2_extracted_output_fq} \
+    #         --taxid 9606 \
+    #         --exclude \
+    #         --include-parents \
+    #         2>&1 | tee {log};
+    #         '''
 
     rule extract_kraken2_report:
         input:
             krak2_output = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_kraken2_output/{sample}/{sample}_kraken2_output.txt"),
-            krak2_report = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_kraken2_report/custom/{sample}/{sample}_kraken2_report.txt"),
-            krak2_mpa_report=os.path.join(
-                config["output"]["classifier"],
-                "rmhost_kraken2_report/mpa/{sample}/{sample}_kraken2_mpa_report.txt")
+            # krak2_report = os.path.join(
+            #     config["output"]["classifier"],
+            #     "rmhost_kraken2_report/custom/{sample}/{sample}_kraken2_report.txt"),
+            # krak2_mpa_report=os.path.join(
+            #     config["output"]["classifier"],
+            #     "rmhost_kraken2_report/mpa/{sample}/{sample}_kraken2_mpa_report.txt")
         output:
             krak2_extracted_output = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified_output.txt"),
         log:
             os.path.join(config["logs"]["classifier"],
                         "rmhost_kraken2uniq_extracted/{sample}_kraken2uniq_classifier_report_extracted.log")
-        params:
-            extract_microbiome_output_script = config["scripts"]["extract_microbiome_output"]
-        threads:
-            8
+        # params:
+        #     extract_kraken_output_script = config["scripts"]["extract_kraken_output"]
+        # threads:
+        #     8
         priority: 
             14
-        conda:
-            config["envs"]["kmer_qc"]
+        # conda:
+        #     config["envs"]["kmer_python"]
         shell:
+            # '''
+            # python {params.extract_kraken_output_script} \
+            # --output_file {input.krak2_output} \
+            # --kraken_report {input.krak2_report} \
+            # --mpa_report {input.krak2_mpa_report} \
+            # --extract_file {output.krak2_extracted_output}\
+            # --cores {threads} \
+            # --ntaxid 6000 \
+            # 2>&1 | tee {log};
+            # '''
             '''
-            Rscript {params.extract_microbiome_output_script} \
-            --output_file {input.krak2_output} \
-            --kraken_report {input.krak2_report} \
-            --mpa_report {input.krak2_mpa_report} \
-            --extract_file {output.krak2_extracted_output}\
-            --cores {threads} \
-            --ntaxid 6000 \
-            2>&1 | tee {log};
+            awk -F'\t' '$1 == "C" {{print}}' {input.krak2_output} > {output.krak2_extracted_output} 2>&1 | tee {log};
             '''
 
-    rule k_mer_test:
+    rule krak_sample_denosing:
         input:
-            krak2_extracted_output_fq = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified.fq"),
             krak2_extracted_output = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified_output.txt"),
             krak2_report = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_kraken2_report/custom/{sample}/{sample}_kraken2_report.txt"),
+            unmapped_bam_sorted_file =os.path.join(
+                    config["output"]["host"],
+                    "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),
             krak2_mpa_report=os.path.join(
                 config["output"]["classifier"],
                 "rmhost_kraken2_report/mpa/{sample}/{sample}_kraken2_mpa_report.txt")
         output:
-            krak2_sckmer_output = os.path.join(
+            krak_sample_denosing_result = os.path.join(
                 config["output"]["classifier"],
-                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_kraken2_sckmer.txt"),
-            krak2_sckmer_test_output = os.path.join(
+                "rmhost_classified_qc/{sample}/{sample}_krak_sample_denosing.txt"),
+            krak_sample_raw_result = os.path.join(
                 config["output"]["classifier"],
-                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_kraken2_sckmer_correlation_test.txt"),
+                "rmhost_classified_qc/{sample}/{sample}_krak_sample_raw.txt"),
         log:
             os.path.join(config["logs"]["classifier"],
-                        "classified_qc/kmer_UMI/{sample}_kraken2uniq_sckmer.log")
+                        "classified_qc/{sample}/{sample}_krak_sample_denosing.log")
         priority: 
             15
         params:
-            cb_len = config["params"]["classifier"]["sckmer"]["cb_len"],
-            umi_len = config["params"]["classifier"]["sckmer"]["umi_len"],
-            min_frac = config["params"]["classifier"]["sckmer"]["min_frac"],
-            kmer_len = config["params"]["classifier"]["sckmer"]["kmer_len"],
-            nsample = config["params"]["classifier"]["sckmer"]["nsample"],
-            sckmer_unpaired_script= config["scripts"]["sckmer_unpaired"]
+            min_frac = config["params"]["classifier"]["krak_sample_denosing"]["min_frac"],
+            kmer_len = config["params"]["classifier"]["krak_sample_denosing"]["kmer_len"],
+            min_entropy = config["params"]["classifier"]["krak_sample_denosing"]["min_entropy"],
+            min_dust = config["params"]["classifier"]["krak_sample_denosing"]["min_dust"],
+            krak_sample_denosing_script= config["scripts"]["krak_sample_denosing"],
+            inspect_file = os.path.join(config["params"]["classifier"]["kraken2uniq"]["kraken2_database"],
+                                        "inspect.txt"),
+            nodes_dump_file = os.path.join(config["params"]["classifier"]["kraken2uniq"]["kraken2_database"],
+                                        "taxonomy/nodes.dmp")
         conda:
-            config["envs"]["kmer_qc"]
+            config["envs"]["kmer_python"]
+        benchmark:
+            os.path.join(config["benchmarks"]["classifier"],
+                        "rmhost_classified_qc/{sample}_sample_denosing_benchmark.tsv")
+        threads:
+            8
         shell:
             '''
-            Rscript {params.sckmer_unpaired_script} \
-            --fa1 {input.krak2_extracted_output_fq} \
-            --microbiome_output_file {input.krak2_extracted_output} \
-            --cb_len {params.cb_len} \
-            --umi_len {params.umi_len} \
-            --kraken_report {input.krak2_report} \
-            --mpa_report {input.krak2_mpa_report} \
+            python {params.krak_sample_denosing_script} \
+            --krak_report {input.krak2_report} \
+            --krak_output {input.krak2_extracted_output} \
+            --krak_mpa_report {input.krak2_mpa_report} \
+            --bam {input.unmapped_bam_sorted_file} \
+            --nodes_dump {params.nodes_dump_file}\
+            --inspect {params.inspect_file} \
             --min_frac {params.min_frac} \
-            --kmer_len {params.kmer_len} \
-            --nsample {params.nsample} \
-            --kmer_file {output.krak2_sckmer_output} \
-            --kmer_test_file {output.krak2_sckmer_test_output} \
-            2>&1 | tee {log};
-            '''
-    rule sample_denosing:
-        input:
-            krak2_sckmer_test_output = os.path.join(
-                                config["output"]["classifier"],
-                                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_kraken2_sckmer_correlation_test.txt"),
+            --num_processes {threads} \
+            --min_entropy {params.min_entropy} \
+            --min_dust {params.min_dust}\
+            --qc_output_file {output.krak_sample_denosing_result} \
+            --raw_qc_output_file {output.krak_sample_raw_result} \
+            --log_file {log};
+            '''
+    rule krak_study_denosing:
+        input:
+            krak_sample_denosing_result = os.path.join(
+                config["output"]["classifier"],
+                "rmhost_classified_qc/{sample}/{sample}_krak_sample_denosing.txt"),
         output:
-            krak2_sample_denosing = os.path.join(
-                                config["output"]["classifier"],
-                                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_sample_denosing.txt"),
+            krak_study_denosing_output = os.path.join(
+                config["output"]["classifier"],
+                "rmhost_classified_qc/{sample}/{sample}_krak_study_denosing.txt"),
         priority: 
-            16
+            15
+        log:
+            os.path.join(config["logs"]["classifier"],
+                        "classified_qc/{sample}/{sample}_krak_study_denosing.log")
         params:
-            krak2_report_dir = os.path.join(
+            krak_sample_denosing_output_dir = os.path.join(
                 config["output"]["classifier"],
-                "rmhost_kraken2_report/custom/"),
+                "rmhost_classified_qc/"),
             SampleID="{sample}",
-            sample_denosing_script= config["scripts"]["sample_denosing"]
+            min_reads = config["params"]["classifier"]["krak_study_denosing"]["min_reads"],
+            min_uniq = config["params"]["classifier"]["krak_study_denosing"]["min_uniq"],
+            cell_line_file = config["params"]["classifier"]["krak_study_denosing"]["cell_line"],
+            krak_study_denosing_script= config["scripts"]["krak_study_denosing"]
         conda:
-            config["envs"]["kmer_qc"]
+            config["envs"]["kmer_python"]
         shell:
             '''
-            Rscript  {params.sample_denosing_script}\
-            --path {params.krak2_report_dir} \
-            --kmer_data {input.krak2_sckmer_test_output} \
-            --out_path {output.krak2_sample_denosing} \
-            --sample_names {params.SampleID} \
-            --min_reads 2 
+            python  {params.krak_study_denosing_script}\
+            --path {params.krak_sample_denosing_output_dir} \
+            --out_path {output.krak_study_denosing_output} \
+            --sample_name {params.SampleID} \
+            --min_reads {params.min_reads} \
+            --min_uniq {params.min_uniq} \
+            --cell_line {params.cell_line_file} \
+            --log_file {log}
             '''
 
     rule krak2_output_denosing:
         input:
             krak2_extracted_output = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_extracted_classified_output/{sample}/{sample}_kraken2_extracted_classified_output.txt"),
-            krak2_sample_denosing = os.path.join(
-                config["output"]["classifier"],
-                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_sample_denosing.txt"),
+            krak_study_denosing_output = os.path.join(
+                            config["output"]["classifier"],
+                            "rmhost_classified_qc/{sample}/{sample}_krak_study_denosing.txt")
         output:
             krak2_output_denosing = os.path.join(
                 config["output"]["classifier"],
-                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_kraken2_output_denosing.txt"),
+                "rmhost_classified_qc/{sample}/{sample}_kraken2_output_denosing.txt"),
         conda:
-            config["envs"]["kmer_qc"]
+            config["envs"]["kmer_python"]
         priority: 
             17
         params:
             krak2_output_denosing_script = config["scripts"]["krak2_output_denosing"]
         shell:
             '''
-            Rscript {params.krak2_output_denosing_script} \
-            --output_file {input.krak2_extracted_output} \
-            --taxa {input.krak2_sample_denosing} \
+            python {params.krak2_output_denosing_script} \
+            --krak_output_file {input.krak2_extracted_output} \
+            --krak_study_denosing_file {input.krak_study_denosing_output} \
             --out_krak2_denosing {output.krak2_output_denosing}
             '''
     rule krak2_matrix_build:
         input:
             krak2_output_denosing = os.path.join(
                 config["output"]["classifier"],
-                "rmhost_classified_qc/kmer_UMI/{sample}/{sample}_kraken2_output_denosing.txt"),
+                "rmhost_classified_qc/{sample}/{sample}_kraken2_output_denosing.txt"),
             unmapped_bam_sorted_file =os.path.join(
                 config["output"]["host"],
                 "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
         output:
-            krak2_output_denosing_label = os.path.join(config["output"]["classifier"],"microbiome_matrix_build/{sample}/data.txt")
+            krak2sc_barcode = os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/barcodes.tsv"),
+            krak2sc_matrix = os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/matrix.mtx"),
+            krak2sc_feature = os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/features.tsv")
         params:
             database = config["params"]["classifier"]["kraken2uniq"]["kraken2_database"],
             matrix_outdir = os.path.join(config["output"]["classifier"],
                 "microbiome_matrix_build/{sample}/"),
             kraken2sc_script = config["scripts"]["kraken2sc"]
         priority: 
             18
@@ -378,15 +406,24 @@
             --log_file {log} \
             --processors {threads} \
             --outdir {params.matrix_outdir}
             '''
             
     rule kraken2uniq_classified_all:
         input:
-            expand(os.path.join(config["output"]["classifier"],"microbiome_matrix_build/{sample}/data.txt"),sample=SAMPLES_ID_LIST)
+            expand(os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/barcodes.tsv"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/matrix.mtx"),sample=SAMPLES_ID_LIST),
+            expand(os.path.join(
+                config["output"]["classifier"],
+                "microbiome_matrix_build/{sample}/features.tsv"),sample=SAMPLES_ID_LIST)
+
 else:
     rule kraken2uniq_classified_all:
         input:    
 
 if config["params"]["classifier"]["krakenuniq"]["do"]:
     rule krakenuniq_classifier:
         input:
```

### Comparing `microcat-0.2.6rc0/microcat/single_wf/rules/database.smk` & `microcat-0.2.7b0/microcat/single_wf/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/rules/host.smk` & `microcat-0.2.7b0/microcat/single_wf/rules/host.smk`

 * *Files 5% similar despite different names*

```diff
@@ -112,14 +112,15 @@
                     soloUMIdedup = config["params"]["host"]["starsolo"]["algorithm"]["soloUMIdedup"],
                     soloCBmatchWLtype = config["params"]["host"]["starsolo"]["algorithm"]["soloCBmatchWLtype"],
                     soloUMIfiltering = config["params"]["host"]["starsolo"]["algorithm"]["soloUMIfiltering"],
                     soloCellFilter = config["params"]["host"]["starsolo"]["algorithm"]["soloCellFilter"],
                     clipAdapterType = config["params"]["host"]["starsolo"]["algorithm"]["clipAdapterType"],
                     outFilterScoreMin = config["params"]["host"]["starsolo"]["algorithm"]["outFilterScoreMin"],
                     soloMultiMappers = config["params"]["host"]["starsolo"]["algorithm"]["soloMultiMappers"],
+                    variousParams_condition = "True" if config["params"]["host"]["starsolo"]["variousParams"] else "False",
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -129,28 +130,35 @@
                 threads:
                     config["resources"]["starsolo"]["threads"]
                 shell:
                     '''
                     mkdir -p {params.starsolo_out}; 
                     cd {params.starsolo_out} ;
 
+                    if {params.variousParams_condition} == "True"; then
+                        variousParams='--variousParams {params.variousParams}'
+                    else
+                        variousParams=''
+                    fi
+                    
                     bash {params.starsolo_10X_auto} \
                     --barcode_reads {params.barcode_reads} \
                     --cdna_reads {params.cdna_reads} \
                     --barcode_data_dir {params.barcode_data_dir} \
                     --sample {wildcards.sample} \
                     --threads {threads} \
                     --reference {params.reference} \
                     --soloUMIdedup {params.soloUMIdedup} \
                     --soloCBmatchWLtype {params.soloCBmatchWLtype} \
                     --soloUMIfiltering {params.soloUMIfiltering} \
                     --soloCellFilter {params.soloCellFilter} \
                     --outFilterScoreMin {params.outFilterScoreMin} \
                     --soloMultiMappers {params.soloMultiMappers} \
                     --clipAdapterType {params.clipAdapterType}\
+                    $variousParams \
                     2>&1 | tee ../../../{log} ;
                     '''
         else:
             rule starsolo_CB_UMI_Simple_count:
                 input:
                     # Directory containing input fastq files
                     fastqs_dir=lambda wildcards: microcat.get_fastqs_dir(SAMPLES,wildcards),
@@ -249,14 +257,17 @@
                 mapped_bam_file = os.path.join(
                     config["output"]["host"],
                     "starsolo_count/{sample}/Aligned_sortedByCoord_out.bam")
             output:
                 unmapped_bam_sorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
+                unmapped_bam_sorted_index = os.path.join(
+                        config["output"]["host"],
+                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai")
             params:
                 unmapped_bam_unsorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByCoord_unmapped_out.bam")
             ## because bam is sorted by Coord,it's necessary to sort it by read name
             conda:
                 config["envs"]["star"]
@@ -264,19 +275,23 @@
                 config["resources"]["samtools_extract"]["threads"]
             resources:
                 mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             shell:
                 '''
                 samtools view --threads  {threads}  -b -f 4   {input.mapped_bam_file}  >  {params.unmapped_bam_unsorted_file};\
                 samtools sort -n  --threads  {threads} {params.unmapped_bam_unsorted_file} -o {output.unmapped_bam_sorted_file};\
+                samtools index --threads  {threads} {output.unmapped_sorted_bam_file} -o {output.unmapped_bam_sorted_index};\
                 rm -rf {params.unmapped_bam_unsorted_file};
                 '''
         rule starsolo_CB_UMI_Simple_all:
             input:
                 expand(os.path.join(config["output"]["host"],"unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),sample=SAMPLES_ID_LIST) 
+                expand(os.path.join(
+                        config["output"]["host"],
+                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai"), sample=SAMPLES_ID_LIST)
         
     else:
         rule starsolo_CB_UMI_Simple_all:
             input: 
 
     if config["params"]["host"]["starsolo"]["soloType"]=="SmartSeq":
         rule generate_pe_manifest_file:
@@ -383,47 +398,26 @@
             resources:
                 mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             shell:
                 '''
                 samtools view --threads  {threads}  -b -f 4   {input.mapped_bam_file}  >  {output.unmapped_bam_unsorted_file}
                 '''
 
-        # rule starsolo_SmartSeq_unmapped_sorted_bam:
-        #     input:
-        #         unmapped_bam_unsorted_file = os.path.join(
-        #             config["output"]["host"],
-        #             "starsolo_count/Aligned_out_unmapped.bam")
-        #     output:
-        #         unmapped_sorted_bam = os.path.join(
-        #             config["output"]["host"],
-        #             "starsolo_count/Aligned_out_unmapped_RGsorted.bam"),
-        #     params:
-        #         threads=40,
-        #         tag="RG"
-        #     log:
-        #         os.path.join(config["logs"]["host"],
-        #                     "starsolo/unmapped_sorted_bam.log")
-        #     benchmark:
-        #         os.path.join(config["benchmarks"]["host"],
-        #                     "starsolo/unmapped_sorted_bam.benchmark")
-        #     conda:
-        #         config["envs"]["star"]
-        #     shell:
-        #         '''
-        #         samtools sort -@ {threads} -t {params.tag} -o {output.unmapped_sorted_bam}  {input.unmapped_bam_unsorted_file};
-        #         '''
         rule starsolo_smartseq_unmapped_sorted_bam:
             input:
                 unmapped_bam_unsorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_out_unmapped.bam")
             output:
-                unmapped_sorted_bam = os.path.join(
+                unmapped_sorted_bam_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),
+                unmapped_bam_sorted_index = os.path.join(
+                        config["output"]["host"],
+                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai")
             params:
                 tag="RG"
             log:
                 os.path.join(config["logs"]["host"],
                             "starsolo/{sample}/unmapped_sorted_bam.log")
             benchmark:
                 os.path.join(config["benchmarks"]["host"],
@@ -432,15 +426,16 @@
                 config["resources"]["samtools_extract"]["threads"]
             resources:
                 mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             conda:
                 config["envs"]["star"]
             shell:
                 '''
-                samtools sort -n  --threads  {threads} {input.unmapped_bam_unsorted_file} -o {output.unmapped_sorted_bam}
+                samtools sort -n  --threads  {threads} {input.unmapped_bam_unsorted_file} -o {output.unmapped_sorted_bam_file};\
+                samtools index --threads  {threads} {output.unmapped_sorted_bam_file} -o {output.unmapped_bam_sorted_index};\
                 '''
         # checkpoint starsolo_smartseq_demultiplex_bam_by_read_group:
         #     input:
         #         unmapped_sorted_bam = os.path.join(
         #             config["output"]["host"],
         #             "starsolo_count/Aligned_out_unmapped_RGsorted.bam")
         #     output:
@@ -484,15 +479,18 @@
         #         --output_bam {output.unmapped_bam_sorted_file} 
         #         '''
 
         rule starsolo_SmartSeq_all:
             input:
                 expand(os.path.join(
                         config["output"]["host"],
-                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),sample=SAMPLES_ID_LIST)
+                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"), sample=SAMPLES_ID_LIST)
+                expand(os.path.join(
+                        config["output"]["host"],
+                        "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai"), sample=SAMPLES_ID_LIST)
         
     else:
         rule starsolo_SmartSeq_all:
             input: 
     #ALL Input
 
     if config["params"]["host"]["starsolo"]["soloType"]=="CB_UMI_Complex":
@@ -690,14 +688,17 @@
             mapped_bam_file = os.path.join(
             config["output"]["host"],
             "cellranger_count/{sample}/{sample}_mappped2human_bam.bam")
         output:
             unmapped_bam_sorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
+            unmapped_bam_sorted_index = os.path.join(
+                    config["output"]["host"],
+                    "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai")
         params:
             unmapped_bam_unsorted_file = os.path.join(
                 config["output"]["host"],
                 "unmapped_host/{sample}/Aligned_sortedByCoord_unmapped_out.bam")
         ## because bam is sorted by Coord,it's necessary to sort it by read name
         resources:
             mem_mb=config["resources"]["samtools_extract"]["mem_mb"]
@@ -705,27 +706,29 @@
             config["resources"]["samtools_extract"]["threads"]
         conda:
             config["envs"]["star"]
         shell:
             '''
             samtools view --threads  {threads}  -b -f 4   {input.mapped_bam_file}  >  {params.unmapped_bam_unsorted_file};\
             samtools sort -n  --threads  {threads} {params.unmapped_bam_unsorted_file} -o {output.unmapped_bam_sorted_file};\
-            rm -rf {params.unmapped_bam_unsorted_file}
+            samtools index --threads  {threads} {output.unmapped_bam_sorted_file} -o {output.unmapped_bam_sorted_index};\
+            rm -rf {params.unmapped_bam_unsorted_file} 
             '''
 
     rule cellranger_all:
         input:
-            expand( os.path.join(
+            expand(os.path.join(
                     config["output"]["host"],
-                    "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),sample=SAMPLES_ID_LIST)
+                    "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"), sample=SAMPLES_ID_LIST)
+            expand(os.path.join(
+                    config["output"]["host"],
+                    "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bai"), sample=SAMPLES_ID_LIST)
+
 
 else:
     rule cellranger_all:
         input:
 
 rule host_all:
     input:
         rules.starsolo_all.input,
-        rules.cellranger_all.input,
-
-
-
+        rules.cellranger_all.input,
```

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/INVADEseq.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/create_hdf5.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/extract_kraken_reads.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/extract_microbiome_output.R` & `microcat-0.2.7b0/microcat/single_wf/scripts/extract_microbiome_output.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/generate_PE_manifest_file.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/generate_PE_manifest_file.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/get_ncbi_domains.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/krak2_output_denosing.R` & `microcat-0.2.7b0/microcat/single_wf/scripts/krak2_output_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2mpa.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/kraken2sc.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/kraken2sc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pysam
-import regex as re
+import re
 import collections.abc
 from scipy.sparse import csr_matrix
 from scipy.io import mmwrite
 import csv
 import logging
 import os
 import argparse
@@ -30,28 +30,27 @@
 args = parser.parse_args()
 bamfile = args.bam
 mgfile = args.krak_output
 outdir = args.outdir
 dbfile = args.dbfile
 log_file = args.log_file
 n_processors =args.proc
-# 示例用法
-word = "Hello, World!"
+
 
 if not os.path.exists(outdir):
     os.system('mkdir -p '+outdir)
 
 def mg2sc(bamfile, mgfile, dbfile, outdir):
     """ Main Function. 
     Creates a sparse matrix with transcript count per organism for each cell."""
 
     # Generate variables based on input
     matrixfile = os.path.join(outdir,'matrix.mtx')
     cellfile = os.path.join(outdir, 'barcodes.tsv')
-    taxfile = os.path.join(outdir,'taxonomy.tsv')
+    taxfile = os.path.join(outdir,'features.tsv')
     dbfile = os.path.join(dbfile, 'inspect.txt')
     # dbfile_out =os.path.join(outdir,'hierarchy.txt')
 
     # Extract taxonomy IDs for each transcript
     mg_dict = extract_ids(bamfile, mgfile)
 
     # Find most frequent taxonomy for each transcript
@@ -323,54 +322,39 @@
 #             taxname = line[5].lstrip()
             
 #             if taxid_db in taxid_list:
 #                 taxdict[taxid_db] = taxname
     
 #     return taxdict
 
-def extract_taxref(file):
-    """ 
-    Extract taxonomy reference for each read.
-    Input:  viral track output .bam file
-    Output: dictionary with {readname: taxonomy ID}, list of unique taxonomy IDs
-    """
-    # extract taxref for each read
-    tdict = {}
-    line = 0
-    skipped = 0
-    taxref_list = set('0')
+# def extract_taxref(file):
+#     """ 
+#     Extract taxonomy reference for each read.
+#     Input:  viral track output .bam file
+#     Output: dictionary with {readname: taxonomy ID}, list of unique taxonomy IDs
+#     """
+#     # extract taxref for each read
+#     tdict = {}
+#     line = 0
+#     skipped = 0
+#     taxref_list = set('0')
     
-    for read in pysam.AlignmentFile(file, "rb"):
-        # count the total number of reads analysed
-        line += 1
-        try:
-            # Extract readname and taxonomy reference
-            taxref = read.to_dict().get('ref_name').split('|')[1]
-            taxref_list.add(taxref)
-            tdict[read.query_name] = taxref
-        except:
-            # in case some reads are unmapped or don't work
-            skipped += 1
-    logging.info("Reads in ViralTrack output: {}, reads without taxonomy reference or that failed: {}".format(line, skipped))
-    return(tdict, taxref_list)
-
-
-def save_data(data, outdir):
-    # 创建目录
-    os.makedirs(outdir, exist_ok=True)
-
-    # 生成保存数据的文件路径
-    filename = os.path.join(outdir, 'data.txt')
-
-    # 将数据写入文件
-    with open(filename, 'w') as f:
-        f.write(data)
-
-
-
+#     for read in pysam.AlignmentFile(file, "rb"):
+#         # count the total number of reads analysed
+#         line += 1
+#         try:
+#             # Extract readname and taxonomy reference
+#             taxref = read.to_dict().get('ref_name').split('|')[1]
+#             taxref_list.add(taxref)
+#             tdict[read.query_name] = taxref
+#         except:
+#             # in case some reads are unmapped or don't work
+#             skipped += 1
+#     logging.info("Reads in ViralTrack output: {}, reads without taxonomy reference or that failed: {}".format(line, skipped))
+#     return(tdict, taxref_list)
 
 
 def extract_bc(file):
     """ 
     Extracts cellbarcode and UMI for each readname
     Input:  unmapped .bam file
     Output: dictionary with {readname: [cellbarcode, UMI]}
@@ -408,13 +392,12 @@
 
     # 添加日志处理器到logger对象
     logger = logging.getLogger()
     logger.addHandler(handler)
     # multi process
     pool = mp.Pool(processes=int(n_processors))
     mg2sc(bamfile=bamfile, mgfile=mgfile, dbfile=dbfile, outdir=outdir)
-    save_data(word, outdir)
     # 关闭进程池
     pool.close()
     pool.join()
```

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/microcat_bam_handle.Rmd` & `microcat-0.2.7b0/microcat/single_wf/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/sample_denosing.R` & `microcat-0.2.7b0/microcat/single_wf/scripts/sample_denosing.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/sckmer_unpaired.R` & `microcat-0.2.7b0/microcat/single_wf/scripts/sckmer_unpaired.R`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/spilt_bam_by_tag.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.2.7b0/microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/single_wf/scripts/starsolo_tenX_auto.sh` & `microcat-0.2.7b0/microcat/single_wf/scripts/starsolo_tenX_auto.sh`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     *)
       echo "Invalid args: $1" >&2
       exit 1
       ;;
   esac
 done
 
+
 green=$(tput setaf 2)
 blue=$(tput setaf 4)
 reset=$(tput sgr0)
 red=$(tput setaf 1)
 
 echo "Running preflight checks (please wait)..."
 
@@ -343,30 +344,33 @@
     STAR --runThreadN $threads --genomeDir $reference --readFilesIn $barcode_reads $cdna_reads --runDirPerm All_RWX $file_command \
     --soloBarcodeMate 1 --clip5pNbases 39 0 \
     --soloType CB_UMI_Simple --soloCBwhitelist $BC --soloCBstart 1 --soloCBlen $CBLEN --soloUMIstart $((CBLEN+1)) --soloUMIlen $UMILEN --soloStrand Forward \
     --soloUMIdedup $soloUMIdedup --soloCBmatchWLtype $soloCBmatchWLtype --soloUMIfiltering $soloUMIfiltering \
     --soloCellFilter $soloCellFilter --outFilterScoreMin $outFilterScoreMin \
     --soloMultiMappers $soloMultiMappers \
     --outSAMtype BAM SortedByCoordinate \
+    --outSAMunmapped Within \
     --outSAMattrRGline ID:$sample PL:illumina SM:$sample LB:$CHEMISTRY \
     --outSAMattributes NH HI AS nM CB UB CR CY UR UY GX GN \
     --outFileNamePrefix ./$sample/\
     $variousParams  
 else 
     STAR --runThreadN $threads --genomeDir $reference --readFilesIn $cdna_reads $barcode_reads --runDirPerm All_RWX $file_command \
     --soloType CB_UMI_Simple --soloCBwhitelist $BC --soloBarcodeReadLength 0 --soloCBlen $CBLEN --soloUMIstart $((CBLEN+1)) --soloUMIlen $UMILEN --soloStrand $STRAND \
     --soloUMIdedup $soloUMIdedup --soloCBmatchWLtype $soloCBmatchWLtype --soloUMIfiltering $soloUMIfiltering \
     --soloCellFilter $soloCellFilter --outFilterScoreMin $outFilterScoreMin \
     --soloMultiMappers $soloMultiMappers \
     --clipAdapterType CellRanger4 \
     --outSAMtype BAM SortedByCoordinate \
+    --outSAMunmapped Within \
     --outSAMattrRGline ID:$sample PL:illumina SM:$sample LB:$CHEMISTRY \
     --outSAMattributes NH HI AS nM CB UB CR CY UR UY GX GN \
     --outFileNamePrefix ./$sample/ \
     $variousParams
+
 fi
 
 
 
 current_date=$(date +%Y-%m-%d)
 current_time=$(date +%H:%M:%S)
 state="[runtime] (ready)"
```

### Comparing `microcat-0.2.6rc0/microcat/single_wf/snakefiles/single_wf.smk` & `microcat-0.2.7b0/microcat/single_wf/snakefiles/single_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.6rc0/microcat/spatial_wf/config/config.yaml` & `microcat-0.2.7b0/microcat/single_wf/config/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -61,20 +61,24 @@
       bowtie2db: "/data/database/metaphlan_database/"
       db_index: "mpa_vOct22_CHOCOPhlAnSGB_202212"
       metaphlan_other_params: ''
     krakenuniq:
       do: false
       krakenuniq_database: "/data/database/krakenuniq_database/krakuniq_refseqV218/"
       estimate_precision: 12
-    sckmer:
-      cb_len: 16
-      umi_len: 10
+    krak_sample_denosing:
       min_frac: 0.5
       kmer_len: 35
-      nsample: 1000
+      min_dust: 0.1
+      min_entropy: 1.2
+    krak_study_denosing:
+      min_reads: 2
+      min_uniq: 2
+      cell_line: /data/project/host-microbiome/microcat/microcat/single_wf/data/cell.lines.txt
+
 
 
 output:
   simulate: results/00.simulate
   raw: results/00.raw
   trimming: results/01.trimming
   host: results/02.host
@@ -127,17 +131,17 @@
   pathseq:
     threads: 24
     mem_mb: 200000
   
 
 
 scripts:
-  extract_microbiome_output: scripts/extract_microbiome_output.R
+  extract_kraken_output: scripts/extract_kraken_output.py
   kraken2mpa: scripts/kraken2mpa.py
   kraken2sc: scripts/kraken2sc.py
   extract_kraken_reads: scripts/extract_kraken_reads.py
-  krak2_output_denosing: scripts/krak2_output_denosing.R
-  sckmer_unpaired: scripts/sckmer_unpaired.R
+  krak2_output_denosing: scripts/krak2_output_denosing.py
+  krak_sample_denosing: scripts/krak_sample_denosing.py
+  krak_study_denosing: scripts/krak_study_denosing.py
   spilt_bam_by_tag: scripts/spilt_bam_by_tag.py
-  sample_denosing: scripts/sample_denosing.R
   INVADEseq: scripts/INVADEseq.py
   starsolo_10X_auto: scripts/starsolo_tenX_auto.sh
```

### Comparing `microcat-0.2.6rc0/microcat.egg-info/PKG-INFO` & `microcat-0.2.7b0/microcat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.6rc0
+Version: 0.2.7b0
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.6rc0/microcat.egg-info/SOURCES.txt` & `microcat-0.2.7b0/microcat.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 microcat/__about__.py
 microcat/__init__.py
 microcat/chemistry_defs.json
 microcat/cli.py
 microcat/configer.py
+microcat/download_celline.py
 microcat/prepare.py
 microcat/sample.py
 microcat.egg-info/PKG-INFO
 microcat.egg-info/SOURCES.txt
 microcat.egg-info/dependency_links.txt
 microcat.egg-info/entry_points.txt
 microcat.egg-info/requires.txt
@@ -41,19 +42,25 @@
 microcat/single_wf/rules/build.smk
 microcat/single_wf/rules/classfier.smk
 microcat/single_wf/rules/database.smk
 microcat/single_wf/rules/host.smk
 microcat/single_wf/scripts/INVADEseq.py
 microcat/single_wf/scripts/add_tags_to_PathSeq_bam.py
 microcat/single_wf/scripts/create_hdf5.py
+microcat/single_wf/scripts/extract_kraken_output.py
 microcat/single_wf/scripts/extract_kraken_reads.py
 microcat/single_wf/scripts/extract_microbiome_output.R
+microcat/single_wf/scripts/extrat_test.py
 microcat/single_wf/scripts/generate_PE_manifest_file.py
 microcat/single_wf/scripts/get_ncbi_domains.py
 microcat/single_wf/scripts/krak2_output_denosing.R
+microcat/single_wf/scripts/krak2_output_denosing.py
+microcat/single_wf/scripts/krak_cell_denosing copy.py
+microcat/single_wf/scripts/krak_sample_denosing.py
+microcat/single_wf/scripts/krak_study_denosing.py
 microcat/single_wf/scripts/kraken2mpa.py
 microcat/single_wf/scripts/kraken2sc.py
 microcat/single_wf/scripts/microcat_bam_handle.Rmd
 microcat/single_wf/scripts/sample_denosing.R
 microcat/single_wf/scripts/sckmer_unpaired.R
 microcat/single_wf/scripts/spilt_bam_by_tag.py
 microcat/single_wf/scripts/split_Starsolo_BAM_by_RG.py
```

### Comparing `microcat-0.2.6rc0/setup.py` & `microcat-0.2.7b0/setup.py`

 * *Files identical despite different names*

