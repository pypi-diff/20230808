# Comparing `tmp/thingsvision-2.3.9.tar.gz` & `tmp/thingsvision-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.3.9.tar", last modified: Mon Mar  6 10:23:53 2023, max compression
+gzip compressed data, was "thingsvision-2.4.0.tar", last modified: Tue Aug  8 13:02:23 2023, max compression
```

## Comparing `thingsvision-2.3.9.tar` & `thingsvision-2.4.0.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.808122 thingsvision-2.3.9/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.3.9/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14022 2023-03-06 10:23:53.807833 thingsvision-2.3.9/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13419 2023-03-02 12:32:50.000000 thingsvision-2.3.9/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2023-03-06 10:23:53.808197 thingsvision-2.3.9/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1824 2023-03-06 10:23:19.000000 thingsvision-2.3.9/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.784160 thingsvision-2.3.9/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.3.9/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.786024 thingsvision-2.3.9/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.9/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.788524 thingsvision-2.3.9/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.3.9/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.3.9/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2023-02-24 09:48:38.000000 thingsvision-2.3.9/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1656 2023-01-18 14:03:54.000000 thingsvision-2.3.9/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2359 2023-01-17 18:07:38.000000 thingsvision-2.3.9/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2022-10-26 15:18:20.000000 thingsvision-2.3.9/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.3.9/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8661 2023-03-02 18:14:59.000000 thingsvision-2.3.9/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.3.9/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.3.9/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.790125 thingsvision-2.3.9/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.3.9/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2023-03-06 10:23:28.000000 thingsvision-2.3.9/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.792168 thingsvision-2.3.9/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.3.9/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.793126 thingsvision-2.3.9/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.795974 thingsvision-2.3.9/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      193 2023-02-15 09:26:37.000000 thingsvision-2.3.9/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8269 2023-02-17 14:03:21.000000 thingsvision-2.3.9/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    13241 2023-02-22 09:56:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7934 2023-03-02 12:32:50.000000 thingsvision-2.3.9/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2750 2023-02-24 09:48:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5199 2023-02-24 09:48:38.000000 thingsvision-2.3.9/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.797214 thingsvision-2.3.9/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.3.9/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.3.9/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.802365 thingsvision-2.3.9/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      327 2023-03-02 18:14:59.000000 thingsvision-2.3.9/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      619 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      624 2022-12-20 12:41:31.000000 thingsvision-2.3.9/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.804288 thingsvision-2.3.9/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.3.9/thingsvision/custom_models/custom.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1301 2023-03-02 18:14:59.000000 thingsvision-2.3.9/thingsvision/custom_models/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      628 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      511 2022-10-26 15:18:20.000000 thingsvision-2.3.9/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      982 2022-10-26 15:18:20.000000 thingsvision-2.3.9/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      622 2022-09-22 09:46:01.000000 thingsvision-2.3.9/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      615 2023-02-24 09:48:36.000000 thingsvision-2.3.9/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-01-18 10:11:35.000000 thingsvision-2.3.9/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5812 2022-12-13 13:51:38.000000 thingsvision-2.3.9/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.804632 thingsvision-2.3.9/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.3.9/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.805995 thingsvision-2.3.9/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.3.9/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.3.9/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.806432 thingsvision-2.3.9/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.807254 thingsvision-2.3.9/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.3.9/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.3.9/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-03-06 10:23:53.791922 thingsvision-2.3.9/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14022 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2185 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      380 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2023-03-06 10:23:53.000000 thingsvision-2.3.9/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.668479 thingsvision-2.4.0/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.4.0/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15214 2023-08-08 13:02:23.668114 thingsvision-2.4.0/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14611 2023-08-08 13:01:35.000000 thingsvision-2.4.0/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2023-08-08 13:02:23.668567 thingsvision-2.4.0/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.4.0/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.639160 thingsvision-2.4.0/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.4.0/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.640655 thingsvision-2.4.0/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.4.0/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.643386 thingsvision-2.4.0/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.4.0/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.4.0/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2023-02-24 09:48:38.000000 thingsvision-2.4.0/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1656 2023-01-18 14:03:54.000000 thingsvision-2.4.0/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2359 2023-01-17 18:07:38.000000 thingsvision-2.4.0/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2022-10-26 15:18:20.000000 thingsvision-2.4.0/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.4.0/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11153 2023-08-08 13:01:35.000000 thingsvision-2.4.0/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.4.0/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.4.0/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.644820 thingsvision-2.4.0/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.4.0/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2023-08-08 13:01:49.000000 thingsvision-2.4.0/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.646987 thingsvision-2.4.0/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.4.0/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.647995 thingsvision-2.4.0/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.651147 thingsvision-2.4.0/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      193 2023-08-04 09:13:22.000000 thingsvision-2.4.0/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     9192 2023-08-04 09:05:08.000000 thingsvision-2.4.0/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15646 2023-08-08 13:01:35.000000 thingsvision-2.4.0/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8405 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2855 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5845 2023-08-04 10:28:52.000000 thingsvision-2.4.0/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.652305 thingsvision-2.4.0/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.4.0/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.4.0/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.658717 thingsvision-2.4.0/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.4.0/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.4.0/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.661031 thingsvision-2.4.0/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.4.0/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.661721 thingsvision-2.4.0/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1972 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.662645 thingsvision-2.4.0/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.4.0/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.4.0/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.4.0/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.4.0/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.4.0/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.4.0/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.4.0/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.4.0/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5902 2023-04-30 10:10:52.000000 thingsvision-2.4.0/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.663140 thingsvision-2.4.0/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.4.0/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.663351 thingsvision-2.4.0/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.4.0/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.665763 thingsvision-2.4.0/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.4.0/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.4.0/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.4.0/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.4.0/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.666389 thingsvision-2.4.0/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.667264 thingsvision-2.4.0/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.4.0/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.4.0/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2023-08-08 13:02:23.646687 thingsvision-2.4.0/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15214 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2393 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2023-08-08 13:02:23.000000 thingsvision-2.4.0/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.3.9/LICENSE` & `thingsvision-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/PKG-INFO` & `thingsvision-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: thingsvision
-Version: 2.3.9
-Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
-Home-page: https://github.com/ViCCo-Group/thingsvision
-Author: Lukas Muttenthaler
-Author-email: muttenthaler@cbs.mpg.de
-License: MIT License
-Keywords: feature extraction
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a name="readme-top"></a>
 <div align="center">
     <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
         <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
     </a>
     <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
         <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
