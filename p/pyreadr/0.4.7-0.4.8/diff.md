# Comparing `tmp/pyreadr-0.4.7.tar.gz` & `tmp/pyreadr-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreadr-0.4.7.tar", last modified: Sat Sep 24 13:35:34 2022, max compression
+gzip compressed data, was "pyreadr-0.4.8.tar", last modified: Tue Aug  8 12:59:11 2023, max compression
```

## Comparing `pyreadr-0.4.7.tar` & `pyreadr-0.4.8.tar`

### file list

```diff
@@ -1,75 +1,90 @@
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.736727 pyreadr-0.4.7/
--rw-rw-r--   0 otto      (1000) otto      (1000)      264 2021-04-02 10:32:26.000000 pyreadr-0.4.7/MANIFEST.in
--rw-rw-r--   0 otto      (1000) otto      (1000)     1147 2022-09-24 13:35:34.736727 pyreadr-0.4.7/PKG-INFO
--rw-rw-r--   0 otto      (1000) otto      (1000)    16337 2021-04-02 13:27:32.000000 pyreadr-0.4.7/README.md
--rw-rw-r--   0 otto      (1000) otto      (1000)      114 2022-09-24 12:46:03.000000 pyreadr-0.4.7/pyproject.toml
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.715726 pyreadr-0.4.7/pyreadr/
--rw-rw-r--   0 otto      (1000) otto      (1000)      160 2022-09-24 12:48:53.000000 pyreadr-0.4.7/pyreadr/__init__.py
--rw-rw-r--   0 otto      (1000) otto      (1000)    16382 2021-04-02 13:21:49.000000 pyreadr-0.4.7/pyreadr/_pyreadr_parser.py
--rw-rw-r--   0 otto      (1000) otto      (1000)     9249 2022-09-24 12:46:03.000000 pyreadr-0.4.7/pyreadr/_pyreadr_writer.py
--rw-rw-r--   0 otto      (1000) otto      (1000)       86 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/custom_errors.py
--rw-rw-r--   0 otto      (1000) otto      (1000)   487654 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr/librdata.c
--rw-rw-r--   0 otto      (1000) otto      (1000)     7527 2022-09-24 12:46:03.000000 pyreadr-0.4.7/pyreadr/librdata.pxd
--rw-rw-r--   0 otto      (1000) otto      (1000)    12567 2022-09-24 12:46:03.000000 pyreadr-0.4.7/pyreadr/librdata.pyx
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.712726 pyreadr-0.4.7/pyreadr/libs/
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.716727 pyreadr-0.4.7/pyreadr/libs/bzip2/
--rw-rw-r--   0 otto      (1000) otto      (1000)     7192 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/bzip2/bzlib.h
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.717727 pyreadr-0.4.7/pyreadr/libs/iconv/
--rw-rw-r--   0 otto      (1000) otto      (1000)     9859 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/iconv/iconv.h
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.712726 pyreadr-0.4.7/pyreadr/libs/librdata/
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.719727 pyreadr-0.4.7/pyreadr/libs/librdata/src/
--rw-rw-r--   0 otto      (1000) otto      (1000)     5434 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/CKHashTable.c
--rw-rw-r--   0 otto      (1000) otto      (1000)     1079 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/CKHashTable.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     7052 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     1152 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_bits.c
--rw-rw-r--   0 otto      (1000) otto      (1000)      267 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_bits.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     1981 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_error.c
--rw-rw-r--   0 otto      (1000) otto      (1000)     2797 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_internal.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     2458 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_io_unistd.c
--rw-rw-r--   0 otto      (1000) otto      (1000)      555 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_io_unistd.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     3069 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_parser.c
--rw-rw-r--   0 otto      (1000) otto      (1000)    57640 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_read.c
--rw-rw-r--   0 otto      (1000) otto      (1000)    16693 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_write.c
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.719727 pyreadr-0.4.7/pyreadr/libs/lzma/
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.726727 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/
--rw-rw-r--   0 otto      (1000) otto      (1000)    24858 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/base.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     2630 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/bcj.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    22107 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/block.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     4255 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/check.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    24844 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/container.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     1865 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/delta.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    16520 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/filter.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     2604 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/hardware.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    23491 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/index.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     3914 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/index_hash.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    14744 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/lzma12.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     8253 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/stream_flags.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     3497 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/version.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     6546 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma/vli.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     9866 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/lzma/lzma.h
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.727727 pyreadr-0.4.7/pyreadr/libs/zlib/
--rw-rw-r--   0 otto      (1000) otto      (1000)    16349 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/zlib/zconf.h
--rw-rw-r--   0 otto      (1000) otto      (1000)    96239 2021-04-02 10:32:26.000000 pyreadr-0.4.7/pyreadr/libs/zlib/zlib.h
--rw-rw-r--   0 otto      (1000) otto      (1000)     8425 2021-06-05 12:27:54.000000 pyreadr-0.4.7/pyreadr/pyreadr.py
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.716727 pyreadr-0.4.7/pyreadr.egg-info/
--rw-rw-r--   0 otto      (1000) otto      (1000)     1147 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr.egg-info/PKG-INFO
--rw-rw-r--   0 otto      (1000) otto      (1000)     1752 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr.egg-info/SOURCES.txt
--rw-rw-r--   0 otto      (1000) otto      (1000)        1 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr.egg-info/dependency_links.txt
--rw-rw-r--   0 otto      (1000) otto      (1000)       14 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr.egg-info/requires.txt
--rw-rw-r--   0 otto      (1000) otto      (1000)        8 2022-09-24 13:35:34.000000 pyreadr-0.4.7/pyreadr.egg-info/top_level.txt
--rw-rw-r--   0 otto      (1000) otto      (1000)       38 2022-09-24 13:35:34.737727 pyreadr-0.4.7/setup.cfg
--rw-rw-r--   0 otto      (1000) otto      (1000)     3481 2022-09-24 12:48:40.000000 pyreadr-0.4.7/setup.py
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.712726 pyreadr-0.4.7/win_libs/
-drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2022-09-24 13:35:34.735727 pyreadr-0.4.7/win_libs/64bit/
--rw-rw-r--   0 otto      (1000) otto      (1000)    12288 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/charset.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)   938496 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/iconv.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)     3210 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/iconv.lib
--rw-rw-r--   0 otto      (1000) otto      (1000)    73888 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/libbz2-1.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/liblzma-5.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/liblzma.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/z.lib
--rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/zdll.lib
--rw-rw-r--   0 otto      (1000) otto      (1000)    83968 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/zlib.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/zlib.lib
--rw-rw-r--   0 otto      (1000) otto      (1000)    93830 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/zlib1.dll
--rw-rw-r--   0 otto      (1000) otto      (1000)   180950 2021-04-02 10:32:26.000000 pyreadr-0.4.7/win_libs/64bit/zlibstatic.lib
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.459877 pyreadr-0.4.8/
+-rw-rw-r--   0 otto      (1000) otto      (1000)    34523 2021-11-30 09:21:27.000000 pyreadr-0.4.8/LICENSE
+-rw-rw-r--   0 otto      (1000) otto      (1000)     7651 2021-11-30 09:21:27.000000 pyreadr-0.4.8/LICENSE_jamovi_readstat
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1091 2021-11-30 09:21:27.000000 pyreadr-0.4.8/LICENSE_librdata
+-rw-rw-r--   0 otto      (1000) otto      (1000)      252 2023-08-08 12:54:58.000000 pyreadr-0.4.8/MANIFEST.in
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1171 2023-08-08 12:59:11.459877 pyreadr-0.4.8/PKG-INFO
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16337 2021-11-30 09:21:27.000000 pyreadr-0.4.8/README.md
+-rw-rw-r--   0 otto      (1000) otto      (1000)      114 2022-10-24 10:57:07.000000 pyreadr-0.4.8/pyproject.toml
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.423859 pyreadr-0.4.8/pyreadr/
+-rw-rw-r--   0 otto      (1000) otto      (1000)      160 2023-08-08 12:54:58.000000 pyreadr-0.4.8/pyreadr/__init__.py
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16566 2022-08-05 11:48:30.000000 pyreadr-0.4.8/pyreadr/_pyreadr_parser.py
+-rw-rw-r--   0 otto      (1000) otto      (1000)     9539 2022-08-05 11:44:59.000000 pyreadr-0.4.8/pyreadr/_pyreadr_writer.py
+-rw-rw-r--   0 otto      (1000) otto      (1000)    12288 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/charset.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)       86 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/custom_errors.py
+-rw-rw-r--   0 otto      (1000) otto      (1000)   938496 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/iconv.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3210 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/iconv.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    73888 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/libbz2-1.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/liblzma-5.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/liblzma.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   734784 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr/librdata.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)     8373 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/librdata.pxd
+-rw-rw-r--   0 otto      (1000) otto      (1000)    12744 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/librdata.pyx
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.415855 pyreadr-0.4.8/pyreadr/libs/
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.427861 pyreadr-0.4.8/pyreadr/libs/bzip2/
+-rw-rw-r--   0 otto      (1000) otto      (1000)     7192 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/bzip2/bzlib.h
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.427861 pyreadr-0.4.8/pyreadr/libs/iconv/
+-rw-rw-r--   0 otto      (1000) otto      (1000)     9859 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/iconv/iconv.h
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.415855 pyreadr-0.4.8/pyreadr/libs/librdata/
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.435865 pyreadr-0.4.8/pyreadr/libs/librdata/src/
+-rw-rw-r--   0 otto      (1000) otto      (1000)     5434 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/CKHashTable.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1079 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/CKHashTable.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     7052 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1152 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_bits.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)      267 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_bits.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1981 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_error.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)     2797 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_internal.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     2458 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_io_unistd.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)      555 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_io_unistd.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3069 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_parser.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)    57640 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_read.c
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16693 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_write.c
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.435865 pyreadr-0.4.8/pyreadr/libs/lzma/
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.443869 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/
+-rw-rw-r--   0 otto      (1000) otto      (1000)    24858 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/base.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     2630 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/bcj.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    22107 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/block.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     4255 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/check.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    24844 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/container.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1865 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/delta.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16520 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/filter.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     2604 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/hardware.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    23491 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/index.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3914 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/index_hash.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    14744 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/lzma12.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     8253 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/stream_flags.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3497 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/version.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     6546 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma/vli.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     9866 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/lzma/lzma.h
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.443869 pyreadr-0.4.8/pyreadr/libs/zlib/
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16349 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/zlib/zconf.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)    96239 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/libs/zlib/zlib.h
+-rw-rw-r--   0 otto      (1000) otto      (1000)     8425 2021-11-30 09:21:27.000000 pyreadr-0.4.8/pyreadr/pyreadr.py
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/z.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/zdll.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    83968 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/zlib.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/zlib.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    93830 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/zlib1.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   180950 2023-08-08 12:41:22.000000 pyreadr-0.4.8/pyreadr/zlibstatic.lib
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.427861 pyreadr-0.4.8/pyreadr.egg-info/
+-rw-rw-r--   0 otto      (1000) otto      (1000)     1171 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr.egg-info/PKG-INFO
+-rw-rw-r--   0 otto      (1000) otto      (1000)     2026 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr.egg-info/SOURCES.txt
+-rw-rw-r--   0 otto      (1000) otto      (1000)        1 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr.egg-info/dependency_links.txt
+-rw-rw-r--   0 otto      (1000) otto      (1000)       14 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr.egg-info/requires.txt
+-rw-rw-r--   0 otto      (1000) otto      (1000)        8 2023-08-08 12:59:11.000000 pyreadr-0.4.8/pyreadr.egg-info/top_level.txt
+-rw-rw-r--   0 otto      (1000) otto      (1000)       38 2023-08-08 12:59:11.459877 pyreadr-0.4.8/setup.cfg
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3523 2023-08-08 12:54:58.000000 pyreadr-0.4.8/setup.py
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.415855 pyreadr-0.4.8/win_libs/
+drwxrwxr-x   0 otto      (1000) otto      (1000)        0 2023-08-08 12:59:11.455875 pyreadr-0.4.8/win_libs/64bit/
+-rw-rw-r--   0 otto      (1000) otto      (1000)    12288 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/charset.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   938496 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/iconv.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)     3210 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/iconv.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    73888 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/libbz2-1.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/liblzma-5.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   152064 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/liblzma.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/z.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/zdll.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    83968 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/zlib.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)    16228 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/zlib.lib
+-rw-rw-r--   0 otto      (1000) otto      (1000)    93830 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/zlib1.dll
+-rw-rw-r--   0 otto      (1000) otto      (1000)   180950 2021-11-30 09:21:27.000000 pyreadr-0.4.8/win_libs/64bit/zlibstatic.lib
```

### Comparing `pyreadr-0.4.7/PKG-INFO` & `pyreadr-0.4.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pyreadr
-Version: 0.4.7
+Version: 0.4.8
 Summary: Reads/writes R RData and Rds files into/from pandas data frames.
 Home-page: https://github.com/ofajardo/pyreadr
 Author: Otto Fajardo
 Author-email: pleasecontactviagithub@notvalid.com
 License: AGPLv3
 Download-URL: https://pypi.org/project/pyreadr/#files
-Description:  A Python package to read and write R RData and Rds files
-        into/from pandas data frames. It does not need to have R or other external
-        dependencies installed.
-        It is based on the C library librdata and
-        a modified version of the cython wrapper jamovi-readstat.<br>
-        Please visit out project home page for more information:<br>
-        https://github.com/ofajardo/pyreadr
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_jamovi_readstat
+License-File: LICENSE_librdata
+
+ A Python package to read and write R RData and Rds files
+into/from pandas data frames. It does not need to have R or other external
+dependencies installed.
+It is based on the C library librdata and
+a modified version of the cython wrapper jamovi-readstat.<br>
+Please visit out project home page for more information:<br>
+https://github.com/ofajardo/pyreadr
+
+
```

### Comparing `pyreadr-0.4.7/README.md` & `pyreadr-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/_pyreadr_parser.py` & `pyreadr-0.4.8/pyreadr/_pyreadr_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                     data = data.astype('bool')
                     data = data.astype(object)
                     data[na_index] = np.nan
             else:
                 if dtype.name == "LOGICAL":
                     data = data.astype('bool')
 
+
         self.arraylike_data = data
 
     def _arraylike_buildf(self):
         """"
         Transform the one dimensional array to a dataframe with several rows and columns
         """
         data = self.arraylike_data
@@ -238,23 +239,26 @@
                 # in pandas we only have np.nan to represent missing
                 # values, therefore we need to change the data type to
                 # object to be able to mix integers and the float nan
                 # In addition bool(np.nan) evaluates to True, we have to take care of that
                 na_index = df[colname] <= -2147483648
                 if np.any(na_index):
                     if dtype.name == "INTEGER":
-                        df[colname] = df[colname].astype(object)
+                        #df[colname] = df[colname].astype(object)
+                        df[colname] = df[colname].astype("Int32")
                         df.loc[na_index, colname] = np.nan
                     elif dtype.name == "LOGICAL":
                         df[colname] = df[colname].astype('bool')
                         df[colname] = df[colname].astype(object)
                         df.loc[na_index, colname] = np.nan
                 else:
                     if dtype.name == "LOGICAL":
                         df[colname] = df[colname].astype('bool')
+                    elif dtype.name == "INTEGER":
+                        df[colname] = df[colname].astype('Int32')
 
     def _handle_row_names(self):
         """
         For dataframes, set rownames as index
         """
         if self.row_names:
             self.df['rownames'] = self.row_names
```

### Comparing `pyreadr-0.4.7/pyreadr/_pyreadr_writer.py` & `pyreadr-0.4.8/pyreadr/_pyreadr_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,26 @@
 pyreadr_to_librdata_types = {"INTEGER": "INTEGER", "NUMERIC": "NUMERIC",
                         "LOGICAL": "LOGICAL", "CHARACTER": "CHARACTER",
                         "OBJECT": "CHARACTER", "DATE": "CHARACTER",
                         "DATETIME":"CHARACTER"}
                         
 librdata_min_integer = -2147483648
 
