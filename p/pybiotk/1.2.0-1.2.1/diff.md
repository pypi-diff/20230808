# Comparing `tmp/pybiotk-1.2.0.tar.gz` & `tmp/pybiotk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiotk-1.2.0.tar", last modified: Mon Jun 19 02:25:39 2023, max compression
+gzip compressed data, was "pybiotk-1.2.1.tar", last modified: Tue Aug  8 07:50:16 2023, max compression
```

## Comparing `pybiotk-1.2.0.tar` & `pybiotk-1.2.1.tar`

### file list

```diff
@@ -1,137 +1,138 @@
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      590 2022-07-04 07:56:59.000000 pybiotk-1.2.0/.coveragerc
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      583 2022-07-07 06:33:07.000000 pybiotk-1.2.0/.gitignore
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      490 2022-07-04 07:56:59.000000 pybiotk-1.2.0/.readthedocs.yml
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       77 2022-07-04 07:56:59.000000 pybiotk-1.2.0/AUTHORS.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      128 2022-07-04 07:56:59.000000 pybiotk-1.2.0/CHANGELOG.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    13815 2022-07-04 07:56:59.000000 pybiotk-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1079 2022-07-04 07:56:59.000000 pybiotk-1.2.0/LICENSE.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3351 2023-06-19 02:25:39.000000 pybiotk-1.2.0/PKG-INFO
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2932 2023-05-15 09:36:22.000000 pybiotk-1.2.0/README.md
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4004 2023-05-15 09:36:22.000000 pybiotk-1.2.0/README.rst
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/docs/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1154 2022-07-04 07:56:59.000000 pybiotk-1.2.0/docs/Makefile
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/docs/_static/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       18 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/_static/.gitignore
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       41 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/authors.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       43 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/changelog.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9734 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/conf.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       33 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/contributing.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2313 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/index.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       67 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/license.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       39 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/readme.rst
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      122 2022-08-02 09:43:12.000000 pybiotk-1.2.0/docs/requirements.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      408 2022-07-19 02:24:18.000000 pybiotk-1.2.0/pyproject.toml
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/rscripts/
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     7058 2023-06-08 09:57:01.000000 pybiotk-1.2.0/rscripts/diff_expr_DESeq2.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     5704 2023-04-02 13:07:58.000000 pybiotk-1.2.0/rscripts/diff_expr_edgeR.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)    16758 2023-06-08 09:57:01.000000 pybiotk-1.2.0/rscripts/diff_expr_plot.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3017 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/peak_anno.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3112 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_FRiPs.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     2517 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_bar.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     8523 2023-04-02 13:09:25.000000 pybiotk-1.2.0/rscripts/plot_chip_summary.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3661 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_corr.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3921 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_deeptools_fragmentsize.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1918 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_hist.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     4114 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_peak_width.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3086 2023-04-14 12:58:41.000000 pybiotk-1.2.0/rscripts/plot_rep_cor.R
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     2079 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_venn.R
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/scripts/
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      196 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fasta_len.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      147 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fasta_u2t.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      206 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fastq_len.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      165 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/get_chrom_length.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1010 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/gtfparser.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      555 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/merge_subseq.sh
--rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1296 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/remove_duplicates.sh
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2358 2023-06-19 02:22:37.000000 pybiotk-1.2.0/setup.cfg
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1222 2022-07-19 09:16:34.000000 pybiotk-1.2.0/setup.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:37.000000 pybiotk-1.2.0/src/
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/bx/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7429 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/binBits.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      830 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/binBits.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6253 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/bits.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1814 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/bits.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9273 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/bitset.pyx
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8110 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/cluster.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      905 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/cluster.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3795 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/cluster.pyx
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1508 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/common.c
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      639 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/common.h
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    17210 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/intersection.pyx
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:01.000000 pybiotk-1.2.0/src/pybiotk/__init__.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/annodb/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       99 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/annodb/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7267 2022-10-26 08:57:07.000000 pybiotk-1.2.0/src/pybiotk/annodb/anno.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8702 2022-10-25 09:30:11.000000 pybiotk-1.2.0/src/pybiotk/annodb/gene.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8634 2023-01-30 02:31:13.000000 pybiotk-1.2.0/src/pybiotk/annodb/merged_transcript.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6068 2022-10-25 09:30:11.000000 pybiotk-1.2.0/src/pybiotk/annodb/transcript.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/convert/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/convert/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3813 2022-09-06 07:47:21.000000 pybiotk-1.2.0/src/pybiotk/convert/bam2fastx.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1149 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/convert/bampe_order_by_name.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1697 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/convert/bed2bedgraph.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      709 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/convert/fq2fasta.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4691 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/convert/gtf2bed.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/data/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    11177 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/hg38.chrom.sizes
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2410 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/mm10.chrom.sizes
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/intervals/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       79 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4555 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/grange.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2441 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/merge_bed3.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2642 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/merge_intervals.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/io/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      451 2023-04-26 11:55:13.000000 pybiotk-1.2.0/src/pybiotk/io/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10840 2022-10-10 08:54:31.000000 pybiotk-1.2.0/src/pybiotk/io/bam.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6230 2022-09-26 13:01:34.000000 pybiotk-1.2.0/src/pybiotk/io/bed.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7710 2023-02-01 07:48:01.000000 pybiotk-1.2.0/src/pybiotk/io/bw.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4575 2023-04-26 12:15:18.000000 pybiotk-1.2.0/src/pybiotk/io/fasta.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4346 2022-09-14 15:02:58.000000 pybiotk-1.2.0/src/pybiotk/io/fastq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    19645 2023-05-15 09:36:23.000000 pybiotk-1.2.0/src/pybiotk/io/gtf.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/pybiotk/string/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       44 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      946 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/motif.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      714 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/sequence.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/pybiotk/utils/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       21 2022-07-04 07:57:03.000000 pybiotk-1.2.0/src/pybiotk/utils/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2525 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/bam_random.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1230 2023-04-26 11:55:13.000000 pybiotk-1.2.0/src/pybiotk/utils/fasta_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5292 2022-09-14 15:02:58.000000 pybiotk-1.2.0/src/pybiotk/utils/fastq_join.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3985 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/fastq_uniq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1708 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/fastx_rename.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4182 2022-08-02 09:43:12.000000 pybiotk-1.2.0/src/pybiotk/utils/fragment_size.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9967 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/genomefetcher.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2936 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/gtf_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5805 2023-04-02 13:09:25.000000 pybiotk-1.2.0/src/pybiotk/utils/merge_row.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2391 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/utils/merge_subseq.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3664 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/normalize.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10682 2023-04-26 11:55:14.000000 pybiotk-1.2.0/src/pybiotk/utils/pyanno.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3284 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/read_tables.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2234 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/utils/reference_count.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1620 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/reverse_fastx.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3114 2023-05-15 09:36:23.000000 pybiotk-1.2.0/src/pybiotk/utils/rmats_filter.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2778 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/seq_random.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4093 2022-09-06 07:47:21.000000 pybiotk-1.2.0/src/pybiotk/utils/subseq_analysis.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    14283 2023-04-02 13:09:25.000000 pybiotk-1.2.0/src/pybiotk/utils/summary_log.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9118 2023-06-08 10:23:58.000000 pybiotk-1.2.0/src/pybiotk/utils/utils.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk.egg-info/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3351 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/PKG-INFO
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2961 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/SOURCES.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/dependency_links.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1102 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/entry_points.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2022-07-04 07:59:58.000000 pybiotk-1.2.0/src/pybiotk.egg-info/not-zip-safe
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       93 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/requires.txt
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       15 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/top_level.txt
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/stream/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       20 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/stream/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10873 2023-06-08 10:05:34.000000 pybiotk-1.2.0/src/stream/pipe.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7886 2022-09-14 14:59:43.000000 pybiotk-1.2.0/src/stream/stream.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/tests/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/__init__.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      132 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/conftest.py
-drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/tests/test_stream/
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      195 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/test_stream/test_pipe.py
--rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2575 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tox.ini
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      590 2023-08-08 07:07:16.000000 pybiotk-1.2.1/.coveragerc
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      583 2023-08-08 07:07:16.000000 pybiotk-1.2.1/.gitignore
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      490 2023-08-08 07:07:16.000000 pybiotk-1.2.1/.readthedocs.yml
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       77 2023-08-08 07:07:16.000000 pybiotk-1.2.1/AUTHORS.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      128 2023-08-08 07:07:16.000000 pybiotk-1.2.1/CHANGELOG.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    13815 2023-08-08 07:07:16.000000 pybiotk-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1079 2023-08-08 07:07:16.000000 pybiotk-1.2.1/LICENSE.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3351 2023-08-08 07:50:16.136702 pybiotk-1.2.1/PKG-INFO
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2932 2023-08-08 07:07:16.000000 pybiotk-1.2.1/README.md
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4004 2023-08-08 07:07:16.000000 pybiotk-1.2.1/README.rst
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/docs/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1154 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/Makefile
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/docs/_static/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       18 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/_static/.gitignore
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       41 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/authors.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       43 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/changelog.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9734 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/conf.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       33 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/contributing.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2313 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/index.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       67 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/license.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       39 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/readme.rst
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      122 2023-08-08 07:07:16.000000 pybiotk-1.2.1/docs/requirements.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      415 2023-08-08 07:07:16.000000 pybiotk-1.2.1/pyproject.toml
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/rscripts/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7058 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/diff_expr_DESeq2.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5704 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/diff_expr_edgeR.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    16758 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/diff_expr_plot.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3017 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/peak_anno.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3112 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_FRiPs.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2517 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_bar.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     8523 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_chip_summary.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3661 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_corr.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3921 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_deeptools_fragmentsize.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1918 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_hist.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4114 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_peak_width.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3086 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_rep_cor.R
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2079 2023-08-08 07:48:35.000000 pybiotk-1.2.1/rscripts/plot_venn.R
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/scripts/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      196 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/fasta_len.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      147 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/fasta_u2t.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      206 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/fastq_len.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      165 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/get_chrom_length.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1010 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/gtfparser.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      555 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/merge_subseq.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1296 2023-08-08 07:48:35.000000 pybiotk-1.2.1/scripts/remove_duplicates.sh
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2399 2023-08-08 07:50:16.136702 pybiotk-1.2.1/setup.cfg
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1222 2023-08-08 07:07:16.000000 pybiotk-1.2.1/setup.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.126702 pybiotk-1.2.1/src/
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/bx/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7429 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/binBits.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      830 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/binBits.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     6253 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/bits.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1814 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/bits.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9273 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/bitset.pyx
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     8110 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/cluster.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      905 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/cluster.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3795 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/cluster.pyx
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1508 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/common.c
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      639 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/common.h
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    17210 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/bx/intersection.pyx
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/__init__.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/annodb/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       99 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/annodb/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7473 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/annodb/anno.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     8766 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/annodb/gene.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    11882 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/annodb/merged_transcript.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     6311 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/annodb/transcript.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/convert/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3813 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/bam2fastx.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1149 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/bampe_order_by_name.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1697 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/bed2bedgraph.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      672 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/fa2fastq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      709 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/fq2fasta.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4691 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/convert/gtf2bed.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/data/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/data/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    11177 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/data/hg38.chrom.sizes
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2410 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/data/mm10.chrom.sizes
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/intervals/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       79 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/intervals/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4842 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/intervals/grange.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2441 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/intervals/merge_bed3.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2642 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/intervals/merge_intervals.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/io/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      451 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    10840 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/bam.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     6230 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/bed.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7710 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/bw.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4795 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/fasta.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4505 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/fastq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    19645 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/io/gtf.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/string/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       44 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/string/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      946 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/string/motif.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      714 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/string/sequence.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk/utils/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       21 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2525 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/bam_random.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1230 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/fasta_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5292 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/fastq_join.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3985 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/fastq_uniq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1708 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/fastx_rename.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4182 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/fragment_size.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9967 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/genomefetcher.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2936 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/gtf_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     5805 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/merge_row.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2391 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/merge_subseq.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3664 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/normalize.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    10762 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/pyanno.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3284 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/read_tables.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2234 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/reference_count.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1620 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/reverse_fastx.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3114 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/rmats_filter.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2778 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/seq_random.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     4093 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/subseq_analysis.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    14283 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/summary_log.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     9118 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/pybiotk/utils/utils.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/pybiotk.egg-info/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     3351 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/PKG-INFO
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2993 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        1 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     1142 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/entry_points.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        1 2023-08-08 07:40:46.000000 pybiotk-1.2.1/src/pybiotk.egg-info/not-zip-safe
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       93 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/requires.txt
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       15 2023-08-08 07:50:16.000000 pybiotk-1.2.1/src/pybiotk.egg-info/top_level.txt
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/src/stream/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)       20 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/stream/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)    10873 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/stream/pipe.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     7886 2023-08-08 07:07:16.000000 pybiotk-1.2.1/src/stream/stream.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/tests/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:07:16.000000 pybiotk-1.2.1/tests/__init__.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      132 2023-08-08 07:07:16.000000 pybiotk-1.2.1/tests/conftest.py
+drwxr-xr-x   0 liqiming  (1000) liqiming  (1000)        0 2023-08-08 07:50:16.136702 pybiotk-1.2.1/tests/test_stream/
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)      195 2023-08-08 07:07:16.000000 pybiotk-1.2.1/tests/test_stream/test_pipe.py
+-rw-r--r--   0 liqiming  (1000) liqiming  (1000)     2575 2023-08-08 07:07:16.000000 pybiotk-1.2.1/tox.ini
```

### Comparing `pybiotk-1.2.0/.coveragerc` & `pybiotk-1.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/.gitignore` & `pybiotk-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/CONTRIBUTING.rst` & `pybiotk-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/LICENSE.txt` & `pybiotk-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/PKG-INFO` & `pybiotk-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiotk
-Version: 1.2.0
+Version: 1.2.1
 Summary: pybiotk: A python toolkit for bioinformatics analysis.
 Home-page: https://github.com/liqiming-whu/pybiotk
 Author: liqiming_whu
 Author-email: liqiming@whu.edu.cn
 License: MIT
 Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
 Platform: any
