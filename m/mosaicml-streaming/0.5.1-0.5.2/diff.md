# Comparing `tmp/mosaicml-streaming-0.5.1.tar.gz` & `tmp/mosaicml-streaming-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.5.1.tar", last modified: Mon Jun 19 05:49:43 2023, max compression
+gzip compressed data, was "mosaicml-streaming-0.5.2.tar", last modified: Tue Aug  8 04:40:44 2023, max compression
```

## Comparing `mosaicml-streaming-0.5.1.tar` & `mosaicml-streaming-0.5.2.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 05:49:43.000000 mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.323979 mosaicml-streaming-0.5.1/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    54779 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11487 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/base/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/partition/orig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shared/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/shuffle/py2s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/spanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22606 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.327978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py
--rw-r--r--   0 runner    (1001) docker     (123)    20461 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/multimodal/webvid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.331978 mosaicml-streaming-0.5.1/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 05:49:43.335978 mosaicml-streaming-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_eviction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_spanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10559 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-06-19 05:49:29.000000 mosaicml-streaming-0.5.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.997958 mosaicml-streaming-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-08-08 04:40:43.997958 mosaicml-streaming-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.981958 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-08-08 04:40:43.000000 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-08 04:40:43.000000 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 04:40:43.000000 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-08 04:40:43.000000 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 04:40:43.000000 mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 04:40:43.997958 mosaicml-streaming-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.981958 mosaicml-streaming-0.5.2/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58235 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/base/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15146 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.985957 mosaicml-streaming-0.5.2/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/partition/orig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/base/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shared/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/shuffle/py2s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/spanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27637 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21446 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20455 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/multimodal/webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.989958 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.993958 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.993958 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.993958 mosaicml-streaming-0.5.2/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.993958 mosaicml-streaming-0.5.2/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 04:40:43.997958 mosaicml-streaming-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_eviction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15855 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-08-08 04:40:23.000000 mosaicml-streaming-0.5.2/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.5.1/LICENSE` & `mosaicml-streaming-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/PKG-INFO` & `mosaicml-streaming-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.5.1
+Version: 0.5.2
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.2 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.5.1/README.md` & `mosaicml-streaming-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.5.1
+Version: 0.5.2
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.1 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.5.2 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.5.1/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.5.2/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,12 +113,13 @@
 tests/test_local.py
 tests/test_mixing.py
 tests/test_partition.py
 tests/test_reader.py
 tests/test_shared.py
 tests/test_shuffle.py
 tests/test_spanner.py
+tests/test_stream.py
 tests/test_streaming.py
 tests/test_streaming_remote.py
 tests/test_upload.py
 tests/test_util.py
 tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.5.1/pyproject.toml` & `mosaicml-streaming-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/setup.py` & `mosaicml-streaming-0.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,51 +40,55 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 ]
 
 install_requires = [
     'boto3>=1.21.45,<2',
     'Brotli>=1.0.9',
+    'google-cloud-storage>=2.9.0',
     'matplotlib>=3.5.2,<4',
     'paramiko>=2.11.0,<4',
     'python-snappy>=0.6.1,<1',
     'torch>=1.10,<3',
     'torchtext>=0.10',
     'torchvision>=0.10',
     'tqdm>=4.64.0,<5',
     'transformers>=4.21.3,<5',
     'xxhash>=3.0.0,<4',
     'zstd>=1.5.2.5,<2',
     'oci>=2.88,<3',
     'azure-storage-blob>=12.0.0,<13',
+    'azure-storage-file-datalake>=12.11.0,<13',
+    'azure-identity>=1.13.0',
 ]
 
 extra_deps = {}
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
-    'pytest==7.3.2',
+    'pytest==7.4.0',
     'pytest_codeblocks==0.16.1',
     'pytest-cov>=4,<5',
     'toml==0.10.2',
     'yamllint==1.32.0',
     'moto>=4.0,<5',
-    'fastapi==0.97.0',
-    'pydantic==1.10.9',
-    'uvicorn==0.22.0',
+    'fastapi==0.100.0',
+    'pydantic==2.1.1',
+    'uvicorn==0.23.1',
+    'pytest-split==0.8.1',
 ]
 
 extra_deps['docs'] = [
-    'GitPython==3.1.31',
+    'GitPython==3.1.32',
     'docutils==0.18.1',
-    'furo==2023.5.20',
-    'myst-parser==1.0.0',
+    'furo==2023.7.26',
+    'myst-parser==2.0.0',
     'nbsphinx==0.9.2',
     'pandoc==2.3',
     'pypandoc==1.11',
     'sphinx-argparse==0.4.0',
     'sphinx-copybutton==0.5.2',
     'sphinx==6.2.1',
     'sphinx-tabs==3.4.1',
```

### Comparing `mosaicml-streaming-0.5.1/streaming/__init__.py` & `mosaicml-streaming-0.5.2/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/array.py` & `mosaicml-streaming-0.5.2/streaming/base/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/compression.py` & `mosaicml-streaming-0.5.2/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/constant.py` & `mosaicml-streaming-0.5.2/streaming/base/constant.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/dataloader.py` & `mosaicml-streaming-0.5.2/streaming/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/dataset.py` & `mosaicml-streaming-0.5.2/streaming/base/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,43 +27,45 @@
 from streaming.base.format import get_index_basename
 from streaming.base.partition import get_partitions
 from streaming.base.shared import (SharedArray, SharedBarrier, SharedMemory, SharedScalar,
                                    _get_path, get_shm_prefix)
 from streaming.base.shuffle import get_shuffle
 from streaming.base.spanner import Spanner
 from streaming.base.stream import Stream
-from streaming.base.util import bytes_to_int
+from streaming.base.util import bytes_to_int, number_abbrev_to_int
 from streaming.base.world import World
 
 # An arbitrary time in the future, used for cold shard eviction.
 NEVER = np.iinfo(np.uint64).max
 
 
 class _ShardState(IntEnum):
     """The download status of a shard.
 
     Restrictions:
     - The initial state of INVALID must be zero.
-    - State transitions: MISSING -> DOWNLOADING -> PRESENT -> MISSING.
+    - State transitions: REMOTE -> PREPARING -> LOCAL -> REMOTE.
     """
-    INVALID = 0
-    MISSING = 1
-    DOWNLOADING = 2
-    PRESENT = 3
+    INVALID = 0  # The state is allocated (e.g., in an array), but not initialized yet.
+    REMOTE = 1  # The shard exists only at the remote source.
+    PREPARING = 2  # The shard is currently being worked on: (a) downloading from remote to local,
+    # (b) decompressing zip-only, etc.
+    LOCAL = 3  # Some form of the shard (raw or zip) exists locally (as well as remotely).
 
 
 class _IterState(IntEnum):
     """The iter status of an _Iterator.
 
     Restrictions:
     - State transitions: ITERATING -> EXITING -> EXITED.
     """
-    ITERATING = 0
-    EXITING = 1
-    EXITED = 2
+    ITERATING = 0  # We are currently iterating through an epoch.
+    EXITING = 1  # We have been signalled to end the epoch (either we hit end of __iter__, or
+    # someone else started a new epoch, of which only one can be valid at a time).
+    EXITED = 2  # All threads have noticed the exit signal and exited.
 
 
 class _Iterator:
     """State of StreamingDataset __iter__, used to track and coordinate its threads.
 
     Has methods to implement early exit when a new epoch is started before the last one is done.
 
@@ -84,15 +86,15 @@
     # returning. The `yield` main thread exits at the end of epoch(s).
     _num_threads_to_exit = 2
 
     def __init__(self, sample_ids: NDArray[np.int64]) -> None:
         self.sample_ids = sample_ids
 
         self.total = len(sample_ids)
-        self.download_index = 0
+        self.prepare_index = 0
         self.ready_index = 0
         self.yield_index = 0
         self.eviction_index = 0
 
         self._lock = Lock()
         self._state = 0
         self._num_exited = 0
@@ -192,14 +194,19 @@
       * Shuffling:
 
         * ``shuffle``
         * ``shuffle_algo``
         * ``shuffle_seed``
         * ``shuffle_block_size``
 
+      * Sampling:
+
+        * ``sampling_method``
+
+
     Args:
         streams (Sequence[Stream], optional): One or more streams to stream/cache samples from,
             which may be upsampled or downsampled. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
@@ -212,18 +219,19 @@
         download_timeout (float): Number of seconds to wait for a shard to download before raising
             an exception. Defaults to ``60``.
         validate_hash (str, optional): Optional hash or checksum algorithm to use to validate
             shards. Defaults to ``None``.
         keep_zip (bool): Whether to keep or delete the compressed form when decompressing
             downloaded shards. If ``False``, keep iff remote is local or no remote. Defaults to
             ``False``.
-        epoch_size (int, optional): Number of samples to draw per epoch balanced across all
+        epoch_size (Union[int, str], optional): Number of samples to draw per epoch balanced across all
             streams. If ``None``, takes its value from the total number of underlying samples.
             Provide this field if you are weighting streams relatively to target a larger or
-            smaller epoch size. Defaults to ``None``.
+            smaller epoch size. Defaults to ``None``. Can also take in human-readable number
+            abbreviations (e.g., ``"100k"``, ``"64M"``, ``"77b"``, and so on). Defaults to ``None``.
         predownload (int, optional): Target number of samples ahead to download the shards per
             number of workers provided in a dataloader while iterating. If ``None``, its value
             gets derived using batch size and number of canonical nodes
             ``max(batch_size, 256 * batch_size // num_canonical_nodes)``. Defaults to ``None``.
         cache_limit (Union[int, str], optional): Maximum size in bytes of this StreamingDataset's
             shard cache. Before downloading a shard, the least recently used resident shard(s)
             may be evicted (deleted from the local cache) in order to stay under the limit.
@@ -245,67 +253,98 @@
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
+        sampling_method (str): Which sampling method to use, either ``balanced`` or ``fixed``.
+            Defaults to ``balanced``.
     """
 
     def __init__(self,
                  *,
                  streams: Optional[Sequence[Stream]] = None,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
                  download_retry: int = 2,
                  download_timeout: float = 60,
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
-                 epoch_size: Optional[int] = None,
+                 epoch_size: Optional[Union[int, str]] = None,
                  predownload: Optional[int] = None,
                  cache_limit: Optional[Union[int, str]] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
                  shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
-                 shuffle_block_size: int = 1 << 18) -> None:
+                 shuffle_block_size: int = 1 << 18,
+                 sampling_method: str = 'balanced') -> None:
         # Global arguments (which do not live in Streams).
         self.predownload = predownload
         self.cache_limit = cache_limit
         self.partition_algo = partition_algo
         self.num_canonical_nodes = num_canonical_nodes
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.shuffle_algo = shuffle_algo
         self.shuffle_seed = shuffle_seed
         self.shuffle_block_size = shuffle_block_size
+        self.sampling_method = sampling_method.lower().strip()
 
         # Check streams vs remote/local.
         if bool(streams) == (bool(remote) or bool(local)):
             raise ValueError(
                 'You must provide either `streams` or `remote`/`local`, but not both.')
 
-        # Initialize the Stream defaults.
-        default = Stream(remote=remote,
-                         local=local,
-                         split=split,
-                         download_retry=download_retry,
-                         download_timeout=download_timeout,
-                         validate_hash=validate_hash,
-                         keep_zip=keep_zip)
+        # Check sampling method is one of "balanced" or "fixed".
+        if self.sampling_method not in ['balanced', 'fixed']:
+            raise ValueError(
+                f'Invalid sampling method: {sampling_method}. Must be one of `balanced` or `fixed`.'
+            )
+        # Convert epoch size from string to int, if needed. Cannot be negative.
+        epoch_size_value = None
+        if epoch_size:
+            epoch_size_value = number_abbrev_to_int(epoch_size)
+            if epoch_size_value < 0:
+                raise ValueError(f'Epoch size cannot be negative. Received {epoch_size_value}.')
+
+        # Initialize torch dist ourselves, if necessary.
+        destroy_dist = maybe_init_dist()
 
-        # Normalize to a list of Streams.
+        # Initialize the Stream defaults and normalize to a list of Streams.
         if streams:
+            default = {
+                'remote': remote,
+                'local': local,
+                'split': split,
+                'download_retry': download_retry,
+                'download_timeout': download_timeout,
+                'validate_hash': validate_hash,
+                'keep_zip': keep_zip,
+            }
             for stream in streams:
                 stream.apply_default(default)
         else:
+            default = Stream(remote=remote,
+                             local=local,
+                             split=split,
+                             choose=epoch_size_value,
+                             download_retry=download_retry,
+                             download_timeout=download_timeout,
+                             validate_hash=validate_hash,
+                             keep_zip=keep_zip)
             streams = [default]
+            # reset `epoch_size_value` to None when we initialize StreamingDataset with no
+            # streams so that when we `apply_weights` over this single stream we use the
+            # epoch size to absolutely weight the single stream.
+            epoch_size_value = None
 
         # Validate the stream weighting scheme (relative or absolute) to catch errors before we go
         # to the trouble of loading them.
         Stream.validate_weights(streams)
 
         # Set streams.
         self.streams = streams
@@ -314,17 +353,14 @@
         # Initialize the World context.
         #
         # Beware: This information is for the per-rank process. DataLoader worker processes may see
         # different values for these fields. We are saving the rank World here because we cannot
         # instantiate a World inside the StreamingDataset destructor.
         self._rank_world = world = World()
 
-        # Initialize torch dist ourselves, if necessary.
-        destroy_dist = maybe_init_dist()
-
         # Download each stream's index, load their shards, and map streams <-> shards.
         self.num_samples = 0
         self.shards = []
         stream_per_shard = []
         self.shard_offset_per_stream = np.zeros(self.num_streams, np.int64)
         self.shards_per_stream = np.zeros(self.num_streams, np.int64)
         self.sample_offset_per_stream = np.zeros(self.num_streams, np.int64)
@@ -358,16 +394,16 @@
         # Build the shard index (for partitioning and mapping samples to shards).
         self.samples_per_shard = np.array([shard.samples for shard in self.shards], np.int64)
         self.sample_offset_per_shard = self.samples_per_shard.cumsum() - self.samples_per_shard
         self.spanner = Spanner(self.samples_per_shard)
 
         # Now that we know the number of underlying samples of each stream, derive each stream's
         # true proportion/repeat/choose, as well as the total epoch size.
-        self.epoch_size = Stream.apply_weights(self.streams, self.samples_per_stream, epoch_size,
-                                               self.shuffle_seed)
+        self.epoch_size = Stream.apply_weights(self.streams, self.samples_per_stream,
+                                               epoch_size_value, self.shuffle_seed)
 
         # Length (__len__) is the resampled epoch size divided over the number of devices.
         self.length = ceil(self.epoch_size / world.num_ranks)
 
         # Register/lookup our shared memory prefix and filelock root directory.
         my_locals = [os.path.abspath(os.path.join(x.local, x.split)) for x in streams]
         self._shm_prefix_int, self._locals_shm = get_shm_prefix(my_locals, world)
