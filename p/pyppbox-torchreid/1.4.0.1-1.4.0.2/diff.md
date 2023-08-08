# Comparing `tmp/pyppbox-torchreid-1.4.0.1.tar.gz` & `tmp/pyppbox-torchreid-1.4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyppbox-torchreid-1.4.0.1.tar", last modified: Mon Jun 26 16:05:24 2023, max compression
+gzip compressed data, was "pyppbox-torchreid-1.4.0.2.tar", last modified: Tue Aug  8 09:42:18 2023, max compression
```

## Comparing `pyppbox-torchreid-1.4.0.1.tar` & `pyppbox-torchreid-1.4.0.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.249648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.249648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.249648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk02.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk03.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhksysu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/dukemtmcreid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/ilids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/msmt17.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/prid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/sensereid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/university1652.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/viper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/dukemtmcvidreid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/ilidsvid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/prid2011.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/hard_mine_triplet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.253648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/rank_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/test_cython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/hacnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/inceptionresnetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/inceptionv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mlfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mudeep.py
--rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/osnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/osnet_ain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/pcb.py
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnetmid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/shufflenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/shufflenetv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/squeezenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/radam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/loggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/model_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/reidtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/torchtools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:24.249648 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-26 16:05:24.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-26 16:05:24.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:24.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 16:05:24.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 16:05:24.000000 pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:05:24.257648 pyppbox-torchreid-1.4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-26 16:05:06.000000 pyppbox-torchreid-1.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2484 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.227574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.231574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.231574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk03.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhksysu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/dukemtmcreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/ilids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/msmt17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/prid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/sensereid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/university1652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/viper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/dukemtmcvidreid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/ilidsvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/prid2011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/hard_mine_triplet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.235574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.239574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/rank_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/test_cython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11627 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/hacnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/inceptionresnetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/inceptionv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mlfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mudeep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36186 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17098 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/osnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/osnet_ain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/pcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnetmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/shufflenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/shufflenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/squeezenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11626 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/radam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/model_complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/reidtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/torchtools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 09:42:18.231574 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-08 09:42:18.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-08 09:42:18.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 09:42:18.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-08 09:42:18.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 09:42:18.000000 pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 09:42:18.243574 pyppbox-torchreid-1.4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-08 09:41:54.000000 pyppbox-torchreid-1.4.0.2/setup.py
```

### Comparing `pyppbox-torchreid-1.4.0.1/LICENSE` & `pyppbox-torchreid-1.4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/PKG-INFO` & `pyppbox-torchreid-1.4.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyppbox-torchreid
-Version: 1.4.0.1
+Version: 1.4.0.2
 Summary: Customized Torchreid for pyppbox: Deep learning person re-identification.
 Home-page: https://github.com/rathaumons/torchreid-for-pyppbox