```

### Comparing `pybiotk-1.2.0/README.md` & `pybiotk-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/README.rst` & `pybiotk-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/docs/Makefile` & `pybiotk-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/docs/conf.py` & `pybiotk-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/docs/index.rst` & `pybiotk-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/diff_expr_DESeq2.R` & `pybiotk-1.2.1/rscripts/diff_expr_DESeq2.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/diff_expr_edgeR.R` & `pybiotk-1.2.1/rscripts/diff_expr_edgeR.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/diff_expr_plot.R` & `pybiotk-1.2.1/rscripts/diff_expr_plot.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/peak_anno.R` & `pybiotk-1.2.1/rscripts/peak_anno.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_FRiPs.R` & `pybiotk-1.2.1/rscripts/plot_FRiPs.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_bar.R` & `pybiotk-1.2.1/rscripts/plot_bar.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_chip_summary.R` & `pybiotk-1.2.1/rscripts/plot_chip_summary.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_corr.R` & `pybiotk-1.2.1/rscripts/plot_corr.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_deeptools_fragmentsize.R` & `pybiotk-1.2.1/rscripts/plot_deeptools_fragmentsize.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_hist.R` & `pybiotk-1.2.1/rscripts/plot_hist.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_peak_width.R` & `pybiotk-1.2.1/rscripts/plot_peak_width.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_rep_cor.R` & `pybiotk-1.2.1/rscripts/plot_rep_cor.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/rscripts/plot_venn.R` & `pybiotk-1.2.1/rscripts/plot_venn.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/scripts/gtfparser.sh` & `pybiotk-1.2.1/scripts/gtfparser.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/scripts/merge_subseq.sh` & `pybiotk-1.2.1/scripts/merge_subseq.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/scripts/remove_duplicates.sh` & `pybiotk-1.2.1/scripts/remove_duplicates.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/setup.cfg` & `pybiotk-1.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybiotk
-version = 1.2.0
+version = 1.2.1
 description = pybiotk: A python toolkit for bioinformatics analysis.
 author = liqiming_whu
 author_email = liqiming@whu.edu.cn
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -44,14 +44,15 @@
 	pytest-cov
 
 [options.entry_points]
 console_scripts = 
 	gtf2bed = pybiotk.convert.gtf2bed:run
 	bed2bedgraph = pybiotk.convert.bed2bedgraph:run
 	fq2fasta = pybiotk.convert.fq2fasta:run