@@ -405,44 +441,32 @@
                                                _get_path(self._shm_prefix_int, SHARD_ACCESS_TIMES))
 
         # Initialize shared memory objects.
         if world.is_local_leader:
             # Set initial epoch (before any resumption).
             self.next_epoch = 0
 
-            # Normalize each stream's local dir, discovering which shards are present.
-            are_shards_present = []
-            for stream_id, stream in enumerate(self.streams):
-                start = self.shard_offset_per_stream[stream_id]
-                stop = start + self.shards_per_stream[stream_id]
-                stream_shards = self.shards[start:stop]
-                are_shards_present += stream.init_local_dir(stream_shards)
-
-            # Calculate the initial cache usage using shard presence info.
-            #
-            # If we are above cache_limit, do nothing about it until the first download (which will
-            # evict until happy).
+            # Get cache usage due to streams.
             self.cache_usage = 0
             for stream in self.streams:
                 self.cache_usage += stream.get_index_size()
-            for shard_id, is_shard_present in enumerate(are_shards_present):
-                if is_shard_present:
-                    stream_id = self.stream_per_shard[shard_id]
-                    stream = self.streams[stream_id]
-                    shard = self.shards[shard_id]
-                    self.cache_usage += shard.get_persistent_size(stream.safe_keep_zip)
-
-            # Also use shard presence to initialize the shard states array and last access times.
-            for shard_id, is_shard_present in enumerate(are_shards_present):
-                if is_shard_present:
-                    self._shard_states[shard_id] = _ShardState.PRESENT
-                    self._shard_access_times[shard_id] = time_ns()
-                else:
-                    self._shard_states[shard_id] = _ShardState.MISSING
-                    self._shard_access_times[shard_id] = NEVER
+
+            # Get cache usage due to shards.
+            cache_usage_per_shard = np.zeros(self.num_shards, np.int64)
+            for stream_id, stream in enumerate(self.streams):
+                begin = self.shard_offset_per_stream[stream_id]
+                end = begin + self.shards_per_stream[stream_id]
+                stream.set_up_local(self.shards[begin:end], cache_usage_per_shard[begin:end])
+            self.cache_usage += cache_usage_per_shard.sum()
+
+            # If either raw or zip are present after local dir setup, the shard is considered
+            # present for download/eviction logic purposes (may need to decompress upon use).
+            for shard_id, size in enumerate(cache_usage_per_shard):
+                self._shard_states[shard_id] = _ShardState.LOCAL if size else _ShardState.REMOTE
+                self._shard_access_times[shard_id] = time_ns()
 
         if dist.is_available() and dist.is_initialized():
             dist.barrier()
 
         if destroy_dist:
             dist.destroy_process_group()
 
@@ -652,57 +676,69 @@
 
         Args:
             epoch (int): What epoch this is for. Used in seeding the sampling RNG.
 
         Returns:
             Tuple[NDArray[np.int64], NDArray[np.int64]]: Sampled shard sizes and sample mapping.
         """
-        # Initialize random number generator and arrays.
-        rng = np.random.default_rng(self.shuffle_seed + epoch)
+        # Initialize random number generator and arrays. If sampling_method is "fixed", the rng
+        # seed does not change, resulting in the same samples from each stream each epoch.
+        rng = np.random.default_rng(self.shuffle_seed + epoch) \
+            if self.sampling_method == 'balanced' \
+            else np.random.default_rng(self.shuffle_seed)
         shuffle_units = []
         sample_ids = []
 
         # Iterate over each stream.
         for stream_id in range(self.num_streams):
+            # stream's shard offset in list of all shards from all streams
             stream_shard_offset = self.shard_offset_per_stream[stream_id]
             num_stream_shards = self.shards_per_stream[stream_id]
             stream_shard_ids = stream_shard_offset + np.arange(num_stream_shards)
 
             # Calculate choose per stream shard.
             samples_per_stream_shard = self.samples_per_shard[stream_shard_ids]
             stream_samples = sum(samples_per_stream_shard)
+            # the number of items to choose from each stream (calculated during dataset initialization)
             stream_choose = self.streams[stream_id].choose
             if stream_choose == stream_samples:
                 choose_per_stream_shard = samples_per_stream_shard
             else:
                 choose_per_stream_shard = \
                     samples_per_stream_shard * stream_choose // stream_samples
                 shortfall = stream_choose - choose_per_stream_shard.sum()
                 indices = rng.choice(num_stream_shards, shortfall, False)
                 choose_per_stream_shard[indices] += 1
 
             # Iterate over each shard of this stream.
             for shard_id, shard_samples, shard_choose in zip(stream_shard_ids,
                                                              samples_per_stream_shard,
                                                              choose_per_stream_shard):
-                # Calculate shuffle units.
+                # Calculate shuffle units for this shard.
+                # shuffle units are lists where each entry is a number of samples to take
+                # from the shard. If upsampling a shard with 4 samples by 2.5x,
+                # shard_choose will be 10, and shard_shuffle_units will be [4, 4, 2]. If
+                # downsampling that same shard by 0.5x, shard_choose will be 2 and
+                # shard_shuffle_units will be just [2].
                 shard_shuffle_units = [shard_samples] * (shard_choose // shard_samples)
                 remainder = shard_choose % shard_samples
                 if remainder:
                     shard_shuffle_units.append(remainder)
                 shuffle_units.append(shard_shuffle_units)
 
                 # Calculate sample IDs of any full repeats.
                 shard_sample_offset = self.sample_offset_per_shard[shard_id]
                 num_full_repeats = shard_choose // shard_samples
                 if num_full_repeats:
                     full_repeat = shard_sample_offset + np.arange(shard_samples)
                     sample_ids += [full_repeat] * num_full_repeats
 
                 # Calculate sample IDs of a possible partial repeat.
+                # for fixed sampling this partial repeat chooses the same
+                # samples since we have fixed the rng seed.
                 shortfall = shard_choose % shard_samples
                 if shortfall:
                     partial_repeat = shard_sample_offset + rng.choice(
                         shard_samples, shortfall, False)
                     partial_repeat.sort()
                     sample_ids.append(partial_repeat)
 
@@ -843,62 +879,59 @@
 
     def _evict_shard(self, shard_id: int) -> None:
         """Evict the given shard.
 
         Assumes you hold ``_cache_filelock``, preventing anyone else from modifying the cache. We
         expect that shard deletions are very fast.
 
-        This method is called internally by ``download_shard`` to clear space for more downloads.
+        This method is called internally by ``prepare_shard`` to clear space for more downloads.
 
         Args:
             shard_id (int): Shard to evict.
         """
         # Delete the shard's last access time, so that it is not searchable when finding the
         # coldest shard to evict. This is done by setting the time far into the future.
         self._shard_access_times[shard_id] = NEVER
 
         # Set the shard state to missing.
-        self._shard_states[shard_id] = _ShardState.MISSING
+        self._shard_states[shard_id] = _ShardState.REMOTE
 
-        # Perform the eviction.
+        # Perform the eviction, updating cache usage to account for the removal.
         shard = self.shards[shard_id]
-        shard.evict()
-
-        # Lastly, update cache usage to account for the removal.
-        stream_id = self.stream_per_shard[shard_id]
-        stream = self.streams[stream_id]
-        self.cache_usage -= shard.get_persistent_size(stream.safe_keep_zip)
+        self.cache_usage -= shard.evict()
+        if self.cache_usage < 0:
+            raise RuntimeError(f'Negative cache usage: {self.cache_usage}.')
 
     def _evict_coldest_shard(self) -> None:
         """Evict the coldeset (i.e., least recently accessed) shard.
 
         Assumes you hold ``__cache_filelock``, preventing anyone else from modifying the cache. We
         expect that shard deletions are very fast.
 
-        This method is called internally by ``download_shard`` to clear space for more downloads.
+        This method is called internally by ``prepare_shard`` to clear space for more downloads.
         """
         while True:
             # Find the shard with the oldest last access time.
             shard_id = int(self._shard_access_times.numpy().argmin())
 
             # Check the shard's last access time. If it is NEVER, there are no downloaded shards to
             # evict. If any shards are currently being downloaded, wait, else raise an error.
             if self._shard_access_times[shard_id] == NEVER:
-                if (self._shard_states.numpy() == _ShardState.DOWNLOADING).any():
+                if (self._shard_states.numpy() == _ShardState.PREPARING).any():
                     sleep(TICK)
                     continue
                 else:
                     raise ValueError(
                         f'Tried to evict a shard {shard_id}, but no shards are present to evict ' +
                         f'(cache usage {self.cache_usage} of {self.cache_limit})')
 
             # The shard has a valid timestamp. Now, verify that it is actually present. There is an
             # edge case where it may not be present (see the note in get_item()). If not present,
             # pick the next lowest shard.
-            if self._shard_states[shard_id] != _ShardState.PRESENT:
+            if self._shard_states[shard_id] != _ShardState.LOCAL:
                 self._shard_access_times[shard_id] = NEVER
                 continue
 
             # Break on success.
             break
 
         # Evict that shard.
@@ -929,15 +962,15 @@
         # incompatible with spawn, so must be created lazily.
         if not hasattr(self, CACHE_FILELOCK):
             self._cache_filelock = FileLock(self._cache_filelock_path)
 
         with self._cache_filelock:
             self._evict_coldest_shard()
 
-    def download_shard(self, shard_id: int, blocking: bool = True) -> None:
+    def prepare_shard(self, shard_id: int, blocking: bool = True) -> None:
         """Download a shard, either waiting or skipping if in progress by another worker.
 
         This method is multithread/multiprocess-safe.
 
         If cache limit is enabled, this method may delete one or more other shards to make space
         for this download.
 
@@ -953,61 +986,74 @@
         lock = self._cache_filelock
         lock.acquire()
 
         # Get the state of the shard to download.
         state = self._shard_states[shard_id]
 
         # Which state is it in?
-        if state == _ShardState.MISSING:
-            # If missing, transition state to downloading.
-            self._shard_states[shard_id] = _ShardState.DOWNLOADING
+        if state == _ShardState.REMOTE:
+            # If missing, transition state to preparing.
+            self._shard_states[shard_id] = _ShardState.PREPARING
 
             # Get the stream and shard.
             stream_id = self.stream_per_shard[shard_id]
             stream = self.streams[stream_id]
             shard = self.shards[shard_id]
 
             # If cache_limit is enabled, we first may have to make space for the new shard.
             if self.cache_limit:
                 # Evict one shard at a time until our download will stay under the cache limit.
                 # This means both the raw and zip forms of the shard due to decompressing.
-                shard_full_size = shard.get_full_size()
-                while self.cache_limit < self.cache_usage + shard_full_size:
+                shard_max_cache_usage = shard.get_max_size()
+                while self.cache_limit < self.cache_usage + shard_max_cache_usage:
                     self._evict_coldest_shard()
 
-            # Calculate and apply the persistent change in cache usage, which depends on
-            # whether compression was used and keep_zip.
-            self.cache_usage += shard.get_persistent_size(stream.safe_keep_zip)
-
             # With the above preamble done, we can release the cache lock.
             lock.release()
 
-            # Perform the download (shard will not be modified in DOWNLOADING state).
-            stream.download_shard(shard)
+            # Perform the download (shard will not be modified by others in PREPARING state).
+            delta = stream.prepare_shard(shard)
 
-            # Download completed, so note the time and transition shard state to PRESENT.
+            # Download completed, so note the time and transition shard state to LOCAL.
+            lock.acquire()
+            self.cache_usage += delta
             self._shard_access_times[shard_id] = time_ns()
-            self._shard_states[shard_id] = _ShardState.PRESENT
-        elif state == _ShardState.DOWNLOADING:
+            self._shard_states[shard_id] = _ShardState.LOCAL
+            lock.release()
+        elif state == _ShardState.PREPARING:
             # Someone else is currently downloading the shard. Release the lock for others to make
             # progress.
             lock.release()
 
             # Do we wait on them?
             if blocking:
-                # Wait for the shard to transition out of DOWNLOADING state (to PRESENT, although
-                # it would be possible for it to become evicted again before a TICK has elapsed).
-                while self._shard_states[shard_id] == _ShardState.DOWNLOADING:
+                # Wait for the shard to transition out of PREPARING state (to LOCAL, although it would
+                # be possible for it to become evicted again before a TICK has elapsed).
+                while self._shard_states[shard_id] == _ShardState.PREPARING:
                     sleep(TICK)
 
             # There is no need to update the last access time, because that will be set by the
             # process that downloaded the shard.
-        elif state == _ShardState.PRESENT:
-            # Shard is already downloaded. There is nothing to do, except touch the shard.
-            self._shard_access_times[shard_id] = time_ns()
+        elif state == _ShardState.LOCAL:
+            # Get the stream and shard.
+            stream_id = self.stream_per_shard[shard_id]
+            stream = self.streams[stream_id]
+            shard = self.shards[shard_id]
+
+            # We may need to decompress the shard (if local dir just contains zips).
+            raw_info, _ = shard.file_pairs[0]  # Each file pair is present in the same way.
+            raw_filename = os.path.join(stream.local, stream.split, raw_info.basename)  # Find raw.
+            if not os.path.isfile(raw_filename):  # Is raw missing?
+                self._shard_states[shard_id] = _ShardState.PREPARING  # Lock the shard.
+                lock.release()  # Unblock other workers.
+                delta = stream.prepare_shard(shard)  # Decompress and remove zip.
+                lock.acquire()  # Briefly take the lock back.
+                self._shard_states[shard_id] = _ShardState.LOCAL  # Restore shard state.
+                self.cache_usage += delta  # Update accounting.
+            self._shard_access_times[shard_id] = time_ns()  # Touch the shard.
             lock.release()
         else:
             # Unknown state.
             lock.release()
             raise RuntimeError(f'Invalid shard state: {state}')
 
     def get_item(self, sample_id: int, retry: int = 7) -> Any:
@@ -1034,32 +1080,33 @@
         for _ in range(1 + retry):
             try:
                 # Shortcut path: just assume the shard is present. Using exceptions as control flow
                 # is actually faster than checking that the shard is present because python.
                 sample = shard[shard_sample_id]
 
                 # Manually update the last access time afterward. This also happens at the end of
-                # download_shard().
+                # prepare_shard().
                 #
                 # Note: for performance reasons, we have not taken the lock here. This results in
-                # an edge case where a shard has a last access time but is actually not PRESENT.
+                # an edge case where a shard has a last access time but is actually not LOCAL.
                 # This impacts _evict_coldest_shard(), which we modify to handle this case.
                 self._shard_access_times[shard_id] = time_ns()
 
                 # On success, break out.
                 break
             except FileNotFoundError as e:
                 # Fallback: shard file is missing (generates `FileNotFoundError` exception),
                 # ensure the shard file is downloaded, then try to access the sample again.
                 # Loops because it may become evicted in the meantime.
                 errors.append(str(e))
-                self.download_shard(shard_id)
+                self.prepare_shard(shard_id)
         else:
             # Main process failed. Let the threads know to terminate.