-Author: rathaROG
+Author: Ratha SIV
+Maintainer: rathaROG
 License: MIT
 Keywords: Person Re-Identification,Deep Learning,pyppbox
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Scientific/Engineering
@@ -26,69 +26,71 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Windows/Linux + Python [3.8-3.11] .](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml) 
-[![Build `tar.gz` PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml)
+[![Test Build Python [3.8-3.11]](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml) 
+[![Publish to PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml)
 
 # Customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
 `Torchreid` is a library for deep-learning person re-identification using [PyTorch](https://pytorch.org/). 
 
-`pyppbox-torchreid` is a customized of `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
-- Ensures that `Cython` natively works on all OS platform (Windows/Linux), 
+`pyppbox-torchreid` is a customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
+- Ensures that `Cython` natively works on all OS platform (Windows/Linux/macOS), 
 - Enables freedom of passing local model/weight files from anywhere, 
 - Disables some models which are not used in `pyppbox`.
 
 All source credit and more info -> [Original KaiyangZhou's repo](https://github.com/KaiyangZhou/deep-person-reid). 
 
 ## Install
 
-Use [Wheels fron releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from PyPI: 
+Use [Wheels from releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from [PyPI](https://pypi.org/project/pyppbox-torchreid/): 
 
 ```
 pip install pyppbox-torchreid
 ```
 
 Or install from GitHub directly:
 
 ```
 pip install git+https://github.com/rathaumons/torchreid-for-pyppbox.git
 ```
 
-To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/) with ***GPU***:
+To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/); for example, with GPU support:
 
 ```
 pip install opencv-contrib-python
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
-***Note*: [PyTorch](https://pytorch.org/) doesn't support GUP on macOS.**
+***Note*: [PyTorch](https://pytorch.org/) doesn't support GPU on macOS.**
 
 ## Build from source
 
 (Optional, auto install) Building Wheels or source distribution only requires these modules:
 
 ```
 pip install "setuptools>=67.2.0"
 pip install "Cython>=0.29.32"
-pip install "numpy>=1.21.6"
+pip install "numpy>=1.23.5"
 ```
 
 Recommend using `build` for building both `.whl` and `.tar.gz`:
 
 ```
 git clone https://github.com/rathaumons/torchreid-for-pyppbox/
 cd torchreid-for-pyppbox
+python -m pip install --upgrade pip
 pip install wheel build
 python -m build --sdist
 python -m build --wheel
 cd dist
 ```
 
 After you install `pyppbox-torchred`, [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/), you can check if Cython `rank_cy` works:
```

### Comparing `pyppbox-torchreid-1.4.0.1/README.md` & `pyppbox-torchreid-1.4.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-[![Windows/Linux + Python [3.8-3.11] .](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml) 
-[![Build `tar.gz` PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml)
+[![Test Build Python [3.8-3.11]](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml) 
+[![Publish to PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml)
 
 # Customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
 `Torchreid` is a library for deep-learning person re-identification using [PyTorch](https://pytorch.org/). 
 
-`pyppbox-torchreid` is a customized of `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
-- Ensures that `Cython` natively works on all OS platform (Windows/Linux), 
+`pyppbox-torchreid` is a customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
+- Ensures that `Cython` natively works on all OS platform (Windows/Linux/macOS), 
 - Enables freedom of passing local model/weight files from anywhere, 
 - Disables some models which are not used in `pyppbox`.
 
 All source credit and more info -> [Original KaiyangZhou's repo](https://github.com/KaiyangZhou/deep-person-reid). 
 
 ## Install
 
-Use [Wheels fron releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from PyPI: 
+Use [Wheels from releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from [PyPI](https://pypi.org/project/pyppbox-torchreid/): 
 
 ```
 pip install pyppbox-torchreid
 ```
 
 Or install from GitHub directly:
 
 ```
 pip install git+https://github.com/rathaumons/torchreid-for-pyppbox.git
 ```
 
-To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/) with ***GPU***:
+To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/); for example, with GPU support:
 
 ```
 pip install opencv-contrib-python
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
-***Note*: [PyTorch](https://pytorch.org/) doesn't support GUP on macOS.**
+***Note*: [PyTorch](https://pytorch.org/) doesn't support GPU on macOS.**
 
 ## Build from source
 
 (Optional, auto install) Building Wheels or source distribution only requires these modules:
 
 ```
 pip install "setuptools>=67.2.0"
 pip install "Cython>=0.29.32"
-pip install "numpy>=1.21.6"
+pip install "numpy>=1.23.5"
 ```
 
 Recommend using `build` for building both `.whl` and `.tar.gz`:
 
 ```
 git clone https://github.com/rathaumons/torchreid-for-pyppbox/
 cd torchreid-for-pyppbox
+python -m pip install --upgrade pip
 pip install wheel build
 python -m build --sdist
 python -m build --wheel
 cd dist
 ```
 
 After you install `pyppbox-torchred`, [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/), you can check if Cython `rank_cy` works:
```

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datamanager.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datamanager.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/__init__.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/dataset.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk01.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk01.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk02.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk02.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhk03.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhk03.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/cuhksysu.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/cuhksysu.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/dukemtmcreid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/dukemtmcreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/grid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/grid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/ilids.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/ilids.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/market1501.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/market1501.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/msmt17.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/msmt17.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/prid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/prid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/sensereid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/sensereid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/university1652.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/university1652.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/image/viper.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/image/viper.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/dukemtmcvidreid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/dukemtmcvidreid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/ilidsvid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/ilidsvid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/mars.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/mars.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/datasets/video/prid2011.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/datasets/video/prid2011.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/sampler.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/data/transforms.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/data/transforms.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/engine.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/softmax.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/softmax.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/image/triplet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/image/triplet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/softmax.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/softmax.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/engine/video/triplet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/engine/video/triplet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/cross_entropy_loss.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/losses/hard_mine_triplet_loss.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/losses/hard_mine_triplet_loss.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/accuracy.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/distance.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/distance.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/rank_cy.pyx` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/rank_cy.pyx`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/metrics/rank_cylib/test_cython.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/metrics/rank_cylib/test_cython.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/__init__.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/densenet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/densenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/hacnn.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/hacnn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/inceptionresnetv2.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/inceptionv4.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mlfn.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mlfn.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mobilenetv2.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/mudeep.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/mudeep.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/nasnet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/nasnet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/osnet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/osnet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/osnet_ain.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/osnet_ain.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/pcb.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/pcb.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet_ibn_a.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet_ibn_a.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnet_ibn_b.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnet_ibn_b.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/resnetmid.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/resnetmid.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/senet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/senet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/shufflenet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/shufflenetv2.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/squeezenet.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/models/xception.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/models/xception.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/lr_scheduler.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/optimizer.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/optim/radam.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/optim/radam.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/avgmeter.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/avgmeter.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/feature_extractor.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/loggers.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/model_complexity.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/model_complexity.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/reidtools.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/reidtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/rerank.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/rerank.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/tools.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid/utils/torchtools.py` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid/utils/torchtools.py`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/PKG-INFO` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyppbox-torchreid
-Version: 1.4.0.1
+Version: 1.4.0.2
 Summary: Customized Torchreid for pyppbox: Deep learning person re-identification.
 Home-page: https://github.com/rathaumons/torchreid-for-pyppbox
-Author: rathaROG
+Author: Ratha SIV
+Maintainer: rathaROG
 License: MIT
 Keywords: Person Re-Identification,Deep Learning,pyppbox
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Scientific/Engineering
@@ -26,69 +26,71 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Windows/Linux + Python [3.8-3.11] .](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_all.yaml) 
-[![Build `tar.gz` PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/build_pypi.yaml)
+[![Test Build Python [3.8-3.11]](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/test_build.yaml) 
+[![Publish to PyPI](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/torchreid-for-pyppbox/actions/workflows/publish_pypi.yaml)
 
 # Customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox)
 
 `Torchreid` is a library for deep-learning person re-identification using [PyTorch](https://pytorch.org/). 
 
-`pyppbox-torchreid` is a customized of `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
-- Ensures that `Cython` natively works on all OS platform (Windows/Linux), 
+`pyppbox-torchreid` is a customized `Torchreid` for [`pyppbox`](https://github.com/rathaumons/pyppbox) and:
+- Ensures that `Cython` natively works on all OS platform (Windows/Linux/macOS), 
 - Enables freedom of passing local model/weight files from anywhere, 
 - Disables some models which are not used in `pyppbox`.
 
 All source credit and more info -> [Original KaiyangZhou's repo](https://github.com/KaiyangZhou/deep-person-reid). 
 
 ## Install
 
-Use [Wheels fron releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from PyPI: 
+Use [Wheels from releases](https://github.com/rathaumons/torchreid-for-pyppbox/releases) or directly install from [PyPI](https://pypi.org/project/pyppbox-torchreid/): 
 
 ```
 pip install pyppbox-torchreid
 ```
 
 Or install from GitHub directly:
 
 ```
 pip install git+https://github.com/rathaumons/torchreid-for-pyppbox.git
 ```
 
-To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/) with ***GPU***:
+To be able to run, you must install [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/); for example, with GPU support:
 
 ```
 pip install opencv-contrib-python
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 ```
 
-***Note*: [PyTorch](https://pytorch.org/) doesn't support GUP on macOS.**
+***Note*: [PyTorch](https://pytorch.org/) doesn't support GPU on macOS.**
 
 ## Build from source
 
 (Optional, auto install) Building Wheels or source distribution only requires these modules:
 
 ```
 pip install "setuptools>=67.2.0"
 pip install "Cython>=0.29.32"
-pip install "numpy>=1.21.6"
+pip install "numpy>=1.23.5"
 ```
 
 Recommend using `build` for building both `.whl` and `.tar.gz`:
 
 ```
 git clone https://github.com/rathaumons/torchreid-for-pyppbox/
 cd torchreid-for-pyppbox
+python -m pip install --upgrade pip
 pip install wheel build
 python -m build --sdist
 python -m build --wheel
 cd dist
 ```
 
 After you install `pyppbox-torchred`, [OpenCV](https://github.com/opencv/opencv-python) and [PyTorch](https://pytorch.org/), you can check if Cython `rank_cy` works:
```

### Comparing `pyppbox-torchreid-1.4.0.1/pyppbox_torchreid.egg-info/SOURCES.txt` & `pyppbox-torchreid-1.4.0.2/pyppbox_torchreid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyppbox-torchreid-1.4.0.1/setup.py` & `pyppbox-torchreid-1.4.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # # # # # # # # # # # # # # # # # # # # # #
 #    Rewrite on 2023/06/26 by rathaROG    #
+#    Updated on 2023/08/08 by rathaROG    #
 # # # # # # # # # # # # # # # # # # # # # #
 
 
 from setuptools import setup, find_packages
 from distutils.extension import Extension
 
 license='MIT'
@@ -57,31 +58,32 @@
             include_dirs=[numpy_include()],
         )
     ]
     setup(
         name=package_name,
         version=get_version_string(),
         description=description,
-        author='rathaROG',
+        author="Ratha SIV",
+        maintainer="rathaROG",
         license=license,
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/rathaumons/torchreid-for-pyppbox',
         packages=find_packages(),
         keywords=['Person Re-Identification', 'Deep Learning', 'pyppbox'],
         install_requires=read_requirments(),
+        python_requires=">=3.8",
         classifiers=['Development Status :: 4 - Beta',
                      'Environment :: Console',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Education',
                      'Intended Audience :: Information Technology',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: MIT License',
                      'Programming Language :: Python :: 3',
-                     'Programming Language :: Python :: 3.7',
                      'Programming Language :: Python :: 3.8',
                      'Programming Language :: Python :: 3.9',
                      'Programming Language :: Python :: 3.10',
                      'Programming Language :: Python :: 3.11',
                      'Topic :: Education',
                      'Topic :: Education :: Testing',
                      'Topic :: Scientific/Engineering',
```