+	fa2fastq = pybiotk.convert.fa2fastq:run
 	bam2fastx = pybiotk.convert.bam2fastx:run
 	bampe_order_by_name = pybiotk.convert.bampe_order_by_name:run
 	bam_random = pybiotk.utils.bam_random:run
 	gtf_filter = pybiotk.utils.gtf_filter:run
 	fasta_filter = pybiotk.utils.fasta_filter:run
 	fastq_uniq = pybiotk.utils.fastq_uniq:run
 	fastq_join = pybiotk.utils.fastq_join:run
```

### Comparing `pybiotk-1.2.0/setup.py` & `pybiotk-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/binBits.c` & `pybiotk-1.2.1/src/bx/binBits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/binBits.h` & `pybiotk-1.2.1/src/bx/binBits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/bits.c` & `pybiotk-1.2.1/src/bx/bits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/bits.h` & `pybiotk-1.2.1/src/bx/bits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/bitset.pyx` & `pybiotk-1.2.1/src/bx/bitset.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/cluster.c` & `pybiotk-1.2.1/src/bx/cluster.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/cluster.h` & `pybiotk-1.2.1/src/bx/cluster.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/cluster.pyx` & `pybiotk-1.2.1/src/bx/cluster.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/common.c` & `pybiotk-1.2.1/src/bx/common.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/common.h` & `pybiotk-1.2.1/src/bx/common.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/bx/intersection.pyx` & `pybiotk-1.2.1/src/bx/intersection.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/annodb/anno.py` & `pybiotk-1.2.1/src/pybiotk/annodb/anno.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,20 +141,29 @@
     def cds_exons(self) -> List[Tuple[int, int]]: ...
 
     @abstractmethod
     def utr5_exons(self) -> List[Tuple[int, int]]: ...
 
     @abstractmethod
     def utr3_exons(self) -> List[Tuple[int, int]]: ...