-            self._event.set()
+            if hasattr(self, '_event'):
+                self._event.set()
             if self.cache_limit:
                 raise RuntimeError(f'{errors[-1]}. StreamingDataset repeatedly failed to ' +
                                    f'download a shard. This may be due to thrashing caused by ' +
                                    f'`cache_limit` being set too low.')
             else:
                 raise RuntimeError(f'{errors[-1]}. Check if the shard file exists in your ' +
                                    f'remote location or have you deleted the shard file from ' +
@@ -1081,15 +1128,15 @@
         exception = future.exception()
         if exception:
             # Set the event to let the other threadpool threads know about the exception.
             self._event.set()
             # Re-raise the exception.
             raise exception
 
-    def _download_thread(self, it: _Iterator) -> None:
+    def _prepare_thread(self, it: _Iterator) -> None:
         """Download the relevant shards in the background while we are being iterated.
 
         This thread is started at the beginning of each epoch, and exits either when out of samples
         or when a new epoch is started, calling exit() on its state (only one epoch is valid at a
         time).
 
         Each worker has its own download thread, which iterates ahead of the ready thread and yield
@@ -1102,41 +1149,41 @@
         while True:
             # If we've started a new epoch early (__iter__ was called again), exit this thread
             # because there can only be one epoch at once.
             if it.should_exit():
                 break
 
             # If we're out of samples this epoch, exit this thread because we are done downloading.
-            if it.download_index == it.total:
+            if it.prepare_index == it.total:
                 break
 
             # Background thread or a main process crashed, terminate this thread.
             if self._event.is_set():
                 break
 
             # If we are requested to only pre-download so many samples, if we have as many or more
             # downloaded already, we wait and check again later.
             if self.predownload is not None:
-                samples_ahead = it.download_index - it.yield_index
+                samples_ahead = it.prepare_index - it.yield_index
                 if self.predownload <= samples_ahead:
                     sleep(TICK)
                     continue
 
             # If we hit -1, we skip.
-            sample_id = it.sample_ids[it.download_index]
+            sample_id = it.sample_ids[it.prepare_index]
             if sample_id == -1:
-                it.download_index += 1
+                it.prepare_index += 1
                 continue
 
             # Download and decompress the shard for this sample, if not already done.
             shard_id, _ = self.spanner[sample_id]
-            self.download_shard(shard_id, False)
+            self.prepare_shard(shard_id, False)
 
             # Step forward one sample.
-            it.download_index += 1
+            it.prepare_index += 1
 
         # Note that we exited.
         it.on_exit()
 
     def _ready_thread(self, it: _Iterator) -> None:
         """Wait for the relevant shards to become downloaded while we are being iterated.
 
@@ -1179,18 +1226,18 @@
                 it.ready_index += 1
                 continue
 
             # Wait for the shard for this sample to be downloaded and decompressed, if not already.
             shard_id, _ = self.spanner[sample_id]
             # During cold shard eviction, shard state might go in the reverse direction. If a shard
             # is missing while fetching a sample, download it.
-            if self._shard_states[shard_id] == _ShardState.MISSING:
-                self.download_shard(shard_id, False)
+            if self._shard_states[shard_id] == _ShardState.REMOTE:
+                self.prepare_shard(shard_id, False)
             # Wait for a shard file to download completely.
-            while self._shard_states[shard_id] != _ShardState.PRESENT:
+            while self._shard_states[shard_id] != _ShardState.LOCAL:
                 sleep(TICK)
 
             # Step forward one sample.
             it.ready_index += 1
 
         # Note that we exited.
         it.on_exit()
@@ -1217,15 +1264,15 @@
                 break
 
             # Have we yielded all our samples?
             if it.yield_index == it.total:
                 break
 
             # Background thread crashed, terminate the main process
-            if self._event.is_set():
+            if hasattr(self, '_event') and self._event.is_set():
                 break
 
             # Is there a sample ready to yield?
             if it.ready_index <= it.yield_index:
                 sleep(TICK)
                 continue
 
@@ -1267,14 +1314,14 @@
         # Get this worker's partition of samples to process.
         sample_ids = self._get_work(world, epoch, sample_in_epoch)
         if not len(sample_ids):  # Resumed at end of epoch, out of samples.
             return
 
         # Iterate over the samples while downloading ahead.
         self._iterator = it = _Iterator(sample_ids)
-        download_future = self._executor.submit(self._download_thread, it)
-        download_future.add_done_callback(self.on_exception)
+        prepare_future = self._executor.submit(self._prepare_thread, it)
+        prepare_future.add_done_callback(self.on_exception)
         ready_future = self._executor.submit(self._ready_thread, it)
         ready_future.add_done_callback(self.on_exception)
         yield from map(self.__getitem__, self._each_sample_id(it))
-        wait([download_future, ready_future])
+        wait([prepare_future, ready_future])
         it.exit()
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/distributed.py` & `mosaicml-streaming-0.5.2/streaming/base/distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/base/reader.py` & `mosaicml-streaming-0.5.2/streaming/base/format/base/reader.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Read and decode sample from shards."""
 
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Dict, Iterator, List, Optional, Set
+from typing import Any, Dict, Iterator, List, Optional, Set, Union
 
 from streaming.base.array import Array
+from streaming.base.util import bytes_to_int
 
 __all__ = ['FileInfo', 'Reader', 'JointReader', 'SplitReader']
 
 
 @dataclass
 class FileInfo(object):
     """File validation info.
@@ -32,27 +33,37 @@
 
     Args:
         dirname (str): Local dataset directory.
         split (str, optional): Which dataset split to use, if any.
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         samples (int): Number of samples in this shard.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on.
     """
 
     def __init__(
         self,
         dirname: str,
         split: Optional[str],
         compression: Optional[str],
         hashes: List[str],
         samples: int,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
     ) -> None:
+
+        if size_limit:
+            if (isinstance(size_limit, str)):
+                size_limit = bytes_to_int(size_limit)
+            if size_limit < 0:
+                raise ValueError(f'`size_limit` must be greater than zero, instead, ' +
+                                 f'found as {size_limit}.')
+
         self.dirname = dirname
         self.split = split or ''
         self.compression = compression
         self.hashes = hashes
         self.samples = samples
         self.size_limit = size_limit
 
@@ -71,98 +82,141 @@
         """Get the number of samples in this shard.
 
         Returns:
             int: Sample count.
         """
         return self.samples
 
-    def _evict_raw(self) -> None:
-        """Remove all raw files belonging to this shard."""
+    def _evict_raw(self) -> int:
+        """Remove all raw files belonging to this shard.
+
+        Returns:
+            int: Bytes evicted from cache.
+        """
+        size = 0
         for raw_info, _ in self.file_pairs:
             filename = os.path.join(self.dirname, self.split, raw_info.basename)
             if os.path.exists(filename):
                 os.remove(filename)
+                size += raw_info.bytes
+        return size
 
-    def _evict_zip(self) -> None:
-        """Remove all zip files belonging to this shard."""
+    def _evict_zip(self) -> int:
+        """Remove all zip files belonging to this shard.
+
+        Returns:
+            int: Bytes evicted from cache.
+        """
+        size = 0
         for _, zip_info in self.file_pairs:
             if zip_info:
                 filename = os.path.join(self.dirname, self.split, zip_info.basename)
                 if os.path.exists(filename):
                     os.remove(filename)
+                    size += zip_info.bytes
+        return size
 
-    def evict(self) -> None:
-        """Remove all files belonging to this shard."""
-        self._evict_raw()
-        self._evict_zip()
+    def evict(self) -> int:
+        """Remove all files belonging to this shard.
+
+        Returns:
+            int: Bytes evicted from cache.
+        """
+        return self._evict_raw() + self._evict_zip()
 
-    def init_local_dir(self, filenames_present: Set[str], keep_zip: bool) -> bool:
+    def set_up_local(self, listing: Set[str], safe_keep_zip: bool) -> int:
         """Bring what shard files are present to a consistent state, returning whether present.
 
         Args:
-            filenames_present (Set[str]): The listing of all files under dirname/[split/]. This is
-                listed once and then saved because there could potentially be very many shard
-                files.
-            keep_zip (bool): Whether to keep zip files when decompressing. Possible when
+            listing (Set[str]): The listing of all files under dirname/[split/]. This is listed
+                once and then saved because there could potentially be very many shard files.
+            safe_keep_zip (bool): Whether to keep zip files when decompressing. Possible when
                 compression was used. Necessary when local is the remote or there is no remote.
 
         Returns:
             bool: Whether the shard is present.
         """
         # For raw/zip to be considered present, each raw/zip file must be present.
         raw_files_present = 0
         zip_files_present = 0
         for raw_info, zip_info in self.file_pairs:
             if raw_info:
                 filename = os.path.join(self.dirname, self.split, raw_info.basename)
-                if filename in filenames_present:
+                if filename in listing:
                     raw_files_present += 1
             if zip_info:
                 filename = os.path.join(self.dirname, self.split, zip_info.basename)
-                if filename in filenames_present:
+                if filename in listing:
                     zip_files_present += 1
 
         # If the shard raw files are partially present, garbage collect the present ones and mark
         # the shard raw as not present, in order to achieve consistency.
         if not raw_files_present:
-            is_raw_present = False
+            has_raw = False
         elif raw_files_present < len(self.file_pairs):
-            is_raw_present = False
+            has_raw = False
             self._evict_raw()
         else:
-            is_raw_present = True
+            has_raw = True
 
         # Same as the above, but for shard zip files.
         if not zip_files_present:
-            is_zip_present = False
+            has_zip = False
         elif zip_files_present < len(self.file_pairs):
-            is_zip_present = False
+            has_zip = False
             self._evict_zip()
         else:
-            is_zip_present = True
+            has_zip = True
 
-        # Do we keep_zip?
-        if keep_zip:
-            # If we can keep_zip, and we do, and have either raw or zip, we must have the other one
-            # too, because they are downloaded and decompressed together.
-            if self.compression and (is_zip_present != is_raw_present):
-                if is_raw_present:
-                    is_raw_present = False
-                    self._evict_raw()
-                elif is_zip_present:
-                    is_zip_present = False
-                    self._evict_zip()
+        # Enumerate cases of raw/zip presence.
+        if self.compression:
+            if safe_keep_zip:
+                if has_raw:
+                    if has_zip:
+                        # Present (normalized).
+                        pass
+                    else:
+                        # Missing: there is no natural way to arrive at this state, so drop raw.
+                        has_raw = False
+                        self._evict_raw()
+                else:
+                    if has_zip:
+                        # Present: but missing raw, so need to decompress upon use.
+                        pass
+                    else:
+                        # Missing (normalized).
+                        pass
+            else:
+                if has_raw:
+                    if has_zip:
+                        # Present: zip is unnecessary, so evict it.
+                        has_zip = False
+                        self._evict_raw()
+                    else:
+                        # Present (normalized).
+                        pass
+                else:
+                    if has_zip:
+                        # Present: but missing raw, so need to decompress and evict zip upon use.
+                        pass
+                    else:
+                        # Missing (normalized).
+                        pass
         else:
-            # If we don't keep_zip, drop any zip files.
-            if is_zip_present:
-                is_zip_present = False
-                self._evict_zip()
+            if has_zip:
+                raise ValueError('Shard is invalid: compression was not used, but has a ' +
+                                 'compressed form.')
 
-        # Now, the shard is either entirely or not at all present given keep_zip.
-        return is_raw_present
+        # Get cache usage. Shard is present if either raw or zip are present.
+        size = 0
+        if has_raw:
+            size += self.get_raw_size()
+        if has_zip:
+            size += self.get_zip_size() or 0
+        return size
 
     def get_raw_size(self) -> int:
         """Get the raw (uncompressed) size of this shard.
 
         Returns:
             int: Size in bytes.
         """
@@ -180,28 +234,26 @@
         size = 0
         for _, info in self.file_pairs:
             if info is None:
                 return None
             size += info.bytes
         return size
 
-    def get_full_size(self) -> int:
+    def get_max_size(self) -> int:
         """Get the full size of this shard.
 
-        "Full" in this case means both the raw (decompressed) and zip (compressed) versions are
+        "Max" in this case means both the raw (decompressed) and zip (compressed) versions are
         resident (assuming it has a zip form). This is the maximum disk usage the shard can reach.
         When compressed was used, even if keep_zip is ``False``, the zip form must still be
         resident at the same time as the raw form during shard decompression.
 
         Returns:
             int: Size in bytes.
         """
-        raw_size = self.get_raw_size()
-        zip_size = self.get_zip_size() or 0
-        return raw_size + zip_size
+        return self.get_raw_size() + (self.get_zip_size() or 0)
 
     def get_persistent_size(self, keep_zip: bool) -> int:
         """Get the persistent size of this shard.
 
         "Persistent" in this case means whether both raw and zip are present is subject to
         keep_zip. If we are not keeping zip files after decompression, they don't count to the
         shard's persistent size on disk.
@@ -210,15 +262,15 @@
             keep_zip (bool): Whether to keep zip files after decompressing.
 
         Returns:
             int: Size in bytes.
         """
         if self.compression:
             if keep_zip:
-                size = self.get_full_size()
+                size = self.get_max_size()
             else:
                 size = self.get_raw_size()
         else:
             size = self.get_raw_size()
         return size
 
     @abstractmethod
@@ -273,28 +325,28 @@
     Args:
         dirname (str): Local dataset directory.
         split (str, optional): Which dataset split to use, if any.
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         raw_data (FileInfo): Uncompressed data file info.
         samples (int): Number of samples in this shard.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
             shard. If None, puts everything in one shard.
         zip_data (FileInfo, optional): Compressed data file info.
     """
 
     def __init__(
         self,
         dirname: str,
         split: Optional[str],
         compression: Optional[str],
         hashes: List[str],
         raw_data: FileInfo,
         samples: int,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
         zip_data: Optional[FileInfo],
     ) -> None:
         super().__init__(dirname, split, compression, hashes, samples, size_limit)
         self.raw_data = raw_data
         self.zip_data = zip_data
         self.file_pairs.append((raw_data, zip_data))
 
@@ -306,30 +358,30 @@
         dirname (str): Local dataset directory.
         split (str, optional): Which dataset split to use, if any.
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         raw_data (FileInfo): Uncompressed data file info.
         raw_meta (FileInfo): Uncompressed meta file info.
         samples (int): Number of samples in this shard.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
             shard. If None, puts everything in one shard.
         zip_data (FileInfo, optional): Compressed data file info.
         zip_meta (FileInfo, optional): Compressed meta file info.
     """
 
     def __init__(
         self,
         dirname: str,
         split: Optional[str],
         compression: Optional[str],
         hashes: List[str],
         raw_data: FileInfo,
         raw_meta: FileInfo,
         samples: int,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
         zip_data: Optional[FileInfo],
         zip_meta: Optional[FileInfo],
     ) -> None:
         super().__init__(dirname, split, compression, hashes, samples, size_limit)
         self.raw_data = raw_data
         self.raw_meta = raw_meta
         self.zip_data = zip_data
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.5.2/streaming/base/format/base/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from typing_extensions import Self
 
 from streaming.base.compression import compress, get_compression_extension, is_compression
 from streaming.base.format.index import get_index_basename
 from streaming.base.hashing import get_hash, is_hash
 from streaming.base.storage.upload import CloudUploader
+from streaming.base.util import bytes_to_int
 
 __all__ = ['JointWriter', 'SplitWriter']
 
 logger = logging.getLogger(__name__)
 
 
 class Writer(ABC):
@@ -40,16 +41,18 @@
                `local_dir` and also uploaded to a remote location.
         keep_local (bool): If the dataset is uploaded, whether to keep the local dataset directory
             or remove it after uploading. Defaults to ``False``.
         compression (str, optional): Optional compression or compression:level. Defaults to
             ``None``.
         hashes (List[str], optional): Optional list of hash algorithms to apply to shard files.
             Defaults to ``None``.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If ``None``, puts everything in one shard. Defaults to ``1 << 26``.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If ``None``, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on. Defaults to ``1 << 26``.
         extra_bytes_per_shard (int): Extra bytes per serialized shard (for computing shard size
             while writing). Defaults to ``0``.
         extra_bytes_per_sample (int): Extra bytes per serialized sample (for computing shard size
             while writing). Defaults to ``0``.
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
@@ -63,15 +66,15 @@
 
     def __init__(self,
                  *,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  extra_bytes_per_shard: int = 0,
                  extra_bytes_per_sample: int = 0,
                  **kwargs: Any) -> None:
 
         compression = compression or None
         if compression:
             if not is_compression(compression):
@@ -80,25 +83,25 @@
         hashes = hashes or []
         if list(hashes) != sorted(hashes):
             raise ValueError('Hashes must be unique and in sorted order.')
         for algo in hashes:
             if not is_hash(algo):
                 raise ValueError(f'Invalid hash: {algo}.')
 
+        size_limit_value = None
         if size_limit:
-            if size_limit < 0:
+            size_limit_value = bytes_to_int(size_limit)
+            if size_limit_value < 0:
                 raise ValueError(f'`size_limit` must be greater than zero, instead, ' +
-                                 f'found as {size_limit}.')
-        else:
-            size_limit = None
+                                 f'found as {size_limit_value}.')
 
         self.keep_local = keep_local
         self.compression = compression
         self.hashes = hashes
-        self.size_limit = size_limit
+        self.size_limit = size_limit_value
         self.extra_bytes_per_shard = extra_bytes_per_shard
         self.extra_bytes_per_sample = extra_bytes_per_sample
         self.new_samples: List[bytes]
         self.new_shard_size: int
 
         self.shards = []
 
@@ -334,15 +337,15 @@
 
     def __init__(self,
                  *,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  extra_bytes_per_shard: int = 0,
                  extra_bytes_per_sample: int = 0,
                  **kwargs: Any) -> None:
         super().__init__(out=out,
                          keep_local=keep_local,
                          compression=compression,
                          hashes=hashes,
@@ -415,15 +418,15 @@
 
     def __init__(self,
                  *,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  **kwargs: Any) -> None:
         super().__init__(out=out,
                          keep_local=keep_local,
                          compression=compression,
                          hashes=hashes,
                          size_limit=size_limit,
                          extra_bytes_per_shard=self.extra_bytes_per_shard,
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.5.2/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.5.2/streaming/base/format/json/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """:class:`JSONReader` reads samples from `.json` files that were written by :class:`MDSWriter`."""
 
 import json
 import os
 from copy import deepcopy
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 from typing_extensions import Self
 
 from streaming.base.format.base.reader import FileInfo, SplitReader
 
 __all__ = ['JSONReader']
@@ -27,15 +27,17 @@
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         newline (str): Newline character(s).
         raw_data (FileInfo): Uncompressed data file info.
         raw_meta (FileInfo): Uncompressed meta file info.
         samples (int): Number of samples in this shard.
         size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard.
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on.
         zip_data (FileInfo, optional): Compressed data file info.
         zip_meta (FileInfo, optional): Compressed meta file info.
     """
 
     def __init__(
         self,
         dirname: str,
@@ -43,15 +45,15 @@
         columns: Dict[str, str],
         compression: Optional[str],
         hashes: List[str],
         newline: str,
         raw_data: FileInfo,
         raw_meta: FileInfo,
         samples: int,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
         zip_data: Optional[FileInfo],
         zip_meta: Optional[FileInfo],
     ) -> None:
         super().__init__(dirname, split, compression, hashes, raw_data, raw_meta, samples,
                          size_limit, zip_data, zip_meta)
         self.columns = columns
         self.newline = newline
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.5.2/streaming/base/format/json/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,18 @@
                `local_dir` and also uploaded to a remote location.
         keep_local (bool): If the dataset is uploaded, whether to keep the local dataset directory
             or remove it after uploading. Defaults to ``False``.
         compression (str, optional): Optional compression or compression:level. Defaults to
             ``None``.
         hashes (List[str], optional): Optional list of hash algorithms to apply to shard files.
             Defaults to ``None``.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard. Defaults to ``None``.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on. Defaults to ``1 << 26``.
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
@@ -51,15 +53,15 @@
                  *,
                  columns: Dict[str, str],
                  newline: str = '\n',
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  **kwargs: Any) -> None:
         super().__init__(out=out,
                          keep_local=keep_local,
                          compression=compression,
                          hashes=hashes,
                          size_limit=size_limit,
                          **kwargs)
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/mds/encodings.py` & `mosaicml-streaming-0.5.2/streaming/base/format/mds/encodings.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             shape (Tuple[int], optional): The shape, if fixed.
 
         Returns:
             int: The fixed size in bytes, if there is one.
         """
         if dtype is None or shape is None:
             return None
-        return np.prod(shape) * getattr(np, dtype)().nbytes
+        return int(np.prod(shape)) * getattr(np, dtype)().nbytes
 
     def __init__(self, dtype: Optional[str] = None, shape: Optional[Tuple[int]] = None):
         if dtype is not None:
             assert dtype in self._value_dtype2int
         if shape is not None:
             for dim in shape:
                 assert 1 <= dim
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.5.2/streaming/base/format/mds/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """:class:`MDSReader` reads samples in `.mds` files written by :class:`StreamingDatasetWriter`."""
 
 import os
 from copy import deepcopy
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 from typing_extensions import Self
 
 from streaming.base.format.base.reader import FileInfo, JointReader
 from streaming.base.format.mds.encodings import mds_decode
 
@@ -25,31 +25,33 @@
         column_encodings (List[str]): Column encodings.
         column_names (List[str]): Column names.
         column_sizes (List[Optional[int]]): Column fixed sizes, if any.
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         raw_data (FileInfo): Uncompressed data file info.
         samples (int): Number of samples in this shard.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on.
         zip_data (FileInfo, optional): Compressed data file info.
     """
 
     def __init__(
         self,
         dirname: str,
         split: Optional[str],
         column_encodings: List[str],
         column_names: List[str],
         column_sizes: List[Optional[int]],
         compression: Optional[str],
         hashes: List[str],
         raw_data: FileInfo,
         samples: int,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
         zip_data: Optional[FileInfo],
     ) -> None:
         super().__init__(dirname, split, compression, hashes, raw_data, samples, size_limit,
                          zip_data)
         self.column_encodings = column_encodings
         self.column_names = column_names
         self.column_sizes = column_sizes
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.5.2/streaming/base/format/mds/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,16 +30,18 @@
                `local_dir` and also uploaded to a remote location.
         keep_local (bool): If the dataset is uploaded, whether to keep the local dataset directory
             or remove it after uploading. Defaults to ``False``.
         compression (str, optional): Optional compression or compression:level. Defaults to
             ``None``.
         hashes (List[str], optional): Optional list of hash algorithms to apply to shard files.
             Defaults to ``None``.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If ``None``, puts everything in one shard. Defaults to ``1 << 26``.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If ``None``, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on. Defaults to ``1 << 26``.
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
@@ -51,15 +53,15 @@
     def __init__(self,
                  *,
                  columns: Dict[str, str],
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  **kwargs: Any) -> None:
         super().__init__(out=out,
                          keep_local=keep_local,
                          compression=compression,
                          hashes=hashes,
                          size_limit=size_limit,
                          extra_bytes_per_sample=self.extra_bytes_per_sample,
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.5.2/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.5.2/streaming/base/format/xsv/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Reads and decode samples from tabular formatted files such as XSV, CSV, and TSV."""
 
 import os
 from copy import deepcopy
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 from typing_extensions import Self
 
 from streaming.base.format.base.reader import FileInfo, SplitReader
 from streaming.base.format.xsv.encodings import xsv_decode
 
@@ -27,16 +27,18 @@
         compression (str, optional): Optional compression or compression:level.
         hashes (List[str]): Optional list of hash algorithms to apply to shard files.
         newline (str): Newline character(s).
         raw_data (FileInfo): Uncompressed data file info.
         raw_meta (FileInfo): Uncompressed meta file info.
         samples (int): Number of samples in this shard.
         separator (str): Separator character(s).
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on.
         zip_data (FileInfo, optional): Compressed data file info.
         zip_meta (FileInfo, optional): Compressed meta file info.
     """
 
     def __init__(
         self,
         dirname: str,
@@ -46,15 +48,15 @@
         compression: Optional[str],
         hashes: List[str],
         newline: str,
         raw_data: FileInfo,
         raw_meta: FileInfo,
         samples: int,
         separator: str,
-        size_limit: Optional[int],
+        size_limit: Optional[Union[int, str]],
         zip_data: Optional[FileInfo],
         zip_meta: Optional[FileInfo],
     ) -> None:
         super().__init__(dirname, split, compression, hashes, raw_data, raw_meta, samples,
                          size_limit, zip_data, zip_meta)
         self.column_encodings = column_encodings
         self.column_names = column_names
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.5.2/streaming/base/format/xsv/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
                `local_dir` and also uploaded to a remote location.
         keep_local (bool): If the dataset is uploaded, whether to keep the local dataset directory
             or remove it after uploading. Defaults to ``False``.
         compression (str, optional): Optional compression or compression:level. Defaults to
             ``None``.
         hashes (List[str], optional): Optional list of hash algorithms to apply to shard files.
             Defaults to ``None``.
-        size_limit (int, optional): Optional shard size limit, after which point to start a new
-            shard. If None, puts everything in one shard. Defaults to ``None``.
+        size_limit (Union[int, str], optional): Optional shard size limit, after which point to start a new
+            shard. If None, puts everything in one shard. Can specify bytes
+            human-readable format as well, for example ``"100kb"`` for 100 kilobyte
+            (100*1024) and so on. Defaults to ``1 << 26``
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
@@ -53,15 +55,15 @@
                  columns: Dict[str, str],
                  separator: str,
                  newline: str = '\n',
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  compression: Optional[str] = None,
                  hashes: Optional[List[str]] = None,
-                 size_limit: Optional[int] = 1 << 26,
+                 size_limit: Optional[Union[int, str]] = 1 << 26,
                  **kwargs: Any) -> None:
         super().__init__(out=out,
                          keep_local=keep_local,
                          compression=compression,
                          hashes=hashes,
                          size_limit=size_limit,
                          **kwargs)
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/hashing.py` & `mosaicml-streaming-0.5.2/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/local.py` & `mosaicml-streaming-0.5.2/streaming/base/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/partition/orig.py` & `mosaicml-streaming-0.5.2/streaming/base/partition/orig.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,17 @@
                              'the other, otherwise striping slices of shards over nodes may ' +
                              'lead to each node downloading all shards')
 
     batch_size = batch_size or 1
 
     # If drop_first isn't a multiple of num_physical_nodes, round down to make it divisible.
     if drop_first % num_physical_nodes:
-        logger.warn('`drop_first` was not divisible by `num_physical_nodes`. Rounding it down ' +
-                    'to make it divisible.')
+        logger.warning(
+            '`drop_first` was not divisible by `num_physical_nodes`. Rounding it down ' +
+            'to make it divisible.')
         drop_first -= drop_first % num_physical_nodes
 
     # Divide the full dataset sample range into a sample range per canonical node.
     samples_per_canonical_node = (num_samples + num_canonical_nodes - 1) // num_canonical_nodes
     node_ratio = 0
     padding = 0
     if num_canonical_nodes < num_physical_nodes:
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/array.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/barrier.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/memory.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/memory.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/prefix.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/prefix.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shared/scalar.py` & `mosaicml-streaming-0.5.2/streaming/base/shared/scalar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shuffle/naive.py` & `mosaicml-streaming-0.5.2/streaming/base/shuffle/naive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shuffle/py1b.py` & `mosaicml-streaming-0.5.2/streaming/base/shuffle/py1b.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.5.2/streaming/base/shuffle/py1s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.5.2/streaming/base/shuffle/py2s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/spanner.py` & `mosaicml-streaming-0.5.2/streaming/base/spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/base/storage/__init__.py` & `mosaicml-streaming-0.5.2/streaming/base/storage/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Base module for downloading/uploading files from/to cloud storage."""
 
 from streaming.base.storage.download import download_file, download_or_wait
-from streaming.base.storage.upload import (AzureUploader, CloudUploader, GCSUploader,
-                                           LocalUploader, OCIUploader, S3Uploader)
+from streaming.base.storage.upload import (AzureDataLakeUploader, AzureUploader, CloudUploader,
+                                           GCSUploader, LocalUploader, OCIUploader, S3Uploader)
 
 __all__ = [
     'download_file', 'download_or_wait', 'CloudUploader', 'S3Uploader', 'GCSUploader',
-    'OCIUploader', 'LocalUploader', 'AzureUploader'
+    'OCIUploader', 'LocalUploader', 'AzureUploader', 'AzureDataLakeUploader'
 ]
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/storage/download.py` & `mosaicml-streaming-0.5.2/streaming/base/storage/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -154,23 +154,41 @@
 def download_from_gcs(remote: str, local: str) -> None:
     """Download a file from remote GCS to local.
 
     Args:
         remote (str): Remote path (GCS).
         local (str): Local path (local filesystem).
     """
-    import boto3
-    from boto3.s3.transfer import TransferConfig
-    from botocore.exceptions import ClientError
-
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 'gs':
         raise ValueError(
             f'Expected obj.scheme to be `gs`, instead, got {obj.scheme} for remote={remote}')
 
+    if 'GOOGLE_APPLICATION_CREDENTIALS' in os.environ:
+        _gcs_with_service_account(local, obj)
+    elif 'GCS_KEY' in os.environ and 'GCS_SECRET' in os.environ:
+        _gcs_with_hmac(remote, local, obj)
+    else:
+        raise ValueError(f'Either GOOGLE_APPLICATION_CREDENTIALS needs to be set for ' +
+                         f'service level accounts or GCS_KEY and GCS_SECRET needs to be ' +
+                         f'set for HMAC authentication')
+
+
+def _gcs_with_hmac(remote: str, local: str, obj: urllib.parse.ParseResult) -> None:
+    """Download a file from remote GCS to local using user level credentials.
+
+    Args:
+        remote (str): Remote path (GCS).
+        local (str): Local path (local filesystem).
+        obj (ParseResult): ParseResult object of remote.
+    """
+    import boto3
+    from boto3.s3.transfer import TransferConfig
+    from botocore.exceptions import ClientError
+
     # Create a new session per thread
     session = boto3.session.Session()
     # Create a resource client using a thread's session object
     gcs_client = session.client('s3',
                                 region_name='auto',
                                 endpoint_url='https://storage.googleapis.com',
                                 aws_access_key_id=os.environ['GCS_KEY'],
@@ -186,14 +204,30 @@
     except ClientError as e:
         if e.response['Error']['Code'] in BOTOCORE_CLIENT_ERROR_CODES:
             raise FileNotFoundError(f'Object {remote} not found.') from e
     except Exception:
         raise
 
 
+def _gcs_with_service_account(local: str, obj: urllib.parse.ParseResult) -> None:
+    """Download a file from remote GCS to local using service account credentials.
+
+    Args:
+        local (str): Local path (local filesystem).
+        obj (ParseResult): ParseResult object of remote path (GCS).
+    """
+    from google.cloud.storage import Blob, Bucket, Client
+
+    service_account_path = os.environ['GOOGLE_APPLICATION_CREDENTIALS']
+    gcs_client = Client.from_service_account_json(service_account_path)
+
+    blob = Blob(obj.path.lstrip('/'), Bucket(gcs_client, obj.netloc))
+    blob.download_to_filename(local)
+
+
 def download_from_oci(remote: str, local: str) -> None:
     """Download a file from remote OCI to local.
 
     Args:
         remote (str): Remote path (OCI).
         local (str): Local path (local filesystem).
     """
@@ -244,14 +278,46 @@
             blob_data.readinto(my_blob)
     except ResourceNotFoundError:
         raise FileNotFoundError(f'Object {remote} not found.')
     except Exception:
         raise
 
 
+def download_from_azure_datalake(remote: str, local: str) -> None:
+    """Download a file from remote Microsoft Azure Data Lake to local.
+
+    Args:
+        remote (str): Remote path (azure).
+        local (str): Local path (local filesystem).
+    """
+    from azure.core.exceptions import ResourceNotFoundError
+    from azure.storage.filedatalake import DataLakeServiceClient
+
+    obj = urllib.parse.urlparse(remote)
+    if obj.scheme != 'azure-dl':
+        raise ValueError(
+            f'Expected obj.scheme to be `azure-dl`, got {obj.scheme} for remote={remote}')
+
+    # Create a new session per thread
+    service = DataLakeServiceClient(
+        account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.dfs.core.windows.net",
+        credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'],
+    )
+    try:
+        file_client = service.get_file_client(file_system=obj.netloc,
+                                              file_path=obj.path.lstrip('/'))
+        with open(local, 'wb') as my_file:
+            file_data = file_client.download_file()
+            file_data.readinto(my_file)
+    except ResourceNotFoundError:
+        raise FileNotFoundError(f'Object {remote} not found.')
+    except Exception:
+        raise
+
+
 def download_from_local(remote: str, local: str) -> None:
     """Download a file from remote to local.
 
     Args:
         remote (str): Remote path (local filesystem).
         local (str): Local path (local filesystem).
     """
@@ -290,14 +356,16 @@
         download_from_sftp(remote, local)
     elif remote.startswith('gs://'):
         download_from_gcs(remote, local)
     elif remote.startswith('oci://'):
         download_from_oci(remote, local)
     elif remote.startswith('azure://'):
         download_from_azure(remote, local)
+    elif remote.startswith('azure-dl://'):
+        download_from_azure_datalake(remote, local)
     else:
         download_from_local(remote, local)
 
 
 def wait_for_download(local: str, timeout: float = 60) -> None:
     """Wait for a download by another thread/process to complete.
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/storage/upload.py` & `mosaicml-streaming-0.5.2/streaming/base/storage/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,48 @@
 """Write files to remote location which can be either Cloud Storage or a local path."""
 
 import logging
 import os
 import shutil
 import sys
 import urllib.parse