@@ -85,22 +68,23 @@
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
-- `ssl` (Self-Supervised Learning Models)
-  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
-  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
+- `ssl` (self-supervised learning models)
+  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50`
+  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`, `dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-vit-giant-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip)
 - both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
-- [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
+- [Harmonization](https://arxiv.org/abs/2211.04533) models from the official [Harmonization repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.<br> 
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official [DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
@@ -115,17 +99,31 @@
 ```
 
 Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
 
 ```bash
 $ pip install --upgrade thingsvision
 $ pip install git+https://github.com/openai/CLIP.git
+```
+
+If you want to extract features for [harmonized models](https://vicco-group.github.io/thingsvision/AvailableModels.html#harmonization) from the [Harmonization repo](https://github.com/serre-lab/harmonization), you have to additionally run the following `pip` command in your `thingsvision` environment (FYI: as of now, this seems to be working smoothly on Ubuntu only but not on macOS),
+
+```bash
 $ pip install git+https://github.com/serre-lab/Harmonization.git
+$ pip install keras-cv-attention-models>=1.3.5
 ```
 
+If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
+
+```bash
+$ pip install dreamsim==0.1.2
+```
+
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
@@ -145,67 +143,71 @@
 thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
-To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
+To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
 
 ```python
 import torch
 from thingsvision import get_extractor
 from thingsvision.utils.storing import save_features
 from thingsvision.utils.data import ImageDataset, DataLoader
 
-model_name = 'alexnet'
-source = 'torchvision'
+model_name = 'clip'
+source = 'custom'
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
+model_parameters = {
+    'variant': 'ViT-B/32'
+}
 
 extractor = get_extractor(
-    model_name=model_name,
-    source=source,
-    device=device,
-    pretrained=True
+  model_name=model_name,
+  source=source,
+  device=device,
+  pretrained=True,
+  model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
 root='path/to/root/img/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
-    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
+    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
 )
 
 batches = DataLoader(
     dataset=dataset,
     batch_size=batch_size,
     backend=extractor.get_backend() # backend framework of model
 )
 ```
 
-Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
+Now all that is left is to extract the image features and store them on disk! Here we're extracting features from the image encoder layer (`visual`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all the modules.
 
 ```python
-module_name = 'features.10'
+module_name = 'visual'
 
 features = extractor.extract_features(
     batches=batches,
     module_name=module_name,
-    flatten_acts=True, # flatten 2D feature maps from convolutional layer
-    output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
+    flatten_acts=True,
+    output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP is one!)
 )
 
-save_features(features, out_path='path/to/features', file_format='npy')
+save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
 _For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Contributing -->
@@ -247,15 +249,14 @@
 - [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
 - [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
 - [Hannes Hansen](https://github.com/hahahannes) (software dev.)
 - [Johannes Roth](https://jroth.space/) (software dev., design, docs)
 - [Jonas Dippel](https://github.com/jonasd4) (software dev.)
 - [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
 - [Martin N. Hebart](http://martin-hebart.de/) (design)
-- [Oliver Contier](https://olivercontier.com/) (docs)
 - [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
 - [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
 
 sorted alphabetically. 
 
 This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.3.9 Summary: Extracting
-image features from state-of-the-art neural networks for Computer Vision made
-easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
-Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
-Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
-Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [Tests] [Code_Coverage] [Maintenance] [PyPI] [Pepy] [Python_version] [License]
                       [Code_style:_black] [Open_In_Colab]
 
  # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
@@ -39,46 +31,62 @@
 extraction. - perform Centered Kernel Alignment (CKA) to compare image features
 across model-module combinations.
                                                                   (back_to_top)
  ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
-[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (Self-
-Supervised Learning Models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
-`rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://
-github.com/facebookresearch/vissl)) - `barlowtwins-rn50`, `vicreg-rn50`, `dino-
-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`
-(retrieved from [torch.hub](https://pytorch.org/hub/)) - [OpenCLIP](https://
-github.com/mlfoundations/open_clip) - both original [CLIP](https://github.com/
-openai/CLIP) variants (`ViT-B/32` and `RN50`) - a few custom models (Alexnet,
-VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/
-doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet pretrained on
-ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
-sos.html) - each of the many [CORnet](https://github.com/dicarlolab/CORnet)
-versions - [Harmonization](https://arxiv.org/abs/2211.04533) models from the
-[official repo](https://github.com/serre-lab/harmonization). The default
-variant is `ViT_B16`. However, the following encoders are additionally
-available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`,
-`tiny_MaxViT`, `LeViT_small`
+[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
+supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
+`rotnet-rn50`, `swav-rn50`, `pirl-rn50` - `barlowtwins-rn50`, `vicreg-rn50`,
+`dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`,
+`dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-
+vit-giant-p14` - [OpenCLIP](https://github.com/mlfoundations/open_clip) - both
+original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and
+`RN50`) - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3)
+trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather
+than ImageNet and one Alexnet pretrained on ImageNet and fine-tuned on
+[SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html) - each of the many
+[CORnet](https://github.com/dicarlolab/CORnet) versions - [Harmonization]
+(https://arxiv.org/abs/2211.04533) models from the official [Harmonization
+repo](https://github.com/serre-lab/harmonization). The default variant is
+`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
+`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official
+[DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant
+is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs]
+(https://vicco-group.github.io/thingsvision/AvailableModels.html) for more
+information.
                                                                   (back_to_top)
  ## :running: Getting Started  ### :computer: Setting up your environment ####
 Working locally. First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
-//github.com/openai/CLIP.git $ pip install git+https://github.com/serre-lab/
-Harmonization.git ``` #### Google Colab. Alternatively, you can use Google
-Colab to play around with `thingsvision` by uploading your image data to Google
-Drive (via directory mounting). You can find the jupyter notebook using
-`PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/
-thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example
+//github.com/openai/CLIP.git ``` If you want to extract features for
+[harmonized models](https://vicco-group.github.io/thingsvision/
+AvailableModels.html#harmonization) from the [Harmonization repo](https://
+github.com/serre-lab/harmonization), you have to additionally run the following
+`pip` command in your `thingsvision` environment (FYI: as of now, this seems to
+be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
+git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
+attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
+(https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
+github.com/ssundaram21/dreamsim), you have to additionally run the following
+`pip` command in your `thingsvision` environment, ```bash $ pip install
+dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
+AvailableModels.html) for which `DreamSim` models are available in
+`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+play around with `thingsvision` by uploading your image data to Google Drive
+(via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
-master/notebooks/tensorflow.ipynb).
+master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
+colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
+notebooks/tensorflow.ipynb).
                                                                   (back_to_top)
  ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
@@ -89,45 +97,47 @@
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
 package directly and write your own Python script. #### Python commands To do
 this start by importing all the necessary components and instantiating a
-`thingsvision` extractor. Here we're using `AlexNet` from the `torchvision`
-library as the model to extract features from and also load the model to GPU
-for faster inference, ```python import torch from thingsvision import
-get_extractor from thingsvision.utils.storing import save_features from
-thingsvision.utils.data import ImageDataset, DataLoader model_name = 'alexnet'
-source = 'torchvision' device = 'cuda' if torch.cuda.is_available() else 'cpu'
-extractor = get_extractor( model_name=model_name, source=source, device=device,
-pretrained=True ) ``` As a next step, create both dataset and dataloader for
-your images. We assume that all of your images are in a single `root` directory
-which can contain subfolders (e.g., for individual classes). Therefore, we
-leverage the `ImageDataset` class. ```python root='path/to/root/img/directory'
-# (e.g., './images/) batch_size = 32 dataset = ImageDataset( root=root,
-out_path='path/to/features', backend=extractor.get_backend(), # backend
-framework of model transforms=extractor.get_transformations(resize_dim=256,
-crop_dim=224) # set input dimensionality to whatever is required for your
-pretrained model ) batches = DataLoader( dataset=dataset,
-batch_size=batch_size, backend=extractor.get_backend() # backend framework of
-model ) ``` Now all that is left is to extract the image features and store
-them to disk! Here we're extracting features from the last convolutional layer
-of AlexNet (`features.10`), but if you don't know which modules are available
-for a given model, just call `extractor.show_model()` to print all modules.
-```python module_name = 'features.10' features = extractor.extract_features
-( batches=batches, module_name=module_name, flatten_acts=True, # flatten 2D
-feature maps from convolutional layer output_type="ndarray", # or "tensor"
-(only applicable to PyTorch models) ) save_features(features, out_path='path/
-to/features', file_format='npy') ``` _For more examples on the many models
-available in `thingsvision` and explanations of additional functionality like
-how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD
-stimuli), how to perform RSA or CKA, or how to easily extract features for the
-[THINGS image database](https://osf.io/jum2f/), please refer to the
-[Documentation](https://vicco-group.github.io/thingsvision/)._
+`thingsvision` extractor. Here we're using `CLIP` from the official clip repo
+as the model to extract features from and also load the model to GPU for faster
+inference, ```python import torch from thingsvision import get_extractor from
+thingsvision.utils.storing import save_features from thingsvision.utils.data
+import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
+'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
+'ViT-B/32' } extractor = get_extractor( model_name=model_name, source=source,
+device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
+next step, create both dataset and dataloader for your images. We assume that
+all of your images are in a single `root` directory which can contain
+subfolders (e.g., for individual classes). Therefore, we leverage the
+`ImageDataset` class. ```python root='path/to/root/img/directory' # (e.g., './
+images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/to/
+features', backend=extractor.get_backend(), # backend framework of model
+transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
+the input dimensionality to whichever values are required for your pretrained
+model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
+backend=extractor.get_backend() # backend framework of model ) ``` Now all that
+is left is to extract the image features and store them on disk! Here we're
+extracting features from the image encoder layer (`visual`), but if you don't
+know which modules are available for a given model, just call
+`extractor.show_model()` to print all the modules. ```python module_name =
+'visual' features = extractor.extract_features( batches=batches,
+module_name=module_name, flatten_acts=True, output_type="ndarray", # or
+"tensor" (only applicable to PyTorch models of which CLIP is one!) )
+save_features(features, out_path='path/to/features', file_format='npy') #
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` _For more
+examples on the many models available in `thingsvision` and explanations of
+additional functionality like how to optionally turn off center cropping, how
+to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to
+easily extract features for the [THINGS image database](https://osf.io/jum2f/),
+please refer to the [Documentation](https://vicco-group.github.io/thingsvision/
+)._
                                                                   (back_to_top)
  ## :wave: How to contribute If you come across problems or have suggestions
 please submit an issue!
                                                                   (back_to_top)
  ## :warning: License This GitHub repository is licensed under the MIT License
 - see the [LICENSE.md](LICENSE.md) file for details.
                                                                   (back_to_top)
@@ -148,19 +158,18 @@
 and refined into its current form with the help of our many contributors, -
 [Alex Murphy](https://github.com/Alxmrphi) (software dev.) - [Florian Mahner]
 (https://www.cbs.mpg.de/person/mahner/1483114) (software dev.) - [Hannes
 Hansen](https://github.com/hahahannes) (software dev.) - [Johannes Roth](https:
 //jroth.space/) (software dev., design, docs) - [Jonas Dippel](https://
 github.com/jonasd4) (software dev.) - [Lukas Muttenthaler](https://
 lukasmut.github.io/) (software dev., design, docs, general responsibility) -
-[Martin N. Hebart](http://martin-hebart.de/) (design) - [Oliver Contier](https:
-//olivercontier.com/) (docs) - [Philipp Kaniuth](https://www.cbs.mpg.de/person/
-kaniuth/1483114) (design, docs) - [Roman Leipe](https://github.com/RLeipe)
-(sofware dev., docs), sorted alphabetically. This is a joint open-source
-project between the Max Planck Institute for Human Cognitive and Brain
-Sciences, Leipzig, and the Machine Learning Group at Technische UniverstitÃ¤t
-Berlin. Correspondence and requests for contributing should be adressed to
-[Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if
-you want to become a contributor or have any suggestions/feedback. For the
-latter, you could also just post an issue or engange in discussions. We'll try
-to respond as fast as we can.
+[Martin N. Hebart](http://martin-hebart.de/) (design) - [Philipp Kaniuth]
+(https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs) - [Roman Leipe]
+(https://github.com/RLeipe) (sofware dev., docs), sorted alphabetically. This
+is a joint open-source project between the Max Planck Institute for Human
+Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at
+Technische UniverstitÃ¤t Berlin. Correspondence and requests for contributing
+should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel
+free to contact us if you want to become a contributor or have any suggestions/
+feedback. For the latter, you could also just post an issue or engange in
+discussions. We'll try to respond as fast as we can.
                                                                   (back_to_top)
```

### Comparing `thingsvision-2.3.9/README.md` & `thingsvision-2.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: thingsvision
+Version: 2.4.0
+Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
+Home-page: https://github.com/ViCCo-Group/thingsvision
+Author: Lukas Muttenthaler
+Author-email: muttenthaler@cbs.mpg.de
+License: MIT License
+Keywords: feature extraction
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a name="readme-top"></a>
 <div align="center">
     <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml" rel="nofollow">
         <img src="https://github.com/ViCCo-Group/thingsvision/actions/workflows/tests.yml/badge.svg" alt="Tests" />
     </a>
     <a href="https://github.com/ViCCo-Group/thingsvision/actions/workflows/coverage.yml" rel="nofollow">
         <img src="https://codecov.io/gh/ViCCo-Group/thingsvision/branch/master/graph/badge.svg" alt="Code Coverage" />
@@ -68,22 +85,23 @@
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
-- `ssl` (Self-Supervised Learning Models)
-  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
-  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
+- `ssl` (self-supervised learning models)
+  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50`
+  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`, `dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-vit-giant-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip)
 - both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
-- [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
+- [Harmonization](https://arxiv.org/abs/2211.04533) models from the official [Harmonization repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.<br> 
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official [DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
@@ -98,17 +116,31 @@
 ```
 
 Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
 
 ```bash
 $ pip install --upgrade thingsvision
 $ pip install git+https://github.com/openai/CLIP.git
+```
+
+If you want to extract features for [harmonized models](https://vicco-group.github.io/thingsvision/AvailableModels.html#harmonization) from the [Harmonization repo](https://github.com/serre-lab/harmonization), you have to additionally run the following `pip` command in your `thingsvision` environment (FYI: as of now, this seems to be working smoothly on Ubuntu only but not on macOS),
+
+```bash
 $ pip install git+https://github.com/serre-lab/Harmonization.git
+$ pip install keras-cv-attention-models>=1.3.5
 ```
 
+If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
+
+```bash
+$ pip install dreamsim==0.1.2
+```
+
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
@@ -128,67 +160,71 @@
 thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
-To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
+To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
 
 ```python
 import torch
 from thingsvision import get_extractor
 from thingsvision.utils.storing import save_features
 from thingsvision.utils.data import ImageDataset, DataLoader
 
-model_name = 'alexnet'
-source = 'torchvision'
+model_name = 'clip'
+source = 'custom'
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
+model_parameters = {
+    'variant': 'ViT-B/32'
+}
 
 extractor = get_extractor(
-    model_name=model_name,
-    source=source,
-    device=device,
-    pretrained=True
+  model_name=model_name,
+  source=source,
+  device=device,
+  pretrained=True,
+  model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
 root='path/to/root/img/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
-    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
+    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
 )
 
 batches = DataLoader(
     dataset=dataset,
     batch_size=batch_size,
     backend=extractor.get_backend() # backend framework of model
 )
 ```
 
-Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
+Now all that is left is to extract the image features and store them on disk! Here we're extracting features from the image encoder layer (`visual`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all the modules.
 
 ```python
-module_name = 'features.10'
+module_name = 'visual'
 
 features = extractor.extract_features(
     batches=batches,
     module_name=module_name,
-    flatten_acts=True, # flatten 2D feature maps from convolutional layer
-    output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
+    flatten_acts=True,
+    output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP is one!)
 )
 
-save_features(features, out_path='path/to/features', file_format='npy')
+save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
 _For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Contributing -->
@@ -230,15 +266,14 @@
 - [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
 - [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
 - [Hannes Hansen](https://github.com/hahahannes) (software dev.)
 - [Johannes Roth](https://jroth.space/) (software dev., design, docs)
 - [Jonas Dippel](https://github.com/jonasd4) (software dev.)
 - [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
 - [Martin N. Hebart](http://martin-hebart.de/) (design)
-- [Oliver Contier](https://olivercontier.com/) (docs)
 - [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
 - [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
 
 sorted alphabetically. 
 
 This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1 Name: thingsvision Version: 2.4.0 Summary: Extracting
+image features from state-of-the-art neural networks for Computer Vision made
+easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
+Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
+Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
+Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
+MIT License Classifier: Operating System :: OS Independent Requires-Python:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [Tests] [Code_Coverage] [Maintenance] [PyPI] [Pepy] [Python_version] [License]
                       [Code_style:_black] [Open_In_Colab]
 
  # :notebook_with_decorative_cover: Table of Contents - [About the Project]
 (#star2-about-the-project) * [Functionality](#mechanical_arm-functionality) *
 [Model collection](#file_cabinet-model-collection) - [Getting Started]
 (#running-getting-started) * [Setting up your environment](#computer-setting-
@@ -31,46 +39,62 @@
 extraction. - perform Centered Kernel Alignment (CKA) to compare image features
 across model-module combinations.
                                                                   (back_to_top)
  ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
-[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (Self-
-Supervised Learning Models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
-`rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://
-github.com/facebookresearch/vissl)) - `barlowtwins-rn50`, `vicreg-rn50`, `dino-
-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`
-(retrieved from [torch.hub](https://pytorch.org/hub/)) - [OpenCLIP](https://
-github.com/mlfoundations/open_clip) - both original [CLIP](https://github.com/
-openai/CLIP) variants (`ViT-B/32` and `RN50`) - a few custom models (Alexnet,
-VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/
-doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet pretrained on
-ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
-sos.html) - each of the many [CORnet](https://github.com/dicarlolab/CORnet)
-versions - [Harmonization](https://arxiv.org/abs/2211.04533) models from the
-[official repo](https://github.com/serre-lab/harmonization). The default
-variant is `ViT_B16`. However, the following encoders are additionally
-available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`,
-`tiny_MaxViT`, `LeViT_small`
+[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
+supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
+`rotnet-rn50`, `swav-rn50`, `pirl-rn50` - `barlowtwins-rn50`, `vicreg-rn50`,
+`dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`,
+`dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-
+vit-giant-p14` - [OpenCLIP](https://github.com/mlfoundations/open_clip) - both
+original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and
+`RN50`) - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3)
+trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather
+than ImageNet and one Alexnet pretrained on ImageNet and fine-tuned on
+[SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html) - each of the many
+[CORnet](https://github.com/dicarlolab/CORnet) versions - [Harmonization]
+(https://arxiv.org/abs/2211.04533) models from the official [Harmonization
+repo](https://github.com/serre-lab/harmonization). The default variant is
+`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
+`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official
+[DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant
+is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs]
+(https://vicco-group.github.io/thingsvision/AvailableModels.html) for more
+information.
                                                                   (back_to_top)
  ## :running: Getting Started  ### :computer: Setting up your environment ####
 Working locally. First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
-//github.com/openai/CLIP.git $ pip install git+https://github.com/serre-lab/
-Harmonization.git ``` #### Google Colab. Alternatively, you can use Google
-Colab to play around with `thingsvision` by uploading your image data to Google
-Drive (via directory mounting). You can find the jupyter notebook using
-`PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/
-thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example
+//github.com/openai/CLIP.git ``` If you want to extract features for
+[harmonized models](https://vicco-group.github.io/thingsvision/
+AvailableModels.html#harmonization) from the [Harmonization repo](https://
+github.com/serre-lab/harmonization), you have to additionally run the following
+`pip` command in your `thingsvision` environment (FYI: as of now, this seems to
+be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
+git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
+attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
+(https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
+github.com/ssundaram21/dreamsim), you have to additionally run the following
+`pip` command in your `thingsvision` environment, ```bash $ pip install
+dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
+AvailableModels.html) for which `DreamSim` models are available in
+`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+play around with `thingsvision` by uploading your image data to Google Drive
+(via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
-master/notebooks/tensorflow.ipynb).
+master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
+colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
+notebooks/tensorflow.ipynb).
                                                                   (back_to_top)
  ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
@@ -81,45 +105,47 @@
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
 package directly and write your own Python script. #### Python commands To do
 this start by importing all the necessary components and instantiating a
-`thingsvision` extractor. Here we're using `AlexNet` from the `torchvision`
-library as the model to extract features from and also load the model to GPU
-for faster inference, ```python import torch from thingsvision import
-get_extractor from thingsvision.utils.storing import save_features from
-thingsvision.utils.data import ImageDataset, DataLoader model_name = 'alexnet'
-source = 'torchvision' device = 'cuda' if torch.cuda.is_available() else 'cpu'
-extractor = get_extractor( model_name=model_name, source=source, device=device,
-pretrained=True ) ``` As a next step, create both dataset and dataloader for
-your images. We assume that all of your images are in a single `root` directory
-which can contain subfolders (e.g., for individual classes). Therefore, we
-leverage the `ImageDataset` class. ```python root='path/to/root/img/directory'
-# (e.g., './images/) batch_size = 32 dataset = ImageDataset( root=root,
-out_path='path/to/features', backend=extractor.get_backend(), # backend
-framework of model transforms=extractor.get_transformations(resize_dim=256,
-crop_dim=224) # set input dimensionality to whatever is required for your
-pretrained model ) batches = DataLoader( dataset=dataset,
-batch_size=batch_size, backend=extractor.get_backend() # backend framework of
-model ) ``` Now all that is left is to extract the image features and store
-them to disk! Here we're extracting features from the last convolutional layer
-of AlexNet (`features.10`), but if you don't know which modules are available
-for a given model, just call `extractor.show_model()` to print all modules.
-```python module_name = 'features.10' features = extractor.extract_features
-( batches=batches, module_name=module_name, flatten_acts=True, # flatten 2D
-feature maps from convolutional layer output_type="ndarray", # or "tensor"
-(only applicable to PyTorch models) ) save_features(features, out_path='path/
-to/features', file_format='npy') ``` _For more examples on the many models
-available in `thingsvision` and explanations of additional functionality like
-how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD
-stimuli), how to perform RSA or CKA, or how to easily extract features for the
-[THINGS image database](https://osf.io/jum2f/), please refer to the
-[Documentation](https://vicco-group.github.io/thingsvision/)._
+`thingsvision` extractor. Here we're using `CLIP` from the official clip repo
+as the model to extract features from and also load the model to GPU for faster
+inference, ```python import torch from thingsvision import get_extractor from
+thingsvision.utils.storing import save_features from thingsvision.utils.data
+import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
+'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
+'ViT-B/32' } extractor = get_extractor( model_name=model_name, source=source,
+device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
+next step, create both dataset and dataloader for your images. We assume that
+all of your images are in a single `root` directory which can contain
+subfolders (e.g., for individual classes). Therefore, we leverage the
+`ImageDataset` class. ```python root='path/to/root/img/directory' # (e.g., './
+images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/to/
+features', backend=extractor.get_backend(), # backend framework of model
+transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
+the input dimensionality to whichever values are required for your pretrained
+model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
+backend=extractor.get_backend() # backend framework of model ) ``` Now all that
+is left is to extract the image features and store them on disk! Here we're
+extracting features from the image encoder layer (`visual`), but if you don't
+know which modules are available for a given model, just call
+`extractor.show_model()` to print all the modules. ```python module_name =
+'visual' features = extractor.extract_features( batches=batches,
+module_name=module_name, flatten_acts=True, output_type="ndarray", # or
+"tensor" (only applicable to PyTorch models of which CLIP is one!) )
+save_features(features, out_path='path/to/features', file_format='npy') #
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` _For more
+examples on the many models available in `thingsvision` and explanations of
+additional functionality like how to optionally turn off center cropping, how
+to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to
+easily extract features for the [THINGS image database](https://osf.io/jum2f/),
+please refer to the [Documentation](https://vicco-group.github.io/thingsvision/
+)._
                                                                   (back_to_top)
  ## :wave: How to contribute If you come across problems or have suggestions
 please submit an issue!
                                                                   (back_to_top)
  ## :warning: License This GitHub repository is licensed under the MIT License
 - see the [LICENSE.md](LICENSE.md) file for details.
                                                                   (back_to_top)
@@ -140,19 +166,18 @@
 and refined into its current form with the help of our many contributors, -
 [Alex Murphy](https://github.com/Alxmrphi) (software dev.) - [Florian Mahner]
 (https://www.cbs.mpg.de/person/mahner/1483114) (software dev.) - [Hannes
 Hansen](https://github.com/hahahannes) (software dev.) - [Johannes Roth](https:
 //jroth.space/) (software dev., design, docs) - [Jonas Dippel](https://
 github.com/jonasd4) (software dev.) - [Lukas Muttenthaler](https://
 lukasmut.github.io/) (software dev., design, docs, general responsibility) -
-[Martin N. Hebart](http://martin-hebart.de/) (design) - [Oliver Contier](https:
-//olivercontier.com/) (docs) - [Philipp Kaniuth](https://www.cbs.mpg.de/person/
-kaniuth/1483114) (design, docs) - [Roman Leipe](https://github.com/RLeipe)
-(sofware dev., docs), sorted alphabetically. This is a joint open-source
-project between the Max Planck Institute for Human Cognitive and Brain
-Sciences, Leipzig, and the Machine Learning Group at Technische UniverstitÃ¤t
-Berlin. Correspondence and requests for contributing should be adressed to
-[Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if
-you want to become a contributor or have any suggestions/feedback. For the
-latter, you could also just post an issue or engange in discussions. We'll try
-to respond as fast as we can.
+[Martin N. Hebart](http://martin-hebart.de/) (design) - [Philipp Kaniuth]
+(https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs) - [Roman Leipe]
+(https://github.com/RLeipe) (sofware dev., docs), sorted alphabetically. This
+is a joint open-source project between the Max Planck Institute for Human
+Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at
+Technische UniverstitÃ¤t Berlin. Correspondence and requests for contributing
+should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel
+free to contact us if you want to become a contributor or have any suggestions/
+feedback. For the latter, you could also just post an issue or engange in
+discussions. We'll try to respond as fast as we can.
                                                                   (back_to_top)
```

### Comparing `thingsvision-2.3.9/setup.py` & `thingsvision-2.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,34 +5,33 @@
 
 # activate __version__ variable
 exec(open("thingsvision/_version.py").read())
 
 requirements = [
     "ftfy",
     "h5py",
-    "keras-cv-attention-models>=1.3.5",
+    # "keras-cv-attention-models>=1.3.5",
     "matplotlib",
     "numba",
-    "numpy>=1.22.*",
+    "numpy",
     "open_clip_torch==2.0.*",
-    "pandas>=1.3.*",
+    "pandas",
     "regex",
     "scikit-image",
     "scikit-learn",
     "scipy",
     "tensorflow==2.9.* ; sys_platform != 'darwin' or platform_machine != 'arm64'",
     "tensorflow-macos==2.9.* ; sys_platform == 'darwin' and platform_machine == 'arm64'",
     "timm==0.6.*",
-    "torch>=1.13.1",
+    "torch==1.13.*",
     "torchvision==0.14.*",
     "torchtyping",
     "tqdm",
     "CLIP",
-    # "Harmonization",
-    # 'CLIP @ git+ssh://git@github.com/openai/CLIP@v1.0#egg=CLIP'
+    # 'CLIP @ git+ssh://git@github.com/openai/CLIP@v1.0#egg=CLIP' # TODO: see issue #111
 ]
 
 setuptools.setup(
     name="thingsvision",
     version=__version__,
     author="Lukas Muttenthaler",
     author_email="muttenthaler@cbs.mpg.de",
@@ -50,10 +49,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={"console_scripts": ["thingsvision = thingsvision.thingsvision:main"]},
     python_requires=">=3.8",
     dependency_links=[
         "git+https://github.com/openai/CLIP.git",
-        # "git+https://github.com/serre-lab/Harmonization.git",
     ],
 )
```

### Comparing `thingsvision-2.3.9/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.4.0/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.4.0/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.4.0/tests/extractor/extraction/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.4.0/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/extractor/test_load_extractor.py` & `thingsvision-2.4.0/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/extractor/test_transformations.py` & `thingsvision-2.4.0/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/helper.py` & `thingsvision-2.4.0/tests/helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,140 +12,229 @@
 from thingsvision.utils.data import DataLoader, ImageDataset
 from thingsvision import get_extractor
 
 DATA_PATH = "./data"
 TEST_PATH = "./test_images"
 OUT_PATH = "./test"
 
-SSL_RN50_DEFAULT_CONFIG = {
-    "modules": ["avgpool"],
-    "pretrained": True,
-    "source": "ssl",
-}
-
 MODEL_AND_MODULE_NAMES = {
     # Torchvision models
     "vgg16": {
+        "model_name": "vgg16",
         "modules": ["features.23", "classifier.3"],
         "pretrained": True,
         "source": "torchvision",
     },
     "vgg19_bn": {
+        "model_name": "vgg19_bn",
         "modules": ["features.23", "classifier.3"],
         "pretrained": False,
         "source": "torchvision",
     },
     # Hardcoded models
     "cornet_r": {
+        "model_name": "cornet_r",
         "modules": ["decoder.flatten"],
         "pretrained": True,
         "source": "custom",
     },
     "cornet_rt": {
+        "model_name": "cornet_rt",
         "modules": ["decoder.flatten"],
         "pretrained": False,
         "source": "custom",
     },
     "cornet_s": {
+        "model_name": "cornet_s",
         "modules": ["decoder.flatten"],
         "pretrained": False,
         "source": "custom",
     },
     "cornet_z": {
+        "model_name": "cornet_z",
         "modules": ["decoder.flatten"],
         "pretrained": True,
         "source": "custom",
     },
     # Custom models
     "VGG16_ecoset": {
+        "model_name": "VGG16_ecoset",
         "modules": ["classifier.3"],
         "pretrained": True,
         "source": "custom",
     },
-    "clip": {
+    "clip_vitb32": {
+        "model_name": "clip",
         "modules": ["visual"],
         "pretrained": True,
         "source": "custom",
         "clip": True,
         "kwargs": {"variant": "ViT-B/32"},
     },
-    "clip": {
+    "clip_rn50": {
+        "model_name": "clip",
         "modules": ["visual"],
         "pretrained": True,
         "source": "custom",
         "clip": True,
         "kwargs": {"variant": "RN50"},
     },
-    "OpenCLIP": {
+    "OpenCLIP_vitb32": {
+        "model_name": "OpenCLIP",
         "modules": ["visual"],
         "pretrained": True,
         "source": "custom",
         "clip": True,
         "kwargs": {"variant": "ViT-B-32", "dataset": "openai"},
     },
     # Timm models
-    "mixnet_l": {"modules": ["conv_head"], "pretrained": True, "source": "timm"},
-    "gluon_inception_v3": {
-        "modules": ["Mixed_6d"],
-        "pretrained": False,
-        "source": "timm",
+    "mixnet_l": {
+        "model_name": "mixnet_l",
+        "modules": ["conv_head"],
+        "pretrained": True,
+        "source": "timm"
     },
     # Keras models
-    "VGG16": {
+    "VGG16_keras": {
+        "model_name": "VGG16",
         "modules": ["block1_conv1", "flatten"],
         "pretrained": True,
         "source": "keras",
     },
-    "VGG19": {
+    "VGG19_keras": {
+        "model_name": "VGG19",
         "modules": ["block1_conv1", "flatten"],
         "pretrained": False,
         "source": "keras",
     },
     # Vissl models
-    'simclr-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'mocov2-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'jigsaw-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'rotnet-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'swav-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'pirl-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'barlowtwins-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'vicreg-rn50': SSL_RN50_DEFAULT_CONFIG,
-    'dino-rn50' : SSL_RN50_DEFAULT_CONFIG,
-    # Harmonization models
-    "Harmonization": {
-        "modules": ["visual"],
+    "simclr-rn50": {
+        "model_name": "simclr-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "mocov2-rn50": {
+        "model_name": "mocov2-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "jigsaw-rn50": {
+        "model_name": "jigsaw-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "rotnet-rn50": {
+        "model_name": "rotnet-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "swav-rn50": {
+        "model_name": "swav-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "pirl-rn50": {
+        "model_name": "pirl-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "barlowtwins-rn50": {
+        "model_name": "barlowtwins-rn50",
+        "modules": ["avgpool"],
+        "pretrained": True,
+        "source": "ssl",
+    },
+    "dino-vit-tiny-p8": {
+        "model_name": "dino-vit-small-p8",
+        "modules": ["norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True}
+    },
+    "dino-vit-small-p8": {
+        "model_name": "dino-vit-small-p8",
+        "modules": ["norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True}
+    },
+    "dino-vit-base-p8": {
+        "model_name": "dino-vit-base-p8",
+        "modules": ["norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True}
+    },
+    "dinov2-vit-small-p14": {
+        "model_name": "dinov2-vit-small-p14",
+        "modules": ["norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True}
+    },
+    "dinov2-vit-base-p14": {
+        "model_name": "dinov2-vit-base-p14",
+        "modules": ["norm"],
+        "pretrained": True,
+        "source": "ssl",
+        "kwargs": {"extract_cls_token": True}
+    },
+    # Additional models
+    "Harmonization_visual_ResNet50": {
+        "model_name": "Harmonization",
+        "modules": ["avg_pool"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "ResNet50"},
     },
-    "Harmonization": {
+    "Harmonization_fc2_VGG16": {
+        "model_name": "Harmonization",
         "modules": ["fc2"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "VGG16"},
     },
-     "Harmonization": {
+    "Harmonization_head_ViT_B16": {
+        "model_name": "Harmonization",
         "modules": ["head"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "ViT_B16"},
-    }
+    },
+    "DreamSim_mlp_clip_vitb32": {
+        "model_name": "DreamSim",
+        "modules": ["model.mlp"],
+        "pretrained": True,
+        "source": "custom",
+        "kwargs": {"variant": "clip_vitb32"},
+    },
+    "DreamSim_mlp_open_clip_vitb32": {
+        "model_name": "DreamSim",
+        "modules": ["model.mlp"],
+        "pretrained": True,
+        "source": "custom",
+        "kwargs": {"variant": "open_clip_vitb32"},
+    },
 }
 
-
 FILE_FORMATS = ["hdf5", "npy", "mat", "pt", "txt"]
 DISTANCES = ["correlation", "cosine", "euclidean", "gaussian"]
 
 BATCH_SIZE = 16
 NUM_OBJECTS = 1854
 # we want to iterate over two batches to exhaustively test mini-batching
 NUM_SAMPLES = int(BATCH_SIZE * 2)
 DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
 
-
 tf_model = Sequential()
 tf_model.add(Dense(2, input_dim=1, activation="relu", use_bias=False, name="relu"))
 weights = np.array([[[1, 1]]])
 tf_model.get_layer("relu").set_weights(weights)
 tf_model.add(Dense(2, input_dim=2, activation="relu", use_bias=False, name="relu2"))
 weights = np.array([[[1, 1], [1, 1]]])
 tf_model.get_layer("relu2").set_weights(weights)
@@ -213,29 +302,30 @@
         return value
 
     def __len__(self) -> int:
         return len(self.values)
 
 
 def iterate_through_all_model_combinations():
-    for model_name in MODEL_AND_MODULE_NAMES:
-        pretrained = MODEL_AND_MODULE_NAMES[model_name]["pretrained"]
-        source = MODEL_AND_MODULE_NAMES[model_name]["source"]
-        kwargs = MODEL_AND_MODULE_NAMES[model_name].get("kwargs", {})
+    for model_config in MODEL_AND_MODULE_NAMES.values():
+        model_name = model_config['model_name']
+        pretrained = model_config["pretrained"]
+        source = model_config["source"]
+        kwargs = model_config.get("kwargs", {})
         extractor, dataset, batches = create_extractor_and_dataloader(
             model_name, pretrained, source, kwargs
         )
 
-        modules = MODEL_AND_MODULE_NAMES[model_name]["modules"]
-        clip = MODEL_AND_MODULE_NAMES[model_name].get("clip", False)
+        modules = model_config["modules"]
+        clip = model_config.get("clip", False)
         yield extractor, dataset, batches, modules, model_name, clip
 
 
 def create_extractor_and_dataloader(
-    model_name: str, pretrained: bool, source: str, kwargs: dict = {}
+        model_name: str, pretrained: bool, source: str, kwargs: dict = {}
 ):
     """Iterate through models and create model, dataset and data loader."""
     extractor = get_extractor(
         model_name=model_name,
         pretrained=pretrained,
         device=DEVICE,
         source=source,
@@ -278,10 +368,10 @@
                 test_img = np.copy(test_imgs[1])
                 cls = classes[1]
             H, W, C = test_img.shape
             # add random Gaussian noise to test image
             noisy_img = test_img + np.random.randn(H, W, C)
             noisy_img = noisy_img.astype(np.uint8)
             imageio.imsave(
-                os.path.join(TEST_PATH, cls, f"test_img_{i+1:03d}.png"), noisy_img
+                os.path.join(TEST_PATH, cls, f"test_img_{i + 1:03d}.png"), noisy_img
             )
         print("\n...Successfully created image dataset for testing.\n")
```

### Comparing `thingsvision-2.3.9/tests/test_features.py` & `thingsvision-2.4.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/tests/test_rest.py` & `thingsvision-2.4.0/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/core/cka/base.py` & `thingsvision-2.4.0/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/core/extraction/base.py` & `thingsvision-2.4.0/thingsvision/core/extraction/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,55 @@
 import abc
 import os
+import re
 import warnings
 from typing import Callable, Iterator, List, Optional, Union
 
 import numpy as np
+import torch
 from torchtyping import TensorType
 from tqdm.auto import tqdm
 
-import torch
-
 Array = np.ndarray
 
 
 class BaseExtractor(metaclass=abc.ABCMeta):
     def __init__(self, device, preprocess) -> None:
         self.device = device
+        self._check_device()
         self.preprocess = preprocess
 
     def show(self) -> None:
         warnings.warn(
             message="\nThe .show() method is deprecated and will be removed in future versions. Use .show_model() instead.\n",
             category=UserWarning,
         )
         self.show_model()
 
+    def _check_device(self) -> None:
+        if self.device.startswith("cuda"):
+            gpu_index = re.search(r"cuda:(\d+)", self.device)
+
+            if not torch.cuda.is_available():
+                warnings.warn(
+                    "\nCUDA is not available on your system. Switching to device='cpu'.\n",
+                    category=UserWarning,
+                )
+                self.device = "cpu"
+            elif gpu_index and int(gpu_index.group(1)) >= torch.cuda.device_count():
+                warnings.warn(
+                    f"\nGPU index {gpu_index.group(1)} is out of range. "
+                    f"Available GPUs: {torch.cuda.device_count()}. "
+                    f"Switching to device='cuda:0'.\n",
+                    category=UserWarning,
+                )
+                self.device = "cuda:0"
+
+        print("Using device: ", self.device)
+
     @abc.abstractmethod
     def show_model(self) -> None:
         """Show architecture."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_default_transformation(
@@ -146,14 +168,15 @@
             features.append(
                 self._extract_batch(
                     batch=batch, module_name=module_name, flatten_acts=flatten_acts
                 )
             )
 
             image_ct += len(batch)
+            del batch
 
             if output_dir and (i % step_size == 0 or i == len(batches)):
                 if self.get_backend() == "pt":
                     features_subset = torch.cat(features)
                     if output_type == "ndarray":
                         features_subset = self._to_numpy(features_subset)
                         features_subset_file = os.path.join(
@@ -197,15 +220,15 @@
             TensorType["n", "num_maps", "h_prime", "w_prime"],
             TensorType["n", "t", "d"],
             TensorType["n", "p"],
             TensorType["n", "d"],
         ]
     ) -> Array:
         """Move activations to CPU and convert torch.Tensor to np.ndarray."""
-        return features.cpu().numpy()
+        return features.numpy()
 
     def get_transformations(
         self, resize_dim: int = 256, crop_dim: int = 224, apply_center_crop: bool = True
     ) -> Callable:
         """Load image transformations for a specific model. Image transformations depend on the backend."""
         if self.preprocess:
             return self.preprocess
```

### Comparing `thingsvision-2.3.9/thingsvision/core/extraction/extractors.py` & `thingsvision-2.4.0/thingsvision/core/extraction/extractors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
-from typing import Any, Dict
+from dataclasses import field
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
-import timm
-import torchvision
-
 import tensorflow as tf
 import tensorflow.keras.applications as tensorflow_models
+import timm
 import torch
+import torchvision
 
 try:
     from torch.hub import load_state_dict_from_url
 except ImportError:
     from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
+from thingsvision.utils.checkpointing import get_torch_home
+
 from .tensorflow import TensorFlowExtractor
 from .torch import PyTorchExtractor
+from thingsvision.utils.models.dino import vit_tiny, vit_base, vit_small
 
 # neccessary to prevent gpu memory conflicts between torch and tf
 gpus = tf.config.list_physical_devices("GPU")
 if gpus:
     try:
         # Currently, memory growth needs to be the same across GPUs
         for gpu in gpus:
@@ -32,21 +35,23 @@
 
 Tensor = torch.Tensor
 Array = np.ndarray
 
 
 class TorchvisionExtractor(PyTorchExtractor):
     def __init__(
-        self,
-        model_name: str,
-        pretrained: bool,
-        device: str,
-        model_path: str = None,
-        model_parameters: Dict = None,
-        preprocess: Any = None,
+            self,
+            model_name: str,
+            pretrained: bool,
+            device: str,
+            model_path: str = None,
+            model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+                default_factory=lambda: {}
+            ),
+            preprocess: Optional[Callable] = None,
     ) -> None:
         model_parameters = (
             model_parameters if model_parameters else {"weights": "DEFAULT"},
         )
         super().__init__(
             model_name=model_name,
             pretrained=pretrained,
@@ -83,40 +88,42 @@
             self.model = model(weights=self.weights)
         else:
             raise ValueError(
                 f"\nCould not find {self.model_name} in torchvision library.\nChoose a different model.\n"
             )
 
     def get_default_transformation(
-        self,
-        mean,
-        std,
-        resize_dim: int = 256,
-        crop_dim: int = 224,
-        apply_center_crop: bool = True,
+            self,
+            mean,
+            std,
+            resize_dim: int = 256,
+            crop_dim: int = 224,
+            apply_center_crop: bool = True,
     ) -> Any:
         if self.weights:
             transforms = self.weights.transforms()
         else:
             transforms = super().get_default_transformation(
                 mean, std, resize_dim, crop_dim, apply_center_crop
             )
 
         return transforms
 
 
 class TimmExtractor(PyTorchExtractor):
     def __init__(
-        self,
-        model_name: str,
-        pretrained: bool,
-        device: str,
-        model_path: str = None,
-        model_parameters: Dict = None,
-        preprocess: Any = None,
+            self,
+            model_name: str,
+            pretrained: bool,
+            device: str,
+            model_path: str = None,
+            model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+                default_factory=lambda: {}
+            ),
+            preprocess: Optional[Callable] = None,
     ) -> None:
         super().__init__(
             model_name=model_name,
             pretrained=pretrained,
             model_path=model_path,
             model_parameters=model_parameters,
             preprocess=preprocess,
@@ -131,21 +138,23 @@
             raise ValueError(
                 f"\nCould not find {self.model_name} in timm library.\nChoose a different model.\n"
             )
 
 
 class KerasExtractor(TensorFlowExtractor):
     def __init__(
-        self,
-        model_name: str,
-        pretrained: bool,
-        device: str,
-        model_path: str = None,
-        model_parameters: Dict = None,
-        preprocess: Any = None,
+            self,
+            model_name: str,
+            pretrained: bool,
+            device: str,
+            model_path: str = None,
+            model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+                default_factory=lambda: {}
+            ),
+            preprocess: Optional[Callable] = None,
     ) -> None:
         model_parameters = (
             model_parameters if model_parameters else {"weights": "imagenet"}
         )
         super().__init__(
             model_name=model_name,
             pretrained=pretrained,
@@ -169,17 +178,14 @@
         else:
             raise ValueError(
                 f"\nCould not find {self.model_name} among TensorFlow models.\n"
             )
 
 
 class SSLExtractor(PyTorchExtractor):
-    ENV_TORCH_HOME = "TORCH_HOME"
-    ENV_XDG_CACHE_HOME = "XDG_CACHE_HOME"
-    DEFAULT_CACHE_DIR = "~/.cache"
     MODELS = {
         "simclr-rn50": {
             "url": "https://dl.fbaipublicfiles.com/vissl/model_zoo/simclr_rn50_800ep_simclr_8node_resnet_16_07_20.7e8feed1/model_final_checkpoint_phase799.torch",
             "arch": "resnet50",
             "type": "vissl",
         },
         "mocov2-rn50": {
@@ -217,29 +223,33 @@
             "arch": "resnet50",
             "type": "hub",
         },
         "dino-vit-small-p16": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_vits16",
             "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/dino/dino_deitsmall16_pretrain/dino_deitsmall16_pretrain.pth"
         },
-         "dino-vit-small-p8": {
+        "dino-vit-small-p8": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_vits8",
             "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/dino/dino_deitsmall8_pretrain/dino_deitsmall8_pretrain.pth"
         },
-        "dino-vit-big-p16": {
+        "dino-vit-base-p16": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_vitb16",
             "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/dino/dino_vitbase16_pretrain/dino_vitbase16_pretrain.pth"
         },
-        "dino-vit-big-p8": {
+        "dino-vit-base-p8": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_vitb8",
             "type": "hub",
+            "checkpoint_url": "https://dl.fbaipublicfiles.com/dino/dino_vitbase8_pretrain/dino_vitbase8_pretrain.pth"
         },
         "dino-xcit-small-12-p16": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_xcit_small_12_p16",
             "type": "hub",
         },
         "dino-xcit-small-12-p8": {
@@ -258,24 +268,46 @@
             "type": "hub",
         },
         "dino-rn50": {
             "repository": "facebookresearch/dino:main",
             "arch": "dino_resnet50",
             "type": "hub",
         },
+        "dinov2-vit-small-p14": {
+            "repository": "facebookresearch/dinov2",
+            "arch": "dinov2_vits14",
+            "type": "hub",
+        },
+        "dinov2-vit-base-p14": {
+            "repository": "facebookresearch/dinov2",
+            "arch": "dinov2_vitb14",
+            "type": "hub",
+        },
+        "dinov2-vit-large-p14": {
+            "repository": "facebookresearch/dinov2",
+            "arch": "dinov2_vitl14",
+            "type": "hub",
+        },
+        "dinov2-vit-giant-p14": {
+            "repository": "facebookresearch/dinov2",
+            "arch": "dinov2_vitg14",
+            "type": "hub",
+        },
     }
 
     def __init__(
-        self,
-        model_name: str,
-        pretrained: bool,
-        device: str,
-        model_path: str = None,
-        model_parameters: Dict = None,
-        preprocess: Any = None,
+            self,
+            model_name: str,
+            pretrained: bool,
+            device: str,
+            model_path: str = None,
+            model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+                default_factory=lambda: {}
+            ),
+            preprocess: Optional[Callable] = None,
     ) -> None:
         super().__init__(
             model_name=model_name,
             pretrained=pretrained,
             model_path=model_path,
             model_parameters=model_parameters,
             preprocess=preprocess,
@@ -298,75 +330,77 @@
             model_trunk = model
 
         converted_model = self._replace_module_prefix(model_trunk, "_feature_blocks.")
         torch.save(converted_model, output_model_filepath)
         return converted_model
 
     def _replace_module_prefix(
-        self, state_dict: Dict[str, Any], prefix: str, replace_with: str = ""
+            self, state_dict: Dict[str, Any], prefix: str, replace_with: str = ""
     ):
         """
         Remove prefixes in a state_dict needed when loading models that are not VISSL
         trained models.
         Specify the prefix in the keys that should be removed.
         """
         state_dict = {
             (
                 key.replace(prefix, replace_with, 1) if key.startswith(prefix) else key
             ): val
             for (key, val) in state_dict.items()
         }
         return state_dict
 
-    def _get_torch_home(self):
-        """
-        Gets the torch home folder used as a cache directory for the vissl models.
-        """
-        torch_home = os.path.expanduser(
-            os.getenv(
-                SSLExtractor.ENV_TORCH_HOME,
-                os.path.join(
-                    os.getenv(
-                        SSLExtractor.ENV_XDG_CACHE_HOME, SSLExtractor.DEFAULT_CACHE_DIR
-                    ),
-                    "torch",
-                ),
-            )
-        )
-        return torch_home
-
     def load_model_from_source(self) -> None:
         """
         Load a (pretrained) neural network model from vissl. Downloads the model when it is not available.
         Otherwise, loads it from the cache directory.
         """
         if self.model_name in SSLExtractor.MODELS:
             model_config = SSLExtractor.MODELS[self.model_name]
             if model_config["type"] == "vissl":
-                cache_dir = os.path.join(self._get_torch_home(), "vissl")
+                cache_dir = os.path.join(get_torch_home(), "vissl")
                 model_filepath = os.path.join(cache_dir, self.model_name + ".torch")
                 if not os.path.exists(model_filepath):
                     os.makedirs(cache_dir, exist_ok=True)
                     model_state_dict = self._download_and_save_model(
                         model_url=model_config["url"],
                         output_model_filepath=model_filepath,
                     )
                 else:
                     model_state_dict = torch.load(
                         model_filepath, map_location=torch.device("cpu")
                     )
                 self.model = getattr(torchvision.models, model_config["arch"])()
-                if model_config["arch"] == 'resnet50':
+                if model_config["arch"] == "resnet50":
                     self.model.fc = torch.nn.Identity()
                 self.model.load_state_dict(model_state_dict, strict=True)
             elif model_config["type"] == "hub":
-                self.model = torch.hub.load(
-                    model_config["repository"], model_config["arch"]
-                )
-                if model_config["arch"] == 'resnet50':
-                    self.model.fc = torch.nn.Identity()
+                if self.model_name.startswith("dino-vit"):
+                    if self.model_name == "dino-vit-tiny-p8":
+                        model = vit_tiny(patch_size=8)
+                    elif self.model_name == "dino-vit-tiny-p16":
+                        model = vit_tiny(patch_size=16)
+                    elif self.model_name == "dino-vit-small-p8":
+                        model = vit_small(patch_size=8)
+                    elif self.model_name == "dino-vit-small-p16":
+                        model = vit_small(patch_size=16)
+                    elif self.model_name == "dino-vit-base-p8":
+                        model = vit_base(patch_size=8)
+                    elif self.model_name == "dino-vit-base-p16":
+                        model = vit_base(patch_size=16)
+                    else:
+                        raise ValueError(f"\n{self.model_name} is not available.\n")
+                    state_dict = torch.hub.load_state_dict_from_url(model_config["checkpoint_url"])
+                    model.load_state_dict(state_dict, strict=True)
+                    self.model = model
+                else:
+                    self.model = torch.hub.load(
+                        model_config["repository"], model_config["arch"]
+                    )
+                    if model_config["arch"] == "resnet50":
+                        self.model.fc = torch.nn.Identity()
             else:
                 raise ValueError(f"\nUnknown model type.\n")
         else:
             raise ValueError(
                 f"\nCould not find {self.model_name} in the SSLExtractor.\n"
             )
```

### Comparing `thingsvision-2.3.9/thingsvision/core/extraction/helpers.py` & `thingsvision-2.4.0/thingsvision/core/extraction/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,16 @@
+import warnings
 from typing import Any, Callable, Dict, Union
 
 import numpy as np
-import thingsvision.custom_models as custom_models
-import thingsvision.custom_models.cornet as cornet
-from torchtyping import TensorType
-
 import torch
-import warnings
+from torchtyping import TensorType
 
-from .extractors import (
-    KerasExtractor,
-    SSLExtractor,
-    TimmExtractor,
-    TorchvisionExtractor,
-)
+from .extractors import (KerasExtractor, SSLExtractor, TimmExtractor,
+                         TorchvisionExtractor)
 from .tensorflow import TensorFlowExtractor
 from .torch import PyTorchExtractor
 
 Array = np.ndarray
 AxisError = np.AxisError
 
 
@@ -26,32 +19,46 @@
     pretrained: bool,
     device: str,
     model_path: str = None,
     model_parameters: Dict[str, str] = None,
 ) -> Any:
     """Create a custom extractor from a pretrained model."""
     if model_name.startswith("cornet"):
+        import thingsvision.custom_models.cornet as cornet
+
         backend = "pt"
         try:
             model = getattr(cornet, f"cornet_{model_name[-1]}")
         except AttributeError:
             model = getattr(cornet, f"cornet_{model_name[-2:]}")
         model = model(pretrained=pretrained, map_location=torch.device(device))
         model = model.module  # remove DataParallel
         preprocess = None
-    elif hasattr(custom_models, model_name):
+    else:
+        if model_name == "Harmonization":
+            import thingsvision.custom_models.harmonization as harmonization
+
+            custom_model = getattr(harmonization, model_name)
+        elif model_name == "DreamSim":
+            import thingsvision.custom_models.dreamsim as dreamsim
+
+            custom_model = getattr(dreamsim, model_name)
+        else:
+            import thingsvision.custom_models as custom_models
+
+            if hasattr(custom_models, model_name):
+                custom_model = getattr(custom_models, model_name)
+            else:
+                raise ValueError(
+                    f"\nCould not find {model_name} among available custom models.\nChoose a different model that is available.\n"
+                )
         model_parameters = model_parameters if model_parameters else {}
-        custom_model = getattr(custom_models, model_name)
         custom_model = custom_model(device, model_parameters)
         model, preprocess = custom_model.create_model()
         backend = custom_model.get_backend()
-    else:
-        raise ValueError(
-            f"\nCould not find {model_name} among custom models.\nChoose a different model.\n"
-        )
 
     Extractor = PyTorchExtractor if backend == "pt" else TensorFlowExtractor
 
     class CustomExtractor(Extractor):
         def __init__(self, *args, **kwargs) -> None:
             super().__init__(*args, **kwargs)
```

### Comparing `thingsvision-2.3.9/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.4.0/thingsvision/core/extraction/tensorflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from dataclasses import field
-from typing import Any, List
+from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 
 from .base import BaseExtractor
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"  # suppress tensorflow warnings
 import tensorflow as tf
@@ -17,17 +17,19 @@
 class TensorFlowExtractor(BaseExtractor):
     def __init__(
         self,
         model_name: str,
         pretrained: bool,
         device: str,
         model_path: str = None,
-        model_parameters: Any = field(default_factory=lambda: {}),
+        model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+            default_factory=lambda: {}
+        ),
         model: Any = None,
-        preprocess: Any = None,
+        preprocess: Optional[Callable] = None,
     ) -> None:
         super().__init__(device, preprocess)
         self.model_name = model_name
         self.pretrained = pretrained
         self.model_path = model_path
         self.model_parameters = model_parameters
         self.model = model
```

### Comparing `thingsvision-2.3.9/thingsvision/core/extraction/torch.py` & `thingsvision-2.4.0/thingsvision/core/extraction/torch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from dataclasses import field
-from typing import Any, Callable, Iterator, List, Optional, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
 import numpy as np
+import torch
 from torchtyping import TensorType
 from torchvision import transforms as T
 
-import torch
-
 from .base import BaseExtractor
 
 Array = np.ndarray
 
 
 class PyTorchExtractor(BaseExtractor):
     def __init__(
         self,
         model_name: str,
         pretrained: bool,
         device: str,
         model_path: str = None,
-        model_parameters: Any = field(default_factory=lambda: {}),
+        model_parameters: Dict[str, Union[str, bool, List[str]]] = field(
+            default_factory=lambda: {}
+        ),
         model: Any = None,
-        preprocess: Any = None,
+        preprocess: Optional[Callable] = None,
     ) -> None:
         super().__init__(device, preprocess)
         self.model_name = model_name
         self.pretrained = pretrained
         self.model_path = model_path
         self.model_parameters = model_parameters
         self.model = model
         self.activations = {}
         self.hook_handle = None
 
+        if isinstance(self.model_parameters, dict):
+            if "extract_cls_token" in self.model_parameters:
+                self.extract_cls_token = self.model_parameters["extract_cls_token"]
+
         if not self.model:
             self.load_model()
         self.prepare_inference()
 
     def extract_features(
         self,
         batches: Iterator,
@@ -53,15 +58,15 @@
             module_name=module_name,
             flatten_acts=flatten_acts,
             output_type=output_type,
             output_dir=output_dir,
             step_size=step_size,
         )
         if self.hook_handle:
-            self.hook_handle.remove()
+            self._unregister_hook()
         return features
 
     def get_activation(self, name: str) -> Callable:
         """Store copy of activations for a specific layer of the model."""
 
         def hook(model, input, output) -> None:
             # store copy of tensor rather than tensor itself
@@ -79,14 +84,17 @@
     def register_hook(self, module_name: str) -> None:
         """Register a forward hook to store activations."""
         for n, m in self.model.named_modules():
             if n == module_name:
                 self.hook_handle = m.register_forward_hook(self.get_activation(n))
                 break
 
+    def _unregister_hook(self) -> None:
+        self.hook_handle.remove()
+
     @torch.no_grad()
     def _extract_batch(
         self,
         batch: TensorType["b", "c", "h", "w"],
         module_name: str,
         flatten_acts: bool,
     ) -> Union[
@@ -95,19 +103,25 @@
         TensorType["b", "p"],
         TensorType["b", "d"],
     ]:
         # move current batch to torch device
         batch = batch.to(self.device)
         _ = self.forward(batch)
         act = self.activations[module_name]
+        if hasattr(self, "extract_cls_token"):
+            # we are only interested in the representations of the first token, i.e., [cls] token
+            act = act[:, 0, :].clone()
         if flatten_acts:
             if self.model_name.lower().startswith("clip"):
                 act = self.flatten_acts(act, batch, module_name)
             else:
                 act = self.flatten_acts(act)
+        if act.is_cuda or act.get_device() >= 0:
+            torch.cuda.empty_cache()
+            act = act.cpu()
         return act
 
     def forward(
         self, batch: TensorType["b", "c", "h", "w"]
     ) -> TensorType["b", "num_cls"]:
         """Default forward pass."""
         return self.model(batch)
```

### Comparing `thingsvision-2.3.9/thingsvision/core/rsa/helpers.py` & `thingsvision-2.4.0/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.4.0/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Any
+
 import torch
 import torchvision.models as models
 
-from typing import Any
 from .custom import Custom
 
 
 class Alexnet_ecoset(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.4.0/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Any
+
 import torch
 import torchvision.models as models
 
-from typing import Any
 from .custom import Custom
 
+
 class AlexNet_SalObjSub(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
 
     def create_model(self) -> Any:
         model = models.alexnet(weights=None, num_classes=565)
         path_to_weights = "https://osf.io/download/sd3xj/"
         state_dict = torch.hub.load_state_dict_from_url(
             path_to_weights, map_location=self.device, file_name="AlexNet_SalObjSub"
         )
         model.load_state_dict(state_dict)
-        return model, None
+        return model, None
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.4.0/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.4.0/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/harmonization.py` & `thingsvision-2.4.0/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from harmonization.models import (
-    load_ViT_B16,
-    load_ResNet50,
-    load_VGG16,
-    load_EfficientNetB0,
-    load_tiny_ConvNeXT,
-    load_tiny_MaxViT,
-    load_LeViT_small,
-)
 from typing import Any
-from .custom import Custom
+
+from harmonization.models import (load_EfficientNetB0, load_LeViT_small,
+                                  load_ResNet50, load_tiny_ConvNeXT,
+                                  load_tiny_MaxViT, load_VGG16, load_ViT_B16)
+
+from thingsvision.custom_models.custom import Custom
 
 
 class Harmonization(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "tf"
         self.variant = parameters.get("variant", "ViT_B16")
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.4.0/thingsvision/custom_models/inception_ecoset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Any
+
 import torch
 import torchvision.models as models
 
-from typing import Any
 from .custom import Custom
 
 
 class Inception_ecoset(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/openclip.py` & `thingsvision-2.4.0/thingsvision/custom_models/openclip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+from typing import Any
 
 import open_clip
 
-from typing import Any
 from .custom import Custom
 
 
 class OpenCLIP(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
-        self.dataset = parameters.get('dataset', 'laion400m_e32')
-        self.variant = parameters.get('variant', 'ViT-B-32-quickgelu')
+        self.dataset = parameters.get("dataset", "laion400m_e32")
+        self.variant = parameters.get("variant", "ViT-B-32-quickgelu")
 
     def check_available_variants_and_datasets(self):
         found = False
         for variant, dataset in open_clip.list_pretrained():
             if variant == self.variant and dataset == self.dataset:
                 found = True
                 break
         if not found:
-            raise ValueError(f'\nCould not find an OpenCLIP model with variant: {self.variant} and dataset: {self.dataset}.\n')
+            raise ValueError(
+                f"\nCould not find an OpenCLIP model with variant: {self.variant} and dataset: {self.dataset}.\n"
+            )
 
     def create_model(self) -> Any:
         self.check_available_variants_and_datasets()
-        model, _, preprocess = open_clip.create_model_and_transforms(self.variant, pretrained=self.dataset)
+        model, _, preprocess = open_clip.create_model_and_transforms(
+            self.variant, pretrained=self.dataset
+        )
         return model, preprocess
-
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.4.0/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from typing import Any
+
 import torch
 import torchvision.models as models
 
-from typing import Any
 from .custom import Custom
 
 
 class Resnet50_ecoset(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
```

### Comparing `thingsvision-2.3.9/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.4.0/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from typing import Any
+
 import torch
 import torchvision.models as models
 
-from typing import Any
 from .custom import Custom
 
 
 class VGG16_ecoset(Custom):
     def __init__(self, device, parameters) -> None:
         super().__init__(device)
         self.backend = "pt"
 
     def create_model(self) -> Any:
         model = models.vgg16(weights=None, num_classes=565)
         path_to_weights = "https://osf.io/z5uf3/download"
         state_dict = torch.hub.load_state_dict_from_url(
-            path_to_weights, map_location=self.device, file_name="VGG16bn_ecoset"
+            path_to_weights, map_location=self.device, file_name="VGG16_ecoset"
         )
         model.load_state_dict(state_dict)
         return model, None
```

### Comparing `thingsvision-2.3.9/thingsvision/thingsvision.py` & `thingsvision-2.4.0/thingsvision/thingsvision.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 #!/usr/bin/env python3
 
 """ This is the command-line interface for the thingsvision toolbox """
 
 import argparse
-import torch
 import textwrap
 import sys
+import re
 import pkg_resources
 
+def device_type(device_str: str) -> str:
+    if device_str == "cpu" or device_str == "cuda" or re.match(r"cuda:\d+", device_str):
+        return device_str
+    else:
+        raise argparse.ArgumentTypeError(f"Invalid device string: '{device_str}'. Expected 'cpu', 'cuda', or 'cuda:x'.")
 
 def get_parsers():
     parent_parser = argparse.ArgumentParser(
         add_help=False,
         prog="thingsvision",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=textwrap.dedent(
@@ -31,18 +36,18 @@
         type=str,
         default="torchvision",
         choices=["torchvision", "keras", "timm", "custom"],
         help="Source of the model to use for feature extraction. (default: torchvision)",
     )
     common_parser.add_argument(
         "--device",
-        type=str,
-        default="cpu",
-        choices=["cpu", "cuda"],
-        help="Device to use for the extractor. (default: cpu)",
+        type=device_type,
+        default="cuda",
+        help="""Device to use for the extractor. Options are 'cpu', 'cuda', or 'cuda:x', 
+                where x is the GPU index. (default: cuda)""",
     )
 
     subparsers = parent_parser.add_subparsers(
         title="Subcommands",
         description="Valid subcommands are",
         help="Additional help available is available within  each subcommand",
         dest="command",
@@ -63,32 +68,27 @@
     parser_extract.add_argument(
         "--image-root",
         type=str,
         help="Path to directory containing images. (default: ./images)",
         default="./images",
     )
     parser_extract.add_argument(
-        "--class-names",
-        type=str,
-        help="optional list of class names for class dataset. (default: None)",
-        default=None,
-    )
-    parser_extract.add_argument(
-        "--file-names",
-        type=str,
-        help="optional list of file names for class dataset. (default: None)",
-        default=None,
-    )
-    parser_extract.add_argument(
         "--batch-size",
         type=int,
         default=32,
         help="Batch size used for feature extraction. (default: 32)",
     )
     parser_extract.add_argument(
+        "--output-type",
+        type=str,
+        default="ndarray",
+        help="Output type of the extracted features.",
+        choices=["ndarray", "tensor"],
+    )
+    parser_extract.add_argument(
         "--out-path",
         type=str,
         default="./features",
         help="Path to directory where features should be stored. (default: ./features)",
     )
     parser_extract.add_argument(
         "--flatten-acts", action="store_true", help="Flatten activations before saving."
@@ -141,50 +141,46 @@
     elif len(sys.argv) == 2:
         print("\nPlease specify optional commands and arguments:\n")
         if args.command == "show-model":
             parser_model.print_help(sys.stderr)
         elif args.command == "extract-features":
             parser_extract.print_help(sys.stderr)
         sys.exit(1)
-
-    device = torch.device(args.device)
-
+    
     from thingsvision import get_extractor
     from thingsvision.utils.storing import save_features
     from thingsvision.utils.data import ImageDataset, DataLoader
 
     extractor = get_extractor(
         model_name=args.model_name,
-        model_path=None,
+        source=args.source, 
         pretrained=True,
-        source=args.source,
-        device=device,
+        device=args.device,
     )
 
     if args.command == "show-model":
         extractor.show_model()
         sys.exit(1)
 
     if args.command == "extract-features":
         dataset = ImageDataset(
             root=args.image_root,
             out_path=args.out_path,
             backend=extractor.get_backend(),
             transforms=extractor.get_transformations(),
-            class_names=args.class_names,
-            file_names=args.file_names,
         )
         batches = DataLoader(
             dataset=dataset, batch_size=args.batch_size, backend=extractor.backend
         )
 
         features = extractor.extract_features(
             batches=batches,
             module_name=args.module_name,
             flatten_acts=args.flatten_acts,
+            output_type=args.output_type,
         )
 
         save_features(
             features=features, out_path=args.out_path, file_format=args.file_format
         )
```

### Comparing `thingsvision-2.3.9/thingsvision/utils/data/__init__.py` & `thingsvision-2.4.0/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/utils/data/data_loader.py` & `thingsvision-2.4.0/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/utils/data/dataset.py` & `thingsvision-2.4.0/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/utils/data/helpers.py` & `thingsvision-2.4.0/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.4.0/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision/utils/storing/helpers.py` & `thingsvision-2.4.0/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.3.9/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.4.0/thingsvision.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.3.9
+Version: 2.4.0
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -85,22 +85,23 @@
 
 <!-- Model collection -->
 ### :file_cabinet: Model collection
 Neural networks come from different sources. With `thingsvision`, you can extract image representations of all models from:
 - [torchvision](https://pytorch.org/vision/0.8/models.html)
 - [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications)
 - [timm](https://github.com/rwightman/pytorch-image-models)
-- `ssl` (Self-Supervised Learning Models)
-  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://github.com/facebookresearch/vissl))
-  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50` (retrieved from [torch.hub](https://pytorch.org/hub/))
+- `ssl` (self-supervised learning models)
+  - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`, `rotnet-rn50`, `swav-rn50`, `pirl-rn50`
+  - `barlowtwins-rn50`, `vicreg-rn50`, `dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`, `dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-vit-giant-p14`
 - [OpenCLIP](https://github.com/mlfoundations/open_clip)
 - both original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and `RN50`)
 - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather than ImageNet  and one Alexnet pretrained on ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html)
 - each of the many [CORnet](https://github.com/dicarlolab/CORnet) versions
-- [Harmonization](https://arxiv.org/abs/2211.04533) models from the [official repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. However, the following encoders are additionally available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, `LeViT_small`<br> 
+- [Harmonization](https://arxiv.org/abs/2211.04533) models from the official [Harmonization repo](https://github.com/serre-lab/harmonization). The default variant is `ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.<br> 
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official [DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for more information.
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Getting Started -->
 ## :running: Getting Started
 
@@ -115,17 +116,31 @@
 ```
 
 Then, activate the environment and simply install `thingsvision` via running the following `pip` command in your terminal.
 
 ```bash
 $ pip install --upgrade thingsvision
 $ pip install git+https://github.com/openai/CLIP.git
+```
+
+If you want to extract features for [harmonized models](https://vicco-group.github.io/thingsvision/AvailableModels.html#harmonization) from the [Harmonization repo](https://github.com/serre-lab/harmonization), you have to additionally run the following `pip` command in your `thingsvision` environment (FYI: as of now, this seems to be working smoothly on Ubuntu only but not on macOS),
+
+```bash
 $ pip install git+https://github.com/serre-lab/Harmonization.git
+$ pip install keras-cv-attention-models>=1.3.5
+```
+
+If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
+
+```bash
+$ pip install dreamsim==0.1.2
 ```
 
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Basic usage -->
@@ -145,67 +160,71 @@
 thingsvision extract_features --image-root "./data" --model-name "alexnet" --module-name "features.10" --batch-size 32 --device "cuda" --source "torchvision" --file-format "npy" --out-path "./features"
 ```
 
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a list of all possible arguments. Note that the CLI provides just the basic extraction functionalities but is probably enough for most users that don't want to dive too deep into various models and modules. If you need more fine-grained control over the extraction itself, we recommend to use the python package directly and write your own Python script.
 
 #### Python commands
 
-To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `AlexNet` from the `torchvision` library as the model to extract features from and also load the model to GPU for faster inference,
+To do this start by importing all the necessary components and instantiating a `thingsvision` extractor. Here we're using `CLIP` from the official clip repo as the model to extract features from and also load the model to GPU for faster inference,
 
 ```python
 import torch
 from thingsvision import get_extractor
 from thingsvision.utils.storing import save_features
 from thingsvision.utils.data import ImageDataset, DataLoader
 
-model_name = 'alexnet'
-source = 'torchvision'
+model_name = 'clip'
+source = 'custom'
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
+model_parameters = {
+    'variant': 'ViT-B/32'
+}
 
 extractor = get_extractor(
-    model_name=model_name,
-    source=source,
-    device=device,
-    pretrained=True
+  model_name=model_name,
+  source=source,
+  device=device,
+  pretrained=True,
+  model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
 root='path/to/root/img/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
-    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set input dimensionality to whatever is required for your pretrained model
+    transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
 )
 
 batches = DataLoader(
     dataset=dataset,
     batch_size=batch_size,
     backend=extractor.get_backend() # backend framework of model
 )
 ```
 
-Now all that is left is to extract the image features and store them to disk! Here we're extracting features from the last convolutional layer of AlexNet (`features.10`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all modules.
+Now all that is left is to extract the image features and store them on disk! Here we're extracting features from the image encoder layer (`visual`), but if you don't know which modules are available for a given model, just call `extractor.show_model()` to print all the modules.
 
 ```python
-module_name = 'features.10'
+module_name = 'visual'
 
 features = extractor.extract_features(
     batches=batches,
     module_name=module_name,
-    flatten_acts=True, # flatten 2D feature maps from convolutional layer
-    output_type="ndarray", # or "tensor" (only applicable to PyTorch models)
+    flatten_acts=True,
+    output_type="ndarray", # or "tensor" (only applicable to PyTorch models of which CLIP is one!)
 )
 
-save_features(features, out_path='path/to/features', file_format='npy')
+save_features(features, out_path='path/to/features', file_format='npy') # file_format can be set to "npy", "txt", "mat", "pt", or "hdf5"
 ```
 
 _For more examples on the many models available in `thingsvision` and explanations of additional functionality like how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to easily extract features for the [THINGS image database](https://osf.io/jum2f/), please refer to the [Documentation](https://vicco-group.github.io/thingsvision/)._
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- Contributing -->
@@ -247,15 +266,14 @@
 - [Alex Murphy](https://github.com/Alxmrphi) (software dev.)
 - [Florian Mahner](https://www.cbs.mpg.de/person/mahner/1483114) (software dev.)
 - [Hannes Hansen](https://github.com/hahahannes) (software dev.)
 - [Johannes Roth](https://jroth.space/) (software dev., design, docs)
 - [Jonas Dippel](https://github.com/jonasd4) (software dev.)
 - [Lukas Muttenthaler](https://lukasmut.github.io/) (software dev., design, docs, general responsibility)
 - [Martin N. Hebart](http://martin-hebart.de/) (design)
-- [Oliver Contier](https://olivercontier.com/) (docs)
 - [Philipp Kaniuth](https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs)
 - [Roman Leipe](https://github.com/RLeipe) (sofware dev., docs),
 
 sorted alphabetically. 
 
 This is a joint open-source project between the Max Planck Institute for Human Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at Technische Universtität Berlin. Correspondence and requests for contributing should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if you want to become a contributor or have any suggestions/feedback. For the latter, you could also just post an issue or engange in discussions. We'll try to respond as fast as we can.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.3.9 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.4.0 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -39,46 +39,62 @@
 extraction. - perform Centered Kernel Alignment (CKA) to compare image features
 across model-module combinations.
                                                                   (back_to_top)
  ### :file_cabinet: Model collection Neural networks come from different
 sources. With `thingsvision`, you can extract image representations of all
 models from: - [torchvision](https://pytorch.org/vision/0.8/models.html) -
 [Keras](https://www.tensorflow.org/api_docs/python/tf/keras/applications) -
-[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (Self-
-Supervised Learning Models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
-`rotnet-rn50`, `swav-rn50`, `pirl-rn50` (retrieved from [vissl](https://
-github.com/facebookresearch/vissl)) - `barlowtwins-rn50`, `vicreg-rn50`, `dino-
-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`
-(retrieved from [torch.hub](https://pytorch.org/hub/)) - [OpenCLIP](https://
-github.com/mlfoundations/open_clip) - both original [CLIP](https://github.com/
-openai/CLIP) variants (`ViT-B/32` and `RN50`) - a few custom models (Alexnet,
-VGG-16, Resnet50, and Inception_v3) trained on [Ecoset](https://www.pnas.org/
-doi/10.1073/pnas.2011417118) rather than ImageNet and one Alexnet pretrained on
-ImageNet and fine-tuned on [SalObjSub](https://cs-people.bu.edu/jmzhang/
-sos.html) - each of the many [CORnet](https://github.com/dicarlolab/CORnet)
-versions - [Harmonization](https://arxiv.org/abs/2211.04533) models from the
-[official repo](https://github.com/serre-lab/harmonization). The default
-variant is `ViT_B16`. However, the following encoders are additionally
-available: `ResNet50`, `VGG16`, `EfficientNetB0`, `tiny_ConvNeXT`,
-`tiny_MaxViT`, `LeViT_small`
+[timm](https://github.com/rwightman/pytorch-image-models) - `ssl` (self-
+supervised learning models) - `simclr-rn50`, `mocov2-rn50`, `jigsaw-rn50`,
+`rotnet-rn50`, `swav-rn50`, `pirl-rn50` - `barlowtwins-rn50`, `vicreg-rn50`,
+`dino-vit{s/b}{8/16}`, `dino-xcit-{small/medium}-{12/24}-p{8/16}`, `dino-rn50`,
+`dinov2-vit-small-p14`, `dinov2-vit-base-p14`, `dinov2-vit-large-p14`, `dinov2-
+vit-giant-p14` - [OpenCLIP](https://github.com/mlfoundations/open_clip) - both
+original [CLIP](https://github.com/openai/CLIP) variants (`ViT-B/32` and
+`RN50`) - a few custom models (Alexnet, VGG-16, Resnet50, and Inception_v3)
+trained on [Ecoset](https://www.pnas.org/doi/10.1073/pnas.2011417118) rather
+than ImageNet and one Alexnet pretrained on ImageNet and fine-tuned on
+[SalObjSub](https://cs-people.bu.edu/jmzhang/sos.html) - each of the many
+[CORnet](https://github.com/dicarlolab/CORnet) versions - [Harmonization]
+(https://arxiv.org/abs/2211.04533) models from the official [Harmonization
+repo](https://github.com/serre-lab/harmonization). The default variant is
+`ViT_B16`. Other available models are `ResNet50`, `VGG16`, `EfficientNetB0`,
+`tiny_ConvNeXT`, `tiny_MaxViT`, and `LeViT_small`.
+- [DreamSim](https://dreamsim-nights.github.io/) models from the official
+[DreamSim repo](https://github.com/ssundaram21/dreamsim). The default variant
+is `open_clip_vitb32`. Other available models are `clip_vitb32`. See the [docs]
+(https://vicco-group.github.io/thingsvision/AvailableModels.html) for more
+information.
                                                                   (back_to_top)
  ## :running: Getting Started  ### :computer: Setting up your environment ####
 Working locally. First, create a new `conda environment` with Python version
 3.8, 3.9, or 3.10 e.g. by using `conda`: ```bash $ conda create -n thingsvision
 python=3.9 $ conda activate thingsvision ``` Then, activate the environment and
 simply install `thingsvision` via running the following `pip` command in your
 terminal. ```bash $ pip install --upgrade thingsvision $ pip install git+https:
-//github.com/openai/CLIP.git $ pip install git+https://github.com/serre-lab/
-Harmonization.git ``` #### Google Colab. Alternatively, you can use Google
-Colab to play around with `thingsvision` by uploading your image data to Google
-Drive (via directory mounting). You can find the jupyter notebook using
-`PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/
-thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example
+//github.com/openai/CLIP.git ``` If you want to extract features for
+[harmonized models](https://vicco-group.github.io/thingsvision/
+AvailableModels.html#harmonization) from the [Harmonization repo](https://
+github.com/serre-lab/harmonization), you have to additionally run the following
+`pip` command in your `thingsvision` environment (FYI: as of now, this seems to
+be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
+git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
+attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
+(https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
+github.com/ssundaram21/dreamsim), you have to additionally run the following
+`pip` command in your `thingsvision` environment, ```bash $ pip install
+dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
+AvailableModels.html) for which `DreamSim` models are available in
+`thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
+play around with `thingsvision` by uploading your image data to Google Drive
+(via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
-master/notebooks/tensorflow.ipynb).
+master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
+colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
+notebooks/tensorflow.ipynb).
                                                                   (back_to_top)
  ### :mag: Basic usage #### Command Line Interface (CLI) `thingsvision` was
 designed to simplify feature extraction. If you have some folder of images
 (e.g., `./images`) and want to extract features for each of these images
 without opening a Jupyter Notebook instance or writing a Python script, it's
 probably easiest to use our CLI. The interface includes two options, -
 `thingsvision show-model` - `thingsvision extract-features` Example calls might
@@ -89,45 +105,47 @@
 See `thingsvision show-model -h` and `thingsvision extract-features -h` for a
 list of all possible arguments. Note that the CLI provides just the basic
 extraction functionalities but is probably enough for most users that don't
 want to dive too deep into various models and modules. If you need more fine-
 grained control over the extraction itself, we recommend to use the python
 package directly and write your own Python script. #### Python commands To do
 this start by importing all the necessary components and instantiating a
-`thingsvision` extractor. Here we're using `AlexNet` from the `torchvision`
-library as the model to extract features from and also load the model to GPU
-for faster inference, ```python import torch from thingsvision import
-get_extractor from thingsvision.utils.storing import save_features from
-thingsvision.utils.data import ImageDataset, DataLoader model_name = 'alexnet'
-source = 'torchvision' device = 'cuda' if torch.cuda.is_available() else 'cpu'
-extractor = get_extractor( model_name=model_name, source=source, device=device,
-pretrained=True ) ``` As a next step, create both dataset and dataloader for
-your images. We assume that all of your images are in a single `root` directory
-which can contain subfolders (e.g., for individual classes). Therefore, we
-leverage the `ImageDataset` class. ```python root='path/to/root/img/directory'
-# (e.g., './images/) batch_size = 32 dataset = ImageDataset( root=root,
-out_path='path/to/features', backend=extractor.get_backend(), # backend
-framework of model transforms=extractor.get_transformations(resize_dim=256,
-crop_dim=224) # set input dimensionality to whatever is required for your
-pretrained model ) batches = DataLoader( dataset=dataset,
-batch_size=batch_size, backend=extractor.get_backend() # backend framework of
-model ) ``` Now all that is left is to extract the image features and store
-them to disk! Here we're extracting features from the last convolutional layer
-of AlexNet (`features.10`), but if you don't know which modules are available
-for a given model, just call `extractor.show_model()` to print all modules.
-```python module_name = 'features.10' features = extractor.extract_features
-( batches=batches, module_name=module_name, flatten_acts=True, # flatten 2D
-feature maps from convolutional layer output_type="ndarray", # or "tensor"
-(only applicable to PyTorch models) ) save_features(features, out_path='path/
-to/features', file_format='npy') ``` _For more examples on the many models
-available in `thingsvision` and explanations of additional functionality like
-how to optionally turn off center cropping, how to use HDF5 datasets (e.g. NSD
-stimuli), how to perform RSA or CKA, or how to easily extract features for the
-[THINGS image database](https://osf.io/jum2f/), please refer to the
-[Documentation](https://vicco-group.github.io/thingsvision/)._
+`thingsvision` extractor. Here we're using `CLIP` from the official clip repo
+as the model to extract features from and also load the model to GPU for faster
+inference, ```python import torch from thingsvision import get_extractor from
+thingsvision.utils.storing import save_features from thingsvision.utils.data
+import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
+'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
+'ViT-B/32' } extractor = get_extractor( model_name=model_name, source=source,
+device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
+next step, create both dataset and dataloader for your images. We assume that
+all of your images are in a single `root` directory which can contain
+subfolders (e.g., for individual classes). Therefore, we leverage the
+`ImageDataset` class. ```python root='path/to/root/img/directory' # (e.g., './
+images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/to/
+features', backend=extractor.get_backend(), # backend framework of model
+transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
+the input dimensionality to whichever values are required for your pretrained
+model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
+backend=extractor.get_backend() # backend framework of model ) ``` Now all that
+is left is to extract the image features and store them on disk! Here we're
+extracting features from the image encoder layer (`visual`), but if you don't
+know which modules are available for a given model, just call
+`extractor.show_model()` to print all the modules. ```python module_name =
+'visual' features = extractor.extract_features( batches=batches,
+module_name=module_name, flatten_acts=True, output_type="ndarray", # or
+"tensor" (only applicable to PyTorch models of which CLIP is one!) )
+save_features(features, out_path='path/to/features', file_format='npy') #
+file_format can be set to "npy", "txt", "mat", "pt", or "hdf5" ``` _For more
+examples on the many models available in `thingsvision` and explanations of
+additional functionality like how to optionally turn off center cropping, how
+to use HDF5 datasets (e.g. NSD stimuli), how to perform RSA or CKA, or how to
+easily extract features for the [THINGS image database](https://osf.io/jum2f/),
+please refer to the [Documentation](https://vicco-group.github.io/thingsvision/
+)._
                                                                   (back_to_top)
  ## :wave: How to contribute If you come across problems or have suggestions
 please submit an issue!
                                                                   (back_to_top)
  ## :warning: License This GitHub repository is licensed under the MIT License
 - see the [LICENSE.md](LICENSE.md) file for details.
                                                                   (back_to_top)
@@ -148,19 +166,18 @@
 and refined into its current form with the help of our many contributors, -
 [Alex Murphy](https://github.com/Alxmrphi) (software dev.) - [Florian Mahner]
 (https://www.cbs.mpg.de/person/mahner/1483114) (software dev.) - [Hannes
 Hansen](https://github.com/hahahannes) (software dev.) - [Johannes Roth](https:
 //jroth.space/) (software dev., design, docs) - [Jonas Dippel](https://
 github.com/jonasd4) (software dev.) - [Lukas Muttenthaler](https://
 lukasmut.github.io/) (software dev., design, docs, general responsibility) -
-[Martin N. Hebart](http://martin-hebart.de/) (design) - [Oliver Contier](https:
-//olivercontier.com/) (docs) - [Philipp Kaniuth](https://www.cbs.mpg.de/person/
-kaniuth/1483114) (design, docs) - [Roman Leipe](https://github.com/RLeipe)
-(sofware dev., docs), sorted alphabetically. This is a joint open-source
-project between the Max Planck Institute for Human Cognitive and Brain
-Sciences, Leipzig, and the Machine Learning Group at Technische UniverstitÃ¤t
-Berlin. Correspondence and requests for contributing should be adressed to
-[Lukas Muttenthaler](https://lukasmut.github.io/). Feel free to contact us if
-you want to become a contributor or have any suggestions/feedback. For the
-latter, you could also just post an issue or engange in discussions. We'll try
-to respond as fast as we can.
+[Martin N. Hebart](http://martin-hebart.de/) (design) - [Philipp Kaniuth]
+(https://www.cbs.mpg.de/person/kaniuth/1483114) (design, docs) - [Roman Leipe]
+(https://github.com/RLeipe) (sofware dev., docs), sorted alphabetically. This
+is a joint open-source project between the Max Planck Institute for Human
+Cognitive and Brain Sciences, Leipzig, and the Machine Learning Group at
+Technische UniverstitÃ¤t Berlin. Correspondence and requests for contributing
+should be adressed to [Lukas Muttenthaler](https://lukasmut.github.io/). Feel
+free to contact us if you want to become a contributor or have any suggestions/
+feedback. For the latter, you could also just post an issue or engange in
+discussions. We'll try to respond as fast as we can.
                                                                   (back_to_top)
```

### Comparing `thingsvision-2.3.9/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.4.0/thingsvision.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,31 @@
 thingsvision/core/rsa/__init__.py
 thingsvision/core/rsa/base.py
 thingsvision/core/rsa/helpers.py
 thingsvision/custom_models/__init__.py
 thingsvision/custom_models/alexnet_ecoset.py
 thingsvision/custom_models/alexnet_salobjsub.py
 thingsvision/custom_models/custom.py
-thingsvision/custom_models/harmonization.py
 thingsvision/custom_models/inception_ecoset.py
 thingsvision/custom_models/official_clip.py
 thingsvision/custom_models/openclip.py
 thingsvision/custom_models/resnet50_ecoset.py
 thingsvision/custom_models/vgg16_ecoset.py
 thingsvision/custom_models/vgg16bn_ecoset.py
 thingsvision/custom_models/cornet/__init__.py
 thingsvision/custom_models/cornet/cornet_r.py
 thingsvision/custom_models/cornet/cornet_rt.py
 thingsvision/custom_models/cornet/cornet_s.py
 thingsvision/custom_models/cornet/cornet_z.py
+thingsvision/custom_models/dreamsim/__init__.py
+thingsvision/custom_models/dreamsim/dreamsim.py
+thingsvision/custom_models/harmonization/__init__.py
+thingsvision/custom_models/harmonization/harmonization.py
 thingsvision/utils/__init__.py
+thingsvision/utils/checkpointing/__init__.py
 thingsvision/utils/data/__init__.py
 thingsvision/utils/data/data_loader.py
 thingsvision/utils/data/dataset.py
 thingsvision/utils/data/helpers.py
 thingsvision/utils/imagenet/__init__.py
 thingsvision/utils/storing/__init__.py
 thingsvision/utils/storing/helpers.py
```