+    
+    @abstractmethod
+    def length(self) -> int: ...
 
     def exons_len(self) -> int:
         return blocks_len(self.exons())
+    
+    def exons_count(self) -> int:
+        return len(self.exons())
 
     def introns_len(self) -> int:
         return blocks_len(self.introns())
+    
+    def introns_count(self) -> int:
+        return len(self.introns())
 
     def cds_len(self) -> int:
         return blocks_len(self.cds_exons())
 
     def utr5_len(self) -> int:
         return blocks_len(self.utr5_exons())
```

### Comparing `pybiotk-1.2.0/src/pybiotk/annodb/gene.py` & `pybiotk-1.2.1/src/pybiotk/annodb/gene.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,10 +210,13 @@
             self._classify_exons()
         return self._utr5_exons
 
     def utr3_exons(self) -> List[Tuple[int, int]]:
         if self._utr3_exons is None:
             self._classify_exons()
         return self._utr3_exons
+    
+    def length(self):
+        return self.end - self.start
 
     def annotation(self, blocks: List[Tuple[int, int]], tss_region: Tuple[int, int] = (-1000, 1000), downstream: int = 3000) -> GenomicAnnotation:
         return GenomicAnnotation(self.gene_id, self.gene_name, self.start, self.end, self.gene_type, self.anno(blocks, tss_region, downstream))