+from enum import Enum
 from tempfile import mkdtemp
 from typing import Any, Tuple, Union
 
 import tqdm
 
 from streaming.base.storage.download import BOTOCORE_CLIENT_ERROR_CODES
 
 __all__ = [
-    'CloudUploader', 'S3Uploader', 'GCSUploader', 'OCIUploader', 'AzureUploader', 'LocalUploader'
+    'CloudUploader',
+    'S3Uploader',
+    'GCSUploader',
+    'OCIUploader',
+    'AzureUploader',
+    'LocalUploader',
 ]
 
 logger = logging.getLogger(__name__)
 
 UPLOADERS = {
     's3': 'S3Uploader',
     'gs': 'GCSUploader',
     'oci': 'OCIUploader',
     'azure': 'AzureUploader',
+    'azure-dl': 'AzureDataLakeUploader',
     '': 'LocalUploader',
 }
 
 
+class GCSAuthentication(Enum):
+    HMAC = 1
+    SERVICE_ACCOUNT = 2
+
+
 class CloudUploader:
     """Upload local files to a cloud storage."""
 
     @classmethod
     def get(cls,
             out: Union[str, Tuple[str, str]],
             keep_local: bool = False,
@@ -78,18 +90,17 @@
             ValueError: Invalid number of `out` argument.
             ValueError: Invalid Cloud provider prefix.
         """
         if isinstance(out, str):
             obj = urllib.parse.urlparse(out)
         else:
             if len(out) != 2:
-                raise ValueError(''.join([
-                    f'Invalid `out` argument. It is either a string of local/remote directory ',
-                    'or a list of two strings with [local, remote].'
-                ]))
+                raise ValueError(f'Invalid `out` argument. It is either a string of ' +
+                                 f'local/remote directory or a list of two strings with ' +
+                                 f'[local, remote].')
             obj = urllib.parse.urlparse(out[1])
         if obj.scheme not in UPLOADERS:
             raise ValueError(f'Invalid Cloud provider prefix: {obj.scheme}.')
 
     def __init__(self,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
@@ -177,14 +188,15 @@
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         super().__init__(out, keep_local, progress_bar)
 
         import boto3
         from botocore.config import Config
+
         config = Config()
         # Create a session and use it to make our client. Unlike Resources and Sessions,
         # clients are generally thread-safe.
         session = boto3.session.Session()
         self.s3 = session.client('s3',
                                  config=config,
                                  endpoint_url=os.environ.get('S3_ENDPOINT_URL'))
@@ -255,69 +267,98 @@
 
     def __init__(self,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         super().__init__(out, keep_local, progress_bar)
 
-        import boto3
+        if 'GOOGLE_APPLICATION_CREDENTIALS' in os.environ:
+            from google.cloud.storage import Client
+
+            service_account_path = os.environ['GOOGLE_APPLICATION_CREDENTIALS']
+            self.gcs_client = Client.from_service_account_json(service_account_path)
+            self.authentication = GCSAuthentication.SERVICE_ACCOUNT
+        elif 'GCS_KEY' in os.environ and 'GCS_SECRET' in os.environ:
+            import boto3
+
+            # Create a session and use it to make our client. Unlike Resources and Sessions,
+            # clients are generally thread-safe.
+            session = boto3.session.Session()
+            self.gcs_client = session.client(
+                's3',
+                region_name='auto',
+                endpoint_url='https://storage.googleapis.com',
+                aws_access_key_id=os.environ['GCS_KEY'],
+                aws_secret_access_key=os.environ['GCS_SECRET'],
+            )
+            self.authentication = GCSAuthentication.HMAC
+        else:
+            raise ValueError(f'Either GOOGLE_APPLICATION_CREDENTIALS needs to be set for ' +
+                             f'service level accounts or GCS_KEY and GCS_SECRET needs to ' +
+                             f'be set for HMAC authentication')
 
-        # Create a session and use it to make our client. Unlike Resources and Sessions,
-        # clients are generally thread-safe.
-        session = boto3.session.Session()
-        self.gcs_client = session.client('s3',
-                                         region_name='auto',
-                                         endpoint_url='https://storage.googleapis.com',
-                                         aws_access_key_id=os.environ['GCS_KEY'],
-                                         aws_secret_access_key=os.environ['GCS_SECRET'])
         self.check_bucket_exists(self.remote)  # pyright: ignore
 
-    def upload_file(self, filename: str):
+    def upload_file(self, filename: str) -> None:
         """Upload file from local instance to Google Cloud Storage bucket.
 
         Args:
             filename (str): File to upload.
         """
         local_filename = os.path.join(self.local, filename)
         remote_filename = os.path.join(self.remote, filename)  # pyright: ignore
         obj = urllib.parse.urlparse(remote_filename)
         logger.debug(f'Uploading to {remote_filename}')
-        file_size = os.stat(local_filename).st_size
-        with tqdm.tqdm(total=file_size,
-                       unit='B',
-                       unit_scale=True,
-                       desc=f'Uploading to {remote_filename}',
-                       disable=(not self.progress_bar)) as pbar:
-            self.gcs_client.upload_file(
-                local_filename,
-                obj.netloc,
-                obj.path.lstrip('/'),
-                Callback=lambda bytes_transferred: pbar.update(bytes_transferred),
-            )
+
+        if self.authentication == GCSAuthentication.HMAC:
+            file_size = os.stat(local_filename).st_size
+            with tqdm.tqdm(
+                    total=file_size,
+                    unit='B',
+                    unit_scale=True,
+                    desc=f'Uploading to {remote_filename}',
+                    disable=(not self.progress_bar),
+            ) as pbar:
+                self.gcs_client.upload_file(
+                    local_filename,
+                    obj.netloc,
+                    obj.path.lstrip('/'),
+                    Callback=lambda bytes_transferred: pbar.update(bytes_transferred),
+                )
+        elif self.authentication == GCSAuthentication.SERVICE_ACCOUNT:
+            from google.cloud.storage import Blob, Bucket
+
+            blob = Blob(obj.path.lstrip('/'), Bucket(self.gcs_client, obj.netloc))
+            blob.upload_from_filename(local_filename)
+
         self.clear_local(local=local_filename)
 
-    def check_bucket_exists(self, remote: str):
+    def check_bucket_exists(self, remote: str) -> None:
         """Raise an exception if the bucket does not exist.
 
         Args:
             remote (str): GCS bucket path.
 
         Raises:
             error: Bucket does not exist.
         """
-        from botocore.exceptions import ClientError
-
         bucket_name = urllib.parse.urlparse(remote).netloc
-        try:
-            self.gcs_client.head_bucket(Bucket=bucket_name)
-        except ClientError as error:
-            if error.response['Error']['Code'] == BOTOCORE_CLIENT_ERROR_CODES:
-                error.args = (f'Either bucket `{bucket_name}` does not exist! ' +
-                              f'or check the bucket permission.',)
-            raise error
+
+        if self.authentication == GCSAuthentication.HMAC:
+            from botocore.exceptions import ClientError
+
+            try:
+                self.gcs_client.head_bucket(Bucket=bucket_name)
+            except ClientError as error:
+                if (error.response['Error']['Code'] == BOTOCORE_CLIENT_ERROR_CODES):
+                    error.args = (f'Either bucket `{bucket_name}` does not exist! ' +
+                                  f'or check the bucket permission.',)
+                raise error
+        elif self.authentication == GCSAuthentication.SERVICE_ACCOUNT:
+            self.gcs_client.get_bucket(bucket_name)
 
 
 class OCIUploader(CloudUploader):
     """Upload file from local machine to Oracle Cloud Infrastructure (OCI) Cloud Storage.
 
     Args:
         out (str | Tuple[str, str]): Output dataset directory to save shard files.
@@ -337,14 +378,15 @@
     def __init__(self,
                  out: Union[str, Tuple[str, str]],
                  keep_local: bool = False,
                  progress_bar: bool = False) -> None:
         super().__init__(out, keep_local, progress_bar)
 
         import oci
+
         config = oci.config.from_file()
         self.client = oci.object_storage.ObjectStorageClient(
             config=config, retry_strategy=oci.retry.DEFAULT_RETRY_STRATEGY)
         self.namespace = self.client.get_namespace().data
         self.upload_manager = oci.object_storage.UploadManager(self.client)
         self.check_bucket_exists(self.remote)  # pyright: ignore
 
@@ -424,15 +466,16 @@
 
         from azure.storage.blob import BlobServiceClient
 
         # Create a session and use it to make our client. Unlike Resources and Sessions,
         # clients are generally thread-safe.
         self.azure_service = BlobServiceClient(
             account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.blob.core.windows.net",
-            credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'])
+            credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'],
+        )
         self.check_bucket_exists(self.remote)  # pyright: ignore
 
     def upload_file(self, filename: str):
         """Upload file from local instance to Microsoft Azure bucket.
 
         Args:
             filename (str): File to upload.
@@ -471,14 +514,89 @@
         bucket_name = urllib.parse.urlparse(remote).netloc
         if self.azure_service.get_container_client(container=bucket_name).exists() is False:
             raise FileNotFoundError(
                 f'Either bucket `{bucket_name}` does not exist! ' +
                 f'or check the bucket permission.',)
 
 
+class AzureDataLakeUploader(CloudUploader):
+    """Upload file from local machine to Microsoft Azure DataLake.
+
+    Args:
+        out (str | Tuple[str, str]): Output dataset directory to save shard files.
+
+            1. If ``out`` is a local directory, shard files are saved locally.
+            2. If ``out`` is a remote directory, a local temporary directory is created to
+               cache the shard files and then the shard files are uploaded to a remote
+               location. At the end, the temp directory is deleted once shards are uploaded.
+            3. If ``out`` is a tuple of ``(local_dir, remote_dir)``, shard files are saved in
+               the `local_dir` and also uploaded to a remote location.
+        keep_local (bool): If the dataset is uploaded, whether to keep the local dataset
+            shard file or remove it after uploading. Defaults to ``False``.
+        progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
+            a remote location. Default to ``False``.
+    """
+
+    def __init__(self,
+                 out: Union[str, Tuple[str, str]],
+                 keep_local: bool = False,
+                 progress_bar: bool = False) -> None:
+        super().__init__(out, keep_local, progress_bar)
+
+        from azure.storage.filedatalake import DataLakeServiceClient
+
+        # Create a session and use it to make our client. Unlike Resources and Sessions,
+        # clients are generally thread-safe.
+        self.azure_service = DataLakeServiceClient(
+            account_url=f"https://{os.environ['AZURE_ACCOUNT_NAME']}.dfs.core.windows.net",
+            credential=os.environ['AZURE_ACCOUNT_ACCESS_KEY'])
+        self.check_container_exists(self.remote)  # pyright: ignore
+
+    def upload_file(self, filename: str):
+        """Upload file from local instance to Azure DataLalke container.
+
+        Args:
+            filename (str): File to upload.
+        """
+        local_filename = os.path.join(self.local, filename)
+        local_filename = local_filename.replace('\\', '/')
+        remote_filename = os.path.join(self.remote, filename)  # pyright: ignore
+        remote_filename = remote_filename.replace('\\', '/')
+        obj = urllib.parse.urlparse(remote_filename)
+        logger.debug(f'Uploading to {remote_filename}')
+        file_size = os.stat(local_filename).st_size
+        file_client = self.azure_service.get_file_client(file_system=obj.netloc,
+                                                         file_path=obj.path.lstrip('/'))
+
+        with tqdm.tqdm(total=file_size,
+                       unit='B',
+                       unit_scale=True,
+                       desc=f'Uploading to {remote_filename}',
+                       disable=(not self.progress_bar)) as pbar:
+            with open(local_filename, 'rb') as data:
+                file_client.upload_data(data=data, overwrite=True)
+                pbar.update(file_size)
+        self.clear_local(local=local_filename)
+
+    def check_container_exists(self, remote: str):
+        """Raise an exception if the container does not exist.
+
+        Args:
+            remote (str): azure container path.
+
+        Raises:
+            error: Container does not exist.
+        """
+        container_name = urllib.parse.urlparse(remote).netloc
+        if self.azure_service.get_file_system_client(file_system=container_name).exists() is False:
+            raise FileNotFoundError(
+                f'Either container `{container_name}` does not exist! ' +
+                f'or check the container permission.',)
+
+
 class LocalUploader(CloudUploader):
     """Copy file from one local directory to another local directory.
 
     Args:
         out (str | Tuple[str, str]): Output dataset directory to save shard files.
 
             1. If ``out`` is a local directory, shard files are saved locally.
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/stream.py` & `mosaicml-streaming-0.5.2/streaming/base/stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A dataset, or sub-dataset if mixing, from which we stream/cache samples."""
 
+import hashlib
 import json
 import os
-from tempfile import mkdtemp
+import tempfile
 from typing import List, Optional, Sequence
 
 import numpy as np
 from numpy.typing import NDArray
 from typing_extensions import Self
 
 from streaming.base.compression import decompress
 from streaming.base.constant import TICK
+from streaming.base.distributed import barrier, get_local_rank
 from streaming.base.format import FileInfo, Reader, get_index_basename, reader_from_json
 from streaming.base.hashing import get_hash
 from streaming.base.storage import download_file
 from streaming.base.util import wait_for_file_to_exist
 from streaming.base.world import World
 
 
@@ -94,15 +96,14 @@
                  choose: Optional[int] = None,
                  download_retry: Optional[int] = None,
                  download_timeout: Optional[float] = None,
                  validate_hash: Optional[str] = None,
                  keep_zip: Optional[bool] = None) -> None:
         self.remote = remote
         self._local = local
-        self.local = local or mkdtemp()
         self.split = split or ''
 
         has_proportion = proportion is not None
         has_repeat = repeat is not None
         has_choose = choose is not None
         if not (0 <= has_proportion + has_repeat + has_choose <= 1):
             raise ValueError('At most one of `proportion`, `repeat`, and `choose` may be ' +
@@ -136,41 +137,62 @@
         if download_timeout is not None:
             if download_timeout <= 0:
                 raise ValueError('`download_timeout` must be positive')
             self.download_timeout = download_timeout
 
         self.validate_hash = validate_hash
 
+        if local is None:
+            self.local = self._get_temporary_directory()
+            if get_local_rank() == 0:
+                if os.path.exists(self.local):
+                    raise ValueError(
+                        f'Could not create a temporary local directory {self.local} . Either ' +
+                        f'delete the directory or specify a unique local directory with the ' +
+                        f'`local` value.')
+                os.makedirs(self.local)
+            barrier()
+        else:
+            self.local = local
+
         self._keep_zip = keep_zip
         if keep_zip is not None:
             self.keep_zip = keep_zip
             self.safe_keep_zip = self.keep_zip or self.remote in {None, self.local}
 
-    def apply_default(self, default: Self) -> None:
+    def _get_temporary_directory(self) -> str:
+        """Construct a path to a temporary directory based on remote and split."""
+        root = tempfile.gettempdir()
+        hash = ''
+        if self.remote is not None:
+            hash = hashlib.blake2s(self.remote.encode('utf-8'), digest_size=16).hexdigest()
+        return os.path.join(root, hash, self.split)
+
+    def apply_default(self, default: dict) -> None:
         """Apply defaults, setting any unset fields.
 
         We use pairs of (name, _name) in order to make type checking happy.
 
         Args:
             default (Self): Stream containing default values for all optional fields.
         """
         if not (self.remote or self._local):
             raise ValueError('`remote` and/or `local` path must be provided')
 
         if not self.split:
-            self.split = default.split or ''
+            self.split = default['split'] or ''
         if self._download_retry is None:
-            self.download_retry = default.download_retry
+            self.download_retry = default['download_retry']
         if self._download_timeout is None:
-            self.download_timeout = default.download_timeout
+            self.download_timeout = default['download_timeout']
         if self.validate_hash is None:
-            self.validate_hash = default.validate_hash or None
+            self.validate_hash = default['validate_hash'] or None
         if self._keep_zip is None:
-            self.keep_zip = default.keep_zip
-            self.safe_keep_zip = self.keep_zip or self.remote in {None, self.local}
+            self.keep_zip = default['keep_zip']
+            self.safe_keep_zip = default['keep_zip'] or self.remote in {None, self.local}
 
     @classmethod
     def validate_weights(cls, streams: Sequence[Self]) -> bool:
         """Validate stream weights, returning whether relative or absolute weighting was used.
 
         Args:
             streams (Sequence[Stream]): Every stream comprising the dataset.
@@ -309,65 +331,86 @@
         data = decompress(compression, data)  # pyright: ignore
         tmp_filename = raw_filename + '.tmp'
         with open(tmp_filename, 'wb') as out:
             out.write(data)
         os.rename(tmp_filename, raw_filename)
 
         # Maybe remove compressed to save space.
-        if not self.keep_zip and self.remote != self.local:
+        if not self.safe_keep_zip:
             os.remove(zip_filename)
 
-    def _download_shard_part(self,
-                             raw_info: FileInfo,
-                             zip_info: Optional[FileInfo] = None,
-                             compression: Optional[str] = None) -> None:
-        """Download shard data given metadata for the raw and compressed versions of it.
+    def _prepare_shard_part(self,
+                            raw_info: FileInfo,
+                            zip_info: Optional[FileInfo] = None,
+                            compression: Optional[str] = None) -> int:
+        """Get shard data given metadata for the raw and compressed versions of it.
 
         MDS format uses joint shards (ie, one file per shard). Other formats supported by streaming
         use split shards (ie, shard data lives in two files per shard: the raw data itself and
         metadata in a separate file).
 
         Args:
             raw_info (FileInfo): Raw file info.
             zip_info (FileInfo, optional): Zip file info. Defaults to ``None``.
             compression (str, optional): Compression algorithm used for zip_info. Defaults to
                 ``None``.
+
+        Returns:
+            int: Change in cache usage.
         """
-        # If the local raw file already exists, this is a no-op.
+        # Has raw?
+        delta = 0
         raw_filename = os.path.join(self.local, self.split, raw_info.basename)
         if os.path.isfile(raw_filename):
-            return
-
-        # Is compression used?
-        if zip_info:
-            # Download the compressed form if missing.
-            zip_filename = os.path.join(self.local, self.split, zip_info.basename)
-            if not os.path.isfile(zip_filename):
-                self._download_file(zip_info.basename)
-
-            # Validate and decompress.
-            self._decompress_shard_part(zip_info, zip_filename, raw_filename, compression)
+            # Has raw.
+            if zip_info and not self.safe_keep_zip:
+                zip_filename = os.path.join(self.local, self.split, zip_info.basename)
+                if os.path.isfile(zip_filename):
+                    # If don't keep zip and it has a zip, drop the zip.
+                    os.remove(zip_filename)
+                    delta -= zip_info.bytes
         else:
-            # Download the raw form.
-            self._download_file(raw_info.basename)
-
-            # Validate if requested.
-            if self.validate_hash:
-                data = open(raw_filename, 'rb').read()
-                if get_hash(self.validate_hash, data) != raw_info.hashes[self.validate_hash]:
-                    raise ValueError(f'Checksum failure: {raw_filename}')
+            # Missing raw. Uses zip?
+            if zip_info:
+                # Ensure has zip.
+                zip_filename = os.path.join(self.local, self.split, zip_info.basename)
+                if not os.path.isfile(zip_filename):
+                    self._download_file(zip_info.basename)
+                    delta += zip_info.bytes
+
+                # Validate and decompress.
+                self._decompress_shard_part(zip_info, zip_filename, raw_filename, compression)
+                delta += raw_info.bytes
+                if not self.safe_keep_zip:
+                    delta -= zip_info.bytes
+            else:
+                # Download raw.
+                self._download_file(raw_info.basename)
+                delta += raw_info.bytes
+
+                # Validate.
+                if self.validate_hash:
+                    data = open(raw_filename, 'rb').read()
+                    if get_hash(self.validate_hash, data) != raw_info.hashes[self.validate_hash]:
+                        raise ValueError(f'Checksum failure: {raw_filename}')
+        return delta
 
-    def download_shard(self, shard: Reader) -> None:
-        """Download the given shard.
+    def prepare_shard(self, shard: Reader) -> int:
+        """Ensure (download, validate, extract, etc.) that we have the given shard.
 
         Args:
             shard (Reader): Which shard.
+
+        Returns:
+            int: Change in cache usage.
         """
+        delta = 0
         for raw_info, zip_info in shard.file_pairs:
-            self._download_shard_part(raw_info, zip_info, shard.compression)
+            delta += self._prepare_shard_part(raw_info, zip_info, shard.compression)
+        return delta
 
     def get_shards(self, world: World) -> List[Reader]:
         """Load this Stream's index, retrieving its shard readers.
 
         Args:
             world (World): Distributed context.
 
@@ -375,14 +418,18 @@
             `List[Reader]: Shard readers.
         """
         # Download the index.
         basename = get_index_basename()
         filename = os.path.join(self.local, self.split, basename)  # pyright: ignore
         if world.is_local_leader:
             if self.remote:
+                # Downloads the `index.json` as `index.json.tmp` fully and then rename it to
+                # `index.json` since only one process downloads the `index.json` file while
+                # other processes wait for it to get downloaded. Hence, It avoids loading the
+                # in-progress downloading `index.json`.
                 tmp_filename = self._download_file(basename, basename + '.tmp')
                 os.rename(tmp_filename, filename)
             else:
                 if not os.path.exists(filename):
                     raise RuntimeError(f'No `remote` provided, but local file {filename} ' +
                                        'does not exist either')
         else:
@@ -407,37 +454,32 @@
         shards = []
         for info in obj['shards']:
             shard = reader_from_json(self.local, self.split, info)
             shards.append(shard)
 
         return shards
 
-    def init_local_dir(self, shards: List[Reader]) -> List[bool]:
+    def set_up_local(self, shards: List[Reader], cache_usage_per_shard: NDArray[np.int64]) -> None:
         """Bring a local directory into a consistent state, getting which shards are present.
 
         Args:
             shards (List[Reader]): List of this stream's shards.
-
-        Returns:
-            List[bool]: List of whether each stream shard is present.
+            cache_usage_per_shard (NDArray[np.int64]): Cache usage per shard of this stream.
         """
         # List the cache directory (so that we hit the filesystem once).
         local_dirname = os.path.join(self.local, self.split)
         listing = set()
         for dirname, _, subfiles in os.walk(local_dirname):
             for subfile in subfiles:
                 filename = os.path.join(dirname, subfile)
                 listing.add(filename)
 
         # Determine which shards are present, making local dir consistent.
-        are_shards_present = []
-        for shard in shards:
-            is_shard_present = shard.init_local_dir(listing, self.safe_keep_zip)
-            are_shards_present.append(is_shard_present)
-        return are_shards_present
+        for i, shard in enumerate(shards):
+            cache_usage_per_shard[i] = shard.set_up_local(listing, self.safe_keep_zip)
 
     def get_index_size(self) -> int:
         """Get the size of the index file in bytes.
 
         Returns:
             int: Size in bytes.
         """
```

### Comparing `mosaicml-streaming-0.5.1/streaming/base/world.py` & `mosaicml-streaming-0.5.2/streaming/base/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.5.2/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid.py` & `mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py` & `mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py` & `mosaicml-streaming-0.5.2/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.5.2/streaming/multimodal/webvid.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,42 +353,42 @@
         while True:
             # If we've started a new epoch early (__iter__ was called again), exit this thread
             # because there can only be one epoch at once.
             if it.should_exit():
                 break
 
             # If we're out of samples this epoch, exit this thread because we are done downloading.
-            if it.download_index == it.total:
+            if it.prepare_index == it.total:
                 break
 
             # If we are requested to only pre-download so many samples, if we have as many or more
             # downloaded already, we wait and check again later.
             if self.predownload is not None:
-                samples_ahead = it.download_index - it.yield_index
+                samples_ahead = it.prepare_index - it.yield_index
                 if self.predownload <= samples_ahead:
                     sleep(TICK)
                     continue
 
             # If we hit -1, we skip.
-            sample_id = it.sample_ids[it.download_index]
+            sample_id = it.sample_ids[it.prepare_index]
             if sample_id == -1:
-                it.download_index += 1
+                it.prepare_index += 1
                 continue
 
             # Download and decompress the shard for this sample, if not already done.
             shard_id, _ = self.spanner[sample_id]
-            self.download_shard(shard_id, False)
+            self.prepare_shard(shard_id, False)
 
             # Predownload the sample's extra data.
             obj = super().get_item(sample_id)
             if self.extra_local and self.extra_remote:
                 rel_path = obj['content_path']
                 local = os.path.join(self.extra_local, rel_path)
                 remote = os.path.join(self.extra_remote, rel_path)
                 if not os.path.exists(local):
                     download_file(remote, local, self.download_timeout)
 
             # Step forward one sample.
-            it.download_index += 1
+            it.prepare_index += 1
 
         # Note that we exited.
         it.on_exit()
```

### Comparing `mosaicml-streaming-0.5.1/streaming/text/c4.py` & `mosaicml-streaming-0.5.2/streaming/text/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/c4.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/convert/pile.py` & `mosaicml-streaming-0.5.2/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/enwiki.py` & `mosaicml-streaming-0.5.2/streaming/text/enwiki.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/text/pile.py` & `mosaicml-streaming-0.5.2/streaming/text/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/ade20k.py` & `mosaicml-streaming-0.5.2/streaming/vision/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/base.py` & `mosaicml-streaming-0.5.2/streaming/vision/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/cifar10.py` & `mosaicml-streaming-0.5.2/streaming/vision/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/coco.py` & `mosaicml-streaming-0.5.2/streaming/vision/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/base.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.5.2/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/streaming/vision/imagenet.py` & `mosaicml-streaming-0.5.2/streaming/vision/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_array.py` & `mosaicml-streaming-0.5.2/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_barrier.py` & `mosaicml-streaming-0.5.2/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_compression.py` & `mosaicml-streaming-0.5.2/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_distributed.py` & `mosaicml-streaming-0.5.2/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_download.py` & `mosaicml-streaming-0.5.2/tests/test_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import Any, Tuple
 from unittest.mock import Mock, patch
 
 import boto3
 import pytest
 from botocore.exceptions import ClientError
 
-from streaming.base.storage.download import (download_file, download_from_azure, download_from_gcs,
+from streaming.base.storage.download import (download_file, download_from_azure,
+                                             download_from_azure_datalake, download_from_gcs,
                                              download_from_local, download_from_s3,
                                              download_or_wait)
 from tests.conftest import GCS_URL, MY_BUCKET, R2_URL
 
 MY_PREFIX = 'train'
 
 
@@ -38,14 +39,15 @@
 
     @pytest.mark.usefixtures('remote_local_file')
     def test_invalid_cloud_prefix(self, remote_local_file: Any):
         with pytest.raises(ValueError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(
                 cloud_prefix='aaazure://')
             download_from_azure(mock_remote_filepath, mock_local_filepath)
+            download_from_azure_datalake(mock_remote_filepath, mock_local_filepath)
 
 
 class TestS3Client:
 
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
     def test_download_from_s3(self, remote_local_file: Any):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
@@ -78,35 +80,35 @@
         with pytest.raises(ValueError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='s9://')
             download_from_s3(mock_remote_filepath, mock_local_filepath, 60)
 
 
 class TestGCSClient:
 
-    @pytest.mark.usefixtures('gcs_client', 'gcs_test', 'remote_local_file')
+    @pytest.mark.usefixtures('gcs_hmac_client', 'gcs_test', 'remote_local_file')
     def test_download_from_gcs(self, remote_local_file: Any):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
             file_name = tmp.name.split(os.sep)[-1]
             mock_remote_filepath, _ = remote_local_file(cloud_prefix='gs://', filename=file_name)
             client = boto3.client('s3',
                                   region_name='us-east-1',
                                   endpoint_url=GCS_URL,
                                   aws_access_key_id=os.environ['GCS_KEY'],
                                   aws_secret_access_key=os.environ['GCS_SECRET'])
             client.put_object(Bucket=MY_BUCKET, Key=os.path.join(MY_PREFIX, file_name), Body='')
             download_from_gcs(mock_remote_filepath, tmp.name)
             assert os.path.isfile(tmp.name)
 
-    @pytest.mark.usefixtures('gcs_client', 'gcs_test', 'remote_local_file')
+    @pytest.mark.usefixtures('gcs_hmac_client', 'gcs_test', 'remote_local_file')
     def test_filenotfound_exception(self, remote_local_file: Any):
         with pytest.raises(FileNotFoundError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='gs://')
             download_from_gcs(mock_remote_filepath, mock_local_filepath)
 
-    @pytest.mark.usefixtures('gcs_client', 'gcs_test', 'remote_local_file')
+    @pytest.mark.usefixtures('gcs_hmac_client', 'gcs_test', 'remote_local_file')
     def test_invalid_cloud_prefix(self, remote_local_file: Any):
         with pytest.raises(ValueError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='s3://')
             download_from_gcs(mock_remote_filepath, mock_local_filepath)
 
 
 def test_download_from_local():
@@ -145,14 +147,23 @@
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_azure_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='azure://')
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
 
+    @patch('streaming.base.storage.download.download_from_azure_datalake')
+    @pytest.mark.usefixtures('remote_local_file')
+    def test_download_from_azure_datalake_gets_called(self, mocked_requests: Mock,
+                                                      remote_local_file: Any):
+        mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='azure-dl://')
+        download_file(mock_remote_filepath, mock_local_filepath, 60)
+        mocked_requests.assert_called_once()
+        mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
+
     @patch('streaming.base.storage.download.download_from_sftp')
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_sftp_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='sftp://')
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
```

### Comparing `mosaicml-streaming-0.5.1/tests/test_encodings.py` & `mosaicml-streaming-0.5.2/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_eviction.py` & `mosaicml-streaming-0.5.2/tests/test_eviction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 import operator
 import os
 from shutil import rmtree