+def pandas_column_to_list(col):
+    """
+    Transforms a pandas column to a list
+    """
+
+    # pandas array 
+    val = col.values
+    if not type(val) == np.ndarray:
+        val = val.to_numpy()
+    l = val.tolist()
+    return val.tolist()
+
 
 def get_pyreadr_column_types(df):
     """
     From a pandas data frame, get an OrderedDict with column name as key
     and pyreadr column type as value, and also a list with boolean 
     values indicating if the column has missing values (np.nan).
     The pyreadr column types are needed for downstream processing.
@@ -220,15 +232,16 @@
         for col_name in col_names:
             curtype = librdata_types[col_name]
             self.add_column(str(col_name), curtype)
             
         for indx, column in enumerate(df):
             col = df[column].copy()
             tcol = transform_data(col, pyreadr_types[column], hasmissing[indx], dateformat, datetimeformat)
-            tcol = tcol.values.tolist()
+            #tcol = tcol.values.tolist()
+            tcol = pandas_column_to_list(tcol)
             curtype = librdata_types[column]
             for row_indx, val in enumerate(tcol):
                 self.insert_value(row_indx, indx, val, curtype)
             
         self.close()
 
         if compress:
```

### Comparing `pyreadr-0.4.7/pyreadr/librdata.c` & `pyreadr-0.4.8/pyreadr/librdata.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-/* Generated by Cython 0.29.22 */
+/* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
+            "pyreadr/conditional_includes.h",
             "pyreadr/libs/librdata/src/rdata.h",
             "pyreadr/libs/librdata/src/rdata_io_unistd.h"
         ],
         "extra_compile_args": [
             "-DHAVE_ZLIB",
             "-DHAVE_BZIP2",
             "-DHAVE_LZMA"
@@ -19,42 +20,56 @@
             "z",
             "bz2",
             "lzma"
         ],
         "name": "pyreadr.librdata",
         "sources": [
             "pyreadr/librdata.pyx",
+            "pyreadr/libs/librdata/src/rdata_write.c",
             "pyreadr/libs/librdata/src/rdata_bits.c",
-            "pyreadr/libs/librdata/src/rdata_io_unistd.c",
+            "pyreadr/libs/librdata/src/rdata_read.c",
+            "pyreadr/libs/librdata/src/rdata_parser.c",
             "pyreadr/libs/librdata/src/CKHashTable.c",
             "pyreadr/libs/librdata/src/rdata_error.c",
-            "pyreadr/libs/librdata/src/rdata_read.c",
-            "pyreadr/libs/librdata/src/rdata_write.c",
-            "pyreadr/libs/librdata/src/rdata_parser.c"
+            "pyreadr/libs/librdata/src/rdata_io_unistd.c"
         ]
     },
     "module_name": "pyreadr.librdata"
 }
 END: Cython Metadata */
 
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_22"
-#define CYTHON_HEX_VERSION 0x001D16F0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -65,30 +80,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -105,35 +124,167 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -148,54 +299,55 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -205,35 +357,68 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
-  #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -251,78 +436,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -330,93 +565,225 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return result;
+    }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -439,78 +806,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
+#endif
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define CYTHON_PEP393_ENABLED 1
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -531,16 +986,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -551,46 +1012,46 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
-#endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -602,16 +1063,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -626,15 +1089,24 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
@@ -643,17 +1115,15 @@
 /* Early includes */
 #include <stddef.h>
 #include <time.h>
 #include <stdint.h>
 #include <sys/types.h>
 #include "libs/librdata/src/rdata.h"
 #include "libs/librdata/src/rdata_io_unistd.h"
-#include <sys/stat.h>
-#include <unistd.h>
-#include <fcntl.h>
+#include "conditional_includes.h"
 #include <string.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -715,54 +1185,111 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -776,15 +1303,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -841,38 +1368,39 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "pyreadr/librdata.pyx",
-  "stringsource",
+  "<stringsource>",
 };
+/* #### Code section: utility_code_proto_before_types ### */
+/* #### Code section: numeric_typedefs ### */
+/* #### Code section: complex_type_declarations ### */
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7pyreadr_8librdata_Parser;
 struct __pyx_obj_7pyreadr_8librdata_Column;
 struct __pyx_obj_7pyreadr_8librdata_Writer;
 
-/* "pyreadr/librdata.pyx":140
+/* "pyreadr/librdata.pyx":141
  * 
  * 
  * cdef class Parser:             # <<<<<<<<<<<<<<
  * 
  *     cdef rdata_parser_t *_this
  */
 struct __pyx_obj_7pyreadr_8librdata_Parser {
@@ -881,28 +1409,28 @@
   struct rdata_parser_s *_this;
   int _fd;
   int _row_count;
   int _var_count;
 };
 
 
-/* "pyreadr/librdata.pyx":279
+/* "pyreadr/librdata.pyx":280
  * 
  * 
  * cdef class Column:             # <<<<<<<<<<<<<<
  *     cdef rdata_column_t *_this
  * 
  */
 struct __pyx_obj_7pyreadr_8librdata_Column {
   PyObject_HEAD
   struct rdata_column_s *_this;
 };
 
 
-/* "pyreadr/librdata.pyx":287
+/* "pyreadr/librdata.pyx":288
  * 
  * 
  * cdef class Writer:             # <<<<<<<<<<<<<<
  * 
  *     cdef object _format
  */
 struct __pyx_obj_7pyreadr_8librdata_Writer {
@@ -914,139 +1442,152 @@
   int _current_column_no;
   struct rdata_column_s *_current_column;
   PyObject *_table_name;
 };
 
 
 
-/* "pyreadr/librdata.pyx":140
+/* "pyreadr/librdata.pyx":141
  * 
  * 
  * cdef class Parser:             # <<<<<<<<<<<<<<
  * 
  *     cdef rdata_parser_t *_this
  */
 
 struct __pyx_vtabstruct_7pyreadr_8librdata_Parser {
   PyObject *(*parse)(struct __pyx_obj_7pyreadr_8librdata_Parser *, PyObject *, int __pyx_skip_dispatch);
-  PyObject *(*__pyx___handle_table)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *);
-  PyObject *(*__pyx___handle_column)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long);
-  PyObject *(*__pyx___handle_column_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
-  PyObject *(*__pyx___handle_dim)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long);
-  PyObject *(*__pyx___handle_dim_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
-  PyObject *(*__pyx___handle_row_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
-  PyObject *(*__pyx___handle_text_value)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
-  PyObject *(*__pyx___handle_value_label)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
+  PyObject *(*_Parser__handle_table)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *);
+  PyObject *(*_Parser__handle_column)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long);
+  PyObject *(*_Parser__handle_column_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
+  PyObject *(*_Parser__handle_dim)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long);
+  PyObject *(*_Parser__handle_dim_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
+  PyObject *(*_Parser__handle_row_name)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
+  PyObject *(*_Parser__handle_text_value)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
+  PyObject *(*_Parser__handle_value_label)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int);
 };
 static struct __pyx_vtabstruct_7pyreadr_8librdata_Parser *__pyx_vtabptr_7pyreadr_8librdata_Parser;
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
 
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
-/* IncludeStringH.proto */
-#include <string.h>
-
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1054,18 +1595,26 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
-/* WriteUnraisableException.proto */
-static void __Pyx_WriteUnraisable(const char *name, int clineno,
-                                  int lineno, const char *filename,
-                                  int full_traceback, int nogil);
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
+#else
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
+#endif
+
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
@@ -1087,105 +1636,114 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyCFunctionFastCall.proto */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
-#else
-#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
-#endif
-
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#else
-#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
+#endif
+#endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
-/* PyObjectCall2Args.proto */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
-
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
 
 /* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
 /* GetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -1206,46 +1764,108 @@
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
 /* SetItemInt.proto */
 #define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
                __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
                                                int is_list, int wraparound, int boundscheck);
 
+/* PyObject_Str.proto */
+#define __Pyx_PyObject_Str(obj)\
+    (likely(PyString_CheckExact(obj)) ? __Pyx_NewRef(obj) : PyObject_Str(obj))
+
 /* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kwdict, const char* function_name, int kw_allowed);
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* PyObjectCallNoArg.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-#else
-#define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
+
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
+
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
+#endif
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1253,76 +1873,225 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable);
+static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
 
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+/* GetVTable.proto */
+static void* __Pyx_GetVtable(PyTypeObject *type);
+
+/* MergeVTables.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type);
+#endif
 
 /* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
+/* Py3UpdateBases.proto */
+static PyObject* __Pyx_PEP560_update_bases(PyObject *bases);
+
 /* CalculateMetaclass.proto */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases);
 
 /* SetNameInClass.proto */
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? _PyDict_SetItem_KnownHash(ns, name, value, ((PyASCIIObject *) name)->hash) : PyObject_SetItem(ns, name, value))
 #elif CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_SetNameInClass(ns, name, value)\
     (likely(PyDict_CheckExact(ns)) ? PyDict_SetItem(ns, name, value) : PyObject_SetItem(ns, name, value))
 #else
 #define __Pyx_SetNameInClass(ns, name, value)  PyObject_SetItem(ns, name, value)
 #endif
 
+/* PyObjectCall2Args.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
+
+/* PyObjectLookupSpecial.proto */
+#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_LookupSpecialNoError(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 0)
+#define __Pyx_PyObject_LookupSpecial(obj, attr_name)  __Pyx__PyObject_LookupSpecial(obj, attr_name, 1)
+static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error);
+#else
+#define __Pyx_PyObject_LookupSpecialNoError(o,n) __Pyx_PyObject_GetAttrStrNoError(o,n)
+#define __Pyx_PyObject_LookupSpecial(o,n) __Pyx_PyObject_GetAttrStr(o,n)
+#endif
+
 /* Py3ClassCreate.proto */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name, PyObject *qualname,
                                            PyObject *mkw, PyObject *modname, PyObject *doc);
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases, PyObject *dict,
                                       PyObject *mkw, int calculate_metaclass, int allow_py2_metaclass);
 
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+#else
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
+#endif
+
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__rdata_type_e(enum rdata_type_e value);
 
 /* CIntToPy.proto */
@@ -1336,241 +2105,237 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int32_t __Pyx_PyInt_As_int32_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
 static PyObject *__pyx_f_7pyreadr_8librdata_6Parser_parse(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, PyObject *__pyx_v_path, int __pyx_skip_dispatch); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_table(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_column(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_column_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_dim(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_datatype, void *__pyx_v_data, long __pyx_v_count); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_dim_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_row_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_text_value(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index); /* proto*/
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_value_label(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index); /* proto*/
-
-/* Module declarations from 'libc.stddef' */
-
-/* Module declarations from 'libc.time' */
-
-/* Module declarations from 'libc.stdint' */
-
-/* Module declarations from 'libc.string' */
-
-/* Module declarations from 'pyreadr.librdata' */
-static PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Parser = 0;
-static PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Column = 0;
-static PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Writer = 0;
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_table(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_datatype, void *__pyx_v_data, long __pyx_v_count); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_row_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_text_value(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index); /* proto*/
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_value_label(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index); /* proto*/
+
+/* Module declarations from "libc.stddef" */
+
+/* Module declarations from "libc.time" */
+
+/* Module declarations from "libc.stdint" */
+
+/* Module declarations from "libc.string" */
+
+/* Module declarations from "pyreadr.librdata" */
 static int __pyx_f_7pyreadr_8librdata__os_open(PyObject *, PyObject *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__os_close(int); /*proto*/
+static int __pyx_f_7pyreadr_8librdata__handle_open(char const *, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_table(char const *, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_column(char const *, enum rdata_type_e, void *, long, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_dim(char const *, enum rdata_type_e, void *, long, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_column_name(char const *, int, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_dim_name(char const *, int, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_row_name(char const *, int, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_text_value(char const *, int, void *); /*proto*/
 static int __pyx_f_7pyreadr_8librdata__handle_value_label(char const *, int, void *); /*proto*/
 static Py_ssize_t __pyx_f_7pyreadr_8librdata__handle_write(void const *, size_t, void *); /*proto*/
+/* #### Code section: typeinfo ### */
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "pyreadr.librdata"
 extern int __pyx_module_is_main_pyreadr__librdata;
 int __pyx_module_is_main_pyreadr__librdata = 0;
 
-/* Implementation of 'pyreadr.librdata' */
+/* Implementation of "pyreadr.librdata" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
+/* #### Code section: string_decls ### */
+static const char __pyx_k_[] = "";
 static const char __pyx_k_r[] = "r";
 static const char __pyx_k_w[] = "w";
-static const char __pyx_k__5[] = "";
+static const char __pyx_k__2[] = "*";
+static const char __pyx_k__3[] = ".";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_pd[] = "pd";
+static const char __pyx_k__38[] = "?";
+static const char __pyx_k_col[] = "col";
 static const char __pyx_k_doc[] = "__doc__";
+static const char __pyx_k_fmt[] = "fmt";
 static const char __pyx_k_nan[] = "nan";
 static const char __pyx_k_rds[] = "rds";
 static const char __pyx_k_DATE[] = "DATE";
 static const char __pyx_k_Enum[] = "Enum";
 static const char __pyx_k_data[] = "data";
+static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_enum[] = "enum";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
+static const char __pyx_k_open[] = "open";
 static const char __pyx_k_path[] = "path";
+static const char __pyx_k_self[] = "self";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_close[] = "close";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_error[] = "_error";
 static const char __pyx_k_index[] = "index";
 static const char __pyx_k_int32[] = "int32";
+static const char __pyx_k_label[] = "label";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_parse[] = "parse";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_rdata[] = "rdata";
+static const char __pyx_k_super[] = "super";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_value[] = "value";
 static const char __pyx_k_Column[] = "Column";
 static const char __pyx_k_Parser[] = "Parser";
 static const char __pyx_k_Writer[] = "Writer";
 static const char __pyx_k_col_no[] = "col_no";
+static const char __pyx_k_column[] = "column";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_isfile[] = "isfile";
 static const char __pyx_k_isnull[] = "isnull";
+static const char __pyx_k_labels[] = "labels";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_row_no[] = "row_no";
+static const char __pyx_k_status[] = "status";
+static const char __pyx_k_system[] = "system";
 static const char __pyx_k_INTEGER[] = "INTEGER";
 static const char __pyx_k_LOGICAL[] = "LOGICAL";
 static const char __pyx_k_NUMERIC[] = "NUMERIC";
+static const char __pyx_k_Windows[] = "Windows";
+static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float64[] = "float64";
 static const char __pyx_k_os_path[] = "os.path";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_DataType[] = "DataType";
+static const char __pyx_k_fsdecode[] = "fsdecode";
 static const char __pyx_k_getstate[] = "__getstate__";
+static const char __pyx_k_platform[] = "platform";
 static const char __pyx_k_qualname[] = "__qualname__";
+static const char __pyx_k_set_name[] = "__set_name__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_CHARACTER[] = "CHARACTER";
 static const char __pyx_k_TIMESTAMP[] = "TIMESTAMP";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_data_type[] = "data_type";
+static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_metaclass[] = "__metaclass__";
+static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_row_count[] = "row_count";
+static const char __pyx_k_add_column[] = "add_column";
 static const char __pyx_k_handle_dim[] = "handle_dim";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_Writer_open[] = "Writer.open";
+static const char __pyx_k_mro_entries[] = "__mro_entries__";
+static const char __pyx_k_Parser_parse[] = "Parser.parse";
 static const char __pyx_k_PyreadrError[] = "PyreadrError";
+static const char __pyx_k_Writer_close[] = "Writer.close";
 static const char __pyx_k_handle_table[] = "handle_table";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_insert_value[] = "insert_value";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_LibrdataError[] = "LibrdataError";
 static const char __pyx_k_custom_errors[] = "custom_errors";
 static const char __pyx_k_handle_column[] = "handle_column";
+static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_set_row_count[] = "set_row_count";
+static const char __pyx_k_set_table_name[] = "set_table_name";
 static const char __pyx_k_handle_dim_name[] = "handle_dim_name";
 static const char __pyx_k_handle_row_name[] = "handle_row_name";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_add_level_labels[] = "add_level_labels";
 static const char __pyx_k_pyreadr_librdata[] = "pyreadr.librdata";
+static const char __pyx_k_Parser_handle_dim[] = "Parser.handle_dim";
 static const char __pyx_k_Unknown_data_type[] = "Unknown data type";
+static const char __pyx_k_Writer_add_column[] = "Writer.add_column";
+static const char __pyx_k_handle_row_name_2[] = "_handle_row_name";
 static const char __pyx_k_handle_text_value[] = "handle_text_value";
 static const char __pyx_k_Unsupported_format[] = "Unsupported format";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_handle_column_name[] = "handle_column_name";
 static const char __pyx_k_handle_value_label[] = "handle_value_label";
+static const char __pyx_k_Parser_handle_table[] = "Parser.handle_table";
 static const char __pyx_k_Unknown_data_type_s[] = "Unknown data type: %s";
+static const char __pyx_k_Writer_insert_value[] = "Writer.insert_value";
 static const char __pyx_k_parse_current_table[] = "parse_current_table";
+static const char __pyx_k_Parser_handle_column[] = "Parser.handle_column";
+static const char __pyx_k_Writer_set_row_count[] = "Writer.set_row_count";
+static const char __pyx_k_pyreadr_librdata_pyx[] = "pyreadr/librdata.pyx";
+static const char __pyx_k_Writer_set_table_name[] = "Writer.set_table_name";
+static const char __pyx_k_Column___reduce_cython[] = "Column.__reduce_cython__";
+static const char __pyx_k_Parser___reduce_cython[] = "Parser.__reduce_cython__";
+static const char __pyx_k_Parser_handle_dim_name[] = "Parser.handle_dim_name";
+static const char __pyx_k_Writer___reduce_cython[] = "Writer.__reduce_cython__";
+static const char __pyx_k_Column_add_level_labels[] = "Column.add_level_labels";
+static const char __pyx_k_Parser__handle_row_name[] = "Parser._handle_row_name";
+static const char __pyx_k_Column___setstate_cython[] = "Column.__setstate_cython__";
+static const char __pyx_k_Parser___setstate_cython[] = "Parser.__setstate_cython__";
+static const char __pyx_k_Parser_handle_text_value[] = "Parser.handle_text_value";
+static const char __pyx_k_Writer___setstate_cython[] = "Writer.__setstate_cython__";
+static const char __pyx_k_Parser_handle_column_name[] = "Parser.handle_column_name";
+static const char __pyx_k_Parser_handle_value_label[] = "Parser.handle_value_label";
 static const char __pyx_k_Wrong_data_type_s_for_dimensions[] = "Wrong data type %s for dimensions.";
 static const char __pyx_k_self__current_column_self__write[] = "self._current_column,self._writer cannot be converted to a Python object for pickling";
 static const char __pyx_k_self__this_cannot_be_converted_t[] = "self._this cannot be converted to a Python object for pickling";
-static PyObject *__pyx_n_s_CHARACTER;
-static PyObject *__pyx_n_u_CHARACTER;
-static PyObject *__pyx_n_s_Column;
-static PyObject *__pyx_n_s_DATE;
-static PyObject *__pyx_n_s_DataType;
-static PyObject *__pyx_n_s_Enum;
-static PyObject *__pyx_n_s_INTEGER;
-static PyObject *__pyx_n_u_INTEGER;
-static PyObject *__pyx_n_s_LOGICAL;
-static PyObject *__pyx_n_u_LOGICAL;
-static PyObject *__pyx_n_s_LibrdataError;
-static PyObject *__pyx_n_s_NUMERIC;
-static PyObject *__pyx_n_u_NUMERIC;
-static PyObject *__pyx_n_s_Parser;
-static PyObject *__pyx_n_s_PyreadrError;
-static PyObject *__pyx_n_s_TIMESTAMP;
-static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_kp_u_Unknown_data_type;
-static PyObject *__pyx_kp_u_Unknown_data_type_s;
-static PyObject *__pyx_kp_u_Unsupported_format;
-static PyObject *__pyx_n_s_Writer;
-static PyObject *__pyx_kp_u_Wrong_data_type_s_for_dimensions;
-static PyObject *__pyx_kp_b__5;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_col_no;
-static PyObject *__pyx_n_s_count;
-static PyObject *__pyx_n_s_custom_errors;
-static PyObject *__pyx_n_s_data;
-static PyObject *__pyx_n_s_data_type;
-static PyObject *__pyx_n_s_doc;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_empty;
-static PyObject *__pyx_n_s_encode;
-static PyObject *__pyx_n_s_enum;
-static PyObject *__pyx_n_s_error;
-static PyObject *__pyx_n_s_float64;
-static PyObject *__pyx_n_s_format;
-static PyObject *__pyx_n_s_getstate;
-static PyObject *__pyx_n_s_handle_column;
-static PyObject *__pyx_n_s_handle_column_name;
-static PyObject *__pyx_n_s_handle_dim;
-static PyObject *__pyx_n_s_handle_dim_name;
-static PyObject *__pyx_n_s_handle_row_name;
-static PyObject *__pyx_n_s_handle_table;
-static PyObject *__pyx_n_s_handle_text_value;
-static PyObject *__pyx_n_s_handle_value_label;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_index;
-static PyObject *__pyx_n_s_int32;
-static PyObject *__pyx_n_s_isfile;
-static PyObject *__pyx_n_s_isnull;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_metaclass;
-static PyObject *__pyx_n_s_module;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_n_s_name_2;
-static PyObject *__pyx_n_s_nan;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_n_s_os;
-static PyObject *__pyx_n_s_os_path;
-static PyObject *__pyx_n_s_pandas;
-static PyObject *__pyx_n_s_parse;
-static PyObject *__pyx_n_s_parse_current_table;
-static PyObject *__pyx_n_s_path;
-static PyObject *__pyx_n_s_pd;
-static PyObject *__pyx_n_s_prepare;
-static PyObject *__pyx_n_s_pyreadr_librdata;
-static PyObject *__pyx_n_s_pyx_vtable;
-static PyObject *__pyx_n_s_qualname;
-static PyObject *__pyx_n_u_r;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_u_rdata;
-static PyObject *__pyx_n_u_rds;
-static PyObject *__pyx_n_s_reduce;
-static PyObject *__pyx_n_s_reduce_cython;
-static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_row_no;
-static PyObject *__pyx_kp_s_self__current_column_self__write;
-static PyObject *__pyx_kp_s_self__this_cannot_be_converted_t;
-static PyObject *__pyx_n_s_setstate;
-static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_kp_u_utf_8;
-static PyObject *__pyx_n_s_value;
-static PyObject *__pyx_n_u_w;
+/* #### Code section: decls ### */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_parse(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, PyObject *__pyx_v_path); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_2handle_table(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_4handle_column(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_data_type, CYTHON_UNUSED PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_count); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_6handle_column_name(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_index); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_8handle_dim(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_data_type, CYTHON_UNUSED PyObject *__pyx_v_data, CYTHON_UNUSED PyObject *__pyx_v_count); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_10handle_dim_name(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_index); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_12_handle_row_name(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name, CYTHON_UNUSED PyObject *__pyx_v_index); /* proto */
@@ -1589,152 +2354,1267 @@
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_10insert_value(struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_row_no, PyObject *__pyx_v_col_no, PyObject *__pyx_v_value, PyObject *__pyx_v_dtype); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_12add_column(struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, PyObject *__pyx_v_name, PyObject *__pyx_v_dtype); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Parser(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Column(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Writer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_int_0;
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__7;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_7pyreadr_8librdata_Parser;
+  PyObject *__pyx_type_7pyreadr_8librdata_Column;
+  PyObject *__pyx_type_7pyreadr_8librdata_Writer;
+  #endif
+  PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Parser;
+  PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Column;
+  PyTypeObject *__pyx_ptype_7pyreadr_8librdata_Writer;
+  PyObject *__pyx_kp_b_;
+  PyObject *__pyx_n_s_CHARACTER;
+  PyObject *__pyx_n_u_CHARACTER;
+  PyObject *__pyx_n_s_Column;
+  PyObject *__pyx_n_s_Column___reduce_cython;
+  PyObject *__pyx_n_s_Column___setstate_cython;
+  PyObject *__pyx_n_s_Column_add_level_labels;
+  PyObject *__pyx_n_s_DATE;
+  PyObject *__pyx_n_s_DataType;
+  PyObject *__pyx_n_s_Enum;
+  PyObject *__pyx_n_s_INTEGER;
+  PyObject *__pyx_n_u_INTEGER;
+  PyObject *__pyx_n_s_LOGICAL;
+  PyObject *__pyx_n_u_LOGICAL;
+  PyObject *__pyx_n_s_LibrdataError;
+  PyObject *__pyx_n_s_NUMERIC;
+  PyObject *__pyx_n_u_NUMERIC;
+  PyObject *__pyx_n_s_Parser;
+  PyObject *__pyx_n_s_Parser___reduce_cython;
+  PyObject *__pyx_n_s_Parser___setstate_cython;
+  PyObject *__pyx_n_s_Parser__handle_row_name;
+  PyObject *__pyx_n_s_Parser_handle_column;
+  PyObject *__pyx_n_s_Parser_handle_column_name;
+  PyObject *__pyx_n_s_Parser_handle_dim;
+  PyObject *__pyx_n_s_Parser_handle_dim_name;
+  PyObject *__pyx_n_s_Parser_handle_table;
+  PyObject *__pyx_n_s_Parser_handle_text_value;
+  PyObject *__pyx_n_s_Parser_handle_value_label;
+  PyObject *__pyx_n_s_Parser_parse;
+  PyObject *__pyx_n_s_PyreadrError;
+  PyObject *__pyx_n_s_TIMESTAMP;
+  PyObject *__pyx_n_s_TypeError;
+  PyObject *__pyx_kp_u_Unknown_data_type;
+  PyObject *__pyx_kp_u_Unknown_data_type_s;
+  PyObject *__pyx_kp_u_Unsupported_format;
+  PyObject *__pyx_n_u_Windows;
+  PyObject *__pyx_n_s_Writer;
+  PyObject *__pyx_n_s_Writer___reduce_cython;
+  PyObject *__pyx_n_s_Writer___setstate_cython;
+  PyObject *__pyx_n_s_Writer_add_column;
+  PyObject *__pyx_n_s_Writer_close;
+  PyObject *__pyx_n_s_Writer_insert_value;
+  PyObject *__pyx_n_s_Writer_open;
+  PyObject *__pyx_n_s_Writer_set_row_count;
+  PyObject *__pyx_n_s_Writer_set_table_name;
+  PyObject *__pyx_kp_u_Wrong_data_type_s_for_dimensions;
+  PyObject *__pyx_n_s__2;
+  PyObject *__pyx_kp_u__3;
+  PyObject *__pyx_n_s__38;
+  PyObject *__pyx_n_s_add_column;
+  PyObject *__pyx_n_s_add_level_labels;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_close;
+  PyObject *__pyx_n_s_col;
+  PyObject *__pyx_n_s_col_no;
+  PyObject *__pyx_n_s_column;
+  PyObject *__pyx_n_s_count;
+  PyObject *__pyx_n_s_custom_errors;
+  PyObject *__pyx_n_s_data;
+  PyObject *__pyx_n_s_data_type;
+  PyObject *__pyx_n_s_dict;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_s_doc;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_empty;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_encode;
+  PyObject *__pyx_n_s_enum;
+  PyObject *__pyx_n_s_error;
+  PyObject *__pyx_n_s_float64;
+  PyObject *__pyx_n_s_fmt;
+  PyObject *__pyx_n_s_format;
+  PyObject *__pyx_n_s_fsdecode;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_n_s_handle_column;
+  PyObject *__pyx_n_s_handle_column_name;
+  PyObject *__pyx_n_s_handle_dim;
+  PyObject *__pyx_n_s_handle_dim_name;
+  PyObject *__pyx_n_s_handle_row_name;
+  PyObject *__pyx_n_s_handle_row_name_2;
+  PyObject *__pyx_n_s_handle_table;
+  PyObject *__pyx_n_s_handle_text_value;
+  PyObject *__pyx_n_s_handle_value_label;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_index;
+  PyObject *__pyx_n_s_init_subclass;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_s_insert_value;
+  PyObject *__pyx_n_s_int32;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_isfile;
+  PyObject *__pyx_n_s_isnull;
+  PyObject *__pyx_n_s_label;
+  PyObject *__pyx_n_s_labels;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_metaclass;
+  PyObject *__pyx_n_s_module;
+  PyObject *__pyx_n_s_mro_entries;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_n_s_name_2;
+  PyObject *__pyx_n_s_nan;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_n_s_open;
+  PyObject *__pyx_n_s_os;
+  PyObject *__pyx_n_s_os_path;
+  PyObject *__pyx_n_s_pandas;
+  PyObject *__pyx_n_s_parse;
+  PyObject *__pyx_n_s_parse_current_table;
+  PyObject *__pyx_n_s_path;
+  PyObject *__pyx_n_s_pd;
+  PyObject *__pyx_n_s_platform;
+  PyObject *__pyx_n_s_prepare;
+  PyObject *__pyx_n_s_pyreadr_librdata;
+  PyObject *__pyx_kp_s_pyreadr_librdata_pyx;
+  PyObject *__pyx_n_s_pyx_state;
+  PyObject *__pyx_n_s_pyx_vtable;
+  PyObject *__pyx_n_s_qualname;
+  PyObject *__pyx_n_u_r;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_u_rdata;
+  PyObject *__pyx_n_u_rds;
+  PyObject *__pyx_n_s_reduce;
+  PyObject *__pyx_n_s_reduce_cython;
+  PyObject *__pyx_n_s_reduce_ex;
+  PyObject *__pyx_n_s_row_count;
+  PyObject *__pyx_n_s_row_no;
+  PyObject *__pyx_n_s_self;
+  PyObject *__pyx_kp_s_self__current_column_self__write;
+  PyObject *__pyx_kp_s_self__this_cannot_be_converted_t;
+  PyObject *__pyx_n_s_set_name;
+  PyObject *__pyx_n_s_set_row_count;
+  PyObject *__pyx_n_s_set_table_name;
+  PyObject *__pyx_n_s_setstate;
+  PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_n_s_status;
+  PyObject *__pyx_kp_s_stringsource;
+  PyObject *__pyx_n_s_super;
+  PyObject *__pyx_n_s_system;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_kp_u_utf_8;
+  PyObject *__pyx_n_s_value;
+  PyObject *__pyx_n_u_w;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__5;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__18;
+  PyObject *__pyx_tuple__20;
+  PyObject *__pyx_tuple__22;
+  PyObject *__pyx_tuple__26;
+  PyObject *__pyx_tuple__28;
+  PyObject *__pyx_tuple__32;
+  PyObject *__pyx_tuple__34;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__8;
+  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__12;
+  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__14;
+  PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__16;
+  PyObject *__pyx_codeobj__17;
+  PyObject *__pyx_codeobj__19;
+  PyObject *__pyx_codeobj__21;
+  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__25;
+  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__29;
+  PyObject *__pyx_codeobj__30;
+  PyObject *__pyx_codeobj__31;
+  PyObject *__pyx_codeobj__33;
+  PyObject *__pyx_codeobj__35;
+  PyObject *__pyx_codeobj__36;
+  PyObject *__pyx_codeobj__37;
+} __pyx_mstate;
 
-/* "pyreadr/librdata.pyx":22
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyreadr_8librdata_Parser);
+  Py_CLEAR(clear_module_state->__pyx_type_7pyreadr_8librdata_Parser);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyreadr_8librdata_Column);
+  Py_CLEAR(clear_module_state->__pyx_type_7pyreadr_8librdata_Column);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pyreadr_8librdata_Writer);
+  Py_CLEAR(clear_module_state->__pyx_type_7pyreadr_8librdata_Writer);
+  Py_CLEAR(clear_module_state->__pyx_kp_b_);
+  Py_CLEAR(clear_module_state->__pyx_n_s_CHARACTER);
+  Py_CLEAR(clear_module_state->__pyx_n_u_CHARACTER);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Column___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Column___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Column_add_level_labels);
+  Py_CLEAR(clear_module_state->__pyx_n_s_DATE);
+  Py_CLEAR(clear_module_state->__pyx_n_s_DataType);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Enum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_INTEGER);
+  Py_CLEAR(clear_module_state->__pyx_n_u_INTEGER);
+  Py_CLEAR(clear_module_state->__pyx_n_s_LOGICAL);
+  Py_CLEAR(clear_module_state->__pyx_n_u_LOGICAL);
+  Py_CLEAR(clear_module_state->__pyx_n_s_LibrdataError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_NUMERIC);
+  Py_CLEAR(clear_module_state->__pyx_n_u_NUMERIC);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser__handle_row_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_column_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_dim);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_dim_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_table);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_text_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_handle_value_label);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Parser_parse);
+  Py_CLEAR(clear_module_state->__pyx_n_s_PyreadrError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TIMESTAMP);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_data_type);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unknown_data_type_s);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Unsupported_format);
+  Py_CLEAR(clear_module_state->__pyx_n_u_Windows);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_add_column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_insert_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_open);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_set_row_count);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Writer_set_table_name);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_Wrong_data_type_s_for_dimensions);
+  Py_CLEAR(clear_module_state->__pyx_n_s__2);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s__38);
+  Py_CLEAR(clear_module_state->__pyx_n_s_add_column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_add_level_labels);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_col);
+  Py_CLEAR(clear_module_state->__pyx_n_s_col_no);
+  Py_CLEAR(clear_module_state->__pyx_n_s_column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_count);
+  Py_CLEAR(clear_module_state->__pyx_n_s_custom_errors);
+  Py_CLEAR(clear_module_state->__pyx_n_s_data);
+  Py_CLEAR(clear_module_state->__pyx_n_s_data_type);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dict);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_doc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_empty);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_encode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_enum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_error);
+  Py_CLEAR(clear_module_state->__pyx_n_s_float64);
+  Py_CLEAR(clear_module_state->__pyx_n_s_fmt);
+  Py_CLEAR(clear_module_state->__pyx_n_s_format);
+  Py_CLEAR(clear_module_state->__pyx_n_s_fsdecode);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_column);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_column_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_dim);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_dim_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_row_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_row_name_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_table);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_text_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_handle_value_label);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_index);
+  Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_s_insert_value);
+  Py_CLEAR(clear_module_state->__pyx_n_s_int32);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_isfile);
+  Py_CLEAR(clear_module_state->__pyx_n_s_isnull);
+  Py_CLEAR(clear_module_state->__pyx_n_s_label);
+  Py_CLEAR(clear_module_state->__pyx_n_s_labels);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
+  Py_CLEAR(clear_module_state->__pyx_n_s_module);
+  Py_CLEAR(clear_module_state->__pyx_n_s_mro_entries);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nan);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_n_s_open);
+  Py_CLEAR(clear_module_state->__pyx_n_s_os);
+  Py_CLEAR(clear_module_state->__pyx_n_s_os_path);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pandas);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parse);
+  Py_CLEAR(clear_module_state->__pyx_n_s_parse_current_table);
+  Py_CLEAR(clear_module_state->__pyx_n_s_path);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pd);
+  Py_CLEAR(clear_module_state->__pyx_n_s_platform);
+  Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyreadr_librdata);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_pyreadr_librdata_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_qualname);
+  Py_CLEAR(clear_module_state->__pyx_n_u_r);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_u_rdata);
+  Py_CLEAR(clear_module_state->__pyx_n_u_rds);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
+  Py_CLEAR(clear_module_state->__pyx_n_s_row_count);
+  Py_CLEAR(clear_module_state->__pyx_n_s_row_no);
+  Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_self__current_column_self__write);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_self__this_cannot_be_converted_t);
+  Py_CLEAR(clear_module_state->__pyx_n_s_set_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_set_row_count);
+  Py_CLEAR(clear_module_state->__pyx_n_s_set_table_name);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_n_s_status);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
+  Py_CLEAR(clear_module_state->__pyx_n_s_super);
+  Py_CLEAR(clear_module_state->__pyx_n_s_system);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
+  Py_CLEAR(clear_module_state->__pyx_n_s_value);
+  Py_CLEAR(clear_module_state->__pyx_n_u_w);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__5);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__18);
+  Py_CLEAR(clear_module_state->__pyx_tuple__20);
+  Py_CLEAR(clear_module_state->__pyx_tuple__22);
+  Py_CLEAR(clear_module_state->__pyx_tuple__26);
+  Py_CLEAR(clear_module_state->__pyx_tuple__28);
+  Py_CLEAR(clear_module_state->__pyx_tuple__32);
+  Py_CLEAR(clear_module_state->__pyx_tuple__34);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__16);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__30);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__31);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__33);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__35);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__36);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__37);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyreadr_8librdata_Parser);
+  Py_VISIT(traverse_module_state->__pyx_type_7pyreadr_8librdata_Parser);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyreadr_8librdata_Column);
+  Py_VISIT(traverse_module_state->__pyx_type_7pyreadr_8librdata_Column);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pyreadr_8librdata_Writer);
+  Py_VISIT(traverse_module_state->__pyx_type_7pyreadr_8librdata_Writer);
+  Py_VISIT(traverse_module_state->__pyx_kp_b_);
+  Py_VISIT(traverse_module_state->__pyx_n_s_CHARACTER);
+  Py_VISIT(traverse_module_state->__pyx_n_u_CHARACTER);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Column___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Column___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Column_add_level_labels);
+  Py_VISIT(traverse_module_state->__pyx_n_s_DATE);
+  Py_VISIT(traverse_module_state->__pyx_n_s_DataType);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Enum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_INTEGER);
+  Py_VISIT(traverse_module_state->__pyx_n_u_INTEGER);
+  Py_VISIT(traverse_module_state->__pyx_n_s_LOGICAL);
+  Py_VISIT(traverse_module_state->__pyx_n_u_LOGICAL);
+  Py_VISIT(traverse_module_state->__pyx_n_s_LibrdataError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_NUMERIC);
+  Py_VISIT(traverse_module_state->__pyx_n_u_NUMERIC);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser__handle_row_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_column_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_dim);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_dim_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_table);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_text_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_handle_value_label);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Parser_parse);
+  Py_VISIT(traverse_module_state->__pyx_n_s_PyreadrError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TIMESTAMP);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_data_type);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unknown_data_type_s);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Unsupported_format);
+  Py_VISIT(traverse_module_state->__pyx_n_u_Windows);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_add_column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_insert_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_open);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_set_row_count);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Writer_set_table_name);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_Wrong_data_type_s_for_dimensions);
+  Py_VISIT(traverse_module_state->__pyx_n_s__2);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s__38);
+  Py_VISIT(traverse_module_state->__pyx_n_s_add_column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_add_level_labels);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_col);
+  Py_VISIT(traverse_module_state->__pyx_n_s_col_no);
+  Py_VISIT(traverse_module_state->__pyx_n_s_column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_count);
+  Py_VISIT(traverse_module_state->__pyx_n_s_custom_errors);
+  Py_VISIT(traverse_module_state->__pyx_n_s_data);
+  Py_VISIT(traverse_module_state->__pyx_n_s_data_type);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dict);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_doc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_empty);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_encode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_enum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_error);
+  Py_VISIT(traverse_module_state->__pyx_n_s_float64);
+  Py_VISIT(traverse_module_state->__pyx_n_s_fmt);
+  Py_VISIT(traverse_module_state->__pyx_n_s_format);
+  Py_VISIT(traverse_module_state->__pyx_n_s_fsdecode);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_column);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_column_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_dim);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_dim_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_row_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_row_name_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_table);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_text_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_handle_value_label);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_index);
+  Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_s_insert_value);
+  Py_VISIT(traverse_module_state->__pyx_n_s_int32);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_isfile);
+  Py_VISIT(traverse_module_state->__pyx_n_s_isnull);
+  Py_VISIT(traverse_module_state->__pyx_n_s_label);
+  Py_VISIT(traverse_module_state->__pyx_n_s_labels);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
+  Py_VISIT(traverse_module_state->__pyx_n_s_module);
+  Py_VISIT(traverse_module_state->__pyx_n_s_mro_entries);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nan);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_n_s_open);
+  Py_VISIT(traverse_module_state->__pyx_n_s_os);
+  Py_VISIT(traverse_module_state->__pyx_n_s_os_path);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pandas);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parse);
+  Py_VISIT(traverse_module_state->__pyx_n_s_parse_current_table);
+  Py_VISIT(traverse_module_state->__pyx_n_s_path);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pd);
+  Py_VISIT(traverse_module_state->__pyx_n_s_platform);
+  Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyreadr_librdata);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_pyreadr_librdata_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_qualname);
+  Py_VISIT(traverse_module_state->__pyx_n_u_r);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_u_rdata);
+  Py_VISIT(traverse_module_state->__pyx_n_u_rds);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
+  Py_VISIT(traverse_module_state->__pyx_n_s_row_count);
+  Py_VISIT(traverse_module_state->__pyx_n_s_row_no);
+  Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_self__current_column_self__write);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_self__this_cannot_be_converted_t);
+  Py_VISIT(traverse_module_state->__pyx_n_s_set_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_set_row_count);
+  Py_VISIT(traverse_module_state->__pyx_n_s_set_table_name);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_n_s_status);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
+  Py_VISIT(traverse_module_state->__pyx_n_s_super);
+  Py_VISIT(traverse_module_state->__pyx_n_s_system);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
+  Py_VISIT(traverse_module_state->__pyx_n_s_value);
+  Py_VISIT(traverse_module_state->__pyx_n_u_w);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__5);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__18);
+  Py_VISIT(traverse_module_state->__pyx_tuple__20);
+  Py_VISIT(traverse_module_state->__pyx_tuple__22);
+  Py_VISIT(traverse_module_state->__pyx_tuple__26);
+  Py_VISIT(traverse_module_state->__pyx_tuple__28);
+  Py_VISIT(traverse_module_state->__pyx_tuple__32);
+  Py_VISIT(traverse_module_state->__pyx_tuple__34);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__16);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__30);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__31);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__33);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__35);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__36);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__37);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_7pyreadr_8librdata_Parser __pyx_mstate_global->__pyx_type_7pyreadr_8librdata_Parser
+#define __pyx_type_7pyreadr_8librdata_Column __pyx_mstate_global->__pyx_type_7pyreadr_8librdata_Column
+#define __pyx_type_7pyreadr_8librdata_Writer __pyx_mstate_global->__pyx_type_7pyreadr_8librdata_Writer
+#endif
+#define __pyx_ptype_7pyreadr_8librdata_Parser __pyx_mstate_global->__pyx_ptype_7pyreadr_8librdata_Parser
+#define __pyx_ptype_7pyreadr_8librdata_Column __pyx_mstate_global->__pyx_ptype_7pyreadr_8librdata_Column
+#define __pyx_ptype_7pyreadr_8librdata_Writer __pyx_mstate_global->__pyx_ptype_7pyreadr_8librdata_Writer
+#define __pyx_kp_b_ __pyx_mstate_global->__pyx_kp_b_
+#define __pyx_n_s_CHARACTER __pyx_mstate_global->__pyx_n_s_CHARACTER
+#define __pyx_n_u_CHARACTER __pyx_mstate_global->__pyx_n_u_CHARACTER
+#define __pyx_n_s_Column __pyx_mstate_global->__pyx_n_s_Column
+#define __pyx_n_s_Column___reduce_cython __pyx_mstate_global->__pyx_n_s_Column___reduce_cython
+#define __pyx_n_s_Column___setstate_cython __pyx_mstate_global->__pyx_n_s_Column___setstate_cython
+#define __pyx_n_s_Column_add_level_labels __pyx_mstate_global->__pyx_n_s_Column_add_level_labels
+#define __pyx_n_s_DATE __pyx_mstate_global->__pyx_n_s_DATE
+#define __pyx_n_s_DataType __pyx_mstate_global->__pyx_n_s_DataType
+#define __pyx_n_s_Enum __pyx_mstate_global->__pyx_n_s_Enum
+#define __pyx_n_s_INTEGER __pyx_mstate_global->__pyx_n_s_INTEGER
+#define __pyx_n_u_INTEGER __pyx_mstate_global->__pyx_n_u_INTEGER
+#define __pyx_n_s_LOGICAL __pyx_mstate_global->__pyx_n_s_LOGICAL
+#define __pyx_n_u_LOGICAL __pyx_mstate_global->__pyx_n_u_LOGICAL
+#define __pyx_n_s_LibrdataError __pyx_mstate_global->__pyx_n_s_LibrdataError
+#define __pyx_n_s_NUMERIC __pyx_mstate_global->__pyx_n_s_NUMERIC
+#define __pyx_n_u_NUMERIC __pyx_mstate_global->__pyx_n_u_NUMERIC
+#define __pyx_n_s_Parser __pyx_mstate_global->__pyx_n_s_Parser
+#define __pyx_n_s_Parser___reduce_cython __pyx_mstate_global->__pyx_n_s_Parser___reduce_cython
+#define __pyx_n_s_Parser___setstate_cython __pyx_mstate_global->__pyx_n_s_Parser___setstate_cython
+#define __pyx_n_s_Parser__handle_row_name __pyx_mstate_global->__pyx_n_s_Parser__handle_row_name
+#define __pyx_n_s_Parser_handle_column __pyx_mstate_global->__pyx_n_s_Parser_handle_column
+#define __pyx_n_s_Parser_handle_column_name __pyx_mstate_global->__pyx_n_s_Parser_handle_column_name
+#define __pyx_n_s_Parser_handle_dim __pyx_mstate_global->__pyx_n_s_Parser_handle_dim
+#define __pyx_n_s_Parser_handle_dim_name __pyx_mstate_global->__pyx_n_s_Parser_handle_dim_name
+#define __pyx_n_s_Parser_handle_table __pyx_mstate_global->__pyx_n_s_Parser_handle_table
+#define __pyx_n_s_Parser_handle_text_value __pyx_mstate_global->__pyx_n_s_Parser_handle_text_value
+#define __pyx_n_s_Parser_handle_value_label __pyx_mstate_global->__pyx_n_s_Parser_handle_value_label
+#define __pyx_n_s_Parser_parse __pyx_mstate_global->__pyx_n_s_Parser_parse
+#define __pyx_n_s_PyreadrError __pyx_mstate_global->__pyx_n_s_PyreadrError
+#define __pyx_n_s_TIMESTAMP __pyx_mstate_global->__pyx_n_s_TIMESTAMP
+#define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
+#define __pyx_kp_u_Unknown_data_type __pyx_mstate_global->__pyx_kp_u_Unknown_data_type
+#define __pyx_kp_u_Unknown_data_type_s __pyx_mstate_global->__pyx_kp_u_Unknown_data_type_s
+#define __pyx_kp_u_Unsupported_format __pyx_mstate_global->__pyx_kp_u_Unsupported_format
+#define __pyx_n_u_Windows __pyx_mstate_global->__pyx_n_u_Windows
+#define __pyx_n_s_Writer __pyx_mstate_global->__pyx_n_s_Writer
+#define __pyx_n_s_Writer___reduce_cython __pyx_mstate_global->__pyx_n_s_Writer___reduce_cython
+#define __pyx_n_s_Writer___setstate_cython __pyx_mstate_global->__pyx_n_s_Writer___setstate_cython
+#define __pyx_n_s_Writer_add_column __pyx_mstate_global->__pyx_n_s_Writer_add_column
+#define __pyx_n_s_Writer_close __pyx_mstate_global->__pyx_n_s_Writer_close
+#define __pyx_n_s_Writer_insert_value __pyx_mstate_global->__pyx_n_s_Writer_insert_value
+#define __pyx_n_s_Writer_open __pyx_mstate_global->__pyx_n_s_Writer_open
+#define __pyx_n_s_Writer_set_row_count __pyx_mstate_global->__pyx_n_s_Writer_set_row_count
+#define __pyx_n_s_Writer_set_table_name __pyx_mstate_global->__pyx_n_s_Writer_set_table_name
+#define __pyx_kp_u_Wrong_data_type_s_for_dimensions __pyx_mstate_global->__pyx_kp_u_Wrong_data_type_s_for_dimensions
+#define __pyx_n_s__2 __pyx_mstate_global->__pyx_n_s__2
+#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
+#define __pyx_n_s__38 __pyx_mstate_global->__pyx_n_s__38
+#define __pyx_n_s_add_column __pyx_mstate_global->__pyx_n_s_add_column
+#define __pyx_n_s_add_level_labels __pyx_mstate_global->__pyx_n_s_add_level_labels
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
+#define __pyx_n_s_col __pyx_mstate_global->__pyx_n_s_col
+#define __pyx_n_s_col_no __pyx_mstate_global->__pyx_n_s_col_no
+#define __pyx_n_s_column __pyx_mstate_global->__pyx_n_s_column
+#define __pyx_n_s_count __pyx_mstate_global->__pyx_n_s_count
+#define __pyx_n_s_custom_errors __pyx_mstate_global->__pyx_n_s_custom_errors
+#define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
+#define __pyx_n_s_data_type __pyx_mstate_global->__pyx_n_s_data_type
+#define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_empty __pyx_mstate_global->__pyx_n_s_empty
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
+#define __pyx_n_s_enum __pyx_mstate_global->__pyx_n_s_enum
+#define __pyx_n_s_error __pyx_mstate_global->__pyx_n_s_error
+#define __pyx_n_s_float64 __pyx_mstate_global->__pyx_n_s_float64
+#define __pyx_n_s_fmt __pyx_mstate_global->__pyx_n_s_fmt
+#define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
+#define __pyx_n_s_fsdecode __pyx_mstate_global->__pyx_n_s_fsdecode
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_n_s_handle_column __pyx_mstate_global->__pyx_n_s_handle_column
+#define __pyx_n_s_handle_column_name __pyx_mstate_global->__pyx_n_s_handle_column_name
+#define __pyx_n_s_handle_dim __pyx_mstate_global->__pyx_n_s_handle_dim
+#define __pyx_n_s_handle_dim_name __pyx_mstate_global->__pyx_n_s_handle_dim_name
+#define __pyx_n_s_handle_row_name __pyx_mstate_global->__pyx_n_s_handle_row_name
+#define __pyx_n_s_handle_row_name_2 __pyx_mstate_global->__pyx_n_s_handle_row_name_2
+#define __pyx_n_s_handle_table __pyx_mstate_global->__pyx_n_s_handle_table
+#define __pyx_n_s_handle_text_value __pyx_mstate_global->__pyx_n_s_handle_text_value
+#define __pyx_n_s_handle_value_label __pyx_mstate_global->__pyx_n_s_handle_value_label
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
+#define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_s_insert_value __pyx_mstate_global->__pyx_n_s_insert_value
+#define __pyx_n_s_int32 __pyx_mstate_global->__pyx_n_s_int32
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_isfile __pyx_mstate_global->__pyx_n_s_isfile
+#define __pyx_n_s_isnull __pyx_mstate_global->__pyx_n_s_isnull
+#define __pyx_n_s_label __pyx_mstate_global->__pyx_n_s_label
+#define __pyx_n_s_labels __pyx_mstate_global->__pyx_n_s_labels
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
+#define __pyx_n_s_module __pyx_mstate_global->__pyx_n_s_module
+#define __pyx_n_s_mro_entries __pyx_mstate_global->__pyx_n_s_mro_entries
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
+#define __pyx_n_s_nan __pyx_mstate_global->__pyx_n_s_nan
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_n_s_open __pyx_mstate_global->__pyx_n_s_open
+#define __pyx_n_s_os __pyx_mstate_global->__pyx_n_s_os
+#define __pyx_n_s_os_path __pyx_mstate_global->__pyx_n_s_os_path
+#define __pyx_n_s_pandas __pyx_mstate_global->__pyx_n_s_pandas
+#define __pyx_n_s_parse __pyx_mstate_global->__pyx_n_s_parse
+#define __pyx_n_s_parse_current_table __pyx_mstate_global->__pyx_n_s_parse_current_table
+#define __pyx_n_s_path __pyx_mstate_global->__pyx_n_s_path
+#define __pyx_n_s_pd __pyx_mstate_global->__pyx_n_s_pd
+#define __pyx_n_s_platform __pyx_mstate_global->__pyx_n_s_platform
+#define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
+#define __pyx_n_s_pyreadr_librdata __pyx_mstate_global->__pyx_n_s_pyreadr_librdata
+#define __pyx_kp_s_pyreadr_librdata_pyx __pyx_mstate_global->__pyx_kp_s_pyreadr_librdata_pyx
+#define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
+#define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
+#define __pyx_n_s_qualname __pyx_mstate_global->__pyx_n_s_qualname
+#define __pyx_n_u_r __pyx_mstate_global->__pyx_n_u_r
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_u_rdata __pyx_mstate_global->__pyx_n_u_rdata
+#define __pyx_n_u_rds __pyx_mstate_global->__pyx_n_u_rds
+#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
+#define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
+#define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
+#define __pyx_n_s_row_count __pyx_mstate_global->__pyx_n_s_row_count
+#define __pyx_n_s_row_no __pyx_mstate_global->__pyx_n_s_row_no
+#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_kp_s_self__current_column_self__write __pyx_mstate_global->__pyx_kp_s_self__current_column_self__write
+#define __pyx_kp_s_self__this_cannot_be_converted_t __pyx_mstate_global->__pyx_kp_s_self__this_cannot_be_converted_t
+#define __pyx_n_s_set_name __pyx_mstate_global->__pyx_n_s_set_name
+#define __pyx_n_s_set_row_count __pyx_mstate_global->__pyx_n_s_set_row_count
+#define __pyx_n_s_set_table_name __pyx_mstate_global->__pyx_n_s_set_table_name
+#define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
+#define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_n_s_status __pyx_mstate_global->__pyx_n_s_status
+#define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
+#define __pyx_n_s_super __pyx_mstate_global->__pyx_n_s_super
+#define __pyx_n_s_system __pyx_mstate_global->__pyx_n_s_system
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
+#define __pyx_n_s_value __pyx_mstate_global->__pyx_n_s_value
+#define __pyx_n_u_w __pyx_mstate_global->__pyx_n_u_w
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
+#define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
+#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
+#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
+#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
+#define __pyx_tuple__32 __pyx_mstate_global->__pyx_tuple__32
+#define __pyx_tuple__34 __pyx_mstate_global->__pyx_tuple__34
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
+#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
+#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
+#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
+#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
+#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
+#define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
+#define __pyx_codeobj__31 __pyx_mstate_global->__pyx_codeobj__31
+#define __pyx_codeobj__33 __pyx_mstate_global->__pyx_codeobj__33
+#define __pyx_codeobj__35 __pyx_mstate_global->__pyx_codeobj__35
+#define __pyx_codeobj__36 __pyx_mstate_global->__pyx_codeobj__36
+#define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
+/* #### Code section: module_code ### */
+
+/* "pyreadr/librdata.pyx":23
  * 
  * 
- * cdef int _os_open(path, mode):             # <<<<<<<<<<<<<<
+ * cdef int _os_open(path, mode) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int flags
- *     IF UNAME_SYSNAME == 'Windows':
+ *     cdef Py_ssize_t length
  */
 
 static int __pyx_f_7pyreadr_8librdata__os_open(PyObject *__pyx_v_path, PyObject *__pyx_v_mode) {
   int __pyx_v_flags;
+  Py_ssize_t __pyx_v_length;
+  wchar_t *__pyx_v_u16_path;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  char const *__pyx_t_2;
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  wchar_t *__pyx_t_6;
+  char const *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_os_open", 0);
 
-  /* "pyreadr/librdata.pyx":35
+  /* "pyreadr/librdata.pyx":26
+ *     cdef int flags
+ *     cdef Py_ssize_t length
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *         if mode == 'r':
+ *             flags = _O_RDONLY | _O_BINARY
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_system); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_2, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_Windows, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 26, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_5) {
+
+    /* "pyreadr/librdata.pyx":27
+ *     cdef Py_ssize_t length
+ *     if platform.system() == 'Windows':
+ *         if mode == 'r':             # <<<<<<<<<<<<<<
+ *             flags = _O_RDONLY | _O_BINARY
+ *             u16_path = PyUnicode_AsWideCharString(path, &length)
+ */
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 27, __pyx_L1_error)
+    if (__pyx_t_5) {
+
+      /* "pyreadr/librdata.pyx":28
+ *     if platform.system() == 'Windows':
+ *         if mode == 'r':
+ *             flags = _O_RDONLY | _O_BINARY             # <<<<<<<<<<<<<<
+ *             u16_path = PyUnicode_AsWideCharString(path, &length)
+ *             return _wsopen(u16_path, flags, _SH_DENYWR, _S_IREAD | _S_IWRITE)
+ */
+      __pyx_v_flags = (_O_RDONLY | _O_BINARY);
+
+      /* "pyreadr/librdata.pyx":29
+ *         if mode == 'r':
+ *             flags = _O_RDONLY | _O_BINARY
+ *             u16_path = PyUnicode_AsWideCharString(path, &length)             # <<<<<<<<<<<<<<
+ *             return _wsopen(u16_path, flags, _SH_DENYWR, _S_IREAD | _S_IWRITE)
+ *         else:
+ */
+      __pyx_t_6 = PyUnicode_AsWideCharString(__pyx_v_path, (&__pyx_v_length)); if (unlikely(__pyx_t_6 == ((wchar_t *)NULL))) __PYX_ERR(0, 29, __pyx_L1_error)
+      __pyx_v_u16_path = __pyx_t_6;
+
+      /* "pyreadr/librdata.pyx":30
+ *             flags = _O_RDONLY | _O_BINARY
+ *             u16_path = PyUnicode_AsWideCharString(path, &length)
+ *             return _wsopen(u16_path, flags, _SH_DENYWR, _S_IREAD | _S_IWRITE)             # <<<<<<<<<<<<<<
+ *         else:
+ *             flags = _O_WRONLY | _O_CREAT | _O_BINARY | _O_TRUNC
+ */
+      __pyx_r = _wsopen(__pyx_v_u16_path, __pyx_v_flags, _SH_DENYWR, (_S_IREAD | _S_IWRITE));
+      goto __pyx_L0;
+
+      /* "pyreadr/librdata.pyx":27
+ *     cdef Py_ssize_t length
+ *     if platform.system() == 'Windows':
+ *         if mode == 'r':             # <<<<<<<<<<<<<<
+ *             flags = _O_RDONLY | _O_BINARY
+ *             u16_path = PyUnicode_AsWideCharString(path, &length)
+ */
+    }
+
+    /* "pyreadr/librdata.pyx":32
+ *             return _wsopen(u16_path, flags, _SH_DENYWR, _S_IREAD | _S_IWRITE)
+ *         else:
+ *             flags = _O_WRONLY | _O_CREAT | _O_BINARY | _O_TRUNC             # <<<<<<<<<<<<<<
+ *             u16_path = PyUnicode_AsWideCharString(os.fsdecode(path), &length)
+ *             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)
+ */
+    /*else*/ {
+      __pyx_v_flags = (((_O_WRONLY | _O_CREAT) | _O_BINARY) | _O_TRUNC);
+
+      /* "pyreadr/librdata.pyx":33
+ *         else:
+ *             flags = _O_WRONLY | _O_CREAT | _O_BINARY | _O_TRUNC
+ *             u16_path = PyUnicode_AsWideCharString(os.fsdecode(path), &length)             # <<<<<<<<<<<<<<
+ *             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)
+ *     else:
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fsdecode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = NULL;
+      __pyx_t_4 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __pyx_t_4 = 1;
+        }
+      }
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_path};
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      }
+      __pyx_t_6 = PyUnicode_AsWideCharString(__pyx_t_1, (&__pyx_v_length)); if (unlikely(__pyx_t_6 == ((wchar_t *)NULL))) __PYX_ERR(0, 33, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_v_u16_path = __pyx_t_6;
+
+      /* "pyreadr/librdata.pyx":34
+ *             flags = _O_WRONLY | _O_CREAT | _O_BINARY | _O_TRUNC
+ *             u16_path = PyUnicode_AsWideCharString(os.fsdecode(path), &length)
+ *             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)             # <<<<<<<<<<<<<<
+ *     else:
+ *         if mode == 'r':
+ */
+      __pyx_r = _wsopen(__pyx_v_u16_path, __pyx_v_flags, _SH_DENYRW, (_S_IREAD | _S_IWRITE));
+      goto __pyx_L0;
+    }
+
+    /* "pyreadr/librdata.pyx":26
+ *     cdef int flags
+ *     cdef Py_ssize_t length
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *         if mode == 'r':
+ *             flags = _O_RDONLY | _O_BINARY
+ */
+  }
+
+  /* "pyreadr/librdata.pyx":36
  *             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)
- *     ELSE:
+ *     else:
  *         if mode == 'r':             # <<<<<<<<<<<<<<
  *             flags = O_RDONLY
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 35, __pyx_L1_error)
-  if (__pyx_t_1) {
+  /*else*/ {
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_v_mode, __pyx_n_u_r, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 36, __pyx_L1_error)
+    if (__pyx_t_5) {
 
-    /* "pyreadr/librdata.pyx":36
- *     ELSE:
+      /* "pyreadr/librdata.pyx":37
+ *     else:
  *         if mode == 'r':
  *             flags = O_RDONLY             # <<<<<<<<<<<<<<
  *         else:
  *             flags = O_WRONLY | O_CREAT | O_TRUNC
  */
-    __pyx_v_flags = O_RDONLY;
+      __pyx_v_flags = O_RDONLY;
 
-    /* "pyreadr/librdata.pyx":35
+      /* "pyreadr/librdata.pyx":36
  *             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)
- *     ELSE:
+ *     else:
  *         if mode == 'r':             # <<<<<<<<<<<<<<
  *             flags = O_RDONLY
  *         else:
  */
-    goto __pyx_L3;
-  }
+      goto __pyx_L5;
+    }
 
-  /* "pyreadr/librdata.pyx":38
+    /* "pyreadr/librdata.pyx":39
  *             flags = O_RDONLY
  *         else:
  *             flags = O_WRONLY | O_CREAT | O_TRUNC             # <<<<<<<<<<<<<<
  *         #return open(path.encode('utf-8'), flags, 0644)
  *         return open(path, flags, 0644)
  */
-  /*else*/ {
-    __pyx_v_flags = ((O_WRONLY | O_CREAT) | O_TRUNC);
-  }
-  __pyx_L3:;
+    /*else*/ {
+      __pyx_v_flags = ((O_WRONLY | O_CREAT) | O_TRUNC);
+    }
+    __pyx_L5:;
 
-  /* "pyreadr/librdata.pyx":40
+    /* "pyreadr/librdata.pyx":41
  *             flags = O_WRONLY | O_CREAT | O_TRUNC
  *         #return open(path.encode('utf-8'), flags, 0644)
  *         return open(path, flags, 0644)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L1_error)
-  __pyx_r = open(__pyx_t_2, __pyx_v_flags, 0644);
-  goto __pyx_L0;
+    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L1_error)
+    __pyx_r = open(__pyx_t_7, __pyx_v_flags, 0644);
+    goto __pyx_L0;
+  }
 
-  /* "pyreadr/librdata.pyx":22
+  /* "pyreadr/librdata.pyx":23
  * 
  * 
- * cdef int _os_open(path, mode):             # <<<<<<<<<<<<<<
+ * cdef int _os_open(path, mode) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int flags
- *     IF UNAME_SYSNAME == 'Windows':
+ *     cdef Py_ssize_t length
  */
 
   /* function exit code */
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_WriteUnraisable("pyreadr.librdata._os_open", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":43
+/* "pyreadr/librdata.pyx":44
  * 
  * 
- * cdef int _os_close(int fd):             # <<<<<<<<<<<<<<
- *     IF UNAME_SYSNAME == 'Windows':
+ * cdef int _os_close(int fd) noexcept:             # <<<<<<<<<<<<<<
+ *     if platform.system() == 'Windows':
  *         return _close(fd)
  */
 
 static int __pyx_f_7pyreadr_8librdata__os_close(int __pyx_v_fd) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_os_close", 0);
 
-  /* "pyreadr/librdata.pyx":47
+  /* "pyreadr/librdata.pyx":45
+ * 
+ * cdef int _os_close(int fd) noexcept:
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
  *         return _close(fd)
- *     ELSE:
+ *     else:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_system); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_2, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_Windows, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_5) {
+
+    /* "pyreadr/librdata.pyx":46
+ * cdef int _os_close(int fd) noexcept:
+ *     if platform.system() == 'Windows':
+ *         return _close(fd)             # <<<<<<<<<<<<<<
+ *     else:
+ *         return close(fd)
+ */
+    __pyx_r = _close(__pyx_v_fd);
+    goto __pyx_L0;
+
+    /* "pyreadr/librdata.pyx":45
+ * 
+ * cdef int _os_close(int fd) noexcept:
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *         return _close(fd)
+ *     else:
+ */
+  }
+
+  /* "pyreadr/librdata.pyx":48
+ *         return _close(fd)
+ *     else:
  *         return close(fd)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_r = close(__pyx_v_fd);
-  goto __pyx_L0;
+  /*else*/ {
+    __pyx_r = close(__pyx_v_fd);
+    goto __pyx_L0;
+  }
 
-  /* "pyreadr/librdata.pyx":43
+  /* "pyreadr/librdata.pyx":44
  * 
  * 
- * cdef int _os_close(int fd):             # <<<<<<<<<<<<<<
- *     IF UNAME_SYSNAME == 'Windows':
+ * cdef int _os_close(int fd) noexcept:             # <<<<<<<<<<<<<<
+ *     if platform.system() == 'Windows':
  *         return _close(fd)
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_WriteUnraisable("pyreadr.librdata._os_close", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":50
+/* "pyreadr/librdata.pyx":51
  * 
  * 
- * cdef int _handle_open(const char* path, void* io_ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_open(const char* path, void* io_ctx) noexcept:             # <<<<<<<<<<<<<<
  *     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx
  *     cdef int fd
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_open(char const *__pyx_v_path, void *__pyx_v_io_ctx) {
   struct rdata_unistd_io_ctx_s *__pyx_v_ctx;
   int __pyx_v_fd;
@@ -1742,120 +3622,126 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_t_6;
+  int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_open", 0);
 
-  /* "pyreadr/librdata.pyx":51
+  /* "pyreadr/librdata.pyx":52
  * 
- * cdef int _handle_open(const char* path, void* io_ctx):
+ * cdef int _handle_open(const char* path, void* io_ctx) noexcept:
  *     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx             # <<<<<<<<<<<<<<
  *     cdef int fd
  *     if not os.path.isfile(path):
  */
   __pyx_v_ctx = ((struct rdata_unistd_io_ctx_s *)__pyx_v_io_ctx);
 
-  /* "pyreadr/librdata.pyx":53
+  /* "pyreadr/librdata.pyx":54
  *     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx
  *     cdef int fd
  *     if not os.path.isfile(path):             # <<<<<<<<<<<<<<
  *         return -1
  *     fd = _os_open(path, 'r')
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_os); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isfile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isfile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_path); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_5 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 53, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_6 = ((!__pyx_t_5) != 0);
-  if (__pyx_t_6) {
+  __pyx_t_7 = (!__pyx_t_6);
+  if (__pyx_t_7) {
 
-    /* "pyreadr/librdata.pyx":54
+    /* "pyreadr/librdata.pyx":55
  *     cdef int fd
  *     if not os.path.isfile(path):
  *         return -1             # <<<<<<<<<<<<<<
  *     fd = _os_open(path, 'r')
  *     ctx.fd = fd
  */
     __pyx_r = -1;
     goto __pyx_L0;
 
-    /* "pyreadr/librdata.pyx":53
+    /* "pyreadr/librdata.pyx":54
  *     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx
  *     cdef int fd
  *     if not os.path.isfile(path):             # <<<<<<<<<<<<<<
  *         return -1
  *     fd = _os_open(path, 'r')
  */
   }
 
-  /* "pyreadr/librdata.pyx":55
+  /* "pyreadr/librdata.pyx":56
  *     if not os.path.isfile(path):
  *         return -1
  *     fd = _os_open(path, 'r')             # <<<<<<<<<<<<<<
  *     ctx.fd = fd
  *     return fd
  */
-  __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_path); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_fd = __pyx_f_7pyreadr_8librdata__os_open(__pyx_t_1, __pyx_n_u_r);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":56
+  /* "pyreadr/librdata.pyx":57
  *         return -1
  *     fd = _os_open(path, 'r')
  *     ctx.fd = fd             # <<<<<<<<<<<<<<
  *     return fd
  * 
  */
   __pyx_v_ctx->fd = __pyx_v_fd;
 
-  /* "pyreadr/librdata.pyx":57
+  /* "pyreadr/librdata.pyx":58
  *     fd = _os_open(path, 'r')
  *     ctx.fd = fd
  *     return fd             # <<<<<<<<<<<<<<
  * 
- * cdef int _handle_table(const char *name, void *ctx):
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:
  */
   __pyx_r = __pyx_v_fd;
   goto __pyx_L0;
 
-  /* "pyreadr/librdata.pyx":50
+  /* "pyreadr/librdata.pyx":51
  * 
  * 
- * cdef int _handle_open(const char* path, void* io_ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_open(const char* path, void* io_ctx) noexcept:             # <<<<<<<<<<<<<<
  *     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx
  *     cdef int fd
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -1865,18 +3751,18 @@
   __Pyx_WriteUnraisable("pyreadr.librdata._handle_open", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":59
+/* "pyreadr/librdata.pyx":60
  *     return fd
  * 
- * cdef int _handle_table(const char *name, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_table(char const *__pyx_v_name, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -1898,116 +3784,116 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_table", 0);
 
-  /* "pyreadr/librdata.pyx":60
+  /* "pyreadr/librdata.pyx":61
  * 
- * cdef int _handle_table(const char *name, void *ctx):
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         Parser.__handle_table(parser, name)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":61
- * cdef int _handle_table(const char *name, void *ctx):
+  /* "pyreadr/librdata.pyx":62
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":62
+      /* "pyreadr/librdata.pyx":63
  *     parser = <Parser>ctx
  *     try:
  *         Parser.__handle_table(parser, name)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_table(__pyx_v_parser, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L3_error)
+      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_table(__pyx_v_parser, __pyx_v_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 63, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyreadr/librdata.pyx":63
+      /* "pyreadr/librdata.pyx":64
  *     try:
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":61
- * cdef int _handle_table(const char *name, void *ctx):
+      /* "pyreadr/librdata.pyx":62
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":64
+    /* "pyreadr/librdata.pyx":65
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_5) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_table", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 64, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 65, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":65
+        /* "pyreadr/librdata.pyx":66
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 65, __pyx_L14_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 66, __pyx_L14_error)
 
-        /* "pyreadr/librdata.pyx":66
+        /* "pyreadr/librdata.pyx":67
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L13_return;
       }
 
-      /* "pyreadr/librdata.pyx":64
+      /* "pyreadr/librdata.pyx":65
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -2022,16 +3908,15 @@
           __Pyx_XGOTREF(__pyx_t_11);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __pyx_t_5 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_13);
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
           }
@@ -2041,31 +3926,30 @@
           __Pyx_ErrRestore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
           __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_9;
           goto __pyx_L5_except_error;
         }
         __pyx_L13_return: {
           __pyx_t_8 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_8;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":61
- * cdef int _handle_table(const char *name, void *ctx):
+    /* "pyreadr/librdata.pyx":62
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_table(parser, name)
  *         return rdata_error_t.RDATA_OK
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -2077,18 +3961,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":59
+  /* "pyreadr/librdata.pyx":60
  *     return fd
  * 
- * cdef int _handle_table(const char *name, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_table(const char *name, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2099,18 +3983,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":69
+/* "pyreadr/librdata.pyx":70
  * 
  * 
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_column(char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -2133,138 +4017,138 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_column", 0);
 
-  /* "pyreadr/librdata.pyx":70
+  /* "pyreadr/librdata.pyx":71
  * 
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         if parser.parse_current_table:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":71
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+  /* "pyreadr/librdata.pyx":72
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_column(parser, name, type, data, count)
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":72
+      /* "pyreadr/librdata.pyx":73
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_column(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L3_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 72, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 73, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_5) {
 
-        /* "pyreadr/librdata.pyx":73
+        /* "pyreadr/librdata.pyx":74
  *     try:
  *         if parser.parse_current_table:
  *             Parser.__handle_column(parser, name, type, data, count)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_column(__pyx_v_parser, __pyx_v_name, __pyx_v_type, __pyx_v_data, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 73, __pyx_L3_error)
+        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column(__pyx_v_parser, __pyx_v_name, __pyx_v_type, __pyx_v_data, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "pyreadr/librdata.pyx":72
+        /* "pyreadr/librdata.pyx":73
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_column(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  */
       }
 
-      /* "pyreadr/librdata.pyx":74
+      /* "pyreadr/librdata.pyx":75
  *         if parser.parse_current_table:
  *             Parser.__handle_column(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":71
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+      /* "pyreadr/librdata.pyx":72
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_column(parser, name, type, data, count)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":75
+    /* "pyreadr/librdata.pyx":76
  *             Parser.__handle_column(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_6) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_column", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 75, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_8);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 76, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_e = __pyx_t_7;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":76
+        /* "pyreadr/librdata.pyx":77
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 76, __pyx_L15_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 77, __pyx_L15_error)
 
-        /* "pyreadr/librdata.pyx":77
+        /* "pyreadr/librdata.pyx":78
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L14_return;
       }
 
-      /* "pyreadr/librdata.pyx":75
+      /* "pyreadr/librdata.pyx":76
  *             Parser.__handle_column(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -2279,16 +4163,15 @@
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __Pyx_XGOTREF(__pyx_t_16);
           __pyx_t_6 = __pyx_lineno; __pyx_t_9 = __pyx_clineno; __pyx_t_10 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_XGIVEREF(__pyx_t_16);
             __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
           }
@@ -2298,31 +4181,30 @@
           __Pyx_ErrRestore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
           __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
           __pyx_lineno = __pyx_t_6; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
           goto __pyx_L5_except_error;
         }
         __pyx_L14_return: {
           __pyx_t_9 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_9;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":71
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+    /* "pyreadr/librdata.pyx":72
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_column(parser, name, type, data, count)
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -2334,18 +4216,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":69
+  /* "pyreadr/librdata.pyx":70
  * 
  * 
- * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2356,18 +4238,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":79
+/* "pyreadr/librdata.pyx":80
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_dim(char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -2390,138 +4272,138 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_dim", 0);
 
-  /* "pyreadr/librdata.pyx":80
+  /* "pyreadr/librdata.pyx":81
  * 
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         if parser.parse_current_table:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":81
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+  /* "pyreadr/librdata.pyx":82
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_dim(parser, name, type, data, count)
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":82
+      /* "pyreadr/librdata.pyx":83
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_dim(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L3_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 82, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 83, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_5) {
 
-        /* "pyreadr/librdata.pyx":83
+        /* "pyreadr/librdata.pyx":84
  *     try:
  *         if parser.parse_current_table:
  *             Parser.__handle_dim(parser, name, type, data, count)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_dim(__pyx_v_parser, __pyx_v_name, __pyx_v_type, __pyx_v_data, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L3_error)
+        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim(__pyx_v_parser, __pyx_v_name, __pyx_v_type, __pyx_v_data, __pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "pyreadr/librdata.pyx":82
+        /* "pyreadr/librdata.pyx":83
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_dim(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  */
       }
 
-      /* "pyreadr/librdata.pyx":84
+      /* "pyreadr/librdata.pyx":85
  *         if parser.parse_current_table:
  *             Parser.__handle_dim(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":81
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+      /* "pyreadr/librdata.pyx":82
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_dim(parser, name, type, data, count)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":85
+    /* "pyreadr/librdata.pyx":86
  *             Parser.__handle_dim(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_6) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_dim", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 85, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_8);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 86, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_e = __pyx_t_7;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":86
+        /* "pyreadr/librdata.pyx":87
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 86, __pyx_L15_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 87, __pyx_L15_error)
 
-        /* "pyreadr/librdata.pyx":87
+        /* "pyreadr/librdata.pyx":88
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L14_return;
       }
 
-      /* "pyreadr/librdata.pyx":85
+      /* "pyreadr/librdata.pyx":86
  *             Parser.__handle_dim(parser, name, type, data, count)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -2536,16 +4418,15 @@
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __Pyx_XGOTREF(__pyx_t_16);
           __pyx_t_6 = __pyx_lineno; __pyx_t_9 = __pyx_clineno; __pyx_t_10 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_XGIVEREF(__pyx_t_16);
             __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
           }
@@ -2555,31 +4436,30 @@
           __Pyx_ErrRestore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
           __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
           __pyx_lineno = __pyx_t_6; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
           goto __pyx_L5_except_error;
         }
         __pyx_L14_return: {
           __pyx_t_9 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_9;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":81
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+    /* "pyreadr/librdata.pyx":82
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_dim(parser, name, type, data, count)
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -2591,18 +4471,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":79
+  /* "pyreadr/librdata.pyx":80
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2613,18 +4493,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":90
+/* "pyreadr/librdata.pyx":91
  * 
  * 
- * cdef int _handle_column_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_column_name(char const *__pyx_v_name, int __pyx_v_index, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -2646,116 +4526,116 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_column_name", 0);
 
-  /* "pyreadr/librdata.pyx":91
+  /* "pyreadr/librdata.pyx":92
  * 
- * cdef int _handle_column_name(const char *name, int index, void *ctx):
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         Parser.__handle_column_name(parser, name, index)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":92
- * cdef int _handle_column_name(const char *name, int index, void *ctx):
+  /* "pyreadr/librdata.pyx":93
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":93
+      /* "pyreadr/librdata.pyx":94
  *     parser = <Parser>ctx
  *     try:
  *         Parser.__handle_column_name(parser, name, index)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_column_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L3_error)
+      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyreadr/librdata.pyx":94
+      /* "pyreadr/librdata.pyx":95
  *     try:
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":92
- * cdef int _handle_column_name(const char *name, int index, void *ctx):
+      /* "pyreadr/librdata.pyx":93
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":95
+    /* "pyreadr/librdata.pyx":96
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_5) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_column_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 95, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 96, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":96
+        /* "pyreadr/librdata.pyx":97
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 96, __pyx_L14_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 97, __pyx_L14_error)
 
-        /* "pyreadr/librdata.pyx":97
+        /* "pyreadr/librdata.pyx":98
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L13_return;
       }
 
-      /* "pyreadr/librdata.pyx":95
+      /* "pyreadr/librdata.pyx":96
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -2770,16 +4650,15 @@
           __Pyx_XGOTREF(__pyx_t_11);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __pyx_t_5 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_13);
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
           }
@@ -2789,31 +4668,30 @@
           __Pyx_ErrRestore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
           __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_9;
           goto __pyx_L5_except_error;
         }
         __pyx_L13_return: {
           __pyx_t_8 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_8;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":92
- * cdef int _handle_column_name(const char *name, int index, void *ctx):
+    /* "pyreadr/librdata.pyx":93
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_column_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -2825,18 +4703,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":90
+  /* "pyreadr/librdata.pyx":91
  * 
  * 
- * cdef int _handle_column_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2847,18 +4725,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":99
+/* "pyreadr/librdata.pyx":100
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_dim_name(char const *__pyx_v_name, int __pyx_v_index, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -2880,116 +4758,116 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_dim_name", 0);
 
-  /* "pyreadr/librdata.pyx":100
+  /* "pyreadr/librdata.pyx":101
  * 
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         Parser.__handle_dim_name(parser, name, index)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":101
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):
+  /* "pyreadr/librdata.pyx":102
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":102
+      /* "pyreadr/librdata.pyx":103
  *     parser = <Parser>ctx
  *     try:
  *         Parser.__handle_dim_name(parser, name, index)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_dim_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L3_error)
+      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyreadr/librdata.pyx":103
+      /* "pyreadr/librdata.pyx":104
  *     try:
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":101
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):
+      /* "pyreadr/librdata.pyx":102
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":104
+    /* "pyreadr/librdata.pyx":105
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_5) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_dim_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 104, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 105, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":105
+        /* "pyreadr/librdata.pyx":106
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 105, __pyx_L14_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 106, __pyx_L14_error)
 
-        /* "pyreadr/librdata.pyx":106
+        /* "pyreadr/librdata.pyx":107
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
- * cdef int _handle_row_name(const char *name, int index, void *ctx):
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L13_return;
       }
 
-      /* "pyreadr/librdata.pyx":104
+      /* "pyreadr/librdata.pyx":105
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -3004,16 +4882,15 @@
           __Pyx_XGOTREF(__pyx_t_11);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __pyx_t_5 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_13);
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
           }
@@ -3023,31 +4900,30 @@
           __Pyx_ErrRestore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
           __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_9;
           goto __pyx_L5_except_error;
         }
         __pyx_L13_return: {
           __pyx_t_8 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_8;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":101
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):
+    /* "pyreadr/librdata.pyx":102
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_dim_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -3059,18 +4935,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":99
+  /* "pyreadr/librdata.pyx":100
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_dim_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -3081,18 +4957,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":108
+/* "pyreadr/librdata.pyx":109
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_row_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_row_name(char const *__pyx_v_name, int __pyx_v_index, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -3114,116 +4990,116 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_row_name", 0);
 
-  /* "pyreadr/librdata.pyx":109
+  /* "pyreadr/librdata.pyx":110
  * 
- * cdef int _handle_row_name(const char *name, int index, void *ctx):
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         Parser.__handle_row_name(parser, name, index)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":110
- * cdef int _handle_row_name(const char *name, int index, void *ctx):
+  /* "pyreadr/librdata.pyx":111
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":111
+      /* "pyreadr/librdata.pyx":112
  *     parser = <Parser>ctx
  *     try:
  *         Parser.__handle_row_name(parser, name, index)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_row_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L3_error)
+      __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_row_name(__pyx_v_parser, __pyx_v_name, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "pyreadr/librdata.pyx":112
+      /* "pyreadr/librdata.pyx":113
  *     try:
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":110
- * cdef int _handle_row_name(const char *name, int index, void *ctx):
+      /* "pyreadr/librdata.pyx":111
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":113
+    /* "pyreadr/librdata.pyx":114
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_5) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_row_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 113, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 114, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":114
+        /* "pyreadr/librdata.pyx":115
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 114, __pyx_L14_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 115, __pyx_L14_error)
 
-        /* "pyreadr/librdata.pyx":115
+        /* "pyreadr/librdata.pyx":116
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         goto __pyx_L13_return;
       }
 
-      /* "pyreadr/librdata.pyx":113
+      /* "pyreadr/librdata.pyx":114
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -3238,16 +5114,15 @@
           __Pyx_XGOTREF(__pyx_t_11);
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __pyx_t_5 = __pyx_lineno; __pyx_t_8 = __pyx_clineno; __pyx_t_9 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_13);
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
           }
@@ -3257,31 +5132,30 @@
           __Pyx_ErrRestore(__pyx_t_10, __pyx_t_11, __pyx_t_12);
           __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0;
           __pyx_lineno = __pyx_t_5; __pyx_clineno = __pyx_t_8; __pyx_filename = __pyx_t_9;
           goto __pyx_L5_except_error;
         }
         __pyx_L13_return: {
           __pyx_t_8 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_8;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":110
- * cdef int _handle_row_name(const char *name, int index, void *ctx):
+    /* "pyreadr/librdata.pyx":111
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         Parser.__handle_row_name(parser, name, index)
  *         return rdata_error_t.RDATA_OK
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -3293,18 +5167,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":108
+  /* "pyreadr/librdata.pyx":109
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
- * cdef int _handle_row_name(const char *name, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -3315,18 +5189,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":118
+/* "pyreadr/librdata.pyx":119
  * 
  * 
- * cdef int _handle_text_value(const char *value, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_text_value(char const *__pyx_v_value, int __pyx_v_index, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -3349,138 +5223,138 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_text_value", 0);
 
-  /* "pyreadr/librdata.pyx":119
+  /* "pyreadr/librdata.pyx":120
  * 
- * cdef int _handle_text_value(const char *value, int index, void *ctx):
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         if parser.parse_current_table:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":120
- * cdef int _handle_text_value(const char *value, int index, void *ctx):
+  /* "pyreadr/librdata.pyx":121
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_text_value(parser, value, index)
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":121
+      /* "pyreadr/librdata.pyx":122
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_text_value(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L3_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 121, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 122, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_5) {
 
-        /* "pyreadr/librdata.pyx":122
+        /* "pyreadr/librdata.pyx":123
  *     try:
  *         if parser.parse_current_table:
  *             Parser.__handle_text_value(parser, value, index)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_text_value(__pyx_v_parser, __pyx_v_value, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L3_error)
+        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_text_value(__pyx_v_parser, __pyx_v_value, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "pyreadr/librdata.pyx":121
+        /* "pyreadr/librdata.pyx":122
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_text_value(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  */
       }
 
-      /* "pyreadr/librdata.pyx":123
+      /* "pyreadr/librdata.pyx":124
  *         if parser.parse_current_table:
  *             Parser.__handle_text_value(parser, value, index)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":120
- * cdef int _handle_text_value(const char *value, int index, void *ctx):
+      /* "pyreadr/librdata.pyx":121
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_text_value(parser, value, index)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":124
+    /* "pyreadr/librdata.pyx":125
  *             Parser.__handle_text_value(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_6) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_text_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 124, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_8);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 125, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_e = __pyx_t_7;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":125
+        /* "pyreadr/librdata.pyx":126
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 125, __pyx_L15_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 126, __pyx_L15_error)
 
-        /* "pyreadr/librdata.pyx":126
+        /* "pyreadr/librdata.pyx":127
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L14_return;
       }
 
-      /* "pyreadr/librdata.pyx":124
+      /* "pyreadr/librdata.pyx":125
  *             Parser.__handle_text_value(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -3495,16 +5369,15 @@
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __Pyx_XGOTREF(__pyx_t_16);
           __pyx_t_6 = __pyx_lineno; __pyx_t_9 = __pyx_clineno; __pyx_t_10 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_XGIVEREF(__pyx_t_16);
             __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
           }
@@ -3514,31 +5387,30 @@
           __Pyx_ErrRestore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
           __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
           __pyx_lineno = __pyx_t_6; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
           goto __pyx_L5_except_error;
         }
         __pyx_L14_return: {
           __pyx_t_9 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_9;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":120
- * cdef int _handle_text_value(const char *value, int index, void *ctx):
+    /* "pyreadr/librdata.pyx":121
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_text_value(parser, value, index)
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -3550,18 +5422,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":118
+  /* "pyreadr/librdata.pyx":119
  * 
  * 
- * cdef int _handle_text_value(const char *value, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -3572,18 +5444,18 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":129
+/* "pyreadr/librdata.pyx":130
  * 
  * 
- * cdef int _handle_value_label(const char *value, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
 static int __pyx_f_7pyreadr_8librdata__handle_value_label(char const *__pyx_v_value, int __pyx_v_index, void *__pyx_v_ctx) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_parser = NULL;
   PyObject *__pyx_v_e = NULL;
@@ -3606,138 +5478,138 @@
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_value_label", 0);
 
-  /* "pyreadr/librdata.pyx":130
+  /* "pyreadr/librdata.pyx":131
  * 
- * cdef int _handle_value_label(const char *value, int index, void *ctx):
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx             # <<<<<<<<<<<<<<
  *     try:
  *         if parser.parse_current_table:
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_ctx);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_parser = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":131
- * cdef int _handle_value_label(const char *value, int index, void *ctx):
+  /* "pyreadr/librdata.pyx":132
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_value_label(parser, value, index)
  */
   {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "pyreadr/librdata.pyx":132
+      /* "pyreadr/librdata.pyx":133
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_value_label(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L3_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_parse_current_table); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 132, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 133, __pyx_L3_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (__pyx_t_5) {
 
-        /* "pyreadr/librdata.pyx":133
+        /* "pyreadr/librdata.pyx":134
  *     try:
  *         if parser.parse_current_table:
  *             Parser.__handle_value_label(parser, value, index)             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  */
-        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser___handle_value_label(__pyx_v_parser, __pyx_v_value, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L3_error)
+        __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_value_label(__pyx_v_parser, __pyx_v_value, __pyx_v_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "pyreadr/librdata.pyx":132
+        /* "pyreadr/librdata.pyx":133
  *     parser = <Parser>ctx
  *     try:
  *         if parser.parse_current_table:             # <<<<<<<<<<<<<<
  *             Parser.__handle_value_label(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  */
       }
 
-      /* "pyreadr/librdata.pyx":134
+      /* "pyreadr/librdata.pyx":135
  *         if parser.parse_current_table:
  *             Parser.__handle_value_label(parser, value, index)
  *         return rdata_error_t.RDATA_OK             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         parser._error = e
  */
       __pyx_r = RDATA_OK;
       goto __pyx_L7_try_return;
 
-      /* "pyreadr/librdata.pyx":131
- * cdef int _handle_value_label(const char *value, int index, void *ctx):
+      /* "pyreadr/librdata.pyx":132
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_value_label(parser, value, index)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "pyreadr/librdata.pyx":135
+    /* "pyreadr/librdata.pyx":136
  *             Parser.__handle_value_label(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_6) {
       __Pyx_AddTraceback("pyreadr.librdata._handle_value_label", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 135, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_GOTREF(__pyx_t_8);
+      if (__Pyx_GetException(&__pyx_t_1, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 136, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_1);
+      __Pyx_XGOTREF(__pyx_t_7);
+      __Pyx_XGOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_e = __pyx_t_7;
       /*try:*/ {
 
-        /* "pyreadr/librdata.pyx":136
+        /* "pyreadr/librdata.pyx":137
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:
  *         parser._error = e             # <<<<<<<<<<<<<<
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  * 
  */
-        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 136, __pyx_L15_error)
+        if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_parser), __pyx_n_s_error, __pyx_v_e) < 0) __PYX_ERR(0, 137, __pyx_L15_error)
 
-        /* "pyreadr/librdata.pyx":137
+        /* "pyreadr/librdata.pyx":138
  *     except Exception as e:
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT             # <<<<<<<<<<<<<<
  * 
  * 
  */
         __pyx_r = RDATA_ERROR_USER_ABORT;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L14_return;
       }
 
-      /* "pyreadr/librdata.pyx":135
+      /* "pyreadr/librdata.pyx":136
  *             Parser.__handle_value_label(parser, value, index)
  *         return rdata_error_t.RDATA_OK
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         parser._error = e
  *         return rdata_error_t.RDATA_ERROR_USER_ABORT
  */
       /*finally:*/ {
@@ -3752,16 +5624,15 @@
           __Pyx_XGOTREF(__pyx_t_12);
           __Pyx_XGOTREF(__pyx_t_13);
           __Pyx_XGOTREF(__pyx_t_14);
           __Pyx_XGOTREF(__pyx_t_15);
           __Pyx_XGOTREF(__pyx_t_16);
           __pyx_t_6 = __pyx_lineno; __pyx_t_9 = __pyx_clineno; __pyx_t_10 = __pyx_filename;
           {
-            __Pyx_DECREF(__pyx_v_e);
-            __pyx_v_e = NULL;
+            __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           }
           if (PY_MAJOR_VERSION >= 3) {
             __Pyx_XGIVEREF(__pyx_t_14);
             __Pyx_XGIVEREF(__pyx_t_15);
             __Pyx_XGIVEREF(__pyx_t_16);
             __Pyx_ExceptionReset(__pyx_t_14, __pyx_t_15, __pyx_t_16);
           }
@@ -3771,31 +5642,30 @@
           __Pyx_ErrRestore(__pyx_t_11, __pyx_t_12, __pyx_t_13);
           __pyx_t_11 = 0; __pyx_t_12 = 0; __pyx_t_13 = 0; __pyx_t_14 = 0; __pyx_t_15 = 0; __pyx_t_16 = 0;
           __pyx_lineno = __pyx_t_6; __pyx_clineno = __pyx_t_9; __pyx_filename = __pyx_t_10;
           goto __pyx_L5_except_error;
         }
         __pyx_L14_return: {
           __pyx_t_9 = __pyx_r;
-          __Pyx_DECREF(__pyx_v_e);
-          __pyx_v_e = NULL;
+          __Pyx_DECREF(__pyx_v_e); __pyx_v_e = 0;
           __pyx_r = __pyx_t_9;
           goto __pyx_L6_except_return;
         }
       }
     }
     goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
 
-    /* "pyreadr/librdata.pyx":131
- * cdef int _handle_value_label(const char *value, int index, void *ctx):
+    /* "pyreadr/librdata.pyx":132
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:
  *     parser = <Parser>ctx
  *     try:             # <<<<<<<<<<<<<<
  *         if parser.parse_current_table:
  *             Parser.__handle_value_label(parser, value, index)
  */
+    __pyx_L5_except_error:;
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L1_error;
     __pyx_L7_try_return:;
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -3807,18 +5677,18 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "pyreadr/librdata.pyx":129
+  /* "pyreadr/librdata.pyx":130
  * 
  * 
- * cdef int _handle_value_label(const char *value, int index, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     parser = <Parser>ctx
  *     try:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -3829,305 +5699,379 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_parser);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":148
+/* "pyreadr/librdata.pyx":149
  *     parse_current_table = True
  * 
- *     cpdef parse(self, path):             # <<<<<<<<<<<<<<
+ *     cpdef parse(self, path) noexcept:             # <<<<<<<<<<<<<<
  * 
  *         cdef rdata_error_t status
  */
 
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, PyObject *__pyx_v_path); /*proto*/
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
 static PyObject *__pyx_f_7pyreadr_8librdata_6Parser_parse(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, PyObject *__pyx_v_path, int __pyx_skip_dispatch) {
   enum rdata_error_e __pyx_v_status;
   char const *__pyx_v_message;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  char const *__pyx_t_5;
+  int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_t_7;
+  char const *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
   /* Check if called by wrapper */
   if (unlikely(__pyx_skip_dispatch)) ;
   /* Check if overridden in Python */
-  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
+  else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
-      PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
+      PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_parse); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7pyreadr_8librdata_6Parser_1parse)) {
+      #ifdef __Pyx_CyFunction_USED
+      if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
+      #else
+      if (!PyCFunction_Check(__pyx_t_1)
+      #endif
+              || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_7pyreadr_8librdata_6Parser_1parse)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
+        __pyx_t_5 = 0;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
           if (likely(__pyx_t_4)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_5 = 1;
           }
         }
-        __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_path) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_path);
-        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_2);
-        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_path};
+          __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_2);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       __pyx_obj_dict_version = __Pyx_get_object_dict_version(((PyObject *)__pyx_v_self));
-      if (unlikely(__pyx_type_dict_guard != __pyx_tp_dict_version)) {
+      if (unlikely(__pyx_typedict_guard != __pyx_tp_dict_version)) {
         __pyx_tp_dict_version = __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
       }
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "pyreadr/librdata.pyx":152
+  /* "pyreadr/librdata.pyx":153
  *         cdef rdata_error_t status
  * 
  *         self._this = rdata_parser_init();             # <<<<<<<<<<<<<<
  *         self._fd = 0
  *         self._error = None
  */
   __pyx_v_self->_this = rdata_parser_init();
 
-  /* "pyreadr/librdata.pyx":153
+  /* "pyreadr/librdata.pyx":154
  * 
  *         self._this = rdata_parser_init();
  *         self._fd = 0             # <<<<<<<<<<<<<<
  *         self._error = None
  * 
  */
   __pyx_v_self->_fd = 0;
 
-  /* "pyreadr/librdata.pyx":154
+  /* "pyreadr/librdata.pyx":155
  *         self._this = rdata_parser_init();
  *         self._fd = 0
  *         self._error = None             # <<<<<<<<<<<<<<
  * 
- *         IF UNAME_SYSNAME == 'Windows':  # custom file opener for windows *sigh*
+ *         if platform.system() == 'Windows':
  */
-  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error, Py_None) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error, Py_None) < 0) __PYX_ERR(0, 155, __pyx_L1_error)
 
-  /* "pyreadr/librdata.pyx":159
+  /* "pyreadr/librdata.pyx":157
+ *         self._error = None
+ * 
+ *         if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *             rdata_set_open_handler(self._this, _handle_open)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_system); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_5 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_5 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_2, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_t_6 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_Windows, Py_EQ)); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_6) {
+
+    /* "pyreadr/librdata.pyx":158
+ * 
+ *         if platform.system() == 'Windows':
+ *             rdata_set_open_handler(self._this, _handle_open)             # <<<<<<<<<<<<<<
+ * 
+ *         rdata_set_table_handler(self._this, _handle_table)
+ */
+    (void)(rdata_set_open_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_open));
+
+    /* "pyreadr/librdata.pyx":157
+ *         self._error = None
+ * 
+ *         if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *             rdata_set_open_handler(self._this, _handle_open)
+ * 
+ */
+  }
+
+  /* "pyreadr/librdata.pyx":160
  *             rdata_set_open_handler(self._this, _handle_open)
  * 
  *         rdata_set_table_handler(self._this, _handle_table)             # <<<<<<<<<<<<<<
  *         rdata_set_column_handler(self._this, _handle_column)
  *         rdata_set_column_name_handler(self._this, _handle_column_name)
  */
   (void)(rdata_set_table_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_table));
 
-  /* "pyreadr/librdata.pyx":160
+  /* "pyreadr/librdata.pyx":161
  * 
  *         rdata_set_table_handler(self._this, _handle_table)
  *         rdata_set_column_handler(self._this, _handle_column)             # <<<<<<<<<<<<<<
  *         rdata_set_column_name_handler(self._this, _handle_column_name)
  *         rdata_set_dim_handler(self._this, _handle_dim)
  */
   (void)(rdata_set_column_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_column));
 
-  /* "pyreadr/librdata.pyx":161
+  /* "pyreadr/librdata.pyx":162
  *         rdata_set_table_handler(self._this, _handle_table)
  *         rdata_set_column_handler(self._this, _handle_column)
  *         rdata_set_column_name_handler(self._this, _handle_column_name)             # <<<<<<<<<<<<<<
  *         rdata_set_dim_handler(self._this, _handle_dim)
  *         rdata_set_dim_name_handler(self._this, _handle_dim_name)
  */
   (void)(rdata_set_column_name_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_column_name));
 
-  /* "pyreadr/librdata.pyx":162
+  /* "pyreadr/librdata.pyx":163
  *         rdata_set_column_handler(self._this, _handle_column)
  *         rdata_set_column_name_handler(self._this, _handle_column_name)
  *         rdata_set_dim_handler(self._this, _handle_dim)             # <<<<<<<<<<<<<<
  *         rdata_set_dim_name_handler(self._this, _handle_dim_name)
  *         rdata_set_row_name_handler(self._this, _handle_row_name)
  */
   (void)(rdata_set_dim_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_dim));
 
-  /* "pyreadr/librdata.pyx":163
+  /* "pyreadr/librdata.pyx":164
  *         rdata_set_column_name_handler(self._this, _handle_column_name)
  *         rdata_set_dim_handler(self._this, _handle_dim)
  *         rdata_set_dim_name_handler(self._this, _handle_dim_name)             # <<<<<<<<<<<<<<
  *         rdata_set_row_name_handler(self._this, _handle_row_name)
  *         rdata_set_text_value_handler(self._this, _handle_text_value)
  */
   (void)(rdata_set_dim_name_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_dim_name));
 
-  /* "pyreadr/librdata.pyx":164
+  /* "pyreadr/librdata.pyx":165
  *         rdata_set_dim_handler(self._this, _handle_dim)
  *         rdata_set_dim_name_handler(self._this, _handle_dim_name)
  *         rdata_set_row_name_handler(self._this, _handle_row_name)             # <<<<<<<<<<<<<<
  *         rdata_set_text_value_handler(self._this, _handle_text_value)
  *         rdata_set_value_label_handler(self._this, _handle_value_label)
  */
   (void)(rdata_set_row_name_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_row_name));
 
-  /* "pyreadr/librdata.pyx":165
+  /* "pyreadr/librdata.pyx":166
  *         rdata_set_dim_name_handler(self._this, _handle_dim_name)
  *         rdata_set_row_name_handler(self._this, _handle_row_name)
  *         rdata_set_text_value_handler(self._this, _handle_text_value)             # <<<<<<<<<<<<<<
  *         rdata_set_value_label_handler(self._this, _handle_value_label)
  * 
  */
   (void)(rdata_set_text_value_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_text_value));
 
-  /* "pyreadr/librdata.pyx":166
+  /* "pyreadr/librdata.pyx":167
  *         rdata_set_row_name_handler(self._this, _handle_row_name)
  *         rdata_set_text_value_handler(self._this, _handle_text_value)
  *         rdata_set_value_label_handler(self._this, _handle_value_label)             # <<<<<<<<<<<<<<
  * 
  *         status = rdata_parse(self._this, path, <void*>self)
  */
   (void)(rdata_set_value_label_handler(__pyx_v_self->_this, __pyx_f_7pyreadr_8librdata__handle_value_label));
 
-  /* "pyreadr/librdata.pyx":168
+  /* "pyreadr/librdata.pyx":169
  *         rdata_set_value_label_handler(self._this, _handle_value_label)
  * 
  *         status = rdata_parse(self._this, path, <void*>self)             # <<<<<<<<<<<<<<
  *         #status = rdata_parse(self._this, path.encode('utf-8'), <void*>self)
  *         rdata_parser_free(self._this)
  */
-  __pyx_t_5 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 168, __pyx_L1_error)
-  __pyx_v_status = rdata_parse(__pyx_v_self->_this, __pyx_t_5, ((void *)__pyx_v_self));
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_v_path); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_v_status = rdata_parse(__pyx_v_self->_this, __pyx_t_7, ((void *)__pyx_v_self));
 
-  /* "pyreadr/librdata.pyx":170
+  /* "pyreadr/librdata.pyx":171
  *         status = rdata_parse(self._this, path, <void*>self)
  *         #status = rdata_parse(self._this, path.encode('utf-8'), <void*>self)
  *         rdata_parser_free(self._this)             # <<<<<<<<<<<<<<
  * 
  *         if status != RDATA_OK:
  */
   rdata_parser_free(__pyx_v_self->_this);
 
-  /* "pyreadr/librdata.pyx":172
+  /* "pyreadr/librdata.pyx":173
  *         rdata_parser_free(self._this)
  * 
  *         if status != RDATA_OK:             # <<<<<<<<<<<<<<
  *             if self._error is not None:
  *                 raise self._error
  */
-  __pyx_t_6 = ((__pyx_v_status != RDATA_OK) != 0);
+  __pyx_t_6 = (__pyx_v_status != RDATA_OK);
   if (__pyx_t_6) {
 
-    /* "pyreadr/librdata.pyx":173
+    /* "pyreadr/librdata.pyx":174
  * 
  *         if status != RDATA_OK:
  *             if self._error is not None:             # <<<<<<<<<<<<<<
  *                 raise self._error
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = (__pyx_t_1 != Py_None);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = (__pyx_t_6 != 0);
-    if (unlikely(__pyx_t_7)) {
+    if (unlikely(__pyx_t_6)) {
 
-      /* "pyreadr/librdata.pyx":174
+      /* "pyreadr/librdata.pyx":175
  *         if status != RDATA_OK:
  *             if self._error is not None:
  *                 raise self._error             # <<<<<<<<<<<<<<
  *             else:
  *                 message = rdata_error_message(status)
  */
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_error); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 174, __pyx_L1_error)
+      __PYX_ERR(0, 175, __pyx_L1_error)
 
-      /* "pyreadr/librdata.pyx":173
+      /* "pyreadr/librdata.pyx":174
  * 
  *         if status != RDATA_OK:
  *             if self._error is not None:             # <<<<<<<<<<<<<<
  *                 raise self._error
  *             else:
  */
     }
 
-    /* "pyreadr/librdata.pyx":176
+    /* "pyreadr/librdata.pyx":177
  *                 raise self._error
  *             else:
  *                 message = rdata_error_message(status)             # <<<<<<<<<<<<<<
  *                 raise LibrdataError(message)
  * 
  */
     /*else*/ {
       __pyx_v_message = rdata_error_message(__pyx_v_status);
 
-      /* "pyreadr/librdata.pyx":177
+      /* "pyreadr/librdata.pyx":178
  *             else:
  *                 message = rdata_error_message(status)
  *                 raise LibrdataError(message)             # <<<<<<<<<<<<<<
  * 
  *     def handle_table(self, name):
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_message); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_2 = __Pyx_PyStr_FromString(__pyx_v_message); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
-      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+      __pyx_t_5 = 0;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_4)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_2, function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_5 = 1;
         }
       }
-      __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_2};
+        __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_1);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 177, __pyx_L1_error)
+      __PYX_ERR(0, 178, __pyx_L1_error)
     }
 
-    /* "pyreadr/librdata.pyx":172
+    /* "pyreadr/librdata.pyx":173
  *         rdata_parser_free(self._this)
  * 
  *         if status != RDATA_OK:             # <<<<<<<<<<<<<<
  *             if self._error is not None:
  *                 raise self._error
  */
   }
 
-  /* "pyreadr/librdata.pyx":148
+  /* "pyreadr/librdata.pyx":149
  *     parse_current_table = True
  * 
- *     cpdef parse(self, path):             # <<<<<<<<<<<<<<
+ *     cpdef parse(self, path) noexcept:             # <<<<<<<<<<<<<<
  * 
  *         cdef rdata_error_t status
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -4141,20 +6085,78 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, PyObject *__pyx_v_path); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, PyObject *__pyx_v_path) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_1parse = {"parse", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_1parse, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_1parse(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_path = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("parse (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_parse(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), ((PyObject *)__pyx_v_path));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_path,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "parse") < 0)) __PYX_ERR(0, 149, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_path = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("parse", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 149, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Parser.parse", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_parse(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_path);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_parse(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, PyObject *__pyx_v_path) {
@@ -4162,15 +6164,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("parse", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser_parse(__pyx_v_self, __pyx_v_path, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7pyreadr_8librdata_6Parser_parse(__pyx_v_self, __pyx_v_path, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4179,29 +6181,87 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":179
+/* "pyreadr/librdata.pyx":180
  *                 raise LibrdataError(message)
  * 
  *     def handle_table(self, name):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_3handle_table = {"handle_table", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v_name = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_table (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_2handle_table(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), ((PyObject *)__pyx_v_name));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 180, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_table") < 0)) __PYX_ERR(0, 180, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_name = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("handle_table", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 180, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_table", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_2handle_table(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_2handle_table(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_name) {
@@ -4212,96 +6272,117 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":182
+/* "pyreadr/librdata.pyx":183
  *         pass
  * 
  *     def handle_column(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_5handle_column = {"handle_column", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_data_type = 0;
   CYTHON_UNUSED PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED PyObject *__pyx_v_count = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_column (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_data_type,&__pyx_n_s_data,&__pyx_n_s_count,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_data_type,&__pyx_n_s_data,&__pyx_n_s_count,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_type)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data_type)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 1); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 1); __PYX_ERR(0, 183, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 2); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 2); __PYX_ERR(0, 183, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_count)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 183, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 3); __PYX_ERR(0, 182, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, 3); __PYX_ERR(0, 183, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_column") < 0)) __PYX_ERR(0, 182, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_column") < 0)) __PYX_ERR(0, 183, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_name = values[0];
     __pyx_v_data_type = values[1];
     __pyx_v_data = values[2];
     __pyx_v_count = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 182, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_column", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 183, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_column", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_4handle_column(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_data_type, __pyx_v_data, __pyx_v_count);
 
@@ -4318,74 +6399,93 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":185
+/* "pyreadr/librdata.pyx":186
  *         pass
  * 
  *     def handle_column_name(self, name, index):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_7handle_column_name = {"handle_column_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_index = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_column_name (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 186, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_column_name", 1, 2, 2, 1); __PYX_ERR(0, 185, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_column_name", 1, 2, 2, 1); __PYX_ERR(0, 186, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_column_name") < 0)) __PYX_ERR(0, 185, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_column_name") < 0)) __PYX_ERR(0, 186, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_index = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_column_name", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 185, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_column_name", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 186, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_column_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_6handle_column_name(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_index);
 
@@ -4402,96 +6502,117 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":188
+/* "pyreadr/librdata.pyx":189
  *         pass
  * 
  *     def handle_dim(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_9handle_dim = {"handle_dim", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_data_type = 0;
   CYTHON_UNUSED PyObject *__pyx_v_data = 0;
   CYTHON_UNUSED PyObject *__pyx_v_count = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_dim (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_data_type,&__pyx_n_s_data,&__pyx_n_s_count,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_data_type,&__pyx_n_s_data,&__pyx_n_s_count,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data_type)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data_type)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 1); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 1); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_data)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 2); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 2); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_count)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 3); __PYX_ERR(0, 188, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, 3); __PYX_ERR(0, 189, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_dim") < 0)) __PYX_ERR(0, 188, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_dim") < 0)) __PYX_ERR(0, 189, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_name = values[0];
     __pyx_v_data_type = values[1];
     __pyx_v_data = values[2];
     __pyx_v_count = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 188, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_dim", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 189, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_dim", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_8handle_dim(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_data_type, __pyx_v_data, __pyx_v_count);
 
@@ -4508,74 +6629,93 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":191
+/* "pyreadr/librdata.pyx":192
  *         pass
  * 
  *     def handle_dim_name(self, name, index):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_11handle_dim_name = {"handle_dim_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_index = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_dim_name (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 192, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_dim_name", 1, 2, 2, 1); __PYX_ERR(0, 191, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_dim_name", 1, 2, 2, 1); __PYX_ERR(0, 192, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_dim_name") < 0)) __PYX_ERR(0, 191, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_dim_name") < 0)) __PYX_ERR(0, 192, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_index = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_dim_name", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 191, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_dim_name", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 192, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_dim_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_10handle_dim_name(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_index);
 
@@ -4592,74 +6732,93 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":194
+/* "pyreadr/librdata.pyx":195
  *         pass
  * 
  *     def _handle_row_name(self, name, index):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_13_handle_row_name = {"_handle_row_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_index = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_handle_row_name (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_handle_row_name", 1, 2, 2, 1); __PYX_ERR(0, 194, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_handle_row_name", 1, 2, 2, 1); __PYX_ERR(0, 195, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_handle_row_name") < 0)) __PYX_ERR(0, 194, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_handle_row_name") < 0)) __PYX_ERR(0, 195, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_index = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_handle_row_name", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 194, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_handle_row_name", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 195, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser._handle_row_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_12_handle_row_name(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_index);
 
@@ -4676,74 +6835,93 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":197
+/* "pyreadr/librdata.pyx":198
  *         pass
  * 
  *     def handle_text_value(self, name, index):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_15handle_text_value = {"handle_text_value", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_index = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_text_value (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_text_value", 1, 2, 2, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_text_value", 1, 2, 2, 1); __PYX_ERR(0, 198, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_text_value") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_text_value") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_index = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_text_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_text_value", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 198, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_text_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_14handle_text_value(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_index);
 
@@ -4760,74 +6938,93 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":200
+/* "pyreadr/librdata.pyx":201
  *         pass
  * 
  *     def handle_value_label(self, name, index):             # <<<<<<<<<<<<<<
  *         pass
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_17handle_value_label = {"handle_value_label", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_name = 0;
   CYTHON_UNUSED PyObject *__pyx_v_index = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("handle_value_label (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_index,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_index)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("handle_value_label", 1, 2, 2, 1); __PYX_ERR(0, 200, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("handle_value_label", 1, 2, 2, 1); __PYX_ERR(0, 201, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "handle_value_label") < 0)) __PYX_ERR(0, 200, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "handle_value_label") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_index = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("handle_value_label", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 200, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("handle_value_label", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 201, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Parser.handle_value_label", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_16handle_value_label(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v_name, __pyx_v_index);
 
@@ -4844,146 +7041,157 @@
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":203
+/* "pyreadr/librdata.pyx":204
  *         pass
  * 
- *     cdef __handle_table(self, const char* name):             # <<<<<<<<<<<<<<
+ *     cdef __handle_table(self, const char* name) noexcept:             # <<<<<<<<<<<<<<
  *         if name == NULL:
  *             self.handle_table(None)
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_table(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_table(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_table", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_table", 0);
 
-  /* "pyreadr/librdata.pyx":204
+  /* "pyreadr/librdata.pyx":205
  * 
- *     cdef __handle_table(self, const char* name):
+ *     cdef __handle_table(self, const char* name) noexcept:
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             self.handle_table(None)
  *         else:
  */
-  __pyx_t_1 = ((__pyx_v_name == NULL) != 0);
+  __pyx_t_1 = (__pyx_v_name == NULL);
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":205
- *     cdef __handle_table(self, const char* name):
+    /* "pyreadr/librdata.pyx":206
+ *     cdef __handle_table(self, const char* name) noexcept:
  *         if name == NULL:
  *             self.handle_table(None)             # <<<<<<<<<<<<<<
  *         else:
  *             self.handle_table(name)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_table); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_table); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
+    __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, Py_None) : __Pyx_PyObject_CallOneArg(__pyx_t_3, Py_None);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_4, Py_None};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pyreadr/librdata.pyx":204
+    /* "pyreadr/librdata.pyx":205
  * 
- *     cdef __handle_table(self, const char* name):
+ *     cdef __handle_table(self, const char* name) noexcept:
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             self.handle_table(None)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":207
+  /* "pyreadr/librdata.pyx":208
  *             self.handle_table(None)
  *         else:
  *             self.handle_table(name)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):
+ *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_table); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_table); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = NULL;
+    __pyx_t_6 = NULL;
+    __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_5)) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_4};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":203
+  /* "pyreadr/librdata.pyx":204
  *         pass
  * 
- *     cdef __handle_table(self, const char* name):             # <<<<<<<<<<<<<<
+ *     cdef __handle_table(self, const char* name) noexcept:             # <<<<<<<<<<<<<<
  *         if name == NULL:
  *             self.handle_table(None)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_table", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_table", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":209
+/* "pyreadr/librdata.pyx":210
  *             self.handle_table(name)
  * 
- *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):             # <<<<<<<<<<<<<<
+ *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:             # <<<<<<<<<<<<<<
  *         cdef double *doubles = <double*>data
  *         cdef int *ints = <int*>data
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_column(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_type, void *__pyx_v_data, long __pyx_v_count) {
   double *__pyx_v_doubles;
   int *__pyx_v_ints;
   PyObject *__pyx_v_array = NULL;
   long __pyx_v_i;
   PyObject *__pyx_v_new_name = NULL;
   PyObject *__pyx_v_data_type = NULL;
   PyObject *__pyx_r = NULL;
@@ -4997,1593 +7205,1570 @@
   long __pyx_t_7;
   long __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_column", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_column", 0);
 
-  /* "pyreadr/librdata.pyx":210
+  /* "pyreadr/librdata.pyx":211
  * 
- *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):
+ *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:
  *         cdef double *doubles = <double*>data             # <<<<<<<<<<<<<<
  *         cdef int *ints = <int*>data
  * 
  */
   __pyx_v_doubles = ((double *)__pyx_v_data);
 
-  /* "pyreadr/librdata.pyx":211
- *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):
+  /* "pyreadr/librdata.pyx":212
+ *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:
  *         cdef double *doubles = <double*>data
  *         cdef int *ints = <int*>data             # <<<<<<<<<<<<<<
  * 
  *         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:
  */
   __pyx_v_ints = ((int *)__pyx_v_data);
 
-  /* "pyreadr/librdata.pyx":213
+  /* "pyreadr/librdata.pyx":214
  *         cdef int *ints = <int*>data
  * 
  *         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.float64)
  *             for i in range(count):
  */
   switch (__pyx_v_type) {
     case RDATA_TYPE_REAL:
     case RDATA_TYPE_TIMESTAMP:
     case RDATA_TYPE_DATE:
 
-    /* "pyreadr/librdata.pyx":214
+    /* "pyreadr/librdata.pyx":215
  * 
  *         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:
  *             array = np.empty([count], dtype=np.float64)             # <<<<<<<<<<<<<<
  *             for i in range(count):
  *                 array[i] = doubles[i];
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 215, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_array = __pyx_t_5;
     __pyx_t_5 = 0;
 
-    /* "pyreadr/librdata.pyx":215
+    /* "pyreadr/librdata.pyx":216
  *         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:
  *             array = np.empty([count], dtype=np.float64)
  *             for i in range(count):             # <<<<<<<<<<<<<<
  *                 array[i] = doubles[i];
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:
  */
     __pyx_t_6 = __pyx_v_count;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v_i = __pyx_t_8;
 
-      /* "pyreadr/librdata.pyx":216
+      /* "pyreadr/librdata.pyx":217
  *             array = np.empty([count], dtype=np.float64)
  *             for i in range(count):
  *                 array[i] = doubles[i];             # <<<<<<<<<<<<<<
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:
  *             array = np.empty([count], dtype=np.int32)
  */
-      __pyx_t_5 = PyFloat_FromDouble((__pyx_v_doubles[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 216, __pyx_L1_error)
+      __pyx_t_5 = PyFloat_FromDouble((__pyx_v_doubles[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 217, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0)) __PYX_ERR(0, 216, __pyx_L1_error)
+      if (unlikely((__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_5, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0))) __PYX_ERR(0, 217, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
 
-    /* "pyreadr/librdata.pyx":213
+    /* "pyreadr/librdata.pyx":214
  *         cdef int *ints = <int*>data
  * 
  *         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.float64)
  *             for i in range(count):
  */
     break;
     case RDATA_TYPE_INT32:
 
-    /* "pyreadr/librdata.pyx":217
+    /* "pyreadr/librdata.pyx":218
  *             for i in range(count):
  *                 array[i] = doubles[i];
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  */
     case RDATA_TYPE_LOGICAL:
 
-    /* "pyreadr/librdata.pyx":218
+    /* "pyreadr/librdata.pyx":219
  *                 array[i] = doubles[i];
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:
  *             array = np.empty([count], dtype=np.int32)             # <<<<<<<<<<<<<<
  *             for i in range(count):
  *                 array[i] = ints[i];
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_empty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_5);
     PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_array = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "pyreadr/librdata.pyx":219
+    /* "pyreadr/librdata.pyx":220
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):             # <<<<<<<<<<<<<<
  *                 array[i] = ints[i];
  *         else:
  */
     __pyx_t_6 = __pyx_v_count;
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_v_i = __pyx_t_8;
 
-      /* "pyreadr/librdata.pyx":220
+      /* "pyreadr/librdata.pyx":221
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  *                 array[i] = ints[i];             # <<<<<<<<<<<<<<
  *         else:
  *             array = None
  */
-      __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_ints[__pyx_v_i])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int((__pyx_v_ints[__pyx_v_i])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+      if (unlikely((__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_4, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0))) __PYX_ERR(0, 221, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
 
-    /* "pyreadr/librdata.pyx":217
+    /* "pyreadr/librdata.pyx":218
  *             for i in range(count):
  *                 array[i] = doubles[i];
  *         elif type == rdata_type_t.RDATA_TYPE_INT32 or type == rdata_type_t.RDATA_TYPE_LOGICAL:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  */
     break;
     default:
 
-    /* "pyreadr/librdata.pyx":222
+    /* "pyreadr/librdata.pyx":223
  *                 array[i] = ints[i];
  *         else:
  *             array = None             # <<<<<<<<<<<<<<
  * 
  *         if name == NULL:
  */
     __Pyx_INCREF(Py_None);
     __pyx_v_array = Py_None;
     break;
   }
 
-  /* "pyreadr/librdata.pyx":224
+  /* "pyreadr/librdata.pyx":225
  *             array = None
  * 
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
-  __pyx_t_9 = ((__pyx_v_name == NULL) != 0);
+  __pyx_t_9 = (__pyx_v_name == NULL);
   if (__pyx_t_9) {
 
-    /* "pyreadr/librdata.pyx":225
+    /* "pyreadr/librdata.pyx":226
  * 
  *         if name == NULL:
  *             new_name = None             # <<<<<<<<<<<<<<
  *         else:
  *             new_name = name
  */
     __Pyx_INCREF(Py_None);
     __pyx_v_new_name = Py_None;
 
-    /* "pyreadr/librdata.pyx":224
+    /* "pyreadr/librdata.pyx":225
  *             array = None
  * 
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "pyreadr/librdata.pyx":227
+  /* "pyreadr/librdata.pyx":228
  *             new_name = None
  *         else:
  *             new_name = name             # <<<<<<<<<<<<<<
  *         data_type = DataType(type)
  *         self.handle_column(new_name, data_type, array, count)
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_new_name = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_L7:;
 
-  /* "pyreadr/librdata.pyx":228
+  /* "pyreadr/librdata.pyx":229
  *         else:
  *             new_name = name
  *         data_type = DataType(type)             # <<<<<<<<<<<<<<
  *         self.handle_column(new_name, data_type, array, count)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DataType); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyInt_From_enum__rdata_type_e(__pyx_v_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_enum__rdata_type_e(__pyx_v_type); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
+  __pyx_t_10 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
+      __pyx_t_10 = 1;
     }
   }
-  __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_5};
+    __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  }
   __pyx_v_data_type = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pyreadr/librdata.pyx":229
+  /* "pyreadr/librdata.pyx":230
  *             new_name = name
  *         data_type = DataType(type)
  *         self.handle_column(new_name, data_type, array, count)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_column_name(self, const char *name, int index):
+ *     cdef __handle_column_name(self, const char *name, int index) noexcept:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_column); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_column); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   __pyx_t_10 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_1, function);
       __pyx_t_10 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_3, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_5};
-    __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_1)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_3, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_5};
-    __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_1, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[5] = {__pyx_t_3, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_5};
+    __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_10, 4+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_2 = PyTuple_New(4+__pyx_t_10); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (__pyx_t_3) {
-      __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3); __pyx_t_3 = NULL;
-    }
-    __Pyx_INCREF(__pyx_v_new_name);
-    __Pyx_GIVEREF(__pyx_v_new_name);
-    PyTuple_SET_ITEM(__pyx_t_2, 0+__pyx_t_10, __pyx_v_new_name);
-    __Pyx_INCREF(__pyx_v_data_type);
-    __Pyx_GIVEREF(__pyx_v_data_type);
-    PyTuple_SET_ITEM(__pyx_t_2, 1+__pyx_t_10, __pyx_v_data_type);
-    __Pyx_INCREF(__pyx_v_array);
-    __Pyx_GIVEREF(__pyx_v_array);
-    PyTuple_SET_ITEM(__pyx_t_2, 2+__pyx_t_10, __pyx_v_array);
-    __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_2, 3+__pyx_t_10, __pyx_t_5);
-    __pyx_t_5 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pyreadr/librdata.pyx":209
+  /* "pyreadr/librdata.pyx":210
  *             self.handle_table(name)
  * 
- *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):             # <<<<<<<<<<<<<<
+ *     cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:             # <<<<<<<<<<<<<<
  *         cdef double *doubles = <double*>data
  *         cdef int *ints = <int*>data
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_column", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_column", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_array);
   __Pyx_XDECREF(__pyx_v_new_name);
   __Pyx_XDECREF(__pyx_v_data_type);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":231
+/* "pyreadr/librdata.pyx":232
  *         self.handle_column(new_name, data_type, array, count)
  * 
- *     cdef __handle_column_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_column_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_column_name(name, index)
  * 
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_column_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_column_name", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_column_name", 0);
 
-  /* "pyreadr/librdata.pyx":232
+  /* "pyreadr/librdata.pyx":233
  * 
- *     cdef __handle_column_name(self, const char *name, int index):
+ *     cdef __handle_column_name(self, const char *name, int index) noexcept:
  *         self.handle_column_name(name, index)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count):
+ *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count) noexcept:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_column_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_column_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 232, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-    }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-    __pyx_t_3 = 0;
-    __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":231
+  /* "pyreadr/librdata.pyx":232
  *         self.handle_column(new_name, data_type, array, count)
  * 
- *     cdef __handle_column_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_column_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_column_name(name, index)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_column_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_column_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":234
+/* "pyreadr/librdata.pyx":235
  *         self.handle_column_name(name, index)
  * 
- *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count):             # <<<<<<<<<<<<<<
+ *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count) noexcept:             # <<<<<<<<<<<<<<
  *         cdef int *ints = <int*>data
  * 
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_dim(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_datatype, void *__pyx_v_data, long __pyx_v_count) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, enum rdata_type_e __pyx_v_datatype, void *__pyx_v_data, long __pyx_v_count) {
   int *__pyx_v_ints;
   PyObject *__pyx_v_data_type = NULL;
   PyObject *__pyx_v_array = NULL;
   long __pyx_v_i;
   PyObject *__pyx_v_new_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
-  long __pyx_t_7;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
   long __pyx_t_8;
   long __pyx_t_9;
-  int __pyx_t_10;
+  long __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_dim", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_dim", 0);
 
-  /* "pyreadr/librdata.pyx":235
+  /* "pyreadr/librdata.pyx":236
  * 
- *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count):
+ *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count) noexcept:
  *         cdef int *ints = <int*>data             # <<<<<<<<<<<<<<
  * 
  *         data_type = DataType(datatype)
  */
   __pyx_v_ints = ((int *)__pyx_v_data);
 
-  /* "pyreadr/librdata.pyx":237
+  /* "pyreadr/librdata.pyx":238
  *         cdef int *ints = <int*>data
  * 
  *         data_type = DataType(datatype)             # <<<<<<<<<<<<<<
  *         if datatype == rdata_type_t.RDATA_TYPE_INT32:
  *             array = np.empty([count], dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_DataType); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(__pyx_v_datatype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(__pyx_v_datatype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 238, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_5 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
   __pyx_v_data_type = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":238
+  /* "pyreadr/librdata.pyx":239
  * 
  *         data_type = DataType(datatype)
  *         if datatype == rdata_type_t.RDATA_TYPE_INT32:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  */
-  __pyx_t_5 = ((__pyx_v_datatype == RDATA_TYPE_INT32) != 0);
-  if (likely(__pyx_t_5)) {
+  __pyx_t_6 = (__pyx_v_datatype == RDATA_TYPE_INT32);
+  if (likely(__pyx_t_6)) {
 
-    /* "pyreadr/librdata.pyx":239
+    /* "pyreadr/librdata.pyx":240
  *         data_type = DataType(datatype)
  *         if datatype == rdata_type_t.RDATA_TYPE_INT32:
  *             array = np.empty([count], dtype=np.int32)             # <<<<<<<<<<<<<<
  *             for i in range(count):
  *                 array[i] = ints[i];
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_1);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 239, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_7) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_v_array = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_v_array = __pyx_t_7;
+    __pyx_t_7 = 0;
 
-    /* "pyreadr/librdata.pyx":240
+    /* "pyreadr/librdata.pyx":241
  *         if datatype == rdata_type_t.RDATA_TYPE_INT32:
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):             # <<<<<<<<<<<<<<
  *                 array[i] = ints[i];
  *         else:
  */
-    __pyx_t_7 = __pyx_v_count;
-    __pyx_t_8 = __pyx_t_7;
-    for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
-      __pyx_v_i = __pyx_t_9;
+    __pyx_t_8 = __pyx_v_count;
+    __pyx_t_9 = __pyx_t_8;
+    for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
+      __pyx_v_i = __pyx_t_10;
 
-      /* "pyreadr/librdata.pyx":241
+      /* "pyreadr/librdata.pyx":242
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  *                 array[i] = ints[i];             # <<<<<<<<<<<<<<
  *         else:
  *             raise PyreadrError('Wrong data type %s for dimensions.' % str(data_type))
  */
-      __pyx_t_6 = __Pyx_PyInt_From_int((__pyx_v_ints[__pyx_v_i])); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 241, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0)) __PYX_ERR(0, 241, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_7 = __Pyx_PyInt_From_int((__pyx_v_ints[__pyx_v_i])); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 242, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (unlikely((__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_7, long, 1, __Pyx_PyInt_From_long, 0, 1, 1) < 0))) __PYX_ERR(0, 242, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
 
-    /* "pyreadr/librdata.pyx":238
+    /* "pyreadr/librdata.pyx":239
  * 
  *         data_type = DataType(datatype)
  *         if datatype == rdata_type_t.RDATA_TYPE_INT32:             # <<<<<<<<<<<<<<
  *             array = np.empty([count], dtype=np.int32)
  *             for i in range(count):
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":243
+  /* "pyreadr/librdata.pyx":244
  *                 array[i] = ints[i];
  *         else:
  *             raise PyreadrError('Wrong data type %s for dimensions.' % str(data_type))             # <<<<<<<<<<<<<<
  * 
  *         if name == NULL:
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_data_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Str(__pyx_v_data_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyUnicode_Format(__pyx_kp_u_Wrong_data_type_s_for_dimensions, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Wrong_data_type_s_for_dimensions, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = NULL;
+    __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_1)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_1);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
       }
     }
-    __pyx_t_6 = (__pyx_t_1) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_1, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 243, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_Raise(__pyx_t_6, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 243, __pyx_L1_error)
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_2};
+      __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 244, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
+    __Pyx_Raise(__pyx_t_7, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __PYX_ERR(0, 244, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":245
+  /* "pyreadr/librdata.pyx":246
  *             raise PyreadrError('Wrong data type %s for dimensions.' % str(data_type))
  * 
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
-  __pyx_t_5 = ((__pyx_v_name == NULL) != 0);
-  if (__pyx_t_5) {
+  __pyx_t_6 = (__pyx_v_name == NULL);
+  if (__pyx_t_6) {
 
-    /* "pyreadr/librdata.pyx":246
+    /* "pyreadr/librdata.pyx":247
  * 
  *         if name == NULL:
  *             new_name = None             # <<<<<<<<<<<<<<
  *         else:
  *             new_name = name
  */
     __Pyx_INCREF(Py_None);
     __pyx_v_new_name = Py_None;
 
-    /* "pyreadr/librdata.pyx":245
+    /* "pyreadr/librdata.pyx":246
  *             raise PyreadrError('Wrong data type %s for dimensions.' % str(data_type))
  * 
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "pyreadr/librdata.pyx":248
+  /* "pyreadr/librdata.pyx":249
  *             new_name = None
  *         else:
  *             new_name = name             # <<<<<<<<<<<<<<
  *         self.handle_dim(new_name, data_type, array, count)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 248, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_v_new_name = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_7 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 249, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_v_new_name = __pyx_t_7;
+    __pyx_t_7 = 0;
   }
   __pyx_L6:;
 
-  /* "pyreadr/librdata.pyx":249
+  /* "pyreadr/librdata.pyx":250
  *         else:
  *             new_name = name
  *         self.handle_dim(new_name, data_type, array, count)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_dim_name(self, const char *name, int index):
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v_count); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
-  __pyx_t_10 = 0;
+  __pyx_t_5 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_10 = 1;
+      __pyx_t_5 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_1, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_2};
-    __pyx_t_6 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_1, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_2};
-    __pyx_t_6 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 4+__pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[5] = {__pyx_t_1, __pyx_v_new_name, __pyx_v_data_type, __pyx_v_array, __pyx_t_2};
+    __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 4+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_4 = PyTuple_New(4+__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 249, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    if (__pyx_t_1) {
-      __Pyx_GIVEREF(__pyx_t_1); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1); __pyx_t_1 = NULL;
-    }
-    __Pyx_INCREF(__pyx_v_new_name);
-    __Pyx_GIVEREF(__pyx_v_new_name);
-    PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_10, __pyx_v_new_name);
-    __Pyx_INCREF(__pyx_v_data_type);
-    __Pyx_GIVEREF(__pyx_v_data_type);
-    PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_10, __pyx_v_data_type);
-    __Pyx_INCREF(__pyx_v_array);
-    __Pyx_GIVEREF(__pyx_v_array);
-    PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_10, __pyx_v_array);
-    __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_4, 3+__pyx_t_10, __pyx_t_2);
-    __pyx_t_2 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 249, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pyreadr/librdata.pyx":234
+  /* "pyreadr/librdata.pyx":235
  *         self.handle_column_name(name, index)
  * 
- *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count):             # <<<<<<<<<<<<<<
+ *     cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count) noexcept:             # <<<<<<<<<<<<<<
  *         cdef int *ints = <int*>data
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_dim", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_dim", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data_type);
   __Pyx_XDECREF(__pyx_v_array);
   __Pyx_XDECREF(__pyx_v_new_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":251
+/* "pyreadr/librdata.pyx":252
  *         self.handle_dim(new_name, data_type, array, count)
  * 
- *     cdef __handle_dim_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         if name == NULL:
  *             new_name = None
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_dim_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
   PyObject *__pyx_v_new_name = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_dim_name", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_dim_name", 0);
 
-  /* "pyreadr/librdata.pyx":252
+  /* "pyreadr/librdata.pyx":253
  * 
- *     cdef __handle_dim_name(self, const char *name, int index):
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
-  __pyx_t_1 = ((__pyx_v_name == NULL) != 0);
+  __pyx_t_1 = (__pyx_v_name == NULL);
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":253
- *     cdef __handle_dim_name(self, const char *name, int index):
+    /* "pyreadr/librdata.pyx":254
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:
  *         if name == NULL:
  *             new_name = None             # <<<<<<<<<<<<<<
  *         else:
  *             new_name = name
  */
     __Pyx_INCREF(Py_None);
     __pyx_v_new_name = Py_None;
 
-    /* "pyreadr/librdata.pyx":252
+    /* "pyreadr/librdata.pyx":253
  * 
- *     cdef __handle_dim_name(self, const char *name, int index):
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:
  *         if name == NULL:             # <<<<<<<<<<<<<<
  *             new_name = None
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":255
+  /* "pyreadr/librdata.pyx":256
  *             new_name = None
  *         else:
  *             new_name = name             # <<<<<<<<<<<<<<
  *         self.handle_dim_name(new_name, index)
  * 
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_new_name = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":256
+  /* "pyreadr/librdata.pyx":257
  *         else:
  *             new_name = name
  *         self.handle_dim_name(new_name, index)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_row_name(self, const char *name, int index):
+ *     cdef __handle_row_name(self, const char *name, int index) noexcept:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_dim_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_dim_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_new_name, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_v_new_name, __pyx_t_4};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_v_new_name, __pyx_t_4};
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 256, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-    }
-    __Pyx_INCREF(__pyx_v_new_name);
-    __Pyx_GIVEREF(__pyx_v_new_name);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_new_name);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 256, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyreadr/librdata.pyx":251
+  /* "pyreadr/librdata.pyx":252
  *         self.handle_dim(new_name, data_type, array, count)
  * 
- *     cdef __handle_dim_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_dim_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         if name == NULL:
  *             new_name = None
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_dim_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_dim_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_new_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":258
+/* "pyreadr/librdata.pyx":259
  *         self.handle_dim_name(new_name, index)
  * 
- *     cdef __handle_row_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_row_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_row_name(name, index)
  * 
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_row_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_row_name(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_name, int __pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_row_name", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_row_name", 0);
 
-  /* "pyreadr/librdata.pyx":259
+  /* "pyreadr/librdata.pyx":260
  * 
- *     cdef __handle_row_name(self, const char *name, int index):
+ *     cdef __handle_row_name(self, const char *name, int index) noexcept:
  *         self.handle_row_name(name, index)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_text_value(self, const char *value, int index):
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_row_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_row_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 259, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-    }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-    __pyx_t_3 = 0;
-    __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":258
+  /* "pyreadr/librdata.pyx":259
  *         self.handle_dim_name(new_name, index)
  * 
- *     cdef __handle_row_name(self, const char *name, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_row_name(self, const char *name, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_row_name(name, index)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_row_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_row_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":261
+/* "pyreadr/librdata.pyx":262
  *         self.handle_row_name(name, index)
  * 
- *     cdef __handle_text_value(self, const char *value, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:             # <<<<<<<<<<<<<<
  *         if value != NULL:
  *             self.handle_text_value(value, index)
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_text_value(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_text_value(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_text_value", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_text_value", 0);
 
-  /* "pyreadr/librdata.pyx":262
+  /* "pyreadr/librdata.pyx":263
  * 
- *     cdef __handle_text_value(self, const char *value, int index):
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:
  *         if value != NULL:             # <<<<<<<<<<<<<<
  *             self.handle_text_value(value, index)
  *         else:
  */
-  __pyx_t_1 = ((__pyx_v_value != NULL) != 0);
+  __pyx_t_1 = (__pyx_v_value != NULL);
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":263
- *     cdef __handle_text_value(self, const char *value, int index):
+    /* "pyreadr/librdata.pyx":264
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:
  *         if value != NULL:
  *             self.handle_text_value(value, index)             # <<<<<<<<<<<<<<
  *         else:
  *             self.handle_text_value(np.nan, index)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_text_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_text_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyStr_FromString(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 264, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
+    {
+      PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 264, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    } else
-    #endif
-    {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 263, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      if (__pyx_t_6) {
-        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
-      }
-      __Pyx_GIVEREF(__pyx_t_4);
-      PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_4);
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_5);
-      __pyx_t_4 = 0;
-      __pyx_t_5 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 263, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pyreadr/librdata.pyx":262
+    /* "pyreadr/librdata.pyx":263
  * 
- *     cdef __handle_text_value(self, const char *value, int index):
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:
  *         if value != NULL:             # <<<<<<<<<<<<<<
  *             self.handle_text_value(value, index)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":265
+  /* "pyreadr/librdata.pyx":266
  *             self.handle_text_value(value, index)
  *         else:
  *             self.handle_text_value(np.nan, index)             # <<<<<<<<<<<<<<
  * 
- *     cdef __handle_value_label(self, const char *value, int index):
+ *     cdef __handle_value_label(self, const char *value, int index) noexcept:
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_text_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_text_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_nan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 265, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_4 = NULL;
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_nan); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
+      if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_t_8};
-      __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    } else
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_5, __pyx_t_8};
-      __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    } else
-    #endif
     {
-      __pyx_t_6 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4); __pyx_t_4 = NULL;
-      }
-      __Pyx_GIVEREF(__pyx_t_5);
-      PyTuple_SET_ITEM(__pyx_t_6, 0+__pyx_t_7, __pyx_t_5);
-      __Pyx_GIVEREF(__pyx_t_8);
-      PyTuple_SET_ITEM(__pyx_t_6, 1+__pyx_t_7, __pyx_t_8);
-      __pyx_t_5 = 0;
-      __pyx_t_8 = 0;
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 265, __pyx_L1_error)
+      PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_4, __pyx_t_5};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 266, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":261
+  /* "pyreadr/librdata.pyx":262
  *         self.handle_row_name(name, index)
  * 
- *     cdef __handle_text_value(self, const char *value, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_text_value(self, const char *value, int index) noexcept:             # <<<<<<<<<<<<<<
  *         if value != NULL:
  *             self.handle_text_value(value, index)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_text_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_text_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":267
+/* "pyreadr/librdata.pyx":268
  *             self.handle_text_value(np.nan, index)
  * 
- *     cdef __handle_value_label(self, const char *value, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_value_label(self, const char *value, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_value_label(value, index)
  * 
  */
 
-static PyObject *__pyx_f_7pyreadr_8librdata_6Parser___handle_value_label(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index) {
+static PyObject *__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_value_label(struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, char const *__pyx_v_value, int __pyx_v_index) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
-  PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__handle_value_label", 0);
+  __Pyx_RefNannySetupContext("_Parser__handle_value_label", 0);
 
-  /* "pyreadr/librdata.pyx":268
+  /* "pyreadr/librdata.pyx":269
  * 
- *     cdef __handle_value_label(self, const char *value, int index):
+ *     cdef __handle_value_label(self, const char *value, int index) noexcept:
  *         self.handle_value_label(value, index)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_value_label); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_handle_value_label); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyStr_FromString(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
-  #if CYTHON_FAST_PYCALL
-  if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  #if CYTHON_FAST_PYCCALL
-  if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_3, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  } else
-  #endif
-  {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 268, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    if (__pyx_t_5) {
-      __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5); __pyx_t_5 = NULL;
-    }
-    __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_t_3);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
-    __pyx_t_3 = 0;
-    __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":267
+  /* "pyreadr/librdata.pyx":268
  *             self.handle_text_value(np.nan, index)
  * 
- *     cdef __handle_value_label(self, const char *value, int index):             # <<<<<<<<<<<<<<
+ *     cdef __handle_value_label(self, const char *value, int index) noexcept:             # <<<<<<<<<<<<<<
  *         self.handle_value_label(value, index)
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("pyreadr.librdata.Parser.__handle_value_label", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("pyreadr.librdata.Parser._Parser__handle_value_label", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_19__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_18__reduce_cython__(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__this_cannot_be_converted_t, 0, 0);
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Parser.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Parser_21__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_20__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v___pyx_state = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Parser.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Parser_20__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Parser *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Parser_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Parser *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__this_cannot_be_converted_t, 0, 0);
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Parser.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":271
+/* "pyreadr/librdata.pyx":272
  * 
  * 
- * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int fd = deref(<int*>ctx)
- *     IF UNAME_SYSNAME == 'Windows':
+ *     if platform.system() == 'Windows':
  */
 
 static Py_ssize_t __pyx_f_7pyreadr_8librdata__handle_write(void const *__pyx_v_data, size_t __pyx_v_len, void *__pyx_v_ctx) {
   int __pyx_v_fd;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_handle_write", 0);
 
-  /* "pyreadr/librdata.pyx":272
+  /* "pyreadr/librdata.pyx":273
  * 
- * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx):
+ * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:
  *     cdef int fd = deref(<int*>ctx)             # <<<<<<<<<<<<<<
- *     IF UNAME_SYSNAME == 'Windows':
+ *     if platform.system() == 'Windows':
  *         return _write(fd, data, len)
  */
   __pyx_v_fd = (*((int *)__pyx_v_ctx));
 
-  /* "pyreadr/librdata.pyx":276
+  /* "pyreadr/librdata.pyx":274
+ * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:
+ *     cdef int fd = deref(<int*>ctx)
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
  *         return _write(fd, data, len)
- *     ELSE:
+ *     else:
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_platform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_system); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = NULL;
+  __pyx_t_4 = 0;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+    __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_2)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      __Pyx_INCREF(__pyx_t_2);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_4 = 1;
+    }
+  }
+  {
+    PyObject *__pyx_callargs[1] = {__pyx_t_2, };
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_n_u_Windows, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__pyx_t_5) {
+
+    /* "pyreadr/librdata.pyx":275
+ *     cdef int fd = deref(<int*>ctx)
+ *     if platform.system() == 'Windows':
+ *         return _write(fd, data, len)             # <<<<<<<<<<<<<<
+ *     else:
+ *         return write(fd, data, len)
+ */
+    __pyx_r = _write(__pyx_v_fd, __pyx_v_data, __pyx_v_len);
+    goto __pyx_L0;
+
+    /* "pyreadr/librdata.pyx":274
+ * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:
+ *     cdef int fd = deref(<int*>ctx)
+ *     if platform.system() == 'Windows':             # <<<<<<<<<<<<<<
+ *         return _write(fd, data, len)
+ *     else:
+ */
+  }
+
+  /* "pyreadr/librdata.pyx":277
+ *         return _write(fd, data, len)
+ *     else:
  *         return write(fd, data, len)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_r = write(__pyx_v_fd, __pyx_v_data, __pyx_v_len);
-  goto __pyx_L0;
+  /*else*/ {
+    __pyx_r = write(__pyx_v_fd, __pyx_v_data, __pyx_v_len);
+    goto __pyx_L0;
+  }
 
-  /* "pyreadr/librdata.pyx":271
+  /* "pyreadr/librdata.pyx":272
  * 
  * 
- * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx):             # <<<<<<<<<<<<<<
+ * cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int fd = deref(<int*>ctx)
- *     IF UNAME_SYSNAME == 'Windows':
+ *     if platform.system() == 'Windows':
  */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_WriteUnraisable("pyreadr.librdata._handle_write", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":282
+/* "pyreadr/librdata.pyx":283
  *     cdef rdata_column_t *_this
  * 
  *     def add_level_labels(self, labels):             # <<<<<<<<<<<<<<
  *         for label in labels:
  *             rdata_column_add_factor(self._this, label.encode('utf-8'))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels(PyObject *__pyx_v_self, PyObject *__pyx_v_labels); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels(PyObject *__pyx_v_self, PyObject *__pyx_v_labels) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Column_1add_level_labels = {"add_level_labels", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_labels = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_level_labels (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Column_add_level_labels(((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_v_self), ((PyObject *)__pyx_v_labels));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_labels,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_labels)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "add_level_labels") < 0)) __PYX_ERR(0, 283, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_labels = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("add_level_labels", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 283, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Column.add_level_labels", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Column_add_level_labels(((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_v_self), __pyx_v_labels);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Column_add_level_labels(struct __pyx_obj_7pyreadr_8librdata_Column *__pyx_v_self, PyObject *__pyx_v_labels) {
@@ -6592,108 +8777,114 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   PyObject *(*__pyx_t_3)(PyObject *);
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  char const *__pyx_t_7;
+  int __pyx_t_7;
+  char const *__pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_level_labels", 0);
 
-  /* "pyreadr/librdata.pyx":283
+  /* "pyreadr/librdata.pyx":284
  * 
  *     def add_level_labels(self, labels):
  *         for label in labels:             # <<<<<<<<<<<<<<
  *             rdata_column_add_factor(self._this, label.encode('utf-8'))
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_labels)) || PyTuple_CheckExact(__pyx_v_labels)) {
     __pyx_t_1 = __pyx_v_labels; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 283, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_labels); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 283, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 284, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 284, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 283, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 284, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 283, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 283, __pyx_L1_error)
+          else __PYX_ERR(0, 284, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_label, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "pyreadr/librdata.pyx":284
+    /* "pyreadr/librdata.pyx":285
  *     def add_level_labels(self, labels):
  *         for label in labels:
  *             rdata_column_add_factor(self._this, label.encode('utf-8'))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_label, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 284, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_label, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 285, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
+    __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
       }
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 284, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 284, __pyx_L1_error)
-    (void)(rdata_column_add_factor(__pyx_v_self->_this, __pyx_t_7));
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_kp_u_utf_8};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 285, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __pyx_t_8 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+    (void)(rdata_column_add_factor(__pyx_v_self->_this, __pyx_t_8));
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pyreadr/librdata.pyx":283
+    /* "pyreadr/librdata.pyx":284
  * 
  *     def add_level_labels(self, labels):
  *         for label in labels:             # <<<<<<<<<<<<<<
  *             rdata_column_add_factor(self._this, label.encode('utf-8'))
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":282
+  /* "pyreadr/librdata.pyx":283
  *     cdef rdata_column_t *_this
  * 
  *     def add_level_labels(self, labels):             # <<<<<<<<<<<<<<
  *         for label in labels:
  *             rdata_column_add_factor(self._this, label.encode('utf-8'))
  */
 
@@ -6712,303 +8903,392 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Column_3__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Column_2__reduce_cython__(((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Column_2__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Column *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__this_cannot_be_converted_t, 0, 0);
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Column.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Column_5__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Column_4__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v___pyx_state = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Column.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Column_4__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Column_4__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Column *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__this_cannot_be_converted_t, 0, 0);
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Column.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":297
+/* "pyreadr/librdata.pyx":298
  *     cdef bytes _table_name
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self._format = None
  *         self._row_count = 0
  */
 
 /* Python wrapper */
 static int __pyx_pw_7pyreadr_8librdata_6Writer_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pyreadr_8librdata_6Writer_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
-  if (unlikely(PyTuple_GET_SIZE(__pyx_args) > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__init__", 1, 0, 0, PyTuple_GET_SIZE(__pyx_args)); return -1;}
-  if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__init__", 0))) return -1;
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__init__", 1, 0, 0, __pyx_nargs); return -1;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_VARARGS(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__init__", 0))) return -1;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer___init__(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_pf_7pyreadr_8librdata_6Writer___init__(struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "pyreadr/librdata.pyx":298
+  /* "pyreadr/librdata.pyx":299
  * 
  *     def __init__(self):
  *         self._format = None             # <<<<<<<<<<<<<<
  *         self._row_count = 0
  *         self._writer = NULL
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = Py_None;
 
-  /* "pyreadr/librdata.pyx":299
+  /* "pyreadr/librdata.pyx":300
  *     def __init__(self):
  *         self._format = None
  *         self._row_count = 0             # <<<<<<<<<<<<<<
  *         self._writer = NULL
  *         self._fd = 0
  */
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   __Pyx_GOTREF(__pyx_v_self->_row_count);
   __Pyx_DECREF(__pyx_v_self->_row_count);
   __pyx_v_self->_row_count = __pyx_int_0;
 
-  /* "pyreadr/librdata.pyx":300
+  /* "pyreadr/librdata.pyx":301
  *         self._format = None
  *         self._row_count = 0
  *         self._writer = NULL             # <<<<<<<<<<<<<<
  *         self._fd = 0
  *         self._current_column_no = -1
  */
   __pyx_v_self->_writer = NULL;
 
-  /* "pyreadr/librdata.pyx":301
+  /* "pyreadr/librdata.pyx":302
  *         self._row_count = 0
  *         self._writer = NULL
  *         self._fd = 0             # <<<<<<<<<<<<<<
  *         self._current_column_no = -1
  *         self._current_column = NULL
  */
   __pyx_v_self->_fd = 0;
 
-  /* "pyreadr/librdata.pyx":302
+  /* "pyreadr/librdata.pyx":303
  *         self._writer = NULL
  *         self._fd = 0
  *         self._current_column_no = -1             # <<<<<<<<<<<<<<
  *         self._current_column = NULL
  *         self._table_name = b""
  */
   __pyx_v_self->_current_column_no = -1;
 
-  /* "pyreadr/librdata.pyx":303
+  /* "pyreadr/librdata.pyx":304
  *         self._fd = 0
  *         self._current_column_no = -1
  *         self._current_column = NULL             # <<<<<<<<<<<<<<
  *         self._table_name = b""
  * 
  */
   __pyx_v_self->_current_column = NULL;
 
-  /* "pyreadr/librdata.pyx":304
+  /* "pyreadr/librdata.pyx":305
  *         self._current_column_no = -1
  *         self._current_column = NULL
  *         self._table_name = b""             # <<<<<<<<<<<<<<
  * 
  *     def open(self, path, format):
  */
-  __Pyx_INCREF(__pyx_kp_b__5);
-  __Pyx_GIVEREF(__pyx_kp_b__5);
+  __Pyx_INCREF(__pyx_kp_b_);
+  __Pyx_GIVEREF(__pyx_kp_b_);
   __Pyx_GOTREF(__pyx_v_self->_table_name);
   __Pyx_DECREF(__pyx_v_self->_table_name);
-  __pyx_v_self->_table_name = __pyx_kp_b__5;
+  __pyx_v_self->_table_name = __pyx_kp_b_;
 
-  /* "pyreadr/librdata.pyx":297
+  /* "pyreadr/librdata.pyx":298
  *     cdef bytes _table_name
  * 
  *     def __init__(self):             # <<<<<<<<<<<<<<
  *         self._format = None
  *         self._row_count = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":306
+/* "pyreadr/librdata.pyx":307
  *         self._table_name = b""
  * 
  *     def open(self, path, format):             # <<<<<<<<<<<<<<
  *         cdef rdata_file_format_t fmt;
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_3open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_3open(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_3open(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_3open = {"open", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_3open, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_3open(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_path = 0;
   PyObject *__pyx_v_format = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("open (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_path,&__pyx_n_s_format,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_path,&__pyx_n_s_format,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_path)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_path)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 307, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_format)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 307, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("open", 1, 2, 2, 1); __PYX_ERR(0, 306, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("open", 1, 2, 2, 1); __PYX_ERR(0, 307, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 306, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "open") < 0)) __PYX_ERR(0, 307, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_path = values[0];
     __pyx_v_format = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 306, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 307, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Writer.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_2open(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v_path, __pyx_v_format);
 
@@ -7021,127 +9301,133 @@
   rdata_file_format_t __pyx_v_fmt;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
 
-  /* "pyreadr/librdata.pyx":309
+  /* "pyreadr/librdata.pyx":310
  *         cdef rdata_file_format_t fmt;
  * 
  *         if format == 'rds':             # <<<<<<<<<<<<<<
  *             fmt = RDATA_SINGLE_OBJECT
  *         elif format == 'rdata':
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_format, __pyx_n_u_rds, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_format, __pyx_n_u_rds, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 310, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":310
+    /* "pyreadr/librdata.pyx":311
  * 
  *         if format == 'rds':
  *             fmt = RDATA_SINGLE_OBJECT             # <<<<<<<<<<<<<<
  *         elif format == 'rdata':
  *             fmt = RDATA_WORKSPACE
  */
     __pyx_v_fmt = RDATA_SINGLE_OBJECT;
 
-    /* "pyreadr/librdata.pyx":309
+    /* "pyreadr/librdata.pyx":310
  *         cdef rdata_file_format_t fmt;
  * 
  *         if format == 'rds':             # <<<<<<<<<<<<<<
  *             fmt = RDATA_SINGLE_OBJECT
  *         elif format == 'rdata':
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":311
+  /* "pyreadr/librdata.pyx":312
  *         if format == 'rds':
  *             fmt = RDATA_SINGLE_OBJECT
  *         elif format == 'rdata':             # <<<<<<<<<<<<<<
  *             fmt = RDATA_WORKSPACE
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_format, __pyx_n_u_rdata, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 311, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_format, __pyx_n_u_rdata, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 312, __pyx_L1_error)
   if (likely(__pyx_t_1)) {
 
-    /* "pyreadr/librdata.pyx":312
+    /* "pyreadr/librdata.pyx":313
  *             fmt = RDATA_SINGLE_OBJECT
  *         elif format == 'rdata':
  *             fmt = RDATA_WORKSPACE             # <<<<<<<<<<<<<<
  *         else:
  *             raise PyreadrError('Unsupported format')
  */
     __pyx_v_fmt = RDATA_WORKSPACE;
 
-    /* "pyreadr/librdata.pyx":311
+    /* "pyreadr/librdata.pyx":312
  *         if format == 'rds':
  *             fmt = RDATA_SINGLE_OBJECT
  *         elif format == 'rdata':             # <<<<<<<<<<<<<<
  *             fmt = RDATA_WORKSPACE
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":314
+  /* "pyreadr/librdata.pyx":315
  *             fmt = RDATA_WORKSPACE
  *         else:
  *             raise PyreadrError('Unsupported format')             # <<<<<<<<<<<<<<
  * 
  *         self._writer = rdata_writer_init(_handle_write, fmt)
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
+    __pyx_t_5 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_5 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_Unsupported_format) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_Unsupported_format);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_Unsupported_format};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 314, __pyx_L1_error)
+    __PYX_ERR(0, 315, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":316
+  /* "pyreadr/librdata.pyx":317
  *             raise PyreadrError('Unsupported format')
  * 
  *         self._writer = rdata_writer_init(_handle_write, fmt)             # <<<<<<<<<<<<<<
  *         self._fd = _os_open(path, 'w')
  * 
  */
   __pyx_v_self->_writer = rdata_writer_init(__pyx_f_7pyreadr_8librdata__handle_write, __pyx_v_fmt);
 
-  /* "pyreadr/librdata.pyx":317
+  /* "pyreadr/librdata.pyx":318
  * 
  *         self._writer = rdata_writer_init(_handle_write, fmt)
  *         self._fd = _os_open(path, 'w')             # <<<<<<<<<<<<<<
  * 
  *     def set_row_count(self, row_count):
  */
   __pyx_v_self->_fd = __pyx_f_7pyreadr_8librdata__os_open(__pyx_v_path, __pyx_n_u_w);
 
-  /* "pyreadr/librdata.pyx":306
+  /* "pyreadr/librdata.pyx":307
  *         self._table_name = b""
  * 
  *     def open(self, path, format):             # <<<<<<<<<<<<<<
  *         cdef rdata_file_format_t fmt;
  * 
  */
 
@@ -7156,132 +9442,254 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":319
+/* "pyreadr/librdata.pyx":320
  *         self._fd = _os_open(path, 'w')
  * 
  *     def set_row_count(self, row_count):             # <<<<<<<<<<<<<<
  *         self._row_count = row_count
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count(PyObject *__pyx_v_self, PyObject *__pyx_v_row_count); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count(PyObject *__pyx_v_self, PyObject *__pyx_v_row_count) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_5set_row_count = {"set_row_count", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_row_count = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_row_count (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_4set_row_count(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), ((PyObject *)__pyx_v_row_count));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_row_count,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_row_count)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 320, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_row_count") < 0)) __PYX_ERR(0, 320, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_row_count = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("set_row_count", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 320, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Writer.set_row_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_4set_row_count(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v_row_count);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_4set_row_count(struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, PyObject *__pyx_v_row_count) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_row_count", 0);
 
-  /* "pyreadr/librdata.pyx":320
+  /* "pyreadr/librdata.pyx":321
  * 
  *     def set_row_count(self, row_count):
  *         self._row_count = row_count             # <<<<<<<<<<<<<<
  * 
  *     def set_table_name(self, name):
  */
   __Pyx_INCREF(__pyx_v_row_count);
   __Pyx_GIVEREF(__pyx_v_row_count);
   __Pyx_GOTREF(__pyx_v_self->_row_count);
   __Pyx_DECREF(__pyx_v_self->_row_count);
   __pyx_v_self->_row_count = __pyx_v_row_count;
 
-  /* "pyreadr/librdata.pyx":319
+  /* "pyreadr/librdata.pyx":320
  *         self._fd = _os_open(path, 'w')
  * 
  *     def set_row_count(self, row_count):             # <<<<<<<<<<<<<<
  *         self._row_count = row_count
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":322
+/* "pyreadr/librdata.pyx":323
  *         self._row_count = row_count
  * 
  *     def set_table_name(self, name):             # <<<<<<<<<<<<<<
  *         self._table_name = name.encode("utf-8")
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_7set_table_name = {"set_table_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_name = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_table_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_6set_table_name(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), ((PyObject *)__pyx_v_name));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "set_table_name") < 0)) __PYX_ERR(0, 323, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_name = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("set_table_name", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 323, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Writer.set_table_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_6set_table_name(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_6set_table_name(struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_table_name", 0);
 
-  /* "pyreadr/librdata.pyx":323
+  /* "pyreadr/librdata.pyx":324
  * 
  *     def set_table_name(self, name):
  *         self._table_name = name.encode("utf-8")             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
+  __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_4 = 1;
     }
   }
-  __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
-  __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 323, __pyx_L1_error)
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 324, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_t_1))) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_table_name);
   __Pyx_DECREF(__pyx_v_self->_table_name);
   __pyx_v_self->_table_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":322
+  /* "pyreadr/librdata.pyx":323
  *         self._row_count = row_count
  * 
  *     def set_table_name(self, name):             # <<<<<<<<<<<<<<
  *         self._table_name = name.encode("utf-8")
  * 
  */
 
@@ -7296,28 +9704,48 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":325
+/* "pyreadr/librdata.pyx":326
  *         self._table_name = name.encode("utf-8")
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         if self._writer != NULL:
  *             if self._current_column_no != -1:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_9close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_9close(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_9close(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_9close = {"close", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_9close, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_9close(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("close", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "close", 0))) return NULL;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_8close(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7328,95 +9756,95 @@
   int32_t __pyx_t_2;
   char const *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "pyreadr/librdata.pyx":326
+  /* "pyreadr/librdata.pyx":327
  * 
  *     def close(self):
  *         if self._writer != NULL:             # <<<<<<<<<<<<<<
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  */
-  __pyx_t_1 = ((__pyx_v_self->_writer != NULL) != 0);
+  __pyx_t_1 = (__pyx_v_self->_writer != NULL);
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":327
+    /* "pyreadr/librdata.pyx":328
  *     def close(self):
  *         if self._writer != NULL:
  *             if self._current_column_no != -1:             # <<<<<<<<<<<<<<
  *                 rdata_end_column(self._writer, self._current_column)
  *             rdata_end_table(self._writer, self._row_count, self._table_name)
  */
-    __pyx_t_1 = ((__pyx_v_self->_current_column_no != -1L) != 0);
+    __pyx_t_1 = (__pyx_v_self->_current_column_no != -1L);
     if (__pyx_t_1) {
 
-      /* "pyreadr/librdata.pyx":328
+      /* "pyreadr/librdata.pyx":329
  *         if self._writer != NULL:
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)             # <<<<<<<<<<<<<<
  *             rdata_end_table(self._writer, self._row_count, self._table_name)
  *             rdata_end_file(self._writer)
  */
       (void)(rdata_end_column(__pyx_v_self->_writer, __pyx_v_self->_current_column));
 
-      /* "pyreadr/librdata.pyx":327
+      /* "pyreadr/librdata.pyx":328
  *     def close(self):
  *         if self._writer != NULL:
  *             if self._current_column_no != -1:             # <<<<<<<<<<<<<<
  *                 rdata_end_column(self._writer, self._current_column)
  *             rdata_end_table(self._writer, self._row_count, self._table_name)
  */
     }
 
-    /* "pyreadr/librdata.pyx":329
+    /* "pyreadr/librdata.pyx":330
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  *             rdata_end_table(self._writer, self._row_count, self._table_name)             # <<<<<<<<<<<<<<
  *             rdata_end_file(self._writer)
  *             _os_close(self._fd)
  */
-    __pyx_t_2 = __Pyx_PyInt_As_int32_t(__pyx_v_self->_row_count); if (unlikely((__pyx_t_2 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_As_int32_t(__pyx_v_self->_row_count); if (unlikely((__pyx_t_2 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
     if (unlikely(__pyx_v_self->_table_name == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 329, __pyx_L1_error)
+      __PYX_ERR(0, 330, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyBytes_AsString(__pyx_v_self->_table_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_AsString(__pyx_v_self->_table_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
     (void)(rdata_end_table(__pyx_v_self->_writer, __pyx_t_2, __pyx_t_3));
 
-    /* "pyreadr/librdata.pyx":330
+    /* "pyreadr/librdata.pyx":331
  *                 rdata_end_column(self._writer, self._current_column)
  *             rdata_end_table(self._writer, self._row_count, self._table_name)
  *             rdata_end_file(self._writer)             # <<<<<<<<<<<<<<
  *             _os_close(self._fd)
  * 
  */
     (void)(rdata_end_file(__pyx_v_self->_writer));
 
-    /* "pyreadr/librdata.pyx":331
+    /* "pyreadr/librdata.pyx":332
  *             rdata_end_table(self._writer, self._row_count, self._table_name)
  *             rdata_end_file(self._writer)
  *             _os_close(self._fd)             # <<<<<<<<<<<<<<
  * 
  *     def insert_value(self, row_no, col_no, value, dtype):
  */
     (void)(__pyx_f_7pyreadr_8librdata__os_close(__pyx_v_self->_fd));
 
-    /* "pyreadr/librdata.pyx":326
+    /* "pyreadr/librdata.pyx":327
  * 
  *     def close(self):
  *         if self._writer != NULL:             # <<<<<<<<<<<<<<
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  */
   }
 
-  /* "pyreadr/librdata.pyx":325
+  /* "pyreadr/librdata.pyx":326
  *         self._table_name = name.encode("utf-8")
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         if self._writer != NULL:
  *             if self._current_column_no != -1:
  */
 
@@ -7428,96 +9856,117 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":333
+/* "pyreadr/librdata.pyx":334
  *             _os_close(self._fd)
  * 
  *     def insert_value(self, row_no, col_no, value, dtype):             # <<<<<<<<<<<<<<
  *         cdef rdata_error_t status;
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_11insert_value = {"insert_value", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   CYTHON_UNUSED PyObject *__pyx_v_row_no = 0;
   PyObject *__pyx_v_col_no = 0;
   PyObject *__pyx_v_value = 0;
   PyObject *__pyx_v_dtype = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("insert_value (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_row_no,&__pyx_n_s_col_no,&__pyx_n_s_value,&__pyx_n_s_dtype,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_row_no,&__pyx_n_s_col_no,&__pyx_n_s_value,&__pyx_n_s_dtype,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_row_no)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_row_no)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_col_no)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_col_no)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 1); __PYX_ERR(0, 333, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 1); __PYX_ERR(0, 334, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_value)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 2); __PYX_ERR(0, 333, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 2); __PYX_ERR(0, 334, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dtype)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 334, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 3); __PYX_ERR(0, 333, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, 3); __PYX_ERR(0, 334, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "insert_value") < 0)) __PYX_ERR(0, 333, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "insert_value") < 0)) __PYX_ERR(0, 334, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_row_no = values[0];
     __pyx_v_col_no = values[1];
     __pyx_v_value = values[2];
     __pyx_v_dtype = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 333, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("insert_value", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 334, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Writer.insert_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_10insert_value(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v_row_no, __pyx_v_col_no, __pyx_v_value, __pyx_v_dtype);
 
@@ -7541,420 +9990,440 @@
   char const *__pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("insert_value", 0);
 
-  /* "pyreadr/librdata.pyx":336
+  /* "pyreadr/librdata.pyx":337
  *         cdef rdata_error_t status;
  * 
  *         if self._current_column_no == -1:             # <<<<<<<<<<<<<<
  *             rdata_begin_file(self._writer, &self._fd)
  *             rdata_begin_table(self._writer, self._table_name);
  */
-  __pyx_t_1 = ((__pyx_v_self->_current_column_no == -1L) != 0);
+  __pyx_t_1 = (__pyx_v_self->_current_column_no == -1L);
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":337
+    /* "pyreadr/librdata.pyx":338
  * 
  *         if self._current_column_no == -1:
  *             rdata_begin_file(self._writer, &self._fd)             # <<<<<<<<<<<<<<
  *             rdata_begin_table(self._writer, self._table_name);
  * 
  */
     (void)(rdata_begin_file(__pyx_v_self->_writer, (&__pyx_v_self->_fd)));
 
-    /* "pyreadr/librdata.pyx":338
+    /* "pyreadr/librdata.pyx":339
  *         if self._current_column_no == -1:
  *             rdata_begin_file(self._writer, &self._fd)
  *             rdata_begin_table(self._writer, self._table_name);             # <<<<<<<<<<<<<<
  * 
  *         if col_no != self._current_column_no:
  */
     if (unlikely(__pyx_v_self->_table_name == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-      __PYX_ERR(0, 338, __pyx_L1_error)
+      __PYX_ERR(0, 339, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_self->_table_name); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 338, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_AsString(__pyx_v_self->_table_name); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 339, __pyx_L1_error)
     (void)(rdata_begin_table(__pyx_v_self->_writer, __pyx_t_2));
 
-    /* "pyreadr/librdata.pyx":336
+    /* "pyreadr/librdata.pyx":337
  *         cdef rdata_error_t status;
  * 
  *         if self._current_column_no == -1:             # <<<<<<<<<<<<<<
  *             rdata_begin_file(self._writer, &self._fd)
  *             rdata_begin_table(self._writer, self._table_name);
  */
   }
 
-  /* "pyreadr/librdata.pyx":340
+  /* "pyreadr/librdata.pyx":341
  *             rdata_begin_table(self._writer, self._table_name);
  * 
  *         if col_no != self._current_column_no:             # <<<<<<<<<<<<<<
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_current_column_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->_current_column_no); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_v_col_no, __pyx_t_3, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_v_col_no, __pyx_t_3, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":341
+    /* "pyreadr/librdata.pyx":342
  * 
  *         if col_no != self._current_column_no:
  *             if self._current_column_no != -1:             # <<<<<<<<<<<<<<
  *                 rdata_end_column(self._writer, self._current_column)
  *             self._current_column = rdata_get_column(self._writer, col_no)
  */
-    __pyx_t_1 = ((__pyx_v_self->_current_column_no != -1L) != 0);
+    __pyx_t_1 = (__pyx_v_self->_current_column_no != -1L);
     if (__pyx_t_1) {
 
-      /* "pyreadr/librdata.pyx":342
+      /* "pyreadr/librdata.pyx":343
  *         if col_no != self._current_column_no:
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)             # <<<<<<<<<<<<<<
  *             self._current_column = rdata_get_column(self._writer, col_no)
  *             rdata_begin_column(self._writer, self._current_column, self._row_count)
  */
       (void)(rdata_end_column(__pyx_v_self->_writer, __pyx_v_self->_current_column));
 
-      /* "pyreadr/librdata.pyx":341
+      /* "pyreadr/librdata.pyx":342
  * 
  *         if col_no != self._current_column_no:
  *             if self._current_column_no != -1:             # <<<<<<<<<<<<<<
  *                 rdata_end_column(self._writer, self._current_column)
  *             self._current_column = rdata_get_column(self._writer, col_no)
  */
     }
 
-    /* "pyreadr/librdata.pyx":343
+    /* "pyreadr/librdata.pyx":344
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  *             self._current_column = rdata_get_column(self._writer, col_no)             # <<<<<<<<<<<<<<
  *             rdata_begin_column(self._writer, self._current_column, self._row_count)
  *             self._current_column_no = col_no
  */
-    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_col_no); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_col_no); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 344, __pyx_L1_error)
     __pyx_v_self->_current_column = rdata_get_column(__pyx_v_self->_writer, __pyx_t_5);
 
-    /* "pyreadr/librdata.pyx":344
+    /* "pyreadr/librdata.pyx":345
  *                 rdata_end_column(self._writer, self._current_column)
  *             self._current_column = rdata_get_column(self._writer, col_no)
  *             rdata_begin_column(self._writer, self._current_column, self._row_count)             # <<<<<<<<<<<<<<
  *             self._current_column_no = col_no
  * 
  */
-    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_self->_row_count); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 344, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_self->_row_count); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
     (void)(rdata_begin_column(__pyx_v_self->_writer, __pyx_v_self->_current_column, __pyx_t_5));
 
-    /* "pyreadr/librdata.pyx":345
+    /* "pyreadr/librdata.pyx":346
  *             self._current_column = rdata_get_column(self._writer, col_no)
  *             rdata_begin_column(self._writer, self._current_column, self._row_count)
  *             self._current_column_no = col_no             # <<<<<<<<<<<<<<
  * 
  *         status = RDATA_OK
  */
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_col_no); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_col_no); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L1_error)
     __pyx_v_self->_current_column_no = __pyx_t_6;
 
-    /* "pyreadr/librdata.pyx":340
+    /* "pyreadr/librdata.pyx":341
  *             rdata_begin_table(self._writer, self._table_name);
  * 
  *         if col_no != self._current_column_no:             # <<<<<<<<<<<<<<
  *             if self._current_column_no != -1:
  *                 rdata_end_column(self._writer, self._current_column)
  */
   }
 
-  /* "pyreadr/librdata.pyx":347
+  /* "pyreadr/librdata.pyx":348
  *             self._current_column_no = col_no
  * 
  *         status = RDATA_OK             # <<<<<<<<<<<<<<
  * 
  *         if dtype == "NUMERIC":
  */
   __pyx_v_status = RDATA_OK;
 
-  /* "pyreadr/librdata.pyx":349
+  /* "pyreadr/librdata.pyx":350
  *         status = RDATA_OK
  * 
  *         if dtype == "NUMERIC":             # <<<<<<<<<<<<<<
  *             status = rdata_append_real_value(self._writer, value)
  *         elif dtype == "CHARACTER":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_NUMERIC, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_NUMERIC, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 350, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":350
+    /* "pyreadr/librdata.pyx":351
  * 
  *         if dtype == "NUMERIC":
  *             status = rdata_append_real_value(self._writer, value)             # <<<<<<<<<<<<<<
  *         elif dtype == "CHARACTER":
  *             # in the case of character we could also pass NULL as value to become R's NA
  */
-    __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_7 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_7 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
     __pyx_v_status = rdata_append_real_value(__pyx_v_self->_writer, __pyx_t_7);
 
-    /* "pyreadr/librdata.pyx":349
+    /* "pyreadr/librdata.pyx":350
  *         status = RDATA_OK
  * 
  *         if dtype == "NUMERIC":             # <<<<<<<<<<<<<<
  *             status = rdata_append_real_value(self._writer, value)
  *         elif dtype == "CHARACTER":
  */
     goto __pyx_L6;
   }
 
-  /* "pyreadr/librdata.pyx":351
+  /* "pyreadr/librdata.pyx":352
  *         if dtype == "NUMERIC":
  *             status = rdata_append_real_value(self._writer, value)
  *         elif dtype == "CHARACTER":             # <<<<<<<<<<<<<<
  *             # in the case of character we could also pass NULL as value to become R's NA
  *             # right now passing an empty string has the same effect
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_CHARACTER, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_CHARACTER, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 352, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":354
+    /* "pyreadr/librdata.pyx":355
  *             # in the case of character we could also pass NULL as value to become R's NA
  *             # right now passing an empty string has the same effect
  *             if pd.isnull(value):             # <<<<<<<<<<<<<<
  *                 status = rdata_append_string_value(self._writer, NULL)
  *             else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 355, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isnull); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_isnull); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 355, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_3, __pyx_v_value) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_v_value);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 354, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 354, __pyx_L1_error)
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_value};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 355, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 355, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_1) {
 
-      /* "pyreadr/librdata.pyx":355
+      /* "pyreadr/librdata.pyx":356
  *             # right now passing an empty string has the same effect
  *             if pd.isnull(value):
  *                 status = rdata_append_string_value(self._writer, NULL)             # <<<<<<<<<<<<<<
  *             else:
  *                 status = rdata_append_string_value(self._writer, value.encode('utf-8'))
  */
       __pyx_v_status = rdata_append_string_value(__pyx_v_self->_writer, NULL);
 
-      /* "pyreadr/librdata.pyx":354
+      /* "pyreadr/librdata.pyx":355
  *             # in the case of character we could also pass NULL as value to become R's NA
  *             # right now passing an empty string has the same effect
  *             if pd.isnull(value):             # <<<<<<<<<<<<<<
  *                 status = rdata_append_string_value(self._writer, NULL)
  *             else:
  */
       goto __pyx_L7;
     }
 
-    /* "pyreadr/librdata.pyx":357
+    /* "pyreadr/librdata.pyx":358
  *                 status = rdata_append_string_value(self._writer, NULL)
  *             else:
  *                 status = rdata_append_string_value(self._writer, value.encode('utf-8'))             # <<<<<<<<<<<<<<
  *         elif dtype == "INTEGER":
  *             status = rdata_append_int32_value(self._writer, value)
  */
     /*else*/ {
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 357, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_value, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 358, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_3 = NULL;
+      __pyx_t_6 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_3)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_8, function);
+          __pyx_t_6 = 1;
         }
       }
-      __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_utf_8);
-      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 357, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_utf_8};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 358, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      }
+      __pyx_t_9 = __Pyx_PyObject_AsString(__pyx_t_4); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 358, __pyx_L1_error)
       __pyx_v_status = rdata_append_string_value(__pyx_v_self->_writer, __pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __pyx_L7:;
 
-    /* "pyreadr/librdata.pyx":351
+    /* "pyreadr/librdata.pyx":352
  *         if dtype == "NUMERIC":
  *             status = rdata_append_real_value(self._writer, value)
  *         elif dtype == "CHARACTER":             # <<<<<<<<<<<<<<
  *             # in the case of character we could also pass NULL as value to become R's NA
  *             # right now passing an empty string has the same effect
  */
     goto __pyx_L6;
   }
 
-  /* "pyreadr/librdata.pyx":358
+  /* "pyreadr/librdata.pyx":359
  *             else:
  *                 status = rdata_append_string_value(self._writer, value.encode('utf-8'))
  *         elif dtype == "INTEGER":             # <<<<<<<<<<<<<<
  *             status = rdata_append_int32_value(self._writer, value)
  *         elif dtype == "LOGICAL":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_INTEGER, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 358, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_INTEGER, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 359, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":359
+    /* "pyreadr/librdata.pyx":360
  *                 status = rdata_append_string_value(self._writer, value.encode('utf-8'))
  *         elif dtype == "INTEGER":
  *             status = rdata_append_int32_value(self._writer, value)             # <<<<<<<<<<<<<<
  *         elif dtype == "LOGICAL":
  *             status = rdata_append_logical_value(self._writer, value);
  */
-    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_value); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 359, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int32_t(__pyx_v_value); if (unlikely((__pyx_t_5 == ((int32_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 360, __pyx_L1_error)
     __pyx_v_status = rdata_append_int32_value(__pyx_v_self->_writer, __pyx_t_5);
 
-    /* "pyreadr/librdata.pyx":358
+    /* "pyreadr/librdata.pyx":359
  *             else:
  *                 status = rdata_append_string_value(self._writer, value.encode('utf-8'))
  *         elif dtype == "INTEGER":             # <<<<<<<<<<<<<<
  *             status = rdata_append_int32_value(self._writer, value)
  *         elif dtype == "LOGICAL":
  */
     goto __pyx_L6;
   }
 
-  /* "pyreadr/librdata.pyx":360
+  /* "pyreadr/librdata.pyx":361
  *         elif dtype == "INTEGER":
  *             status = rdata_append_int32_value(self._writer, value)
  *         elif dtype == "LOGICAL":             # <<<<<<<<<<<<<<
  *             status = rdata_append_logical_value(self._writer, value);
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_LOGICAL, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 360, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_LOGICAL, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 361, __pyx_L1_error)
   if (likely(__pyx_t_1)) {
 
-    /* "pyreadr/librdata.pyx":361
+    /* "pyreadr/librdata.pyx":362
  *             status = rdata_append_int32_value(self._writer, value)
  *         elif dtype == "LOGICAL":
  *             status = rdata_append_logical_value(self._writer, value);             # <<<<<<<<<<<<<<
  *         else:
  *             raise PyreadrError("Unknown data type")
  */
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 361, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 362, __pyx_L1_error)
     __pyx_v_status = rdata_append_logical_value(__pyx_v_self->_writer, __pyx_t_6);
 
-    /* "pyreadr/librdata.pyx":360
+    /* "pyreadr/librdata.pyx":361
  *         elif dtype == "INTEGER":
  *             status = rdata_append_int32_value(self._writer, value)
  *         elif dtype == "LOGICAL":             # <<<<<<<<<<<<<<
  *             status = rdata_append_logical_value(self._writer, value);
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "pyreadr/librdata.pyx":363
+  /* "pyreadr/librdata.pyx":364
  *             status = rdata_append_logical_value(self._writer, value);
  *         else:
  *             raise PyreadrError("Unknown data type")             # <<<<<<<<<<<<<<
  * 
  *         if status != RDATA_OK:
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 363, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 364, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_3 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_3, __pyx_kp_u_Unknown_data_type) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_Unknown_data_type);
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 363, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_kp_u_Unknown_data_type};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 363, __pyx_L1_error)
+    __PYX_ERR(0, 364, __pyx_L1_error)
   }
   __pyx_L6:;
 
-  /* "pyreadr/librdata.pyx":365
+  /* "pyreadr/librdata.pyx":366
  *             raise PyreadrError("Unknown data type")
  * 
  *         if status != RDATA_OK:             # <<<<<<<<<<<<<<
  *             raise LibrdataError(rdata_error_message(status))
  * 
  */
-  __pyx_t_1 = ((__pyx_v_status != RDATA_OK) != 0);
+  __pyx_t_1 = (__pyx_v_status != RDATA_OK);
   if (unlikely(__pyx_t_1)) {
 
-    /* "pyreadr/librdata.pyx":366
+    /* "pyreadr/librdata.pyx":367
  * 
  *         if status != RDATA_OK:
  *             raise LibrdataError(rdata_error_message(status))             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 366, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_3 = __Pyx_PyStr_FromString(rdata_error_message(__pyx_v_status)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 366, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyStr_FromString(rdata_error_message(__pyx_v_status)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_10 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_8);
       if (likely(__pyx_t_10)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_10);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_8, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_10, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_3);
-    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 366, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_3};
+      __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 367, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    }
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 366, __pyx_L1_error)
+    __PYX_ERR(0, 367, __pyx_L1_error)
 
-    /* "pyreadr/librdata.pyx":365
+    /* "pyreadr/librdata.pyx":366
  *             raise PyreadrError("Unknown data type")
  * 
  *         if status != RDATA_OK:             # <<<<<<<<<<<<<<
  *             raise LibrdataError(rdata_error_message(status))
  * 
  */
   }
 
-  /* "pyreadr/librdata.pyx":333
+  /* "pyreadr/librdata.pyx":334
  *             _os_close(self._fd)
  * 
  *     def insert_value(self, row_no, col_no, value, dtype):             # <<<<<<<<<<<<<<
  *         cdef rdata_error_t status;
  * 
  */
 
@@ -7970,74 +10439,93 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pyreadr/librdata.pyx":369
+/* "pyreadr/librdata.pyx":370
  * 
  * 
  *     def add_column(self, name, dtype):             # <<<<<<<<<<<<<<
  *         cdef rdata_type_t data_type
  *         cdef rdata_column_t* column
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_13add_column(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_13add_column(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_13add_column(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_13add_column = {"add_column", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_13add_column, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_13add_column(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyObject *__pyx_v_name = 0;
   PyObject *__pyx_v_dtype = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_column (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_dtype,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_dtype,0};
     PyObject* values[2] = {0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (__pyx_nargs) {
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dtype)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("add_column", 1, 2, 2, 1); __PYX_ERR(0, 369, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_column", 1, 2, 2, 1); __PYX_ERR(0, 370, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_column") < 0)) __PYX_ERR(0, 369, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "add_column") < 0)) __PYX_ERR(0, 370, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+    } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_name = values[0];
     __pyx_v_dtype = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_column", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 369, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_column", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 370, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pyreadr.librdata.Writer.add_column", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_12add_column(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v_name, __pyx_v_dtype);
 
@@ -8053,231 +10541,242 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  char const *__pyx_t_6;
+  int __pyx_t_6;
+  char const *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_column", 0);
 
-  /* "pyreadr/librdata.pyx":373
+  /* "pyreadr/librdata.pyx":374
  *         cdef rdata_column_t* column
  * 
  *         if dtype == "NUMERIC":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_REAL
  *         elif dtype == "CHARACTER":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_NUMERIC, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 373, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_NUMERIC, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 374, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":374
+    /* "pyreadr/librdata.pyx":375
  * 
  *         if dtype == "NUMERIC":
  *             data_type = RDATA_TYPE_REAL             # <<<<<<<<<<<<<<
  *         elif dtype == "CHARACTER":
  *             data_type = RDATA_TYPE_STRING
  */
     __pyx_v_data_type = RDATA_TYPE_REAL;
 
-    /* "pyreadr/librdata.pyx":373
+    /* "pyreadr/librdata.pyx":374
  *         cdef rdata_column_t* column
  * 
  *         if dtype == "NUMERIC":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_REAL
  *         elif dtype == "CHARACTER":
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":375
+  /* "pyreadr/librdata.pyx":376
  *         if dtype == "NUMERIC":
  *             data_type = RDATA_TYPE_REAL
  *         elif dtype == "CHARACTER":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_STRING
  *         elif dtype == "INTEGER":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_CHARACTER, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_CHARACTER, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 376, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":376
+    /* "pyreadr/librdata.pyx":377
  *             data_type = RDATA_TYPE_REAL
  *         elif dtype == "CHARACTER":
  *             data_type = RDATA_TYPE_STRING             # <<<<<<<<<<<<<<
  *         elif dtype == "INTEGER":
  *             data_type = RDATA_TYPE_INT32
  */
     __pyx_v_data_type = RDATA_TYPE_STRING;
 
-    /* "pyreadr/librdata.pyx":375
+    /* "pyreadr/librdata.pyx":376
  *         if dtype == "NUMERIC":
  *             data_type = RDATA_TYPE_REAL
  *         elif dtype == "CHARACTER":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_STRING
  *         elif dtype == "INTEGER":
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":377
+  /* "pyreadr/librdata.pyx":378
  *         elif dtype == "CHARACTER":
  *             data_type = RDATA_TYPE_STRING
  *         elif dtype == "INTEGER":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_INT32
  *         elif dtype == "LOGICAL":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_INTEGER, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_INTEGER, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 378, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "pyreadr/librdata.pyx":378
+    /* "pyreadr/librdata.pyx":379
  *             data_type = RDATA_TYPE_STRING
  *         elif dtype == "INTEGER":
  *             data_type = RDATA_TYPE_INT32             # <<<<<<<<<<<<<<
  *         elif dtype == "LOGICAL":
  *             data_type = RDATA_TYPE_LOGICAL
  */
     __pyx_v_data_type = RDATA_TYPE_INT32;
 
-    /* "pyreadr/librdata.pyx":377
+    /* "pyreadr/librdata.pyx":378
  *         elif dtype == "CHARACTER":
  *             data_type = RDATA_TYPE_STRING
  *         elif dtype == "INTEGER":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_INT32
  *         elif dtype == "LOGICAL":
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":379
+  /* "pyreadr/librdata.pyx":380
  *         elif dtype == "INTEGER":
  *             data_type = RDATA_TYPE_INT32
  *         elif dtype == "LOGICAL":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_LOGICAL
  *         else:
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_LOGICAL, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 379, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_dtype, __pyx_n_u_LOGICAL, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 380, __pyx_L1_error)
   if (likely(__pyx_t_1)) {
 
-    /* "pyreadr/librdata.pyx":380
+    /* "pyreadr/librdata.pyx":381
  *             data_type = RDATA_TYPE_INT32
  *         elif dtype == "LOGICAL":
  *             data_type = RDATA_TYPE_LOGICAL             # <<<<<<<<<<<<<<
  *         else:
  *             raise PyreadrError("Unknown data type: %s" % dtype)
  */
     __pyx_v_data_type = RDATA_TYPE_LOGICAL;
 
-    /* "pyreadr/librdata.pyx":379
+    /* "pyreadr/librdata.pyx":380
  *         elif dtype == "INTEGER":
  *             data_type = RDATA_TYPE_INT32
  *         elif dtype == "LOGICAL":             # <<<<<<<<<<<<<<
  *             data_type = RDATA_TYPE_LOGICAL
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "pyreadr/librdata.pyx":382
+  /* "pyreadr/librdata.pyx":383
  *             data_type = RDATA_TYPE_LOGICAL
  *         else:
  *             raise PyreadrError("Unknown data type: %s" % dtype)             # <<<<<<<<<<<<<<
  * 
  *         column = rdata_add_column(self._writer, name.encode('utf-8'), data_type)
  */
   /*else*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Unknown_data_type_s, __pyx_v_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 382, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_Unknown_data_type_s, __pyx_v_dtype); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
+    __pyx_t_6 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
+        __pyx_t_6 = 1;
       }
     }
-    __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 382, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
+      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    }
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 382, __pyx_L1_error)
+    __PYX_ERR(0, 383, __pyx_L1_error)
   }
   __pyx_L3:;
 
-  /* "pyreadr/librdata.pyx":384
+  /* "pyreadr/librdata.pyx":385
  *             raise PyreadrError("Unknown data type: %s" % dtype)
  * 
  *         column = rdata_add_column(self._writer, name.encode('utf-8'), data_type)             # <<<<<<<<<<<<<<
  *         col = Column()
  *         col._this = column
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
+  __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
+      __pyx_t_6 = 1;
     }
   }
-  __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_utf_8);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 384, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L1_error)
-  __pyx_v_column = rdata_add_column(__pyx_v_self->_writer, __pyx_t_6, __pyx_v_data_type);
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_kp_u_utf_8};
+    __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+  __pyx_t_7 = __Pyx_PyObject_AsString(__pyx_t_2); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_v_column = rdata_add_column(__pyx_v_self->_writer, __pyx_t_7, __pyx_v_data_type);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyreadr/librdata.pyx":385
+  /* "pyreadr/librdata.pyx":386
  * 
  *         column = rdata_add_column(self._writer, name.encode('utf-8'), data_type)
  *         col = Column()             # <<<<<<<<<<<<<<
  *         col._this = column
  *         return col
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7pyreadr_8librdata_Column)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_7pyreadr_8librdata_Column)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_col = ((struct __pyx_obj_7pyreadr_8librdata_Column *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pyreadr/librdata.pyx":386
+  /* "pyreadr/librdata.pyx":387
  *         column = rdata_add_column(self._writer, name.encode('utf-8'), data_type)
  *         col = Column()
  *         col._this = column             # <<<<<<<<<<<<<<
  *         return col
  * 
  */
   __pyx_v_col->_this = __pyx_v_column;
 
-  /* "pyreadr/librdata.pyx":387
+  /* "pyreadr/librdata.pyx":388
  *         col = Column()
  *         col._this = column
  *         return col             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_col));
+  __Pyx_INCREF((PyObject *)__pyx_v_col);
   __pyx_r = ((PyObject *)__pyx_v_col);
   goto __pyx_L0;
 
-  /* "pyreadr/librdata.pyx":369
+  /* "pyreadr/librdata.pyx":370
  * 
  * 
  *     def add_column(self, name, dtype):             # <<<<<<<<<<<<<<
  *         cdef rdata_type_t data_type
  *         cdef rdata_column_t* column
  */
 
@@ -8294,167 +10793,256 @@
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_15__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_14__reduce_cython__(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_14__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__current_column_self__write, 0, 0);
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Writer.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pyreadr_8librdata_6Writer_17__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_16__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v___pyx_state = values[0];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pyreadr.librdata.Writer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pyreadr_8librdata_6Writer_16__setstate_cython__(((struct __pyx_obj_7pyreadr_8librdata_Writer *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pyreadr_8librdata_6Writer_16__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pyreadr_8librdata_Writer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_self__current_column_self__write, 0, 0);
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_AddTraceback("pyreadr.librdata.Writer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static struct __pyx_vtabstruct_7pyreadr_8librdata_Parser __pyx_vtable_7pyreadr_8librdata_Parser;
 
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Parser(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7pyreadr_8librdata_Parser *p;
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   p = ((struct __pyx_obj_7pyreadr_8librdata_Parser *)o);
   p->__pyx_vtab = __pyx_vtabptr_7pyreadr_8librdata_Parser;
   return o;
 }
 
 static void __pyx_tp_dealloc_7pyreadr_8librdata_Parser(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_7pyreadr_8librdata_Parser) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_7pyreadr_8librdata_Parser[] = {
-  {"parse", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Parser_1parse, METH_O, 0},
-  {"handle_table", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table, METH_O, 0},
-  {"handle_column", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_column_name", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_dim", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_dim_name", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name, METH_VARARGS|METH_KEYWORDS, 0},
-  {"_handle_row_name", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_text_value", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value, METH_VARARGS|METH_KEYWORDS, 0},
-  {"handle_value_label", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__, METH_O, 0},
+  {"handle_table", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_3handle_table, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_column", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_5handle_column, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_column_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_7handle_column_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_dim", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_9handle_dim, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_dim_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_11handle_dim_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"_handle_row_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_13_handle_row_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_text_value", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_15handle_text_value, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"handle_value_label", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_17handle_value_label, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_19__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Parser_21__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_7pyreadr_8librdata_Parser_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_7pyreadr_8librdata_Parser},
+  {Py_tp_methods, (void *)__pyx_methods_7pyreadr_8librdata_Parser},
+  {Py_tp_new, (void *)__pyx_tp_new_7pyreadr_8librdata_Parser},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_7pyreadr_8librdata_Parser_spec = {
+  "pyreadr.librdata.Parser",
+  sizeof(struct __pyx_obj_7pyreadr_8librdata_Parser),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
+  __pyx_type_7pyreadr_8librdata_Parser_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_7pyreadr_8librdata_Parser = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyreadr.librdata.Parser", /*tp_name*/
+  "pyreadr.librdata.""Parser", /*tp_name*/
   sizeof(struct __pyx_obj_7pyreadr_8librdata_Parser), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_7pyreadr_8librdata_Parser, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -8489,68 +11077,103 @@
   __pyx_methods_7pyreadr_8librdata_Parser, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_7pyreadr_8librdata_Parser, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Column(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   return o;
 }
 
 static void __pyx_tp_dealloc_7pyreadr_8librdata_Column(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_7pyreadr_8librdata_Column) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_7pyreadr_8librdata_Column[] = {
-  {"add_level_labels", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__, METH_O, 0},
+  {"add_level_labels", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_1add_level_labels, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_3__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Column_5__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_7pyreadr_8librdata_Column_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_7pyreadr_8librdata_Column},
+  {Py_tp_methods, (void *)__pyx_methods_7pyreadr_8librdata_Column},
+  {Py_tp_new, (void *)__pyx_tp_new_7pyreadr_8librdata_Column},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_7pyreadr_8librdata_Column_spec = {
+  "pyreadr.librdata.Column",
+  sizeof(struct __pyx_obj_7pyreadr_8librdata_Column),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
+  __pyx_type_7pyreadr_8librdata_Column_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_7pyreadr_8librdata_Column = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyreadr.librdata.Column", /*tp_name*/
+  "pyreadr.librdata.""Column", /*tp_name*/
   sizeof(struct __pyx_obj_7pyreadr_8librdata_Column), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_7pyreadr_8librdata_Column, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -8585,59 +11208,79 @@
   __pyx_methods_7pyreadr_8librdata_Column, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_7pyreadr_8librdata_Column, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyObject *__pyx_tp_new_7pyreadr_8librdata_Writer(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7pyreadr_8librdata_Writer *p;
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   p = ((struct __pyx_obj_7pyreadr_8librdata_Writer *)o);
   p->_format = Py_None; Py_INCREF(Py_None);
   p->_row_count = Py_None; Py_INCREF(Py_None);
   p->_table_name = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_7pyreadr_8librdata_Writer(PyObject *o) {
   struct __pyx_obj_7pyreadr_8librdata_Writer *p = (struct __pyx_obj_7pyreadr_8librdata_Writer *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && !__Pyx_PyObject_GC_IsFinalized(o)) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_7pyreadr_8librdata_Writer) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_format);
   Py_CLEAR(p->_row_count);
   Py_CLEAR(p->_table_name);
   (*Py_TYPE(o)->tp_free)(o);
@@ -8664,28 +11307,46 @@
   tmp = ((PyObject*)p->_row_count);
   p->_row_count = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
 static PyMethodDef __pyx_methods_7pyreadr_8librdata_Writer[] = {
-  {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_3open, METH_VARARGS|METH_KEYWORDS, 0},
-  {"set_row_count", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count, METH_O, 0},
-  {"set_table_name", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name, METH_O, 0},
-  {"close", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Writer_9close, METH_NOARGS, 0},
-  {"insert_value", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value, METH_VARARGS|METH_KEYWORDS, 0},
-  {"add_column", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_13add_column, METH_VARARGS|METH_KEYWORDS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__, METH_O, 0},
+  {"open", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_3open, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"set_row_count", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_5set_row_count, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"set_table_name", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_7set_table_name, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"close", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_9close, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"insert_value", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_11insert_value, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"add_column", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_13add_column, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_15__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pyreadr_8librdata_6Writer_17__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_7pyreadr_8librdata_Writer_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_7pyreadr_8librdata_Writer},
+  {Py_tp_traverse, (void *)__pyx_tp_traverse_7pyreadr_8librdata_Writer},
+  {Py_tp_clear, (void *)__pyx_tp_clear_7pyreadr_8librdata_Writer},
+  {Py_tp_methods, (void *)__pyx_methods_7pyreadr_8librdata_Writer},
+  {Py_tp_init, (void *)__pyx_pw_7pyreadr_8librdata_6Writer_1__init__},
+  {Py_tp_new, (void *)__pyx_tp_new_7pyreadr_8librdata_Writer},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_7pyreadr_8librdata_Writer_spec = {
+  "pyreadr.librdata.Writer",
+  sizeof(struct __pyx_obj_7pyreadr_8librdata_Writer),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC,
+  __pyx_type_7pyreadr_8librdata_Writer_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_7pyreadr_8librdata_Writer = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pyreadr.librdata.Writer", /*tp_name*/
+  "pyreadr.librdata.""Writer", /*tp_name*/
   sizeof(struct __pyx_obj_7pyreadr_8librdata_Writer), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_7pyreadr_8librdata_Writer, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -8720,254 +11381,485 @@
   __pyx_methods_7pyreadr_8librdata_Writer, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   __pyx_pw_7pyreadr_8librdata_6Writer_1__init__, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_7pyreadr_8librdata_Writer, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_librdata(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_librdata},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "librdata",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_CHARACTER, __pyx_k_CHARACTER, sizeof(__pyx_k_CHARACTER), 0, 0, 1, 1},
-  {&__pyx_n_u_CHARACTER, __pyx_k_CHARACTER, sizeof(__pyx_k_CHARACTER), 0, 1, 0, 1},
-  {&__pyx_n_s_Column, __pyx_k_Column, sizeof(__pyx_k_Column), 0, 0, 1, 1},
-  {&__pyx_n_s_DATE, __pyx_k_DATE, sizeof(__pyx_k_DATE), 0, 0, 1, 1},
-  {&__pyx_n_s_DataType, __pyx_k_DataType, sizeof(__pyx_k_DataType), 0, 0, 1, 1},
-  {&__pyx_n_s_Enum, __pyx_k_Enum, sizeof(__pyx_k_Enum), 0, 0, 1, 1},
-  {&__pyx_n_s_INTEGER, __pyx_k_INTEGER, sizeof(__pyx_k_INTEGER), 0, 0, 1, 1},
-  {&__pyx_n_u_INTEGER, __pyx_k_INTEGER, sizeof(__pyx_k_INTEGER), 0, 1, 0, 1},
-  {&__pyx_n_s_LOGICAL, __pyx_k_LOGICAL, sizeof(__pyx_k_LOGICAL), 0, 0, 1, 1},
-  {&__pyx_n_u_LOGICAL, __pyx_k_LOGICAL, sizeof(__pyx_k_LOGICAL), 0, 1, 0, 1},
-  {&__pyx_n_s_LibrdataError, __pyx_k_LibrdataError, sizeof(__pyx_k_LibrdataError), 0, 0, 1, 1},
-  {&__pyx_n_s_NUMERIC, __pyx_k_NUMERIC, sizeof(__pyx_k_NUMERIC), 0, 0, 1, 1},
-  {&__pyx_n_u_NUMERIC, __pyx_k_NUMERIC, sizeof(__pyx_k_NUMERIC), 0, 1, 0, 1},
-  {&__pyx_n_s_Parser, __pyx_k_Parser, sizeof(__pyx_k_Parser), 0, 0, 1, 1},
-  {&__pyx_n_s_PyreadrError, __pyx_k_PyreadrError, sizeof(__pyx_k_PyreadrError), 0, 0, 1, 1},
-  {&__pyx_n_s_TIMESTAMP, __pyx_k_TIMESTAMP, sizeof(__pyx_k_TIMESTAMP), 0, 0, 1, 1},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_kp_u_Unknown_data_type, __pyx_k_Unknown_data_type, sizeof(__pyx_k_Unknown_data_type), 0, 1, 0, 0},
-  {&__pyx_kp_u_Unknown_data_type_s, __pyx_k_Unknown_data_type_s, sizeof(__pyx_k_Unknown_data_type_s), 0, 1, 0, 0},
-  {&__pyx_kp_u_Unsupported_format, __pyx_k_Unsupported_format, sizeof(__pyx_k_Unsupported_format), 0, 1, 0, 0},
-  {&__pyx_n_s_Writer, __pyx_k_Writer, sizeof(__pyx_k_Writer), 0, 0, 1, 1},
-  {&__pyx_kp_u_Wrong_data_type_s_for_dimensions, __pyx_k_Wrong_data_type_s_for_dimensions, sizeof(__pyx_k_Wrong_data_type_s_for_dimensions), 0, 1, 0, 0},
-  {&__pyx_kp_b__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 0, 0, 0},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_col_no, __pyx_k_col_no, sizeof(__pyx_k_col_no), 0, 0, 1, 1},
-  {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
-  {&__pyx_n_s_custom_errors, __pyx_k_custom_errors, sizeof(__pyx_k_custom_errors), 0, 0, 1, 1},
-  {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {&__pyx_n_s_data_type, __pyx_k_data_type, sizeof(__pyx_k_data_type), 0, 0, 1, 1},
-  {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
-  {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
-  {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
-  {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
-  {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
-  {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
-  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_column, __pyx_k_handle_column, sizeof(__pyx_k_handle_column), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_column_name, __pyx_k_handle_column_name, sizeof(__pyx_k_handle_column_name), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_dim, __pyx_k_handle_dim, sizeof(__pyx_k_handle_dim), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_dim_name, __pyx_k_handle_dim_name, sizeof(__pyx_k_handle_dim_name), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_row_name, __pyx_k_handle_row_name, sizeof(__pyx_k_handle_row_name), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_table, __pyx_k_handle_table, sizeof(__pyx_k_handle_table), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_text_value, __pyx_k_handle_text_value, sizeof(__pyx_k_handle_text_value), 0, 0, 1, 1},
-  {&__pyx_n_s_handle_value_label, __pyx_k_handle_value_label, sizeof(__pyx_k_handle_value_label), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
-  {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
-  {&__pyx_n_s_isfile, __pyx_k_isfile, sizeof(__pyx_k_isfile), 0, 0, 1, 1},
-  {&__pyx_n_s_isnull, __pyx_k_isnull, sizeof(__pyx_k_isnull), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
-  {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
-  {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
-  {&__pyx_n_s_os_path, __pyx_k_os_path, sizeof(__pyx_k_os_path), 0, 0, 1, 1},
-  {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
-  {&__pyx_n_s_parse, __pyx_k_parse, sizeof(__pyx_k_parse), 0, 0, 1, 1},
-  {&__pyx_n_s_parse_current_table, __pyx_k_parse_current_table, sizeof(__pyx_k_parse_current_table), 0, 0, 1, 1},
-  {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
-  {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
-  {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
-  {&__pyx_n_s_pyreadr_librdata, __pyx_k_pyreadr_librdata, sizeof(__pyx_k_pyreadr_librdata), 0, 0, 1, 1},
-  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-  {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
-  {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_u_rdata, __pyx_k_rdata, sizeof(__pyx_k_rdata), 0, 1, 0, 1},
-  {&__pyx_n_u_rds, __pyx_k_rds, sizeof(__pyx_k_rds), 0, 1, 0, 1},
-  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_row_no, __pyx_k_row_no, sizeof(__pyx_k_row_no), 0, 0, 1, 1},
-  {&__pyx_kp_s_self__current_column_self__write, __pyx_k_self__current_column_self__write, sizeof(__pyx_k_self__current_column_self__write), 0, 0, 1, 0},
-  {&__pyx_kp_s_self__this_cannot_be_converted_t, __pyx_k_self__this_cannot_be_converted_t, sizeof(__pyx_k_self__this_cannot_be_converted_t), 0, 0, 1, 0},
-  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
-  {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
-  {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_b_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 0, 0},
+    {&__pyx_n_s_CHARACTER, __pyx_k_CHARACTER, sizeof(__pyx_k_CHARACTER), 0, 0, 1, 1},
+    {&__pyx_n_u_CHARACTER, __pyx_k_CHARACTER, sizeof(__pyx_k_CHARACTER), 0, 1, 0, 1},
+    {&__pyx_n_s_Column, __pyx_k_Column, sizeof(__pyx_k_Column), 0, 0, 1, 1},
+    {&__pyx_n_s_Column___reduce_cython, __pyx_k_Column___reduce_cython, sizeof(__pyx_k_Column___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Column___setstate_cython, __pyx_k_Column___setstate_cython, sizeof(__pyx_k_Column___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Column_add_level_labels, __pyx_k_Column_add_level_labels, sizeof(__pyx_k_Column_add_level_labels), 0, 0, 1, 1},
+    {&__pyx_n_s_DATE, __pyx_k_DATE, sizeof(__pyx_k_DATE), 0, 0, 1, 1},
+    {&__pyx_n_s_DataType, __pyx_k_DataType, sizeof(__pyx_k_DataType), 0, 0, 1, 1},
+    {&__pyx_n_s_Enum, __pyx_k_Enum, sizeof(__pyx_k_Enum), 0, 0, 1, 1},
+    {&__pyx_n_s_INTEGER, __pyx_k_INTEGER, sizeof(__pyx_k_INTEGER), 0, 0, 1, 1},
+    {&__pyx_n_u_INTEGER, __pyx_k_INTEGER, sizeof(__pyx_k_INTEGER), 0, 1, 0, 1},
+    {&__pyx_n_s_LOGICAL, __pyx_k_LOGICAL, sizeof(__pyx_k_LOGICAL), 0, 0, 1, 1},
+    {&__pyx_n_u_LOGICAL, __pyx_k_LOGICAL, sizeof(__pyx_k_LOGICAL), 0, 1, 0, 1},
+    {&__pyx_n_s_LibrdataError, __pyx_k_LibrdataError, sizeof(__pyx_k_LibrdataError), 0, 0, 1, 1},
+    {&__pyx_n_s_NUMERIC, __pyx_k_NUMERIC, sizeof(__pyx_k_NUMERIC), 0, 0, 1, 1},
+    {&__pyx_n_u_NUMERIC, __pyx_k_NUMERIC, sizeof(__pyx_k_NUMERIC), 0, 1, 0, 1},
+    {&__pyx_n_s_Parser, __pyx_k_Parser, sizeof(__pyx_k_Parser), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser___reduce_cython, __pyx_k_Parser___reduce_cython, sizeof(__pyx_k_Parser___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser___setstate_cython, __pyx_k_Parser___setstate_cython, sizeof(__pyx_k_Parser___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser__handle_row_name, __pyx_k_Parser__handle_row_name, sizeof(__pyx_k_Parser__handle_row_name), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_column, __pyx_k_Parser_handle_column, sizeof(__pyx_k_Parser_handle_column), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_column_name, __pyx_k_Parser_handle_column_name, sizeof(__pyx_k_Parser_handle_column_name), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_dim, __pyx_k_Parser_handle_dim, sizeof(__pyx_k_Parser_handle_dim), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_dim_name, __pyx_k_Parser_handle_dim_name, sizeof(__pyx_k_Parser_handle_dim_name), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_table, __pyx_k_Parser_handle_table, sizeof(__pyx_k_Parser_handle_table), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_text_value, __pyx_k_Parser_handle_text_value, sizeof(__pyx_k_Parser_handle_text_value), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_handle_value_label, __pyx_k_Parser_handle_value_label, sizeof(__pyx_k_Parser_handle_value_label), 0, 0, 1, 1},
+    {&__pyx_n_s_Parser_parse, __pyx_k_Parser_parse, sizeof(__pyx_k_Parser_parse), 0, 0, 1, 1},
+    {&__pyx_n_s_PyreadrError, __pyx_k_PyreadrError, sizeof(__pyx_k_PyreadrError), 0, 0, 1, 1},
+    {&__pyx_n_s_TIMESTAMP, __pyx_k_TIMESTAMP, sizeof(__pyx_k_TIMESTAMP), 0, 0, 1, 1},
+    {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
+    {&__pyx_kp_u_Unknown_data_type, __pyx_k_Unknown_data_type, sizeof(__pyx_k_Unknown_data_type), 0, 1, 0, 0},
+    {&__pyx_kp_u_Unknown_data_type_s, __pyx_k_Unknown_data_type_s, sizeof(__pyx_k_Unknown_data_type_s), 0, 1, 0, 0},
+    {&__pyx_kp_u_Unsupported_format, __pyx_k_Unsupported_format, sizeof(__pyx_k_Unsupported_format), 0, 1, 0, 0},
+    {&__pyx_n_u_Windows, __pyx_k_Windows, sizeof(__pyx_k_Windows), 0, 1, 0, 1},
+    {&__pyx_n_s_Writer, __pyx_k_Writer, sizeof(__pyx_k_Writer), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer___reduce_cython, __pyx_k_Writer___reduce_cython, sizeof(__pyx_k_Writer___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer___setstate_cython, __pyx_k_Writer___setstate_cython, sizeof(__pyx_k_Writer___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_add_column, __pyx_k_Writer_add_column, sizeof(__pyx_k_Writer_add_column), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_close, __pyx_k_Writer_close, sizeof(__pyx_k_Writer_close), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_insert_value, __pyx_k_Writer_insert_value, sizeof(__pyx_k_Writer_insert_value), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_open, __pyx_k_Writer_open, sizeof(__pyx_k_Writer_open), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_set_row_count, __pyx_k_Writer_set_row_count, sizeof(__pyx_k_Writer_set_row_count), 0, 0, 1, 1},
+    {&__pyx_n_s_Writer_set_table_name, __pyx_k_Writer_set_table_name, sizeof(__pyx_k_Writer_set_table_name), 0, 0, 1, 1},
+    {&__pyx_kp_u_Wrong_data_type_s_for_dimensions, __pyx_k_Wrong_data_type_s_for_dimensions, sizeof(__pyx_k_Wrong_data_type_s_for_dimensions), 0, 1, 0, 0},
+    {&__pyx_n_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 1},
+    {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
+    {&__pyx_n_s__38, __pyx_k__38, sizeof(__pyx_k__38), 0, 0, 1, 1},
+    {&__pyx_n_s_add_column, __pyx_k_add_column, sizeof(__pyx_k_add_column), 0, 0, 1, 1},
+    {&__pyx_n_s_add_level_labels, __pyx_k_add_level_labels, sizeof(__pyx_k_add_level_labels), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+    {&__pyx_n_s_col, __pyx_k_col, sizeof(__pyx_k_col), 0, 0, 1, 1},
+    {&__pyx_n_s_col_no, __pyx_k_col_no, sizeof(__pyx_k_col_no), 0, 0, 1, 1},
+    {&__pyx_n_s_column, __pyx_k_column, sizeof(__pyx_k_column), 0, 0, 1, 1},
+    {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
+    {&__pyx_n_s_custom_errors, __pyx_k_custom_errors, sizeof(__pyx_k_custom_errors), 0, 0, 1, 1},
+    {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
+    {&__pyx_n_s_data_type, __pyx_k_data_type, sizeof(__pyx_k_data_type), 0, 0, 1, 1},
+    {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
+    {&__pyx_n_s_enum, __pyx_k_enum, sizeof(__pyx_k_enum), 0, 0, 1, 1},
+    {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
+    {&__pyx_n_s_float64, __pyx_k_float64, sizeof(__pyx_k_float64), 0, 0, 1, 1},
+    {&__pyx_n_s_fmt, __pyx_k_fmt, sizeof(__pyx_k_fmt), 0, 0, 1, 1},
+    {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
+    {&__pyx_n_s_fsdecode, __pyx_k_fsdecode, sizeof(__pyx_k_fsdecode), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_column, __pyx_k_handle_column, sizeof(__pyx_k_handle_column), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_column_name, __pyx_k_handle_column_name, sizeof(__pyx_k_handle_column_name), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_dim, __pyx_k_handle_dim, sizeof(__pyx_k_handle_dim), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_dim_name, __pyx_k_handle_dim_name, sizeof(__pyx_k_handle_dim_name), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_row_name, __pyx_k_handle_row_name, sizeof(__pyx_k_handle_row_name), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_row_name_2, __pyx_k_handle_row_name_2, sizeof(__pyx_k_handle_row_name_2), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_table, __pyx_k_handle_table, sizeof(__pyx_k_handle_table), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_text_value, __pyx_k_handle_text_value, sizeof(__pyx_k_handle_text_value), 0, 0, 1, 1},
+    {&__pyx_n_s_handle_value_label, __pyx_k_handle_value_label, sizeof(__pyx_k_handle_value_label), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
+    {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_s_insert_value, __pyx_k_insert_value, sizeof(__pyx_k_insert_value), 0, 0, 1, 1},
+    {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_isfile, __pyx_k_isfile, sizeof(__pyx_k_isfile), 0, 0, 1, 1},
+    {&__pyx_n_s_isnull, __pyx_k_isnull, sizeof(__pyx_k_isnull), 0, 0, 1, 1},
+    {&__pyx_n_s_label, __pyx_k_label, sizeof(__pyx_k_label), 0, 0, 1, 1},
+    {&__pyx_n_s_labels, __pyx_k_labels, sizeof(__pyx_k_labels), 0, 0, 1, 1},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
+    {&__pyx_n_s_module, __pyx_k_module, sizeof(__pyx_k_module), 0, 0, 1, 1},
+    {&__pyx_n_s_mro_entries, __pyx_k_mro_entries, sizeof(__pyx_k_mro_entries), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
+    {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
+    {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
+    {&__pyx_n_s_os_path, __pyx_k_os_path, sizeof(__pyx_k_os_path), 0, 0, 1, 1},
+    {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
+    {&__pyx_n_s_parse, __pyx_k_parse, sizeof(__pyx_k_parse), 0, 0, 1, 1},
+    {&__pyx_n_s_parse_current_table, __pyx_k_parse_current_table, sizeof(__pyx_k_parse_current_table), 0, 0, 1, 1},
+    {&__pyx_n_s_path, __pyx_k_path, sizeof(__pyx_k_path), 0, 0, 1, 1},
+    {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
+    {&__pyx_n_s_platform, __pyx_k_platform, sizeof(__pyx_k_platform), 0, 0, 1, 1},
+    {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
+    {&__pyx_n_s_pyreadr_librdata, __pyx_k_pyreadr_librdata, sizeof(__pyx_k_pyreadr_librdata), 0, 0, 1, 1},
+    {&__pyx_kp_s_pyreadr_librdata_pyx, __pyx_k_pyreadr_librdata_pyx, sizeof(__pyx_k_pyreadr_librdata_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+    {&__pyx_n_s_qualname, __pyx_k_qualname, sizeof(__pyx_k_qualname), 0, 0, 1, 1},
+    {&__pyx_n_u_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 1, 0, 1},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_u_rdata, __pyx_k_rdata, sizeof(__pyx_k_rdata), 0, 1, 0, 1},
+    {&__pyx_n_u_rds, __pyx_k_rds, sizeof(__pyx_k_rds), 0, 1, 0, 1},
+    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+    {&__pyx_n_s_row_count, __pyx_k_row_count, sizeof(__pyx_k_row_count), 0, 0, 1, 1},
+    {&__pyx_n_s_row_no, __pyx_k_row_no, sizeof(__pyx_k_row_no), 0, 0, 1, 1},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_kp_s_self__current_column_self__write, __pyx_k_self__current_column_self__write, sizeof(__pyx_k_self__current_column_self__write), 0, 0, 1, 0},
+    {&__pyx_kp_s_self__this_cannot_be_converted_t, __pyx_k_self__this_cannot_be_converted_t, sizeof(__pyx_k_self__this_cannot_be_converted_t), 0, 0, 1, 0},
+    {&__pyx_n_s_set_name, __pyx_k_set_name, sizeof(__pyx_k_set_name), 0, 0, 1, 1},
+    {&__pyx_n_s_set_row_count, __pyx_k_set_row_count, sizeof(__pyx_k_set_row_count), 0, 0, 1, 1},
+    {&__pyx_n_s_set_table_name, __pyx_k_set_table_name, sizeof(__pyx_k_set_table_name), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_n_s_status, __pyx_k_status, sizeof(__pyx_k_status), 0, 0, 1, 1},
+    {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
+    {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
+    {&__pyx_n_s_system, __pyx_k_system, sizeof(__pyx_k_system), 0, 0, 1, 1},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
+    {&__pyx_n_s_value, __pyx_k_value, sizeof(__pyx_k_value), 0, 0, 1, 1},
+    {&__pyx_n_u_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 1, 0, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 215, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 216, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+  /* "pyreadr/librdata.pyx":7
+ * import numpy as np
+ * import pandas as pd
+ * import os.path             # <<<<<<<<<<<<<<
+ * from cython.operator cimport dereference as deref
+ * from libc.string cimport strlen
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_self__this_cannot_be_converted_t); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_os, __pyx_n_s_path); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "(tree fragment)":4
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+  /* "pyreadr/librdata.pyx":149
+ *     parse_current_table = True
+ * 
+ *     cpdef parse(self, path) noexcept:             # <<<<<<<<<<<<<<
+ * 
+ *         cdef rdata_error_t status
+ */
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_path); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_parse, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 149, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":180
+ *                 raise LibrdataError(message)
+ * 
+ *     def handle_table(self, name):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_name); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_table, 180, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 180, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":183
+ *         pass
+ * 
+ *     def handle_column(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_data_type, __pyx_n_s_data, __pyx_n_s_count); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_column, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 183, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":186
+ *         pass
+ * 
+ *     def handle_column_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_tuple__11 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_index); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_column_name, 186, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 186, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":189
+ *         pass
+ * 
+ *     def handle_dim(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_dim, 189, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 189, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":192
+ *         pass
+ * 
+ *     def handle_dim_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_dim_name, 192, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 192, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":195
+ *         pass
+ * 
+ *     def _handle_row_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_row_name_2, 195, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 195, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":198
+ *         pass
+ * 
+ *     def handle_text_value(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_text_value, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 198, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":201
+ *         pass
+ * 
+ *     def handle_value_label(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_handle_value_label, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 201, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_self__this_cannot_be_converted_t); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  /* "(tree fragment)":2
+  /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_self__this_cannot_be_converted_t); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__20 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "(tree fragment)":4
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")
+  /* "pyreadr/librdata.pyx":283
+ *     cdef rdata_column_t *_this
+ * 
+ *     def add_level_labels(self, labels):             # <<<<<<<<<<<<<<
+ *         for label in labels:
+ *             rdata_column_add_factor(self._this, label.encode('utf-8'))
+ */
+  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_labels, __pyx_n_s_label); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_add_level_labels, 283, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 283, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._this cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_self__this_cannot_be_converted_t); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  /* "(tree fragment)":2
+  /* "(tree fragment)":3
  * def __reduce_cython__(self):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_self__current_column_self__write); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 3, __pyx_L1_error)
 
-  /* "(tree fragment)":4
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")
+  /* "pyreadr/librdata.pyx":307
+ *         self._table_name = b""
+ * 
+ *     def open(self, path, format):             # <<<<<<<<<<<<<<
+ *         cdef rdata_file_format_t fmt;
+ * 
+ */
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_path, __pyx_n_s_format, __pyx_n_s_fmt); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_open, 307, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 307, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":320
+ *         self._fd = _os_open(path, 'w')
+ * 
+ *     def set_row_count(self, row_count):             # <<<<<<<<<<<<<<
+ *         self._row_count = row_count
+ * 
+ */
+  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_row_count); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_set_row_count, 320, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 320, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":323
+ *         self._row_count = row_count
+ * 
+ *     def set_table_name(self, name):             # <<<<<<<<<<<<<<
+ *         self._table_name = name.encode("utf-8")
+ * 
+ */
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_set_table_name, 323, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 323, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":326
+ *         self._table_name = name.encode("utf-8")
+ * 
+ *     def close(self):             # <<<<<<<<<<<<<<
+ *         if self._writer != NULL:
+ *             if self._current_column_no != -1:
+ */
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_close, 326, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 326, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":334
+ *             _os_close(self._fd)
+ * 
+ *     def insert_value(self, row_no, col_no, value, dtype):             # <<<<<<<<<<<<<<
+ *         cdef rdata_error_t status;
+ * 
+ */
+  __pyx_tuple__32 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_row_no, __pyx_n_s_col_no, __pyx_n_s_value, __pyx_n_s_dtype, __pyx_n_s_status); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_insert_value, 334, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 334, __pyx_L1_error)
+
+  /* "pyreadr/librdata.pyx":370
+ * 
+ * 
+ *     def add_column(self, name, dtype):             # <<<<<<<<<<<<<<
+ *         cdef rdata_type_t data_type
+ *         cdef rdata_column_t* column
+ */
+  __pyx_tuple__34 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_name, __pyx_n_s_dtype, __pyx_n_s_data_type, __pyx_n_s_column, __pyx_n_s_col); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pyreadr_librdata_pyx, __pyx_n_s_add_column, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 370, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("self._current_column,self._writer cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_self__current_column_self__write); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
+ */
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_globals ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  return 0;
+}
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -9002,53 +11894,95 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_7pyreadr_8librdata_Parser = &__pyx_vtable_7pyreadr_8librdata_Parser;
   __pyx_vtable_7pyreadr_8librdata_Parser.parse = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, PyObject *, int __pyx_skip_dispatch))__pyx_f_7pyreadr_8librdata_6Parser_parse;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_table = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *))__pyx_f_7pyreadr_8librdata_6Parser___handle_table;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_column = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long))__pyx_f_7pyreadr_8librdata_6Parser___handle_column;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_column_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser___handle_column_name;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_dim = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long))__pyx_f_7pyreadr_8librdata_6Parser___handle_dim;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_dim_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser___handle_dim_name;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_row_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser___handle_row_name;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_text_value = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser___handle_text_value;
-  __pyx_vtable_7pyreadr_8librdata_Parser.__pyx___handle_value_label = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser___handle_value_label;
-  if (PyType_Ready(&__pyx_type_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pyreadr_8librdata_Parser.tp_print = 0;
-  #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyreadr_8librdata_Parser.tp_dictoffset && __pyx_type_7pyreadr_8librdata_Parser.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pyreadr_8librdata_Parser.tp_getattro = __Pyx_PyObject_GenericGetAttr;
-  }
-  if (__Pyx_SetVtable(__pyx_type_7pyreadr_8librdata_Parser.tp_dict, __pyx_vtabptr_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *)&__pyx_type_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_table = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_table;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_column = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_column_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_column_name;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_dim = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, enum rdata_type_e, void *, long))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_dim_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_dim_name;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_row_name = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_row_name;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_text_value = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_text_value;
+  __pyx_vtable_7pyreadr_8librdata_Parser._Parser__handle_value_label = (PyObject *(*)(struct __pyx_obj_7pyreadr_8librdata_Parser *, char const *, int))__pyx_f_7pyreadr_8librdata_6Parser__Parser__handle_value_label;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_7pyreadr_8librdata_Parser = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7pyreadr_8librdata_Parser_spec, NULL); if (unlikely(!__pyx_ptype_7pyreadr_8librdata_Parser)) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7pyreadr_8librdata_Parser_spec, __pyx_ptype_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #else
   __pyx_ptype_7pyreadr_8librdata_Parser = &__pyx_type_7pyreadr_8librdata_Parser;
-  if (PyType_Ready(&__pyx_type_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pyreadr_8librdata_Column.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyreadr_8librdata_Column.tp_dictoffset && __pyx_type_7pyreadr_8librdata_Column.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pyreadr_8librdata_Column.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_7pyreadr_8librdata_Parser->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7pyreadr_8librdata_Parser->tp_dictoffset && __pyx_ptype_7pyreadr_8librdata_Parser->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_7pyreadr_8librdata_Parser->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Column, (PyObject *)&__pyx_type_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
+  #endif
+  if (__Pyx_SetVtable(__pyx_ptype_7pyreadr_8librdata_Parser, __pyx_vtabptr_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_MergeVtables(__pyx_ptype_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *) __pyx_ptype_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_7pyreadr_8librdata_Parser) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_7pyreadr_8librdata_Column = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7pyreadr_8librdata_Column_spec, NULL); if (unlikely(!__pyx_ptype_7pyreadr_8librdata_Column)) __PYX_ERR(0, 280, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7pyreadr_8librdata_Column_spec, __pyx_ptype_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  #else
   __pyx_ptype_7pyreadr_8librdata_Column = &__pyx_type_7pyreadr_8librdata_Column;
-  if (PyType_Ready(&__pyx_type_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pyreadr_8librdata_Writer.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pyreadr_8librdata_Writer.tp_dictoffset && __pyx_type_7pyreadr_8librdata_Writer.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pyreadr_8librdata_Writer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_7pyreadr_8librdata_Column->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7pyreadr_8librdata_Column->tp_dictoffset && __pyx_ptype_7pyreadr_8librdata_Column->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_7pyreadr_8librdata_Column->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *)&__pyx_type_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Column, (PyObject *) __pyx_ptype_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_7pyreadr_8librdata_Column) < 0) __PYX_ERR(0, 280, __pyx_L1_error)
+  #endif
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_7pyreadr_8librdata_Writer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7pyreadr_8librdata_Writer_spec, NULL); if (unlikely(!__pyx_ptype_7pyreadr_8librdata_Writer)) __PYX_ERR(0, 288, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7pyreadr_8librdata_Writer_spec, __pyx_ptype_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  #else
   __pyx_ptype_7pyreadr_8librdata_Writer = &__pyx_type_7pyreadr_8librdata_Writer;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_7pyreadr_8librdata_Writer->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7pyreadr_8librdata_Writer->tp_dictoffset && __pyx_ptype_7pyreadr_8librdata_Writer->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_7pyreadr_8librdata_Writer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Writer, (PyObject *) __pyx_ptype_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_7pyreadr_8librdata_Writer) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -9073,14 +12007,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_librdata(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_librdata},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "librdata",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -9123,42 +12106,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -9166,31 +12163,65 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_librdata(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'librdata' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("librdata", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to librdata pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -9201,327 +12232,623 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("librdata", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyreadr__librdata) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pyreadr.librdata")) {
-      if (unlikely(PyDict_SetItemString(modules, "pyreadr.librdata", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "pyreadr.librdata", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "pyreadr/librdata.pyx":3
  * # cython: c_string_type=str, c_string_encoding=utf8, language_level=3
  * 
+ * import platform             # <<<<<<<<<<<<<<
+ * from enum import Enum
+ * import numpy as np
+ */
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_platform, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_platform, __pyx_t_2) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pyreadr/librdata.pyx":4
+ * 
+ * import platform
  * from enum import Enum             # <<<<<<<<<<<<<<
  * import numpy as np
  * import pandas as pd
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Enum);
   __Pyx_GIVEREF(__pyx_n_s_Enum);
-  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Enum);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Enum);
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_enum, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Enum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Enum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Enum, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Enum, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":4
- * 
+  /* "pyreadr/librdata.pyx":5
+ * import platform
  * from enum import Enum
  * import numpy as np             # <<<<<<<<<<<<<<
  * import pandas as pd
  * import os.path
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_3) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":5
+  /* "pyreadr/librdata.pyx":6
  * from enum import Enum
  * import numpy as np
  * import pandas as pd             # <<<<<<<<<<<<<<
  * import os.path
  * from cython.operator cimport dereference as deref
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_pandas, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_ImportDottedModule(__pyx_n_s_pandas, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":6
+  /* "pyreadr/librdata.pyx":7
  * import numpy as np
  * import pandas as pd
  * import os.path             # <<<<<<<<<<<<<<
  * from cython.operator cimport dereference as deref
  * from libc.string cimport strlen
  */
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_os_path, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_2) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_os_path, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_os, __pyx_t_3) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":10
+  /* "pyreadr/librdata.pyx":11
  * from libc.string cimport strlen
  * 
  * from .custom_errors import PyreadrError, LibrdataError             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyList_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_PyreadrError);
   __Pyx_GIVEREF(__pyx_n_s_PyreadrError);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PyreadrError);
+  PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_PyreadrError);
   __Pyx_INCREF(__pyx_n_s_LibrdataError);
   __Pyx_GIVEREF(__pyx_n_s_LibrdataError);
-  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_s_LibrdataError);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_custom_errors, __pyx_t_2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PyreadrError, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_LibrdataError);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_custom_errors, __pyx_t_3, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LibrdataError, __pyx_t_2) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_PyreadrError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_PyreadrError, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_LibrdataError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LibrdataError, __pyx_t_3) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pyreadr/librdata.pyx":13
+  /* "pyreadr/librdata.pyx":14
  * 
  * 
  * class DataType(Enum):             # <<<<<<<<<<<<<<
  *     CHARACTER  = rdata_type_t.RDATA_TYPE_STRING
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Enum); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Enum); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
-  __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_2, __pyx_n_s_DataType, __pyx_n_s_DataType, (PyObject *) NULL, __pyx_n_s_pyreadr_librdata, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 13, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PEP560_update_bases(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_2, __pyx_n_s_DataType, __pyx_n_s_DataType, (PyObject *) NULL, __pyx_n_s_pyreadr_librdata, (PyObject *) NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  if (__pyx_t_2 != __pyx_t_3) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_3) < 0))) __PYX_ERR(0, 14, __pyx_L1_error)
+  }
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":14
+  /* "pyreadr/librdata.pyx":15
  * 
  * class DataType(Enum):
  *     CHARACTER  = rdata_type_t.RDATA_TYPE_STRING             # <<<<<<<<<<<<<<
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
  *     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_STRING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 14, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_CHARACTER, __pyx_t_4) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_CHARACTER, __pyx_t_3) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":15
+  /* "pyreadr/librdata.pyx":16
  * class DataType(Enum):
  *     CHARACTER  = rdata_type_t.RDATA_TYPE_STRING
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32             # <<<<<<<<<<<<<<
  *     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL
  *     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_INT32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_INTEGER, __pyx_t_4) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_INT32); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_INTEGER, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":16
+  /* "pyreadr/librdata.pyx":17
  *     CHARACTER  = rdata_type_t.RDATA_TYPE_STRING
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
  *     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL             # <<<<<<<<<<<<<<
  *     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL
  *     TIMESTAMP  = rdata_type_t.RDATA_TYPE_TIMESTAMP
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_REAL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_NUMERIC, __pyx_t_4) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_REAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_NUMERIC, __pyx_t_3) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":17
+  /* "pyreadr/librdata.pyx":18
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
  *     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL
  *     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL             # <<<<<<<<<<<<<<
  *     TIMESTAMP  = rdata_type_t.RDATA_TYPE_TIMESTAMP
  *     DATE       = rdata_type_t.RDATA_TYPE_DATE
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_LOGICAL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_LOGICAL, __pyx_t_4) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_LOGICAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_LOGICAL, __pyx_t_3) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":18
+  /* "pyreadr/librdata.pyx":19
  *     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL
  *     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL
  *     TIMESTAMP  = rdata_type_t.RDATA_TYPE_TIMESTAMP             # <<<<<<<<<<<<<<
  *     DATE       = rdata_type_t.RDATA_TYPE_DATE
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_TIMESTAMP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_TIMESTAMP, __pyx_t_4) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_TIMESTAMP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_TIMESTAMP, __pyx_t_3) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":19
+  /* "pyreadr/librdata.pyx":20
  *     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL
  *     TIMESTAMP  = rdata_type_t.RDATA_TYPE_TIMESTAMP
  *     DATE       = rdata_type_t.RDATA_TYPE_DATE             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_DATE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_DATE, __pyx_t_4) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_enum__rdata_type_e(RDATA_TYPE_DATE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_DATE, __pyx_t_3) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pyreadr/librdata.pyx":13
+  /* "pyreadr/librdata.pyx":14
  * 
  * 
  * class DataType(Enum):             # <<<<<<<<<<<<<<
  *     CHARACTER  = rdata_type_t.RDATA_TYPE_STRING
  *     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_DataType, __pyx_t_2, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataType, __pyx_t_4) < 0) __PYX_ERR(0, 13, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_DataType, __pyx_t_2, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_DataType, __pyx_t_3) < 0) __PYX_ERR(0, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pyreadr/librdata.pyx":146
+  /* "pyreadr/librdata.pyx":147
  *     cdef int _row_count
  *     cdef int _var_count
  *     parse_current_table = True             # <<<<<<<<<<<<<<
  * 
- *     cpdef parse(self, path):
+ *     cpdef parse(self, path) noexcept:
  */
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_parse_current_table, Py_True) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_parse_current_table, Py_True) < 0) __PYX_ERR(0, 147, __pyx_L1_error)
   PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
 
+  /* "pyreadr/librdata.pyx":149
+ *     parse_current_table = True
+ * 
+ *     cpdef parse(self, path) noexcept:             # <<<<<<<<<<<<<<
+ * 
+ *         cdef rdata_error_t status
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_1parse, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_parse, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_parse, __pyx_t_2) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":180
+ *                 raise LibrdataError(message)
+ * 
+ *     def handle_table(self, name):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_3handle_table, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_table, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_table, __pyx_t_2) < 0) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":183
+ *         pass
+ * 
+ *     def handle_column(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_5handle_column, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_column, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_column, __pyx_t_2) < 0) __PYX_ERR(0, 183, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":186
+ *         pass
+ * 
+ *     def handle_column_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_7handle_column_name, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_column_name, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_column_name, __pyx_t_2) < 0) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":189
+ *         pass
+ * 
+ *     def handle_dim(self, name, data_type, data, count):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_9handle_dim, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_dim, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_dim, __pyx_t_2) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":192
+ *         pass
+ * 
+ *     def handle_dim_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_11handle_dim_name, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_dim_name, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_dim_name, __pyx_t_2) < 0) __PYX_ERR(0, 192, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":195
+ *         pass
+ * 
+ *     def _handle_row_name(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_13_handle_row_name, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser__handle_row_name, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_row_name_2, __pyx_t_2) < 0) __PYX_ERR(0, 195, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":198
+ *         pass
+ * 
+ *     def handle_text_value(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_15handle_text_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_text_value, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_text_value, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "pyreadr/librdata.pyx":201
+ *         pass
+ * 
+ *     def handle_value_label(self, name, index):             # <<<<<<<<<<<<<<
+ *         pass
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_17handle_value_label, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_handle_value_label, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Parser->tp_dict, __pyx_n_s_handle_value_label, __pyx_t_2) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Parser);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_19__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser___reduce_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Parser_21__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser___setstate_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pyreadr/librdata.pyx":283
+ *     cdef rdata_column_t *_this
+ * 
+ *     def add_level_labels(self, labels):             # <<<<<<<<<<<<<<
+ *         for label in labels:
+ *             rdata_column_add_factor(self._this, label.encode('utf-8'))
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Column_1add_level_labels, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Column_add_level_labels, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Column->tp_dict, __pyx_n_s_add_level_labels, __pyx_t_2) < 0) __PYX_ERR(0, 283, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Column);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Column_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Column___reduce_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._this cannot be converted to a Python object for pickling"
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Column_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Column___setstate_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "pyreadr/librdata.pyx":307
+ *         self._table_name = b""
+ * 
+ *     def open(self, path, format):             # <<<<<<<<<<<<<<
+ *         cdef rdata_file_format_t fmt;
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_3open, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_open, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 307, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_open, __pyx_t_2) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "pyreadr/librdata.pyx":320
+ *         self._fd = _os_open(path, 'w')
+ * 
+ *     def set_row_count(self, row_count):             # <<<<<<<<<<<<<<
+ *         self._row_count = row_count
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_5set_row_count, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_set_row_count, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_set_row_count, __pyx_t_2) < 0) __PYX_ERR(0, 320, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "pyreadr/librdata.pyx":323
+ *         self._row_count = row_count
+ * 
+ *     def set_table_name(self, name):             # <<<<<<<<<<<<<<
+ *         self._table_name = name.encode("utf-8")
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_7set_table_name, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_set_table_name, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_set_table_name, __pyx_t_2) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "pyreadr/librdata.pyx":326
+ *         self._table_name = name.encode("utf-8")
+ * 
+ *     def close(self):             # <<<<<<<<<<<<<<
+ *         if self._writer != NULL:
+ *             if self._current_column_no != -1:
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_9close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_close, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_close, __pyx_t_2) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "pyreadr/librdata.pyx":334
+ *             _os_close(self._fd)
+ * 
+ *     def insert_value(self, row_no, col_no, value, dtype):             # <<<<<<<<<<<<<<
+ *         cdef rdata_error_t status;
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_11insert_value, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_insert_value, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_insert_value, __pyx_t_2) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "pyreadr/librdata.pyx":370
+ * 
+ * 
+ *     def add_column(self, name, dtype):             # <<<<<<<<<<<<<<
+ *         cdef rdata_type_t data_type
+ *         cdef rdata_column_t* column
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_13add_column, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer_add_column, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pyreadr_8librdata_Writer->tp_dict, __pyx_n_s_add_column, __pyx_t_2) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pyreadr_8librdata_Writer);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_15__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer___reduce_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "self._current_column,self._writer cannot be converted to a Python object for pickling"
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pyreadr_8librdata_6Writer_17__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Writer___setstate_cython, NULL, __pyx_n_s_pyreadr_librdata, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "pyreadr/librdata.pyx":1
  * # cython: c_string_type=str, c_string_encoding=utf8, language_level=3             # <<<<<<<<<<<<<<
  * 
- * from enum import Enum
+ * import platform
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init pyreadr.librdata", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init pyreadr.librdata");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -9533,255 +12860,162 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* PyObjectGetAttrStr */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro))
-        return tp->tp_getattro(obj, attr_name);
-#if PY_MAJOR_VERSION < 3
-    if (likely(tp->tp_getattr))
-        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
-#endif
-    return PyObject_GetAttr(obj, attr_name);
-}
-#endif
-
-/* GetBuiltinName */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
-        PyErr_Format(PyExc_NameError,
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
-            "name '%U' is not defined", name);
-#else
-            "name '%.200s' is not defined", PyString_AS_STRING(name));
-#endif
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
     }
-    return result;
-}
-
-/* BytesEquals */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-    if (s1 == s2) {
-        return (equals == Py_EQ);
-    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
-        const char *ps1, *ps2;
-        Py_ssize_t length = PyBytes_GET_SIZE(s1);
-        if (length != PyBytes_GET_SIZE(s2))
-            return (equals == Py_NE);
-        ps1 = PyBytes_AS_STRING(s1);
-        ps2 = PyBytes_AS_STRING(s2);
-        if (ps1[0] != ps2[0]) {
-            return (equals == Py_NE);
-        } else if (length == 1) {
-            return (equals == Py_EQ);
-        } else {
-            int result;
-#if CYTHON_USE_UNICODE_INTERNALS
-            Py_hash_t hash1, hash2;
-            hash1 = ((PyBytesObject*)s1)->ob_shash;
-            hash2 = ((PyBytesObject*)s2)->ob_shash;
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                return (equals == Py_NE);
-            }
 #endif
-            result = memcmp(ps1, ps2, (size_t)length);
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
-        return (equals == Py_NE);
-    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
-        return (equals == Py_NE);
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
     }
-#endif
+    return 0;
 }
-
-/* UnicodeEquals */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
 #else
-#if PY_MAJOR_VERSION < 3
-    PyObject* owned_ref = NULL;
-#endif
-    int s1_is_unicode, s2_is_unicode;
-    if (s1 == s2) {
-        goto return_eq;
-    }
-    s1_is_unicode = PyUnicode_CheckExact(s1);
-    s2_is_unicode = PyUnicode_CheckExact(s2);
-#if PY_MAJOR_VERSION < 3
-    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
-        owned_ref = PyUnicode_FromObject(s2);
-        if (unlikely(!owned_ref))
-            return -1;
-        s2 = owned_ref;
-        s2_is_unicode = 1;
-    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
-        owned_ref = PyUnicode_FromObject(s1);
-        if (unlikely(!owned_ref))
-            return -1;
-        s1 = owned_ref;
-        s1_is_unicode = 1;
-    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
-        return __Pyx_PyBytes_Equals(s1, s2, equals);
-    }
-#endif
-    if (s1_is_unicode & s2_is_unicode) {
-        Py_ssize_t length;
-        int kind;
-        void *data1, *data2;
-        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
-            return -1;
-        length = __Pyx_PyUnicode_GET_LENGTH(s1);
-        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
-            goto return_ne;
-        }
-#if CYTHON_USE_UNICODE_INTERNALS
-        {
-            Py_hash_t hash1, hash2;
-        #if CYTHON_PEP393_ENABLED
-            hash1 = ((PyASCIIObject*)s1)->hash;
-            hash2 = ((PyASCIIObject*)s2)->hash;
-        #else
-            hash1 = ((PyUnicodeObject*)s1)->hash;
-            hash2 = ((PyUnicodeObject*)s2)->hash;
-        #endif
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                goto return_ne;
-            }
-        }
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
 #endif
-        kind = __Pyx_PyUnicode_KIND(s1);
-        if (kind != __Pyx_PyUnicode_KIND(s2)) {
-            goto return_ne;
-        }
-        data1 = __Pyx_PyUnicode_DATA(s1);
-        data2 = __Pyx_PyUnicode_DATA(s2);
-        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
-            goto return_ne;
-        } else if (length == 1) {
-            goto return_eq;
-        } else {
-            int result = memcmp(data1, data2, (size_t)(length * kind));
-            #if PY_MAJOR_VERSION < 3
-            Py_XDECREF(owned_ref);
-            #endif
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & s2_is_unicode) {
-        goto return_ne;
-    } else if ((s2 == Py_None) & s1_is_unicode) {
-        goto return_ne;
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
     } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        #if PY_MAJOR_VERSION < 3
-        Py_XDECREF(owned_ref);
-        #endif
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
     }
-return_eq:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_EQ);
-return_ne:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
     #endif
-    return (equals == Py_NE);
-#endif
+    return result;
 }
+#endif
 
 /* PyErrFetchRestore */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
     tstate->curexc_traceback = tb;
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
+#endif
 }
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
     *type = tstate->curexc_type;
     *value = tstate->curexc_value;
     *tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+#endif
 }
 #endif
 
-/* WriteUnraisableException */
-static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
-                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
-                                  int full_traceback, CYTHON_UNUSED int nogil) {
-    PyObject *old_exc, *old_val, *old_tb;
-    PyObject *ctx;
-    __Pyx_PyThreadState_declare
-#ifdef WITH_THREAD
-    PyGILState_STATE state;
-    if (nogil)
-        state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
+/* PyObjectGetAttrStr */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro))
+        return tp->tp_getattro(obj, attr_name);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_getattr))
+        return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
+    return PyObject_GetAttr(obj, attr_name);
+}
 #endif
+
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
-    if (full_traceback) {
-        Py_XINCREF(old_exc);
-        Py_XINCREF(old_val);
-        Py_XINCREF(old_tb);
-        __Pyx_ErrRestore(old_exc, old_val, old_tb);
-        PyErr_PrintEx(1);
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
-    #if PY_MAJOR_VERSION < 3
-    ctx = PyString_FromString(name);
-    #else
-    ctx = PyUnicode_FromString(name);
-    #endif
-    __Pyx_ErrRestore(old_exc, old_val, old_tb);
-    if (!ctx) {
-        PyErr_WriteUnraisable(Py_None);
-    } else {
-        PyErr_WriteUnraisable(ctx);
-        Py_DECREF(ctx);
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
-#ifdef WITH_THREAD
-    if (nogil)
-        PyGILState_Release(state);
+    return result;
+}
+
+/* GetBuiltinName */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
+        PyErr_Format(PyExc_NameError,
+#if PY_MAJOR_VERSION >= 3
+            "name '%U' is not defined", name);
+#else
+            "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
+    }
+    return result;
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -9819,14 +13053,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -9837,39 +13079,16 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* PyCFunctionFastCall */
-#if CYTHON_FAST_PYCCALL
-static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
-    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
-    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
-    PyObject *self = PyCFunction_GET_SELF(func);
-    int flags = PyCFunction_GET_FLAGS(func);
-    assert(PyCFunction_Check(func));
-    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
-    assert(nargs >= 0);
-    assert(nargs == 0 || args != NULL);
-    /* _PyCFunction_FastCallDict() must not be called with an exception set,
-       because it may clear it (directly or indirectly) and so the
-       caller loses its exception */
-    assert(!PyErr_Occurred());
-    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
-        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
-    } else {
-        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
-    }
-}
-#endif
-
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -9890,15 +13109,14 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
-#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -9906,15 +13124,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -9977,21 +13195,20 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
-#endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -9999,43 +13216,14 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCall2Args */
-static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
-    PyObject *args, *result = NULL;
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyFunction_FastCall(function, args, 2);
-    }
-    #endif
-    #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(function)) {
-        PyObject *args[2] = {arg1, arg2};
-        return __Pyx_PyCFunction_FastCall(function, args, 2);
-    }
-    #endif
-    args = PyTuple_New(2);
-    if (unlikely(!args)) goto done;
-    Py_INCREF(arg1);
-    PyTuple_SET_ITEM(args, 0, arg1);
-    Py_INCREF(arg2);
-    PyTuple_SET_ITEM(args, 1, arg2);
-    Py_INCREF(function);
-    result = __Pyx_PyObject_Call(function, args, NULL);
-    Py_DECREF(args);
-    Py_DECREF(function);
-done:
-    return result;
-}
-
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
     cfunc = PyCFunction_GET_FUNCTION(func);
     self = PyCFunction_GET_SELF(func);
@@ -10048,87 +13236,342 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectCallOneArg */
-#if CYTHON_COMPILING_IN_CPYTHON
-static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+/* PyObjectFastCall */
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
     PyObject *result;
-    PyObject *args = PyTuple_New(1);
-    if (unlikely(!args)) return NULL;
-    Py_INCREF(arg);
-    PyTuple_SET_ITEM(args, 0, arg);
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
     return result;
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, &arg, 1);
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
+#endif
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
     }
 #endif
-    if (likely(PyCFunction_Check(func))) {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-            return __Pyx_PyObject_CallMethO(func, arg);
-#if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
-            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+}
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
 #endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
         }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
     }
-    return __Pyx__PyObject_CallOneArg(func, arg);
+#endif
 }
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
 #else
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *result;
-    PyObject *args = PyTuple_Pack(1, arg);
-    if (unlikely(!args)) return NULL;
-    result = __Pyx_PyObject_Call(func, args, NULL);
-    Py_DECREF(args);
-    return result;
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
 }
+
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
 #endif
+    CYTHON_UNUSED_VAR(clineno);
+    CYTHON_UNUSED_VAR(lineno);
+    CYTHON_UNUSED_VAR(filename);
+    CYTHON_MAYBE_UNUSED_VAR(nogil);
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
 
 /* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
            exc_info->previous_item != NULL)
     {
         exc_info = exc_info->previous_item;
     }
     return exc_info;
 }
 #endif
 
 /* SaveResetException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
     *type = exc_info->exc_type;
     *value = exc_info->exc_value;
     *tb = exc_info->exc_traceback;
-    #else
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
     *type = tstate->exc_type;
     *value = tstate->exc_value;
     *tb = tstate->exc_traceback;
-    #endif
     Py_XINCREF(*type);
     Py_XINCREF(*value);
     Py_XINCREF(*tb);
+  #endif
 }
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = type;
@@ -10141,63 +13584,51 @@
     tstate->exc_type = type;
     tstate->exc_value = value;
     tstate->exc_traceback = tb;
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
-}
-#endif
-
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+  #endif
 }
 #endif
 
 /* GetException */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
 #endif
 {
-    PyObject *local_type, *local_value, *local_tb;
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
 #if CYTHON_FAST_THREAD_STATE
     PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
     local_type = tstate->curexc_type;
     local_value = tstate->curexc_value;
     local_tb = tstate->curexc_traceback;
     tstate->curexc_type = 0;
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
+  #endif
 #else
     PyErr_Fetch(&local_type, &local_value, &local_tb);
 #endif
     PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
     if (unlikely(tstate->curexc_type))
 #else
     if (unlikely(PyErr_Occurred()))
 #endif
         goto bad;
     #if PY_MAJOR_VERSION >= 3
     if (local_tb) {
@@ -10211,20 +13642,29 @@
     *type = local_type;
     *value = local_value;
     *tb = local_tb;
 #if CYTHON_FAST_THREAD_STATE
     #if CYTHON_USE_EXC_INFO_STACK
     {
         _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
         tmp_type = exc_info->exc_type;
         tmp_value = exc_info->exc_value;
         tmp_tb = exc_info->exc_traceback;
         exc_info->exc_type = local_type;
         exc_info->exc_value = local_value;
         exc_info->exc_traceback = local_tb;
+      #endif
     }
     #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = local_type;
     tstate->exc_value = local_value;
@@ -10261,30 +13701,49 @@
 }
 #endif
 
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_value = exc_info->exc_value;
+    exc_info->exc_value = *value;
+    if (tmp_value == NULL || tmp_value == Py_None) {
+        Py_XDECREF(tmp_value);
+        tmp_value = NULL;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+    } else {
+        tmp_type = (PyObject*) Py_TYPE(tmp_value);
+        Py_INCREF(tmp_type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        tmp_tb = ((PyBaseExceptionObject*) tmp_value)->traceback;
+        Py_XINCREF(tmp_tb);
+        #else
+        tmp_tb = PyException_GetTraceback(tmp_value);
+        #endif
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
     tmp_value = exc_info->exc_value;
     tmp_tb = exc_info->exc_traceback;
     exc_info->exc_type = *type;
     exc_info->exc_value = *value;
     exc_info->exc_traceback = *tb;
-    #else
+  #else
     tmp_type = tstate->exc_type;
     tmp_value = tstate->exc_value;
     tmp_tb = tstate->exc_traceback;
     tstate->exc_type = *type;
     tstate->exc_value = *value;
     tstate->exc_traceback = *tb;
-    #endif
+  #endif
     *type = tmp_type;
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
@@ -10294,17 +13753,17 @@
     *value = tmp_value;
     *tb = tmp_tb;
 }
 #endif
 
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
     __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -10429,61 +13888,95 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* RaiseArgTupleInvalid */
-static void __Pyx_RaiseArgtupleInvalid(
-    const char* func_name,
-    int exact,
-    Py_ssize_t num_min,
-    Py_ssize_t num_max,
-    Py_ssize_t num_found)
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
 {
-    Py_ssize_t num_expected;
-    const char *more_or_less;
-    if (num_found < num_min) {
-        num_expected = num_min;
-        more_or_less = "at least";
-    } else {
-        num_expected = num_max;
-        more_or_less = "at most";
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
-    if (exact) {
-        more_or_less = "exactly";
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
     }
-    PyErr_Format(PyExc_TypeError,
-                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                 func_name, more_or_less, num_expected,
-                 (num_expected == 1) ? "" : "s", num_found);
+    return NULL;  // not found (no exception set)
 }
+#endif
 
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
@@ -10494,25 +13987,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -10538,19 +14043,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -10581,30 +14087,57 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* RaiseArgTupleInvalid */
+static void __Pyx_RaiseArgtupleInvalid(
+    const char* func_name,
+    int exact,
+    Py_ssize_t num_min,
+    Py_ssize_t num_max,
+    Py_ssize_t num_found)
+{
+    Py_ssize_t num_expected;
+    const char *more_or_less;
+    if (num_found < num_min) {
+        num_expected = num_min;
+        more_or_less = "at least";
+    } else {
+        num_expected = num_max;
+        more_or_less = "at most";
+    }
+    if (exact) {
+        more_or_less = "exactly";
+    }
+    PyErr_Format(PyExc_TypeError,
+                 "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                 func_name, more_or_less, num_expected,
+                 (num_expected == 1) ? "" : "s", num_found);
+}
+
 /* SetItemInt */
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
     int r;
-    if (!j) return -1;
+    if (unlikely(!j)) return -1;
     r = PyObject_SetItem(o, j, v);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
                                                CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
@@ -10614,27 +14147,36 @@
             PyObject* old = PyList_GET_ITEM(o, n);
             Py_INCREF(v);
             PyList_SET_ITEM(o, n, v);
             Py_DECREF(old);
             return 1;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_ass_subscript) {
+            int r;
+            PyObject *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return -1;
+            r = mm->mp_ass_subscript(o, key, v);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_ass_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return -1;
                     PyErr_Clear();
                 }
             }
-            return m->sq_ass_item(o, i, v);
+            return sm->sq_ass_item(o, i, v);
         }
     }
 #else
 #if CYTHON_COMPILING_IN_PYPY
     if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
 #else
     if (is_list || PySequence_Check(o))
@@ -10644,85 +14186,419 @@
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
 /* KeywordStringCheck */
 static int __Pyx_CheckKeywordStrings(
-    PyObject *kwdict,
+    PyObject *kw,
     const char* function_name,
     int kw_allowed)
 {
     PyObject* key = 0;
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
-    if (!kw_allowed && PyDict_Next(kwdict, &pos, &key, 0))
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
         goto invalid_keyword;
     return 1;
 #else
-    while (PyDict_Next(kwdict, &pos, &key, 0)) {
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
+            return 1;
+        if (!kw_allowed) {
+            key = PyTuple_GET_ITEM(kw, 0);
+            goto invalid_keyword;
+        }
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
+            key = PyTuple_GET_ITEM(kw, pos);
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+        }
+#endif
+        return 1;
+    }
+    while (PyDict_Next(kw, &pos, &key, 0)) {
         #if PY_MAJOR_VERSION < 3
         if (unlikely(!PyString_Check(key)))
         #endif
             if (unlikely(!PyUnicode_Check(key)))
                 goto invalid_keyword_type;
     }
-    if ((!kw_allowed) && unlikely(key))
+    if (!kw_allowed && unlikely(key))
         goto invalid_keyword;
     return 1;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     return 0;
 #endif
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
     return 0;
 }
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
 /* PyObjectCallNoArg */
-#if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-#if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCall(func, NULL, 0);
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* FixUpExtensionType */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
+#else
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
+                }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
+            }
+            memb++;
+        }
+        if (changed)
+            PyType_Modified(type);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
-    if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
+    return 0;
+}
+#endif
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
 #else
-    if (likely(PyCFunction_Check(func)))
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
 #endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    for (i = 1; i < n; i++)
     {
-        if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-            return __Pyx_PyObject_CallMethO(func, NULL);
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
         }
     }
-    return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
+    return 0;
 }
 #endif
 
+/* PyType_Ready */
+static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
+    #else
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+    #endif
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
+#else
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
+#endif
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -10755,58 +14631,110 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
-#if PY_VERSION_HEX >= 0x02070000
+static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
+    if (unlikely(!ob))
+        goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
 #else
-    PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
+    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
 #endif
-    if (!ob)
-        goto bad;
-    if (PyDict_SetItem(dict, __pyx_n_s_pyx_vtable, ob) < 0)
         goto bad;
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
+/* GetVTable */
+static void* __Pyx_GetVtable(PyTypeObject *type) {
+    void* ptr;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
+#else
+    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
 #endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    if (!ob)
+        goto bad;
+    ptr = PyCapsule_GetPointer(ob, 0);
+    if (!ptr && !PyErr_Occurred())
+        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
+    Py_DECREF(ob);
+    return ptr;
+bad:
+    Py_XDECREF(ob);
+    return NULL;
+}
+
+/* MergeVTables */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type) {
+    int i;
+    void** base_vtables;
+    __Pyx_TypeName tp_base_name;
+    __Pyx_TypeName base_name;
+    void* unknown = (void*)-1;
+    PyObject* bases = type->tp_bases;
+    int base_depth = 0;
+    {
+        PyTypeObject* base = type->tp_base;
+        while (base) {
+            base_depth += 1;
+            base = base->tp_base;
+        }
+    }
+    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
+    base_vtables[0] = unknown;
+    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
+        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
+        if (base_vtable != NULL) {
+            int j;
+            PyTypeObject* base = type->tp_base;
+            for (j = 0; j < base_depth; j++) {
+                if (base_vtables[j] == unknown) {
+                    base_vtables[j] = __Pyx_GetVtable(base);
+                    base_vtables[j + 1] = unknown;
+                }
+                if (base_vtables[j] == base_vtable) {
+                    break;
+                } else if (base_vtables[j] == NULL) {
+                    goto bad;
+                }
+                base = base->tp_base;
+            }
+        }
     }
-    return result;
+    PyErr_Clear();
+    free(base_vtables);
+    return 0;
+bad:
+    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
+    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
+    PyErr_Format(PyExc_TypeError,
+        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
+    __Pyx_DECREF_TypeName(tp_base_name);
+    __Pyx_DECREF_TypeName(base_name);
+    free(base_vtables);
+    return -1;
 }
+#endif
 
 /* SetupReduce */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
+  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
   }
   if (unlikely(ret < 0)) {
       PyErr_Clear();
@@ -10814,25 +14742,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -10846,15 +14792,15 @@
             reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
             if (likely(reduce_cython)) {
                 ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
             } else if (reduce == object_reduce || PyErr_Occurred()) {
                 goto __PYX_BAD;
             }
-            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
+            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
                 setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
                 if (likely(setstate_cython)) {
                     ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                     ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 } else if (!setstate || PyErr_Occurred()) {
@@ -10862,109 +14808,345 @@
                 }
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
     goto __PYX_GOOD;
 __PYX_BAD:
-    if (!PyErr_Occurred())
-        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
+    if (!PyErr_Occurred()) {
+        __Pyx_TypeName type_obj_name =
+            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
+        PyErr_Format(PyExc_RuntimeError,
+            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
+        __Pyx_DECREF_TypeName(type_obj_name);
+    }
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
+#endif
 
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__2;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
 /* ImportFrom */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
+        const char* module_name_str = 0;
+        PyObject* module_name = 0;
+        PyObject* module_dot = 0;
+        PyObject* full_name = 0;
+        PyErr_Clear();
+        module_name_str = PyModule_GetName(module);
+        if (unlikely(!module_name_str)) { goto modbad; }
+        module_name = PyUnicode_FromString(module_name_str);
+        if (unlikely(!module_name)) { goto modbad; }
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__3);
+        if (unlikely(!module_dot)) { goto modbad; }
+        full_name = PyUnicode_Concat(module_dot, name);
+        if (unlikely(!full_name)) { goto modbad; }
+        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+        {
+            PyObject *modules = PyImport_GetModuleDict();
+            if (unlikely(!modules))
+                goto modbad;
+            value = PyObject_GetItem(modules, full_name);
+        }
+        #else
+        value = PyImport_GetModule(full_name);
+        #endif
+      modbad:
+        Py_XDECREF(full_name);
+        Py_XDECREF(module_dot);
+        Py_XDECREF(module_name);
+    }
+    if (unlikely(!value)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
+/* Py3UpdateBases */
+static PyObject*
+__Pyx_PEP560_update_bases(PyObject *bases)
+{
+    Py_ssize_t i, j, size_bases;
+    PyObject *base, *meth, *new_base, *result, *new_bases = NULL;
+    size_bases = PyTuple_GET_SIZE(bases);
+    for (i = 0; i < size_bases; i++) {
+        base  = PyTuple_GET_ITEM(bases, i);
+        if (PyType_Check(base)) {
+            if (new_bases) {
+                if (PyList_Append(new_bases, base) < 0) {
+                    goto error;
+                }
+            }
+            continue;
+        }
+        meth = __Pyx_PyObject_GetAttrStrNoError(base, __pyx_n_s_mro_entries);
+        if (!meth && PyErr_Occurred()) {
+            goto error;
+        }
+        if (!meth) {
+            if (new_bases) {
+                if (PyList_Append(new_bases, base) < 0) {
+                    goto error;
+                }
+            }
+            continue;
+        }
+        new_base = __Pyx_PyObject_CallOneArg(meth, bases);
+        Py_DECREF(meth);
+        if (!new_base) {
+            goto error;
+        }
+        if (!PyTuple_Check(new_base)) {
+            PyErr_SetString(PyExc_TypeError,
+                            "__mro_entries__ must return a tuple");
+            Py_DECREF(new_base);
+            goto error;
+        }
+        if (!new_bases) {
+            if (!(new_bases = PyList_New(i))) {
+                goto error;
+            }
+            for (j = 0; j < i; j++) {
+                base = PyTuple_GET_ITEM(bases, j);
+                PyList_SET_ITEM(new_bases, j, base);
+                Py_INCREF(base);
+            }
+        }
+        j = PyList_GET_SIZE(new_bases);
+        if (PyList_SetSlice(new_bases, j, j, new_base) < 0) {
+            goto error;
+        }
+        Py_DECREF(new_base);
+    }
+    if (!new_bases) {
+        Py_INCREF(bases);
+        return bases;
+    }
+    result = PyList_AsTuple(new_bases);
+    Py_DECREF(new_bases);
+    return result;
+error:
+    Py_XDECREF(new_bases);
+    return NULL;
+}
+
 /* CalculateMetaclass */
 static PyObject *__Pyx_CalculateMetaclass(PyTypeObject *metaclass, PyObject *bases) {
     Py_ssize_t i, nbases = PyTuple_GET_SIZE(bases);
     for (i=0; i < nbases; i++) {
         PyTypeObject *tmptype;
         PyObject *tmp = PyTuple_GET_ITEM(bases, i);
         tmptype = Py_TYPE(tmp);
@@ -10996,53 +15178,212 @@
         metaclass = &PyType_Type;
 #endif
     }
     Py_INCREF((PyObject*) metaclass);
     return (PyObject*) metaclass;
 }
 
+/* PyObjectCall2Args */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args[3] = {NULL, arg1, arg2};
+    return __Pyx_PyObject_FastCall(function, args+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectLookupSpecial */
+#if CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx__PyObject_LookupSpecial(PyObject* obj, PyObject* attr_name, int with_error) {
+    PyObject *res;
+    PyTypeObject *tp = Py_TYPE(obj);
+#if PY_MAJOR_VERSION < 3
+    if (unlikely(PyInstance_Check(obj)))
+        return with_error ? __Pyx_PyObject_GetAttrStr(obj, attr_name) : __Pyx_PyObject_GetAttrStrNoError(obj, attr_name);
+#endif
+    res = _PyType_Lookup(tp, attr_name);
+    if (likely(res)) {
+        descrgetfunc f = Py_TYPE(res)->tp_descr_get;
+        if (!f) {
+            Py_INCREF(res);
+        } else {
+            res = f(res, obj, (PyObject *)tp);
+        }
+    } else if (with_error) {
+        PyErr_SetObject(PyExc_AttributeError, attr_name);
+    }
+    return res;
+}
+#endif
+
 /* Py3ClassCreate */
 static PyObject *__Pyx_Py3MetaclassPrepare(PyObject *metaclass, PyObject *bases, PyObject *name,
                                            PyObject *qualname, PyObject *mkw, PyObject *modname, PyObject *doc) {
     PyObject *ns;
     if (metaclass) {
-        PyObject *prep = __Pyx_PyObject_GetAttrStr(metaclass, __pyx_n_s_prepare);
+        PyObject *prep = __Pyx_PyObject_GetAttrStrNoError(metaclass, __pyx_n_s_prepare);
         if (prep) {
-            PyObject *pargs = PyTuple_Pack(2, name, bases);
-            if (unlikely(!pargs)) {
-                Py_DECREF(prep);
-                return NULL;
-            }
-            ns = PyObject_Call(prep, pargs, mkw);
+            PyObject *pargs[3] = {NULL, name, bases};
+            ns = __Pyx_PyObject_FastCallDict(prep, pargs+1, 2 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET, mkw);
             Py_DECREF(prep);
-            Py_DECREF(pargs);
         } else {
-            if (unlikely(!PyErr_ExceptionMatches(PyExc_AttributeError)))
+            if (unlikely(PyErr_Occurred()))
                 return NULL;
-            PyErr_Clear();
             ns = PyDict_New();
         }
     } else {
         ns = PyDict_New();
     }
     if (unlikely(!ns))
         return NULL;
     if (unlikely(PyObject_SetItem(ns, __pyx_n_s_module, modname) < 0)) goto bad;
+#if PY_VERSION_HEX >= 0x03030000
     if (unlikely(PyObject_SetItem(ns, __pyx_n_s_qualname, qualname) < 0)) goto bad;
+#else
+    CYTHON_MAYBE_UNUSED_VAR(qualname);
+#endif
     if (unlikely(doc && PyObject_SetItem(ns, __pyx_n_s_doc, doc) < 0)) goto bad;
     return ns;
 bad:
     Py_DECREF(ns);
     return NULL;
 }
+#if PY_VERSION_HEX < 0x030600A4 && CYTHON_PEP487_INIT_SUBCLASS
+static int __Pyx_SetNamesPEP487(PyObject *type_obj) {
+    PyTypeObject *type = (PyTypeObject*) type_obj;
+    PyObject *names_to_set, *key, *value, *set_name, *tmp;
+    Py_ssize_t i = 0;
+#if CYTHON_USE_TYPE_SLOTS
+    names_to_set = PyDict_Copy(type->tp_dict);
+#else
+    {
+        PyObject *d = PyObject_GetAttr(type_obj, __pyx_n_s_dict);
+        names_to_set = NULL;
+        if (likely(d)) {
+            PyObject *names_to_set = PyDict_New();
+            int ret = likely(names_to_set) ? PyDict_Update(names_to_set, d) : -1;
+            Py_DECREF(d);
+            if (unlikely(ret < 0))
+                Py_CLEAR(names_to_set);
+        }
+    }
+#endif
+    if (unlikely(names_to_set == NULL))
+        goto bad;
+    while (PyDict_Next(names_to_set, &i, &key, &value)) {
+        set_name = __Pyx_PyObject_LookupSpecialNoError(value, __pyx_n_s_set_name);
+        if (unlikely(set_name != NULL)) {
+            tmp = __Pyx_PyObject_Call2Args(set_name, type_obj, key);
+            Py_DECREF(set_name);
+            if (unlikely(tmp == NULL)) {
+                __Pyx_TypeName value_type_name =
+                    __Pyx_PyType_GetName(Py_TYPE(value));
+                __Pyx_TypeName type_name = __Pyx_PyType_GetName(type);
+                PyErr_Format(PyExc_RuntimeError,
+#if PY_MAJOR_VERSION >= 3
+                    "Error calling __set_name__ on '" __Pyx_FMT_TYPENAME "' instance %R " "in '" __Pyx_FMT_TYPENAME "'",
+                    value_type_name, key, type_name);
+#else
+                    "Error calling __set_name__ on '" __Pyx_FMT_TYPENAME "' instance %.100s in '" __Pyx_FMT_TYPENAME "'",
+                    value_type_name,
+                    PyString_Check(key) ? PyString_AS_STRING(key) : "?",
+                    type_name);
+#endif
+                goto bad;
+            } else {
+                Py_DECREF(tmp);
+            }
+        }
+        else if (unlikely(PyErr_Occurred())) {
+            goto bad;
+        }
+    }
+    Py_DECREF(names_to_set);
+    return 0;
+bad:
+    Py_XDECREF(names_to_set);
+    return -1;
+}
+static PyObject *__Pyx_InitSubclassPEP487(PyObject *type_obj, PyObject *mkw) {
+#if CYTHON_USE_TYPE_SLOTS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyTypeObject *type = (PyTypeObject*) type_obj;
+    PyObject *mro = type->tp_mro;
+    Py_ssize_t i, nbases;
+    if (unlikely(!mro)) goto done;
+    (void) &__Pyx_GetBuiltinName;
+    Py_INCREF(mro);
+    nbases = PyTuple_GET_SIZE(mro);
+    assert(PyTuple_GET_ITEM(mro, 0) == type_obj);
+    for (i = 1; i < nbases-1; i++) {
+        PyObject *base, *dict, *meth;
+        base = PyTuple_GET_ITEM(mro, i);
+        dict = ((PyTypeObject *)base)->tp_dict;
+        meth = __Pyx_PyDict_GetItemStrWithError(dict, __pyx_n_s_init_subclass);
+        if (unlikely(meth)) {
+            descrgetfunc f = Py_TYPE(meth)->tp_descr_get;
+            PyObject *res;
+            Py_INCREF(meth);
+            if (likely(f)) {
+                res = f(meth, NULL, type_obj);
+                Py_DECREF(meth);
+                if (unlikely(!res)) goto bad;
+                meth = res;
+            }
+            res = __Pyx_PyObject_FastCallDict(meth, NULL, 0, mkw);
+            Py_DECREF(meth);
+            if (unlikely(!res)) goto bad;
+            Py_DECREF(res);
+            goto done;
+        } else if (unlikely(PyErr_Occurred())) {
+            goto bad;
+        }
+    }
+done:
+    Py_XDECREF(mro);
+    return type_obj;
+bad:
+    Py_XDECREF(mro);
+    Py_DECREF(type_obj);
+    return NULL;
+#else
+    PyObject *super_type, *super, *func, *res;
+#if CYTHON_COMPILING_IN_PYPY && !defined(PySuper_Type)
+    super_type = __Pyx_GetBuiltinName(__pyx_n_s_super);
+#else
+    super_type = (PyObject*) &PySuper_Type;
+    (void) &__Pyx_GetBuiltinName;
+#endif
+    super = likely(super_type) ? __Pyx_PyObject_Call2Args(super_type, type_obj, type_obj) : NULL;
+#if CYTHON_COMPILING_IN_PYPY && !defined(PySuper_Type)
+    Py_XDECREF(super_type);
+#endif
+    if (unlikely(!super)) {
+        Py_CLEAR(type_obj);
+        goto done;
+    }
+    func = __Pyx_PyObject_GetAttrStrNoError(super, __pyx_n_s_init_subclass);
+    Py_DECREF(super);
+    if (likely(!func)) {
+        if (unlikely(PyErr_Occurred()))
+            Py_CLEAR(type_obj);
+        goto done;
+    }
+    res = __Pyx_PyObject_FastCallDict(func, NULL, 0, mkw);
+    Py_DECREF(func);
+    if (unlikely(!res))
+        Py_CLEAR(type_obj);
+    Py_XDECREF(res);
+done:
+    return type_obj;
+#endif
+}
+#endif
 static PyObject *__Pyx_Py3ClassCreate(PyObject *metaclass, PyObject *name, PyObject *bases,
                                       PyObject *dict, PyObject *mkw,
                                       int calculate_metaclass, int allow_py2_metaclass) {
-    PyObject *result, *margs;
+    PyObject *result;
     PyObject *owned_metaclass = NULL;
+    PyObject *margs[4] = {NULL, name, bases, dict};
     if (allow_py2_metaclass) {
         owned_metaclass = PyObject_GetItem(dict, __pyx_n_s_metaclass);
         if (owned_metaclass) {
             metaclass = owned_metaclass;
         } else if (likely(PyErr_ExceptionMatches(PyExc_KeyError))) {
             PyErr_Clear();
         } else {
@@ -11052,68 +15393,1130 @@
     if (calculate_metaclass && (!metaclass || PyType_Check(metaclass))) {
         metaclass = __Pyx_CalculateMetaclass((PyTypeObject*) metaclass, bases);
         Py_XDECREF(owned_metaclass);
         if (unlikely(!metaclass))
             return NULL;
         owned_metaclass = metaclass;
     }
-    margs = PyTuple_Pack(3, name, bases, dict);
-    if (unlikely(!margs)) {
-        result = NULL;
+    result = __Pyx_PyObject_FastCallDict(metaclass, margs+1, 3 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET,
+#if PY_VERSION_HEX < 0x030600A4
+        (metaclass == (PyObject*)&PyType_Type) ? NULL : mkw
+#else
+        mkw
+#endif
+    );
+    Py_XDECREF(owned_metaclass);
+#if PY_VERSION_HEX < 0x030600A4 && CYTHON_PEP487_INIT_SUBCLASS
+    if (likely(result) && likely(PyType_Check(result))) {
+        if (unlikely(__Pyx_SetNamesPEP487(result) < 0)) {
+            Py_CLEAR(result);
+        } else {
+            result = __Pyx_InitSubclassPEP487(result, mkw);
+        }
+    }
+#else
+    (void) &__Pyx_GetBuiltinName;
+#endif
+    return result;
+}
+
+/* FetchSharedCythonModule */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+#if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
     } else {
-        result = PyObject_Call(metaclass, margs, mkw);
-        Py_DECREF(margs);
+        result = __Pyx_CyFunction_Call(func, args, kw);
     }
-    Py_XDECREF(owned_metaclass);
     return result;
 }
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -11184,84 +16587,118 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -11269,14 +16706,15 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
@@ -11381,177 +16819,254 @@
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -11615,177 +17130,254 @@
     const int32_t neg_one = (int32_t) -1, const_zero = (int32_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int32_t) < sizeof(long)) {
+        if ((sizeof(int32_t) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int32_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int32_t) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int32_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int32_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int32_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) >= 2 * PyLong_SHIFT) {
-                            return (int32_t) (((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int32_t, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int32_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) >= 2 * PyLong_SHIFT)) {
+                                return (int32_t) (((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int32_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) >= 3 * PyLong_SHIFT) {
-                            return (int32_t) (((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int32_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) >= 3 * PyLong_SHIFT)) {
+                                return (int32_t) (((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int32_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) >= 4 * PyLong_SHIFT) {
-                            return (int32_t) (((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int32_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) >= 4 * PyLong_SHIFT)) {
+                                return (int32_t) (((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int32_t) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int32_t) <= sizeof(unsigned long)) {
+            if ((sizeof(int32_t) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int32_t, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int32_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int32_t) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int32_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int32_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int32_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int32_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int32_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (int32_t) (((int32_t)-1)*(((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int32_t, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int32_t) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int32_t) (((int32_t)-1)*(((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int32_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (int32_t) ((((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int32_t) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int32_t) ((((((int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (int32_t) (((int32_t)-1)*(((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int32_t) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int32_t) (((int32_t)-1)*(((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int32_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (int32_t) ((((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int32_t) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int32_t) ((((((((int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (int32_t) (((int32_t)-1)*(((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int32_t) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int32_t) (((int32_t)-1)*(((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int32_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int32_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (int32_t) ((((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int32_t) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int32_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int32_t) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int32_t) ((((((((((int32_t)digits[3]) << PyLong_SHIFT) | (int32_t)digits[2]) << PyLong_SHIFT) | (int32_t)digits[1]) << PyLong_SHIFT) | (int32_t)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int32_t) <= sizeof(long)) {
+            if ((sizeof(int32_t) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int32_t, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int32_t) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int32_t) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int32_t, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int32_t val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int32_t) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int32_t) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int32_t) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int32_t) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int32_t) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int32_t) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int32_t) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int32_t) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int32_t) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int32_t) 1) << (sizeof(int32_t) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int32_t) -1;
         }
     } else {
         int32_t val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int32_t) -1;
         val = __Pyx_PyInt_As_int32_t(tmp);
@@ -11811,177 +17403,254 @@
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -11994,19 +17663,34 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name_2);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__38));
+    }
+    return name;
+}
+#endif
+
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -12019,14 +17703,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -12043,19 +17743,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -12096,56 +17796,88 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
+#if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -12199,15 +17931,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -12228,30 +17960,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -12309,21 +18045,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -12358,16 +18092,41 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `pyreadr-0.4.7/pyreadr/librdata.pxd` & `pyreadr-0.4.8/pyreadr/librdata.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -128,47 +128,72 @@
     rdata_error_t rdata_end_table(rdata_writer_t *writer, int32_t row_count, const char *datalabel);
     rdata_error_t rdata_end_file(rdata_writer_t *writer);
 
 cdef extern from 'libs/librdata/src/rdata_io_unistd.h':
     cdef struct rdata_unistd_io_ctx_t 'rdata_unistd_io_ctx_s':
         int fd
 
-IF UNAME_SYSNAME == 'Windows':
-
-    cdef extern from 'Python.h':
-        wchar_t* PyUnicode_AsWideCharString(object, Py_ssize_t *) except NULL
-
-    cdef extern from '<fcntl.h>':
-        int _wsopen(const wchar_t *filename, int oflag, int shflag, int pmode)
-        cdef int _O_RDONLY
-        cdef int _O_BINARY
-        cdef int _O_CREAT
-        cdef int _O_WRONLY
-        cdef int _O_TRUNC
-
-    cdef extern from '<io.h>':
-        cdef int _close(int fd)
-        ssize_t _write(int fd, const void *buf, size_t nbyte)
-
-    cdef extern from '<share.h>':
-        cdef int _SH_DENYRW  # Denies read and write access to a file.
-        cdef int _SH_DENYWR  # Denies write access to a file.
-        cdef int _SH_DENYRD  # Denies read access to a file.
-        cdef int _SH_DENYNO
-
-    cdef extern from '<sys/stat.h>':
-        cdef int _S_IREAD
-        cdef int _S_IWRITE
-
-ELSE:
-    cdef extern from '<sys/stat.h>':
-        int open(const char *path, int oflag, int mode)
-
-    cdef extern from '<unistd.h>':
-        int close(int fd)
-        ssize_t write(int fd, const void *buf, size_t nbyte)
-
-    cdef extern from '<fcntl.h>':
-        cdef int O_WRONLY
-        cdef int O_RDONLY
-        cdef int O_CREAT
-        cdef int O_TRUNC
+cdef extern from "conditional_includes.h":
+    wchar_t* PyUnicode_AsWideCharString(object, Py_ssize_t *) except NULL
+    int _wsopen(const wchar_t *filename, int oflag, int shflag, int pmode)
+    int _O_RDONLY
+    int _O_BINARY
+    int _O_WRONLY
+    int _O_CREAT
+    int _O_TRUNC
+    int _SH_DENYRW  # Denies read and write access to a file.
+    int _SH_DENYWR  # Denies write access to a file.
+    int _SH_DENYRD  # Denies read access to a file.
+    int _SH_DENYNO
+    void assign_fd(void *io_ctx, int fd)
+    int _close(int fd)
+    ssize_t _write(int fd, const void *buf, size_t nbyte)
+    int _S_IREAD
+    int _S_IWRITE
+    int open(const char *path, int oflag, int mode)
+    int close(int fd)
+    ssize_t write(int fd, const void *buf, size_t nbyte)
+    int O_WRONLY
+    int O_RDONLY
+    int O_CREAT
+    int O_TRUNC
+
+#IF UNAME_SYSNAME == 'Windows':
+
+    #cdef extern from 'Python.h':
+        #wchar_t* PyUnicode_AsWideCharString(object, Py_ssize_t *) except NULL
+
+    #cdef extern from '<fcntl.h>':
+        #int _wsopen(const wchar_t *filename, int oflag, int shflag, int pmode)
+        #cdef int _O_RDONLY
+        #cdef int _O_BINARY
+        #cdef int _O_CREAT
+        #cdef int _O_WRONLY
+        #cdef int _O_TRUNC
+
+    #cdef extern from '<io.h>':
+        #cdef int _close(int fd)
+        #ssize_t _write(int fd, const void *buf, size_t nbyte)
+
+    #cdef extern from '<share.h>':
+        #cdef int _SH_DENYRW  # Denies read and write access to a file.
+        #cdef int _SH_DENYWR  # Denies write access to a file.
+        #cdef int _SH_DENYRD  # Denies read access to a file.
+        #cdef int _SH_DENYNO
+
+    #cdef extern from '<sys/stat.h>':
+        #cdef int _S_IREAD
+        #cdef int _S_IWRITE
+
+#ELSE:
+    #cdef extern from '<sys/stat.h>':
+        #int open(const char *path, int oflag, int mode)
+
+    #cdef extern from '<unistd.h>':
+        #int close(int fd)
+	#ssize_t write(int fd, const void *buf, size_t nbyte)
+
+    #cdef extern from '<fcntl.h>':
+        #cdef int O_WRONLY
+        #cdef int O_RDONLY
+        #cdef int O_CREAT
+        #cdef int O_TRUNC
```

### Comparing `pyreadr-0.4.7/pyreadr/librdata.pyx` & `pyreadr-0.4.8/pyreadr/librdata.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # cython: c_string_type=str, c_string_encoding=utf8, language_level=3
 
+import platform
 from enum import Enum
 import numpy as np
 import pandas as pd
 import os.path
 from cython.operator cimport dereference as deref
 from libc.string cimport strlen
 
@@ -15,122 +16,122 @@
     INTEGER    = rdata_type_t.RDATA_TYPE_INT32
     NUMERIC    = rdata_type_t.RDATA_TYPE_REAL
     LOGICAL    = rdata_type_t.RDATA_TYPE_LOGICAL
     TIMESTAMP  = rdata_type_t.RDATA_TYPE_TIMESTAMP
     DATE       = rdata_type_t.RDATA_TYPE_DATE
 
 
-cdef int _os_open(path, mode):
+cdef int _os_open(path, mode) noexcept:
     cdef int flags
-    IF UNAME_SYSNAME == 'Windows':
-        cdef Py_ssize_t length
+    cdef Py_ssize_t length
+    if platform.system() == 'Windows':
         if mode == 'r':
             flags = _O_RDONLY | _O_BINARY
             u16_path = PyUnicode_AsWideCharString(path, &length)
             return _wsopen(u16_path, flags, _SH_DENYWR, _S_IREAD | _S_IWRITE)
         else:
             flags = _O_WRONLY | _O_CREAT | _O_BINARY | _O_TRUNC
             u16_path = PyUnicode_AsWideCharString(os.fsdecode(path), &length)
             return _wsopen(u16_path, flags, _SH_DENYRW, _S_IREAD | _S_IWRITE)
-    ELSE:
+    else:
         if mode == 'r':
             flags = O_RDONLY
         else:
             flags = O_WRONLY | O_CREAT | O_TRUNC
         #return open(path.encode('utf-8'), flags, 0644)
         return open(path, flags, 0644)
 
 
-cdef int _os_close(int fd):
-    IF UNAME_SYSNAME == 'Windows':
+cdef int _os_close(int fd) noexcept:
+    if platform.system() == 'Windows':
         return _close(fd)
-    ELSE:
+    else:
         return close(fd)
 
 
-cdef int _handle_open(const char* path, void* io_ctx):
+cdef int _handle_open(const char* path, void* io_ctx) noexcept:
     cdef rdata_unistd_io_ctx_t* ctx = <rdata_unistd_io_ctx_t*>io_ctx
     cdef int fd
     if not os.path.isfile(path):
         return -1
     fd = _os_open(path, 'r')
     ctx.fd = fd
     return fd
 
-cdef int _handle_table(const char *name, void *ctx):
+cdef int _handle_table(const char *name, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         Parser.__handle_table(parser, name)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
 
-cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+cdef int _handle_column(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         if parser.parse_current_table:
             Parser.__handle_column(parser, name, type, data, count)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
-cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx):
+cdef int _handle_dim(const char *name, rdata_type_t type, void *data, long count, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         if parser.parse_current_table:
             Parser.__handle_dim(parser, name, type, data, count)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
 
-cdef int _handle_column_name(const char *name, int index, void *ctx):
+cdef int _handle_column_name(const char *name, int index, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         Parser.__handle_column_name(parser, name, index)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
-cdef int _handle_dim_name(const char *name, int index, void *ctx):
+cdef int _handle_dim_name(const char *name, int index, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         Parser.__handle_dim_name(parser, name, index)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
-cdef int _handle_row_name(const char *name, int index, void *ctx):
+cdef int _handle_row_name(const char *name, int index, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         Parser.__handle_row_name(parser, name, index)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
 
-cdef int _handle_text_value(const char *value, int index, void *ctx):
+cdef int _handle_text_value(const char *value, int index, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         if parser.parse_current_table:
             Parser.__handle_text_value(parser, value, index)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
         return rdata_error_t.RDATA_ERROR_USER_ABORT
 
 
-cdef int _handle_value_label(const char *value, int index, void *ctx):
+cdef int _handle_value_label(const char *value, int index, void *ctx) noexcept:
     parser = <Parser>ctx
     try:
         if parser.parse_current_table:
             Parser.__handle_value_label(parser, value, index)
         return rdata_error_t.RDATA_OK
     except Exception as e:
         parser._error = e
@@ -141,23 +142,23 @@
 
     cdef rdata_parser_t *_this
     cdef int _fd
     cdef int _row_count
     cdef int _var_count
     parse_current_table = True
 
-    cpdef parse(self, path):
+    cpdef parse(self, path) noexcept:
 
         cdef rdata_error_t status
 
         self._this = rdata_parser_init();
         self._fd = 0
         self._error = None
 
-        IF UNAME_SYSNAME == 'Windows':  # custom file opener for windows *sigh*
+        if platform.system() == 'Windows':
             rdata_set_open_handler(self._this, _handle_open)
 
         rdata_set_table_handler(self._this, _handle_table)
         rdata_set_column_handler(self._this, _handle_column)
         rdata_set_column_name_handler(self._this, _handle_column_name)
         rdata_set_dim_handler(self._this, _handle_dim)
         rdata_set_dim_name_handler(self._this, _handle_dim_name)
@@ -196,21 +197,21 @@
 
     def handle_text_value(self, name, index):
         pass
 
     def handle_value_label(self, name, index):
         pass
 
-    cdef __handle_table(self, const char* name):
+    cdef __handle_table(self, const char* name) noexcept:
         if name == NULL:
             self.handle_table(None)
         else:
             self.handle_table(name)
 
-    cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count):
+    cdef __handle_column(self, const char *name, rdata_type_t type, void *data, long count) noexcept:
         cdef double *doubles = <double*>data
         cdef int *ints = <int*>data
 
         if type in [rdata_type_t.RDATA_TYPE_REAL, rdata_type_t.RDATA_TYPE_TIMESTAMP, rdata_type_t.RDATA_TYPE_DATE]:
             array = np.empty([count], dtype=np.float64)
             for i in range(count):
                 array[i] = doubles[i];
@@ -224,18 +225,18 @@
         if name == NULL:
             new_name = None
         else:
             new_name = name
         data_type = DataType(type)
         self.handle_column(new_name, data_type, array, count)
 
-    cdef __handle_column_name(self, const char *name, int index):
+    cdef __handle_column_name(self, const char *name, int index) noexcept: 
         self.handle_column_name(name, index)
 
-    cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count):
+    cdef __handle_dim(self, const char *name, rdata_type_t datatype, void *data, long count) noexcept:
         cdef int *ints = <int*>data
 
         data_type = DataType(datatype)
         if datatype == rdata_type_t.RDATA_TYPE_INT32:
             array = np.empty([count], dtype=np.int32)
             for i in range(count):
                 array[i] = ints[i];
@@ -244,39 +245,39 @@
 
         if name == NULL:
             new_name = None
         else:
             new_name = name
         self.handle_dim(new_name, data_type, array, count)
 
-    cdef __handle_dim_name(self, const char *name, int index):
+    cdef __handle_dim_name(self, const char *name, int index) noexcept:
         if name == NULL:
             new_name = None
         else:
             new_name = name
         self.handle_dim_name(new_name, index)
 
-    cdef __handle_row_name(self, const char *name, int index):
+    cdef __handle_row_name(self, const char *name, int index) noexcept:
         self.handle_row_name(name, index)
 
-    cdef __handle_text_value(self, const char *value, int index):
+    cdef __handle_text_value(self, const char *value, int index) noexcept:
         if value != NULL:
             self.handle_text_value(value, index)
         else:
             self.handle_text_value(np.nan, index)
 
-    cdef __handle_value_label(self, const char *value, int index):
+    cdef __handle_value_label(self, const char *value, int index) noexcept:
         self.handle_value_label(value, index)
 
 
-cdef ssize_t _handle_write(const void *data, size_t len, void *ctx):
+cdef ssize_t _handle_write(const void *data, size_t len, void *ctx) noexcept:
     cdef int fd = deref(<int*>ctx)
-    IF UNAME_SYSNAME == 'Windows':
+    if platform.system() == 'Windows':
         return _write(fd, data, len)
-    ELSE:
+    else:
         return write(fd, data, len)
 
 
 cdef class Column:
     cdef rdata_column_t *_this
 
     def add_level_labels(self, labels):
```

### Comparing `pyreadr-0.4.7/pyreadr/libs/bzip2/bzlib.h` & `pyreadr-0.4.8/pyreadr/libs/bzip2/bzlib.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/iconv/iconv.h` & `pyreadr-0.4.8/pyreadr/libs/iconv/iconv.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/CKHashTable.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/CKHashTable.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/CKHashTable.h` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/CKHashTable.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata.h` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_bits.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_bits.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_error.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_error.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_internal.h` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_internal.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_io_unistd.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_io_unistd.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_io_unistd.h` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_io_unistd.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_parser.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_parser.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_read.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_read.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/librdata/src/rdata_write.c` & `pyreadr-0.4.8/pyreadr/libs/librdata/src/rdata_write.c`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/base.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/base.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/bcj.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/bcj.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/block.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/block.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/check.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/check.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/container.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/container.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/delta.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/delta.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/filter.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/filter.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/hardware.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/hardware.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/index.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/index.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/index_hash.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/index_hash.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/lzma12.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/lzma12.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/stream_flags.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/stream_flags.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/version.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/version.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma/vli.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma/vli.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/lzma/lzma.h` & `pyreadr-0.4.8/pyreadr/libs/lzma/lzma.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/zlib/zconf.h` & `pyreadr-0.4.8/pyreadr/libs/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/libs/zlib/zlib.h` & `pyreadr-0.4.8/pyreadr/libs/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr/pyreadr.py` & `pyreadr-0.4.8/pyreadr/pyreadr.py`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/pyreadr.egg-info/PKG-INFO` & `pyreadr-0.4.8/pyreadr.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: pyreadr
-Version: 0.4.7
+Version: 0.4.8
 Summary: Reads/writes R RData and Rds files into/from pandas data frames.
 Home-page: https://github.com/ofajardo/pyreadr
 Author: Otto Fajardo
 Author-email: pleasecontactviagithub@notvalid.com
 License: AGPLv3
 Download-URL: https://pypi.org/project/pyreadr/#files
-Description:  A Python package to read and write R RData and Rds files
-        into/from pandas data frames. It does not need to have R or other external
-        dependencies installed.
-        It is based on the C library librdata and
-        a modified version of the cython wrapper jamovi-readstat.<br>
-        Please visit out project home page for more information:<br>
-        https://github.com/ofajardo/pyreadr
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: C
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_jamovi_readstat
+License-File: LICENSE_librdata
+
+ A Python package to read and write R RData and Rds files
+into/from pandas data frames. It does not need to have R or other external
+dependencies installed.
+It is based on the C library librdata and
+a modified version of the cython wrapper jamovi-readstat.<br>
+Please visit out project home page for more information:<br>
+https://github.com/ofajardo/pyreadr
+
+
```

### Comparing `pyreadr-0.4.7/pyreadr.egg-info/SOURCES.txt` & `pyreadr-0.4.8/pyreadr.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,34 @@
+LICENSE
+LICENSE_jamovi_readstat
+LICENSE_librdata
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pyreadr/__init__.py
 pyreadr/_pyreadr_parser.py
 pyreadr/_pyreadr_writer.py
+pyreadr/charset.dll
 pyreadr/custom_errors.py
+pyreadr/iconv.dll
+pyreadr/iconv.lib
+pyreadr/libbz2-1.dll
+pyreadr/liblzma-5.dll
+pyreadr/liblzma.dll
 pyreadr/librdata.c
 pyreadr/librdata.pxd
 pyreadr/librdata.pyx
 pyreadr/pyreadr.py
+pyreadr/z.lib
+pyreadr/zdll.lib
+pyreadr/zlib.dll
+pyreadr/zlib.lib
+pyreadr/zlib1.dll
+pyreadr/zlibstatic.lib
 pyreadr.egg-info/PKG-INFO
 pyreadr.egg-info/SOURCES.txt
 pyreadr.egg-info/dependency_links.txt
 pyreadr.egg-info/requires.txt
 pyreadr.egg-info/top_level.txt
 pyreadr/libs/bzip2/bzlib.h
 pyreadr/libs/iconv/iconv.h
```

### Comparing `pyreadr-0.4.7/setup.py` & `pyreadr-0.4.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 import sys
 
 import platform
 import glob
 
 from setuptools import setup, Extension
 from Cython.Build import cythonize
+import Cython
+
+cyver = int(Cython.__version__.split(".")[0])
+if cyver < 3:
+    raise Exception("cython 3.0.0 or newer is required")
 
 librdata_source_files = []
 librdata_source_files += glob.glob('pyreadr/libs/librdata/src/*.c')
 librdata_source_files += ['pyreadr/librdata.pyx']
 
 library_dirs = []
 libraries = []
 include_dirs = []
 extra_link_args = []
 extra_compile_args = ['-DHAVE_ZLIB', '-DHAVE_BZIP2', '-DHAVE_LZMA']
-data_files = []
-data_folder = ""
+package_data ={'pryeadr': ["*.c", "*.pyx", "*.pxd"]}
+exclude_package_data = {'pyreadr': ["*.dll", "*.lib"]}
+include_package_data=True
 
 if platform.system() == 'Darwin':
     libraries.append("iconv")
 elif platform.system() == 'Windows':
     is64bit = sys.maxsize > 2 ** 32
     if not is64bit:
         msg = "Python 32 bit is not supported on Windows. Please use Python 64 bit"
@@ -35,22 +41,18 @@
     include_dirs.append('pyreadr')
     include_dirs.append('pyreadr/libs/zlib')
     include_dirs.append('pyreadr/libs/bzip2')
     include_dirs.append('pyreadr/libs/lzma')
     include_dirs.append('pyreadr/libs/librdata')
     include_dirs.append('pyreadr/libs/iconv')
     library_dirs.append('pyreadr/libs/librdata')
-    
-    data_folder = "win_libs/64bit/"
-    data_files = [("Lib/site-packages/pyreadr", [data_folder + "zlib.dll", data_folder + "iconv.dll",
-                        data_folder + "charset.dll", data_folder + "iconv.lib",
-                        data_folder + "libbz2-1.dll",
-                        data_folder + "liblzma-5.dll"])]
-                        
-    library_dirs.append(data_folder)
+    package_data ={'pryeadr': ["*.c", "*.pyx", "*.pxd", "*.dll", "*.lib"]}
+    exclude_package_data = {}
+    include_package_data=True
+    library_dirs.append("pyreadr")
     libraries.append('z')
     libraries.append('iconv')
     libraries.append('bz2')
     libraries.append('lzma')
     
 elif platform.system() == 'Linux':
     libraries.append('z')
@@ -76,22 +78,21 @@
 It is based on the C library librdata and
 a modified version of the cython wrapper jamovi-readstat.<br>
 Please visit out project home page for more information:<br>
 https://github.com/ofajardo/pyreadr
 """
 
 short_description = "Reads/writes R RData and Rds files into/from pandas data frames."