```

### Comparing `pybiotk-1.2.0/src/pybiotk/annodb/merged_transcript.py` & `pybiotk-1.2.1/src/pybiotk/annodb/merged_transcript.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
  # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import itertools
 import os
+import warnings
 from collections import deque
 from functools import partial
 from typing import List, Dict, Tuple, Literal, Iterable, Iterator, Sequence, Optional, TYPE_CHECKING
 
+from pybiotk.annodb.anno import GFeature
 from pybiotk.intervals import merge_intervals
 from pybiotk.io.bed import Bed6
 from pybiotk.utils import bedtools_sort
-from stream import window, to_list, filter, transform, mapwith, apply, uniq, flatten
+from stream import window, to_list, filter, transform, mapwith, apply, uniq, flatten, skip_while
 
 if TYPE_CHECKING:
     from pybiotk.io import GtfFile
     from pybiotk.annodb import Transcript
 
 
-class MergedTranscript:
+class MergedTranscript(GFeature):
     def __init__(
         self,
         transcript_id: Optional[str] = None,
         transcript_name: Optional[str] = None,
         transcript_type: Optional[str] = None,
         gene_id: Optional[str] = None,
         gene_name: Optional[str] = None,
@@ -45,15 +47,19 @@
         self.gene_type = gene_type
         self.chrom = chrom
         self.start = int(start)
         self.end = int(end)
         self.strand = strand
         self.cds_start = int(cds_start) if cds_start is not None else cds_start
         self.cds_end = int(cds_end) if cds_end is not None else cds_end
-        self.exons = exons
+        self._exons = list(exons)
+        self._introns = None
+        self._cds_exons = None
+        self._utr5_exons = None
+        self._utr3_exons = None
         self.count = count
         self.before = int(before) if before is not None else before
         self.after = int(after) if after is not None else after
 
     def __repr__(self) -> str:
         return f"{self.gene_name}:{self.chrom}:{self.start}-{self.end}({self.strand})"
 
@@ -114,14 +120,71 @@
         chrom = ",".join(list(chroms))
         strand = ",".join(list(strands))
         return cls(transcript_id, transcript_name, transcript_type,
                    gene_id, gene_name, gene_type,
                    chrom, start, end, strand,
                    cds_start, cds_end, exons, count)
 
+    def _classify_exons(self):
+        if self.cds_start is not None and self.cds_end is not None:
+            utr5_exons = []
+            utr3_exons = []
+            cds_exons = []
+            for exon in self.exons():
+                if exon[1] <= self.cds_start:
+                    utr5_exons.append(exon)
+                elif exon[0] >= self.cds_end:
+                    utr3_exons.append(exon)
+                elif self.cds_start <= exon[0] and exon[1] <= self.cds_end:
+                    cds_exons.append(exon)
+                elif exon[0] < self.cds_start < exon[1] <= self.cds_end:
+                    utr5_exons.append((exon[0], self.cds_start))
+                    cds_exons.append((self.cds_start, exon[1]))
+                elif self.cds_start <= exon[0] < self.cds_end < exon[1]:
+                    cds_exons.append((exon[0], self.cds_end))
+                    utr3_exons.append((self.cds_end, exon[1]))
+                elif exon[0] < self.cds_start and self.cds_end < exon[1]:
+                    utr5_exons.append((exon[0], self.cds_start))
+                    cds_exons.append((self.cds_start, self.cds_end))
+                    utr3_exons.append((self.cds_end, exon[1]))
+
+            if self.strand == '-':
+                utr5_exons, utr3_exons = utr3_exons, utr5_exons
+                self._utr5_exons = utr5_exons
+                self._cds_exons = cds_exons
+                self._utr3_exons = utr3_exons
+            loginfo = f"merged exons: {self.exons()}\ncds_start: {self.cds_start}, cds_end: {self.cds_end}"
+            if not cds_exons:
+                warnings.warn(f"cds_exons of {self.gene_id} does not exist, please check:\n{loginfo}")
+        else:
+            self._utr5_exons = []
+            self._cds_exons = []
+            self._utr3_exons = []
+
+    def is_protein_coding(self) -> bool:
+        if self.gene_type == 'protein_coding':
+            return True
+        else:
+            return False
+
+    def exons(self) -> List[Tuple[int, int]]:
+        return self._exons
+
+    def introns(self) -> List[Tuple[int, int]]:
+        if self._introns is None:
+            self._introns = [self.start, *(self.exons() | flatten), self.end] | window(2, 2) | skip_while(lambda x: x[0] == x[1]) | to_list
+        return self._introns
+
+    def tss_region(self, region: Tuple[int, int] = (-1000, 1000)) -> Tuple[int, ...]:
+        if self.strand == '+':
+            region = tuple(i+self.start for i in region)
+        else:
+            region = tuple(reversed(tuple(self.end-i for i in region)))
+        return region
+
     def to_bed6(self) -> Bed6:
         return Bed6(self.chrom, self.start, self.end, self.gene_name, str(self.count), self.strand)
 
     def upStream(self):
         if self.strand == '-':
             return self.after
         else:
@@ -129,14 +192,31 @@
 
     def downStream(self):
         if self.strand == '-':
             return self.before
         else:
             return self.after
 
+    downstream = downStream
+
+    def cds_exons(self) -> List[Tuple[int, int]]:
+        if self._cds_exons is None:
+            self._classify_exons()
+        return self._cds_exons
+
+    def utr5_exons(self) -> List[Tuple[int, int]]:
+        if self._utr5_exons is None:
+            self._classify_exons()
+        return self._utr5_exons
+
+    def utr3_exons(self) -> List[Tuple[int, int]]:
+        if self._utr3_exons is None:
+            self._classify_exons()
+        return self._utr3_exons
+
     def length(self):
         return self.end - self.start
 
 
 def group_overlap_transcripts(iterable: Iterable[Transcript]) -> Iterator[Tuple[Transcript, ...]]:
     a = deque(itertools.islice(iterable, 1))
     max_end = 0
```

### Comparing `pybiotk-1.2.0/src/pybiotk/annodb/transcript.py` & `pybiotk-1.2.1/src/pybiotk/annodb/transcript.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,18 @@
 
     def update(self, gtf: GTF):
         self.end = gtf.end
         self._exons.append((gtf.start-1, gtf.end))
 
     @classmethod
     def init_by_bed(cls, transinfo: TransInfo, bed12: Bed12):
-        return cls(*transinfo.__slots__, bed12.chrom, bed12.start, bed12.end,
+        return cls(transinfo.transcript_id, transinfo.transcript_name,
+                   transinfo.transcript_type, transinfo.gene_id,
+                   transinfo.gene_name, transinfo.gene_type,
+                   bed12.chrom, bed12.start, bed12.end,
                    bed12.strand, bed12.thickStart, bed12.thickEnd, bed12.exons())
 
     def is_protein_coding(self) -> bool:
         if self.transcript_type == 'protein_coding':
             return True
         else:
             return False
@@ -144,10 +147,13 @@
             self._classify_exons()
         return self._utr5_exons
 
     def utr3_exons(self) -> List[Tuple[int, int]]:
         if self._utr3_exons is None:
             self._classify_exons()
         return self._utr3_exons
-
+    
+    def length(self):
+        return self.end - self.start
+    
     def annotation(self, blocks: List[Tuple[int, int]], tss_region: Tuple[int, int] = (-1000, 1000), downstream: int = 3000) -> GenomicAnnotation:
         return GenomicAnnotation(self.transcript_id, self.gene_name, self.start, self.end, self.transcript_type, self.anno(blocks, tss_region, downstream))
```

### Comparing `pybiotk-1.2.0/src/pybiotk/convert/bam2fastx.py` & `pybiotk-1.2.1/src/pybiotk/convert/bam2fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/convert/bampe_order_by_name.py` & `pybiotk-1.2.1/src/pybiotk/convert/bampe_order_by_name.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/convert/bed2bedgraph.py` & `pybiotk-1.2.1/src/pybiotk/convert/bed2bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/convert/fq2fasta.py` & `pybiotk-1.2.1/src/pybiotk/convert/fq2fasta.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/convert/gtf2bed.py` & `pybiotk-1.2.1/src/pybiotk/convert/gtf2bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/data/hg38.chrom.sizes` & `pybiotk-1.2.1/src/pybiotk/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/data/mm10.chrom.sizes` & `pybiotk-1.2.1/src/pybiotk/data/mm10.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/intervals/grange.py` & `pybiotk-1.2.1/src/pybiotk/intervals/grange.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,21 @@
         if self.chrom != other.chrom:
             return False
         if self.strand != other.strand:
             return False
         if not is_overlap((self.start, self.end), (other.start, other.end)):
             return False
         return True
+    
+    def is_match(self, other: GRange, shift_cutoff: int = 2) -> bool:
+        if not self.is_overlap(other):
+            return False
+        if(abs(self.start-other.start) <= shift_cutoff) and (abs(self.end-other.end) <= shift_cutoff):
+            return True
+        return False
 
 
 class GRangeTree:
     def __init__(self, strand: bool = False):
         self.strand: bool = strand
         self._trees: Dict[Union[str, Tuple[str, ...]], IntervalTree] = {}
```

### Comparing `pybiotk-1.2.0/src/pybiotk/intervals/merge_bed3.py` & `pybiotk-1.2.1/src/pybiotk/intervals/merge_bed3.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/intervals/merge_intervals.py` & `pybiotk-1.2.1/src/pybiotk/intervals/merge_intervals.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/io/bam.py` & `pybiotk-1.2.1/src/pybiotk/io/bam.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/io/bed.py` & `pybiotk-1.2.1/src/pybiotk/io/bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/io/bw.py` & `pybiotk-1.2.1/src/pybiotk/io/bw.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/io/fasta.py` & `pybiotk-1.2.1/src/pybiotk/io/fasta.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import random
 import re
 import sys
 from typing import Dict, List, Sequence, Iterable, Iterator, Tuple, Literal, Callable, Optional
 
 import pysam
 
+from pybiotk.io.fastq import OpenFqGzip
 from pybiotk.intervals import GRange
 from pybiotk.utils import reverse_seq
 
 
 class FastaFile(pysam.FastaFile):
     def __init__(self, /, *args, **kwargs):
         super().__init__()
@@ -62,14 +63,19 @@
         if strand == "-":
             sequence = reverse_seq(sequence)
         return sequence
 
     def dict_fetch(self, reference: str, start: int, end: int, strand: Literal["+", "-"] = "+"):
         assert self.reference_dict is not None
         return self.fetch_use_dict(self.reference_dict, reference, start, end, strand)
+    
+    def to_fastq(self, path: str = "-"):
+        with OpenFqGzip(path) as fq:
+            for reference, sequence in self:
+                fq.write_entry(reference, sequence)
 
 
 class GenomeFile(FastaFile):
     def __init__(self, /, *args, **kwargs):
         super().__init__()
         self.custom_chroms: List[str] = self.chroms_norm()
```

### Comparing `pybiotk-1.2.0/src/pybiotk/io/fastq.py` & `pybiotk-1.2.1/src/pybiotk/io/fastq.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,19 @@
     def __init__(self, /, *args, **kwargs):
         super().__init__()
         self.ptr: Optional[int] = None
 
     def to_fasta(self) -> Iterator[str]:
         for entry in self:
             yield f">{entry.name}\n{entry.sequence}"
+    
+    def to_fastq(self, path: str = "-"):
+        with OpenFqGzip(path) as fq:
+            for entry in self:
+                fq.write_fastx_record(entry)
 
     def uniq(self, by: Literal["id", "name", "seq"] = "seq") -> Iterator[pysam.libcfaidx.FastxRecord]:
         self.ptr = 0
         unique = set()
         for entry in self:
             self.ptr += 1
             if by == "seq":
```

### Comparing `pybiotk-1.2.0/src/pybiotk/io/gtf.py` & `pybiotk-1.2.1/src/pybiotk/io/gtf.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/string/motif.py` & `pybiotk-1.2.1/src/pybiotk/string/motif.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/string/sequence.py` & `pybiotk-1.2.1/src/pybiotk/string/sequence.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/bam_random.py` & `pybiotk-1.2.1/src/pybiotk/utils/bam_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/fasta_filter.py` & `pybiotk-1.2.1/src/pybiotk/utils/fasta_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/fastq_join.py` & `pybiotk-1.2.1/src/pybiotk/utils/fastq_join.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/fastq_uniq.py` & `pybiotk-1.2.1/src/pybiotk/utils/fastq_uniq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/fastx_rename.py` & `pybiotk-1.2.1/src/pybiotk/utils/fastx_rename.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/fragment_size.py` & `pybiotk-1.2.1/src/pybiotk/utils/fragment_size.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/genomefetcher.py` & `pybiotk-1.2.1/src/pybiotk/utils/genomefetcher.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/gtf_filter.py` & `pybiotk-1.2.1/src/pybiotk/utils/gtf_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/merge_row.py` & `pybiotk-1.2.1/src/pybiotk/utils/merge_row.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/merge_subseq.py` & `pybiotk-1.2.1/src/pybiotk/utils/merge_subseq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/normalize.py` & `pybiotk-1.2.1/src/pybiotk/utils/normalize.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/pyanno.py` & `pybiotk-1.2.1/src/pybiotk/utils/pyanno.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,16 @@
                 file_obj.write(f"{bed.name}\t{bed.chrom}\t{bed.start}\t{bed.end}\t{bed.strand}\tIntergenic\t*\t*\t*\t*\t*\n")
             else:
                 annoset = AnnoSet(gene.annotation([(bed.start, bed.end)], tss_region, downstream) for gene in genes)
                 gene_types = set(gene.gene_type for gene in genes if gene.id in set(annoset.id))
                 if not ("protein_coding" in gene_types and "protein_coding" not in set(annoset.type)):
                     annoset.type = gene_types
                 anno_str = str(annoset)
-                anno_str = tss_region_name if anno_str == "Promoter" else anno_str
-                anno_str = downstream_name if anno_str == "Downstream" else anno_str
+                anno_str = anno_str.replace("Promoter", tss_region_name) if anno_str.startswith("Promoter") else anno_str
+                anno_str = anno_str.replace("Downstream", downstream_name) if anno_str.startswith("Downstream") else anno_str
                 file_obj.write(f"{bed.name}\t{bed.chrom}\t{bed.start}\t{bed.end}\t{bed.strand}\t{anno_str}\n")
             i += 1
         sys.stderr.write(f"annotate {i} beds.\n")
 
 
 def main(
     filename: str,
```

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/read_tables.py` & `pybiotk-1.2.1/src/pybiotk/utils/read_tables.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/reference_count.py` & `pybiotk-1.2.1/src/pybiotk/utils/reference_count.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/reverse_fastx.py` & `pybiotk-1.2.1/src/pybiotk/utils/reverse_fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/rmats_filter.py` & `pybiotk-1.2.1/src/pybiotk/utils/rmats_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/seq_random.py` & `pybiotk-1.2.1/src/pybiotk/utils/seq_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/subseq_analysis.py` & `pybiotk-1.2.1/src/pybiotk/utils/subseq_analysis.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/summary_log.py` & `pybiotk-1.2.1/src/pybiotk/utils/summary_log.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk/utils/utils.py` & `pybiotk-1.2.1/src/pybiotk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/pybiotk.egg-info/PKG-INFO` & `pybiotk-1.2.1/src/pybiotk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiotk
-Version: 1.2.0
+Version: 1.2.1
 Summary: pybiotk: A python toolkit for bioinformatics analysis.
 Home-page: https://github.com/liqiming-whu/pybiotk
 Author: liqiming_whu
 Author-email: liqiming@whu.edu.cn
 License: MIT
 Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
 Platform: any
```

### Comparing `pybiotk-1.2.0/src/pybiotk.egg-info/SOURCES.txt` & `pybiotk-1.2.1/src/pybiotk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 src/pybiotk/annodb/gene.py
 src/pybiotk/annodb/merged_transcript.py
 src/pybiotk/annodb/transcript.py
 src/pybiotk/convert/__init__.py
 src/pybiotk/convert/bam2fastx.py
 src/pybiotk/convert/bampe_order_by_name.py
 src/pybiotk/convert/bed2bedgraph.py
+src/pybiotk/convert/fa2fastq.py
 src/pybiotk/convert/fq2fasta.py
 src/pybiotk/convert/gtf2bed.py
 src/pybiotk/data/__init__.py
 src/pybiotk/data/hg38.chrom.sizes
 src/pybiotk/data/mm10.chrom.sizes
 src/pybiotk/intervals/__init__.py
 src/pybiotk/intervals/grange.py
```

### Comparing `pybiotk-1.2.0/src/pybiotk.egg-info/entry_points.txt` & `pybiotk-1.2.1/src/pybiotk.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [console_scripts]
 bam2fastx = pybiotk.convert.bam2fastx:run
 bam_random = pybiotk.utils.bam_random:run
 bampe_order_by_name = pybiotk.convert.bampe_order_by_name:run
 bed2bedgraph = pybiotk.convert.bed2bedgraph:run
 count_normalize = pybiotk.utils.normalize:run
+fa2fastq = pybiotk.convert.fa2fastq:run
 fasta_filter = pybiotk.utils.fasta_filter:run
 fastq_join = pybiotk.utils.fastq_join:run
 fastq_uniq = pybiotk.utils.fastq_uniq:run
 fastx_rename = pybiotk.utils.fastx_rename:run
 fq2fasta = pybiotk.convert.fq2fasta:run
 genomefetcher = pybiotk.utils.genomefetcher:run
 gtf2bed = pybiotk.convert.gtf2bed:run
```

### Comparing `pybiotk-1.2.0/src/stream/pipe.py` & `pybiotk-1.2.1/src/stream/pipe.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/src/stream/stream.py` & `pybiotk-1.2.1/src/stream/stream.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.2.0/tox.ini` & `pybiotk-1.2.1/tox.ini`

 * *Files identical despite different names*