-from typing import Tuple
+from typing import Any, Tuple
 
 import pytest
 from torch.utils.data import DataLoader
 
 from streaming import MDSWriter, StreamingDataset
 
 
@@ -88,15 +88,15 @@
 def manual_shard_eviction(remote: str, local: str, keep_zip: bool):
     """
     Manually downloading and evicting shards.
     """
     dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip)
 
     for shard_id in range(dataset.num_shards):
-        dataset.download_shard(shard_id)
+        dataset.prepare_shard(shard_id)
 
     full = set(os.listdir(local))
 
     for shard_id in range(dataset.num_shards):
         dataset.evict_shard(shard_id)
 
     assert os.listdir(local) == ['index.json']
@@ -115,20 +115,23 @@
     with pytest.raises(ValueError):
         dataset = StreamingDataset(remote=remote, local=local, cache_limit='1kb')
         for _ in dataset:
             pass
     rmtree(local, ignore_errors=False)
 
 
-funcs = shard_eviction_disabled, shard_eviction_too_high, shard_eviction, manual_shard_eviction,
-cache_limit_too_low,
+funcs = [
+    shard_eviction_disabled, shard_eviction_too_high, shard_eviction, manual_shard_eviction,
+    cache_limit_too_low
+]
 
 
 @pytest.mark.usefixtures('local_remote_dir')