-
 setup(
     name='pyreadr',
-    version='0.4.7',
+    version='0.4.8',
     ext_modules=cythonize([librdata], force=True),
     packages=["pyreadr"],
-    include_package_data=True,
-    data_files=data_files,
+    include_package_data=include_package_data,
+    exclude_package_data=exclude_package_data,
     install_requires=['pandas>=1.2.0'],
     license="AGPLv3",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Cython",
         "Programming Language :: C",
         "Intended Audience :: Science/Research",
```

### Comparing `pyreadr-0.4.7/win_libs/64bit/charset.dll` & `pyreadr-0.4.8/pyreadr/charset.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/iconv.dll` & `pyreadr-0.4.8/pyreadr/iconv.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/iconv.lib` & `pyreadr-0.4.8/pyreadr/iconv.lib`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/libbz2-1.dll` & `pyreadr-0.4.8/pyreadr/libbz2-1.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/liblzma-5.dll` & `pyreadr-0.4.8/pyreadr/liblzma-5.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/liblzma.dll` & `pyreadr-0.4.8/pyreadr/liblzma.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/z.lib` & `pyreadr-0.4.8/pyreadr/z.lib`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/zdll.lib` & `pyreadr-0.4.8/pyreadr/zdll.lib`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/zlib.dll` & `pyreadr-0.4.8/pyreadr/zlib.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/zlib.lib` & `pyreadr-0.4.8/pyreadr/zlib.lib`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/zlib1.dll` & `pyreadr-0.4.8/pyreadr/zlib1.dll`

 * *Files identical despite different names*

### Comparing `pyreadr-0.4.7/win_libs/64bit/zlibstatic.lib` & `pyreadr-0.4.8/pyreadr/zlibstatic.lib`

 * *Files identical despite different names*