-def test_eviction_nozip(local_remote_dir: Tuple[str, str]):
+@pytest.mark.parametrize('func', [f for f in funcs])
+def test_eviction_nozip(local_remote_dir: Tuple[str, str], func: Any):
     num_samples = 5_000
     local, remote = local_remote_dir
     columns = {'data': 'bytes'}
     compression = None
     hashes = None
     size_limit = 500
 
@@ -137,20 +140,20 @@
                    compression=compression,
                    hashes=hashes,
                    size_limit=size_limit) as out:
         for _ in range(num_samples):
             sample = {'data': b'\0'}
             out.write(sample)
 
-    for func in funcs:
-        func(remote, local, False)
+    func(remote, local, False)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
-def test_eviction_zip_nokeep(local_remote_dir: Tuple[str, str]):
+@pytest.mark.parametrize('func', [f for f in funcs])
+def test_eviction_zip_nokeep(local_remote_dir: Tuple[str, str], func: Any):
     num_samples = 5_000
     local, remote = local_remote_dir
     columns = {'data': 'bytes'}
     compression = 'zstd'
     hashes = None
     size_limit = 500
 
@@ -159,20 +162,20 @@
                    compression=compression,
                    hashes=hashes,
                    size_limit=size_limit) as out:
         for _ in range(num_samples):
             sample = {'data': b'\0'}
             out.write(sample)
 
-    for func in funcs:
-        func(remote, local, False)
+    func(remote, local, False)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
-def test_eviction_zip_keep(local_remote_dir: Tuple[str, str]):
+@pytest.mark.parametrize('func', [f for f in funcs])
+def test_eviction_zip_keep(local_remote_dir: Tuple[str, str], func: Any):
     num_samples = 5_000
     local, remote = local_remote_dir
     columns = {'data': 'bytes'}
     compression = 'zstd'
     hashes = None
     size_limit = 500
 
@@ -181,9 +184,8 @@
                    compression=compression,
                    hashes=hashes,
                    size_limit=size_limit) as out:
         for _ in range(num_samples):
             sample = {'data': b'\0'}
             out.write(sample)
 
-    for func in funcs:
-        func(remote, local, True)
+    func(remote, local, True)
```

### Comparing `mosaicml-streaming-0.5.1/tests/test_hashing.py` & `mosaicml-streaming-0.5.2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_laziness.py` & `mosaicml-streaming-0.5.2/tests/test_laziness.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-from shutil import rmtree
-from typing import Tuple
+from typing import Any, Tuple
 
 import pytest
 
 from streaming import MDSWriter, StreamingDataset
 
 
 def one(remote: str, local: str):
@@ -32,15 +31,14 @@
     """
     Verify __getitem__ downloads/accesses.
     """
     dataset = StreamingDataset(local=local, remote=remote)
     for i in range(dataset.num_samples):
         sample = dataset[i]
         assert sample['value'] == i
-    rmtree(local)
 
 
 def four(remote: str, local: str):
     """
     Verify __iter__ -> __getitem__ downloads/accesses.
     """
     dataset = StreamingDataset(local=local, remote=remote, num_canonical_nodes=1)
@@ -56,15 +54,16 @@
     dataset = StreamingDataset(local=local, remote=remote)
     for i in range(dataset.num_samples):
         sample = dataset[i]
         assert sample['value'] == i
 
 
 @pytest.mark.usefixtures('local_remote_dir')
-def test_laziness(local_remote_dir: Tuple[str, str]):
+@pytest.mark.parametrize('func', [one, two, three, four, five])
+def test_laziness(local_remote_dir: Tuple[str, str], func: Any):
     num_samples = 10_000
     local, remote = local_remote_dir
     columns = {'value': 'int'}
     compression = None
     hashes = None
     size_limit = 1_000
 
@@ -73,9 +72,8 @@
                    compression=compression,
                    hashes=hashes,
                    size_limit=size_limit) as out:
         for i in range(num_samples):
             sample = {'value': i}
             out.write(sample)
 
-    for func in [one, two, three, four, five]:
-        func(remote, local)
+    func(remote, local)
```

### Comparing `mosaicml-streaming-0.5.1/tests/test_local.py` & `mosaicml-streaming-0.5.2/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_mixing.py` & `mosaicml-streaming-0.5.2/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_partition.py` & `mosaicml-streaming-0.5.2/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_reader.py` & `mosaicml-streaming-0.5.2/tests/test_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,53 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 import json
 import logging
 import os
 import shutil
-import tempfile
 import time
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 import pytest
 from numpy.typing import NDArray
 
 from streaming.base import StreamingDataset
-from tests.common.datasets import SequenceDataset, write_mds_dataset
-from tests.common.utils import copy_all_files
+from tests.common.utils import convert_to_mds, copy_all_files
 
 logger = logging.getLogger(__name__)
 
 
-@pytest.fixture(scope='function')
-def mds_dataset_dir():
-    try:
-        mock_dir = tempfile.TemporaryDirectory()
-        remote_dir = os.path.join(mock_dir.name, 'remote')
-        local_dir = os.path.join(mock_dir.name, 'local')
-        num_samples = 117
-        size_limit = 1 << 8
-        dataset = SequenceDataset(num_samples)
-        columns = dict(zip(dataset.column_names, dataset.column_encodings))
-
-        write_mds_dataset(out_root=remote_dir,
-                          columns=columns,
-                          samples=dataset,
-                          size_limit=size_limit)
-        yield remote_dir, local_dir
-    finally:
-        mock_dir.cleanup()  # pyright: ignore
-
-
 @pytest.mark.parametrize('batch_size', [None, 1, 2])
-@pytest.mark.parametrize('remote_arg', ['none', 'same', 'different'])
+@pytest.mark.parametrize('remote_arg', ['empty', 'same', 'different', 'local'])
 @pytest.mark.parametrize('shuffle', [False, True])
 @pytest.mark.parametrize('seed', [5151])
 @pytest.mark.parametrize('num_canonical_nodes', [1])
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_dataset_sample_order(mds_dataset_dir: Any, batch_size: int, remote_arg: str,
-                              shuffle: bool, seed: int, num_canonical_nodes: int):
+@pytest.mark.parametrize('compression', [None, 'zstd:7'])
+@pytest.mark.usefixtures('local_remote_dir')
+def test_dataset_sample_order(local_remote_dir: Any, batch_size: int, remote_arg: str,
+                              shuffle: bool, seed: int, num_canonical_nodes: int,
+                              compression: str):
     num_samples = 117
-    remote_dir, local_dir = mds_dataset_dir
-    if remote_arg == 'none':
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=num_samples,
+                   compression=compression,
+                   size_limit=1 << 8)
+    if remote_arg == 'empty':
         local_dir = remote_dir
         remote_dir = None
     elif remote_arg == 'same':
         local_dir = remote_dir
     elif remote_arg == 'different':
         pass
+    elif remote_arg == 'local':
+        local_dir = None
     else:
         assert False, f'Unknown value of remote_arg: {remote_arg}'
 
     # Build StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
@@ -95,17 +82,24 @@
         dataset
     ) == num_samples, f'Got dataset length={len(dataset)} samples, expected {num_samples}'
 
 
 @pytest.mark.parametrize('batch_size', [None, 1, 2])
 @pytest.mark.parametrize('seed', [8988])
 @pytest.mark.parametrize('shuffle', [False, True])
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_dataset_determinism(mds_dataset_dir: Any, batch_size: int, seed: int, shuffle: bool):
-    remote_dir, local_dir = mds_dataset_dir
+@pytest.mark.parametrize('compression', [None, 'gz:3'])
+@pytest.mark.usefixtures('local_remote_dir')
+def test_dataset_determinism(local_remote_dir: Any, batch_size: int, seed: int, shuffle: bool,
+                             compression: str):
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   compression=compression,
+                   size_limit=1 << 8)
 
     # Build StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
                                shuffle_seed=seed)
@@ -134,17 +128,21 @@
 
 
 @pytest.mark.parametrize(
     'missing_file',
     ['index'],
 )
 @pytest.mark.parametrize('seed', [7777])
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_reader_download_fail(mds_dataset_dir: Any, missing_file: str, seed: int):
-    remote_dir, local_dir = mds_dataset_dir
+@pytest.mark.usefixtures('local_remote_dir')
+def test_reader_download_fail(local_remote_dir: Any, missing_file: str, seed: int):
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
 
     if missing_file == 'index':
         os.remove(os.path.join(remote_dir, 'index.json'))
 
     # Build and iterate over a StreamingDataset
     with pytest.raises(FileNotFoundError) as exc_info:
         dataset = StreamingDataset(local=local_dir,
@@ -156,18 +154,22 @@
             pass
     assert exc_info.match(r'.*No such file or directory*')
 
 
 @pytest.mark.parametrize('created_ago', [0.5, 1.0])
 @pytest.mark.parametrize('download_timeout', [1])
 @pytest.mark.parametrize('seed', [2569])
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_reader_after_crash(mds_dataset_dir: Any, created_ago: float, download_timeout: float,
+@pytest.mark.usefixtures('local_remote_dir')
+def test_reader_after_crash(local_remote_dir: Any, created_ago: float, download_timeout: float,
                             seed: int):
-    remote_dir, local_dir = mds_dataset_dir
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
 
     if not os.path.exists(local_dir):
         os.mkdir(local_dir)
 
     shutil.copy(os.path.join(remote_dir, f'index.json'),
                 os.path.join(local_dir, f'index.json.tmp'))
     shutil.copy(os.path.join(remote_dir, f'shard.00003.mds'),
@@ -216,92 +218,112 @@
 @pytest.mark.parametrize(
     'share_remote_local',
     [
         True,
         # False,
     ],
 )
-@pytest.mark.usefixtures('mds_dataset_dir')
+@pytest.mark.usefixtures('local_remote_dir')
 @pytest.mark.parametrize('index', [
     -1, 0, [17], [44, 98], [-14, -87, -55],
     slice(0, 29, 3),
     slice(-27, -99, -5),
     np.arange(10),
     np.array([3, 19, -70, -32])
 ])
 @pytest.mark.parametrize('seed', [5566])
-def test_reader_getitem(mds_dataset_dir: Any, share_remote_local: bool,
+def test_reader_getitem(local_remote_dir: Any, share_remote_local: bool,
                         index: Union[int, slice, List[int], NDArray[np.int64]], seed: int):
-    remote_dir, local_dir = mds_dataset_dir
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
     if share_remote_local:
         local_dir = remote_dir
 
     # Build a StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=False,
                                shuffle_seed=seed)
 
     # Test retrieving random sample
     sample = dataset[index]
     _validate_sample(index, sample, len(dataset))
 
 
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_dataset_split_instantiation(mds_dataset_dir: Any):
+@pytest.mark.usefixtures('local_remote_dir')
+def test_dataset_split_instantiation(local_remote_dir: Any):
 
     splits = ['train', 'val']
-    remote_dir, local_dir = mds_dataset_dir
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
 
     # Build StreamingDataset for each split
     for split in splits:
         remote_split_dir = os.path.join(remote_dir, split)
         copy_all_files(remote_dir, remote_split_dir)
         _ = StreamingDataset(local=local_dir, remote=remote_dir, split=split)
 
 
-@pytest.mark.usefixtures('mds_dataset_dir')
+@pytest.mark.usefixtures('local_remote_dir')
 def test_invalid_index_json_exception(local_remote_dir: Tuple[str, str]):
-    local_dir, _ = local_remote_dir
+    local_dir, remote_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
     filename = 'index.json'
     if not os.path.exists(local_dir):
         os.mkdir(local_dir)
 
     # Creates an empty file
     with open(os.path.join(local_dir, filename), 'w') as _:
         pass
 
     with pytest.raises(json.decoder.JSONDecodeError,
                        match=f'Index file at.*is empty or corrupted'):
         _ = StreamingDataset(local=local_dir)
 
 
-@pytest.mark.usefixtures('mds_dataset_dir')
+@pytest.mark.usefixtures('local_remote_dir')
 def test_empty_shards_index_json_exception(local_remote_dir: Tuple[str, str]):
-    local_dir, _ = local_remote_dir
+    local_dir, remote_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
     filename = 'index.json'
     content = {'shards': [], 'version': 2}
 
     if not os.path.exists(local_dir):
         os.mkdir(local_dir)
 
     # Creates a `index.json` file and write the content to it
     with open(os.path.join(local_dir, filename), 'w') as outfile:
         json.dump(content, outfile)
 
     with pytest.raises(RuntimeError, match=f'Stream contains no samples: .*'):
         _ = StreamingDataset(local=local_dir)
 
 
-@pytest.mark.usefixtures('mds_dataset_dir')
-def test_accidental_shard_delete_exception(mds_dataset_dir: Any):
-    remote_dir, local_dir = mds_dataset_dir
-    filename = 'shard.00000.mds'
+@pytest.mark.usefixtures('local_remote_dir')
+def test_accidental_shard_delete(local_remote_dir: Any):
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=117,
+                   size_limit=1 << 8)
+    basename = 'shard.00000.mds'
+    filename = os.path.join(local_dir, basename)
     dataset = StreamingDataset(local=local_dir, remote=remote_dir)
-
-    with pytest.raises(RuntimeError,
-                       match=f'.*Check if the shard file exists in your remote location.*'):
-        for _ in dataset:
-            if os.path.exists(os.path.join(local_dir, filename)):
-                os.remove(os.path.join(local_dir, filename))
-            pass
+    is_removed = False
+    for _ in dataset:
+        if os.path.exists(filename) and not is_removed:
+            os.remove(filename)
+            is_removed = True
+    assert os.path.exists(filename), f'{basename} is missing'
     shutil.rmtree(local_dir, ignore_errors=True)
```

### Comparing `mosaicml-streaming-0.5.1/tests/test_shared.py` & `mosaicml-streaming-0.5.2/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_shuffle.py` & `mosaicml-streaming-0.5.2/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_spanner.py` & `mosaicml-streaming-0.5.2/tests/test_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_streaming_remote.py` & `mosaicml-streaming-0.5.2/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.5.1/tests/test_upload.py` & `mosaicml-streaming-0.5.2/tests/test_upload.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,30 +5,43 @@
 import shutil
 import tempfile
 from typing import Any, List, Tuple
 from unittest.mock import Mock, patch
 
 import pytest
 
-from streaming.base.storage.upload import (AzureUploader, CloudUploader, GCSUploader,
-                                           LocalUploader, S3Uploader)
+from streaming.base.storage.upload import (AzureDataLakeUploader, AzureUploader, CloudUploader,
+                                           GCSAuthentication, GCSUploader, LocalUploader,
+                                           S3Uploader)
 from tests.conftest import R2_URL
 
 
 class TestCloudUploader:
 
     @patch('streaming.base.storage.upload.S3Uploader.check_bucket_exists')
     @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
     @pytest.mark.parametrize(
         'mapping',
-        [['s3://bucket/dir/file', S3Uploader], [None, 's3://bucket/dir/file', S3Uploader],
-         ['gs://bucket/dir/file', GCSUploader], [None, 'gs://bucket/dir/file', GCSUploader],
-         ['/tmp/dir/filepath', LocalUploader], ['./relative/dir/filepath', LocalUploader]])
-    def test_instantiation_type(self, s3_mocked_requests: Mock, gcs_mocked_requests: Mock,
-                                local_remote_dir: Tuple[str, str], mapping: List[Any]):
+        [
+            ['s3://bucket/dir/file', S3Uploader],
+            [None, 's3://bucket/dir/file', S3Uploader],
+            ['gs://bucket/dir/file', GCSUploader],
+            [None, 'gs://bucket/dir/file', GCSUploader],
+            ['/tmp/dir/filepath', LocalUploader],
+            ['./relative/dir/filepath', LocalUploader],
+        ],
+    )
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
+    def test_instantiation_type(
+        self,
+        s3_mocked_requests: Mock,
+        gcs_mocked_requests: Mock,
+        local_remote_dir: Tuple[str, str],
+        mapping: List[Any],
+    ):
         s3_mocked_requests.side_effect = None
         gcs_mocked_requests.side_effect = None
         local, _ = local_remote_dir
         if len(mapping) == 2:
             cw = CloudUploader.get(out=mapping[0])
         else:
             mapping[0] = local
@@ -68,29 +81,30 @@
         # Creating an empty file at specified location
         with open(local_file_path, 'w') as _:
             pass
         cw.clear_local(local_file_path)
         assert not os.path.exists(local_file_path)
 
     @pytest.mark.parametrize('out', ['s3://bucket/dir', 'gs://bucket/dir'])
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     def test_check_bucket_exists_exception(self, out: str):
         import botocore
         with pytest.raises(botocore.exceptions.ClientError):
             _ = CloudUploader.get(out=out)
 
 
 class TestS3Uploader:
 
     @patch('streaming.base.storage.upload.S3Uploader.check_bucket_exists')
     @pytest.mark.parametrize('out', ['s3://bucket/dir', ('./dir1', 's3://bucket/dir/')])
     def test_instantiation(self, mocked_requests: Mock, out: Any):
         mocked_requests.side_effect = None
         _ = S3Uploader(out=out)
         if not isinstance(out, str):
-            shutil.rmtree(out[0])
+            shutil.rmtree(out[0], ignore_errors=True)
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir'])
     def test_invalid_remote_str(self, out: str):
         with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = S3Uploader(out=out)
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir', ('./dir1', 'gcs://bucket/dir/')])
@@ -134,78 +148,120 @@
             s3w.upload_file(filename)
             assert os.environ['S3_ENDPOINT_URL'] == R2_URL
             assert not os.path.exists(local_file_path)
 
     @pytest.mark.parametrize('out', ['s3://bucket/dir'])
     def test_check_bucket_exists_exception(self, out: str):
         import botocore
+
         with pytest.raises(botocore.exceptions.ClientError):
             _ = S3Uploader(out=out)
 
 
 class TestGCSUploader:
 
     @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
     @pytest.mark.parametrize('out', ['gs://bucket/dir', ('./dir1', 'gs://bucket/dir/')])
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     def test_instantiation(self, mocked_requests: Mock, out: Any):
         mocked_requests.side_effect = None
         _ = GCSUploader(out=out)
         if not isinstance(out, str):
-            shutil.rmtree(out[0])
+            shutil.rmtree(out[0], ignore_errors=True)
 
     @pytest.mark.parametrize('out', ['gcs://bucket/dir'])
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     def test_invalid_remote_str(self, out: str):
         with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = GCSUploader(out=out)
 
     @pytest.mark.parametrize('out', ['gcs://bucket/dir', ('./dir1', 'ocix://bucket/dir/')])
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     def test_invalid_remote_list(self, out: Any):
         with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = GCSUploader(out=out)
 
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
         with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
             local, _ = local_remote_dir
             os.makedirs(local, exist_ok=True)
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = GCSUploader(out=local)
 
-    @pytest.mark.usefixtures('gcs_client', 'gcs_test')
+    @pytest.mark.usefixtures('gcs_hmac_client', 'gcs_test')
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         with tempfile.NamedTemporaryFile(delete=True, suffix='.txt') as tmp:
             filename = tmp.name.split(os.sep)[-1]
             local, _ = local_remote_dir
             remote = 'gs://streaming-test-bucket/path'
             local_file_path = os.path.join(local, filename)
             gcsw = GCSUploader(out=(local, remote))
             with open(local_file_path, 'w') as _:
                 pass
             gcsw.upload_file(filename)
             assert not os.path.exists(local_file_path)
 
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
     @pytest.mark.parametrize('out', ['gs://bucket/dir'])
     def test_check_bucket_exists_exception(self, out: str):
         import botocore
+
         with pytest.raises(botocore.exceptions.ClientError):
             _ = GCSUploader(out=out)
 
+    @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
+    @pytest.mark.usefixtures('gcs_hmac_credentials')
+    @pytest.mark.parametrize('out', ['gs://bucket/dir'])
+    def test_hmac_authentication(self, mocked_requests: Mock, out: str):
+        uploader = GCSUploader(out=out)
+        assert uploader.authentication == GCSAuthentication.HMAC
+
+    @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
+    @patch('google.cloud.storage.Client.from_service_account_json')
+    @pytest.mark.usefixtures('gcs_service_account_credentials')
+    @pytest.mark.parametrize('out', ['gs://bucket/dir'])
+    def test_service_account_authentication(self, mocked_requests: Mock, mock_client: Mock,
+                                            out: str):
+        uploader = GCSUploader(out=out)
+        assert uploader.authentication == GCSAuthentication.SERVICE_ACCOUNT
+
+    @patch('streaming.base.storage.upload.GCSUploader.check_bucket_exists')
+    @patch('google.cloud.storage.Client.from_service_account_json')
+    @pytest.mark.usefixtures('gcs_service_account_credentials', 'gcs_hmac_credentials')
+    @pytest.mark.parametrize('out', ['gs://bucket/dir'])
+    def test_service_account_and_hmac_authentication(self, mocked_requests: Mock,
+                                                     mock_client: Mock, out: str):
+        uploader = GCSUploader(out=out)
+        assert uploader.authentication == GCSAuthentication.SERVICE_ACCOUNT
+
+    @pytest.mark.parametrize('out', ['gs://bucket/dir'])
+    def test_no_authentication(self, out: str):
+        with pytest.raises(
+                ValueError,
+                match=(f'Either GOOGLE_APPLICATION_CREDENTIALS needs to be set for'
+                       f' service level accounts or GCS_KEY and GCS_SECRET needs to be'
+                       f' set for HMAC authentication'),
+        ):
+            _ = GCSUploader(out=out)
+
 
 class TestAzureUploader:
 
     @patch('streaming.base.storage.upload.AzureUploader.check_bucket_exists')
     @pytest.mark.usefixtures('azure_credentials')
     @pytest.mark.parametrize('out', ['azure://bucket/dir', ('./dir1', 'azure://bucket/dir/')])
     def test_instantiation(self, mocked_requests: Mock, out: Any):
         mocked_requests.side_effect = None
         _ = AzureUploader(out=out)
         if not isinstance(out, str):
-            shutil.rmtree(out[0])
+            shutil.rmtree(out[0], ignore_errors=True)
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir'])
     def test_invalid_remote_str(self, out: str):
         with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
             _ = AzureUploader(out=out)
 
     @pytest.mark.parametrize('out', ['ss4://bucket/dir', ('./dir1', 'gcs://bucket/dir/')])
@@ -220,14 +276,47 @@
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = AzureUploader(out=local)
 
 
+class TestAzureDataLakeUploader:
+
+    @patch('streaming.base.storage.upload.AzureDataLakeUploader.check_container_exists')
+    @pytest.mark.usefixtures('azure_credentials')
+    @pytest.mark.parametrize('out',
+                             ['azure://container/dir', ('./dir1', 'azure://container/dir/')])
+    def test_instantiation(self, mocked_requests: Mock, out: Any):
+        mocked_requests.side_effect = None
+        _ = AzureDataLakeUploader(out=out)
+        if not isinstance(out, str):
+            shutil.rmtree(out[0], ignore_errors=True)
+
+    @pytest.mark.parametrize('out', ['ss4://container/dir'])
+    def test_invalid_remote_str(self, out: str):
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
+            _ = AzureDataLakeUploader(out=out)
+
+    @pytest.mark.parametrize('out', ['ss4://container/dir', ('./dir1', 'gcs://container/dir/')])
+    def test_invalid_remote_list(self, out: Any):
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
+            _ = AzureDataLakeUploader(out=out)
+
+    def test_local_directory_is_empty(self, local_remote_dir: Tuple[str, str]):
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
+            local, _ = local_remote_dir
+            os.makedirs(local, exist_ok=True)
+            local_file_path = os.path.join(local, 'file.txt')
+            # Creating an empty file at specified location
+            with open(local_file_path, 'w') as _:
+                pass
+            _ = AzureDataLakeUploader(out=local)
+
+
 class TestLocalUploader:
 
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         local, remote = local_remote_dir
         filename = 'file.txt'
         local_file_path = os.path.join(local, filename)
         remote_file_path = os.path.join(remote, filename)
```

### Comparing `mosaicml-streaming-0.5.1/tests/test_writer.py` & `mosaicml-streaming-0.5.2/tests/test_writer.py`

 * *Files identical despite different names*

