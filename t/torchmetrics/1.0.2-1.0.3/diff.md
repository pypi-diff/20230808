# Comparing `tmp/torchmetrics-1.0.2.tar.gz` & `tmp/torchmetrics-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmetrics-1.0.2.tar", last modified: Thu Aug  3 19:03:59 2023, max compression
+gzip compressed data, was "torchmetrics-1.0.3.tar", last modified: Tue Aug  8 15:44:56 2023, max compression
```

## Comparing `torchmetrics-1.0.2.tar` & `torchmetrics-1.0.3.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.849223 torchmetrics-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    62234 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (122)    11352 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14392 2023-08-03 19:03:59.845223 torchmetrics-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12618 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.805222 torchmetrics-1.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/audio.txt
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/audio_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/classification_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/detection.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/detection_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/doctest.txt
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/image.txt
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/image_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/integrate.txt
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/multimodal.txt
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/nominal_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/text.txt
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/text_test.txt
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/typing.txt
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements/visual.txt
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 19:03:59.849223 torchmetrics-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)    10482 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.801222 torchmetrics-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.809222 torchmetrics-1.0.2/src/torchmetrics/
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27058 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.809222 torchmetrics-1.0.2/src/torchmetrics/audio/
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10354 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (122)    12714 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (122)     7472 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.813222 torchmetrics-1.0.2/src/torchmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22596 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)    24970 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)    24818 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    17014 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (122)    13482 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)    20879 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    12439 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (122)    17879 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    50255 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (122)    13732 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)    23204 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (122)    15294 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (122)    25190 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    44935 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    32436 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    16414 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)    24921 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    28297 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (122)    22772 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (122)    18498 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)    24369 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/classification/stat_scores.py
--rw-r--r--   0 runner    (1001) docker     (122)    29587 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.813222 torchmetrics-1.0.2/src/torchmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    42164 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/_mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13103 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)    34854 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/mean_ap.py
--rw-r--r--   0 runner    (1001) docker     (122)    17517 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.817222 torchmetrics-1.0.2/src/torchmetrics/functional/
--rw-r--r--   0 runner    (1001) docker     (122)     9467 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.817222 torchmetrics-1.0.2/src/torchmetrics/functional/audio/
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/pesq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9865 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/sdr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/snr.py
--rw-r--r--   0 runner    (1001) docker     (122)    14322 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/srmr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/audio/stoi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.821222 torchmetrics-1.0.2/src/torchmetrics/functional/classification/
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (122)    23525 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/auroc.py
--rw-r--r--   0 runner    (1001) docker     (122)    23096 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    16847 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/calibration_error.py
--rw-r--r--   0 runner    (1001) docker     (122)    11532 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)    27915 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/dice.py
--rw-r--r--   0 runner    (1001) docker     (122)    11693 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/exact_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    35591 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/f_beta.py
--rw-r--r--   0 runner    (1001) docker     (122)    16824 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/group_fairness.py
--rw-r--r--   0 runner    (1001) docker     (122)    20600 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/hamming.py
--rw-r--r--   0 runner    (1001) docker     (122)    12281 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/hinge.py
--rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/jaccard.py
--rw-r--r--   0 runner    (1001) docker     (122)    12258 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/matthews_corrcoef.py
--rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_fixed_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    34975 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_recall.py
--rw-r--r--   0 runner    (1001) docker     (122)    44324 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/ranking.py
--rw-r--r--   0 runner    (1001) docker     (122)    21068 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/recall_fixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    26642 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/roc.py
--rw-r--r--   0 runner    (1001) docker     (122)    18437 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/specificity.py
--rw-r--r--   0 runner    (1001) docker     (122)    22172 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/specificity_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (122)    49456 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/classification/stat_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.821222 torchmetrics-1.0.2/src/torchmetrics/functional/detection/
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/_panoptic_quality_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/ciou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/diou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/giou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3038 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)     7903 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/detection/panoptic_qualities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.825222 torchmetrics-1.0.2/src/torchmetrics/functional/image/
--rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9224 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     5675 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (122)     4544 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    15747 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.825222 torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/
--rw-r--r--   0 runner    (1001) docker     (122)     6009 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/alex.pth
--rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/squeeze.pth
--rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/vgg.pth
--rw-r--r--   0 runner    (1001) docker     (122)     5948 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (122)     4322 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (122)    21491 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/image/uqi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.825222 torchmetrics-1.0.2/src/torchmetrics/functional/multimodal/
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.825222 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7377 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     7151 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/nominal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.825222 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/cosine.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/minkowski.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.829222 torchmetrics-1.0.2/src/torchmetrics/functional/regression/
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (122)    15169 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.829222 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.833222 torchmetrics-1.0.2/src/torchmetrics/functional/text/
--rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13993 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    21050 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7573 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (122)    26029 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17557 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (122)    17030 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/helper_embedding_metric.py
--rw-r--r--   0 runner    (1001) docker     (122)    27953 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (122)    22000 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)    13118 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     9892 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (122)    23230 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/functional/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.837222 torchmetrics-1.0.2/src/torchmetrics/image/
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/d_lambda.py
--rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/ergas.py
--rw-r--r--   0 runner    (1001) docker     (122)    18850 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/fid.py
--rw-r--r--   0 runner    (1001) docker     (122)     9056 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/inception.py
--rw-r--r--   0 runner    (1001) docker     (122)    14539 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/kid.py
--rw-r--r--   0 runner    (1001) docker     (122)     8091 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/lpip.py
--rw-r--r--   0 runner    (1001) docker     (122)    13031 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/mifid.py
--rw-r--r--   0 runner    (1001) docker     (122)     8492 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/psnrb.py
--rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/rase.py
--rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/rmse_sw.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/sam.py
--rw-r--r--   0 runner    (1001) docker     (122)    17135 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/ssim.py
--rw-r--r--   0 runner    (1001) docker     (122)     5305 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/tv.py
--rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/image/uqi.py
--rw-r--r--   0 runner    (1001) docker     (122)    51702 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.837222 torchmetrics-1.0.2/src/torchmetrics/multimodal/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/multimodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/multimodal/clip_score.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.837222 torchmetrics-1.0.2/src/torchmetrics/nominal/
--rw-r--r--   0 runner    (1001) docker     (122)      986 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5928 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/cramers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/fleiss_kappa.py
--rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/theils_u.py
--rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/nominal/tschuprows.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.841222 torchmetrics-1.0.2/src/torchmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5312 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/concordance.py
--rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/explained_variance.py
--rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/kendall.py
--rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/kl_divergence.py
--rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/log_cosh.py
--rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/log_mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/mae.py
--rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/minkowski.py
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/mse.py
--rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/pearson.py
--rw-r--r--   0 runner    (1001) docker     (122)     7330 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/r2.py
--rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/rse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/spearman.py
--rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/symmetric_mape.py
--rw-r--r--   0 runner    (1001) docker     (122)     5889 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/tweedie_deviance.py
--rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/regression/wmape.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.841222 torchmetrics-1.0.2/src/torchmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     5938 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/fall_out.py
--rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/ndcg.py
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/precision.py
--rw-r--r--   0 runner    (1001) docker     (122)    16706 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/precision_recall_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/r_precision.py
--rw-r--r--   0 runner    (1001) docker     (122)     5903 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/recall.py
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/retrieval/reciprocal_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.845223 torchmetrics-1.0.2/src/torchmetrics/text/
--rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8249 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)    14023 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/bert.py
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/cer.py
--rw-r--r--   0 runner    (1001) docker     (122)    10472 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/chrf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6357 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/eed.py
--rw-r--r--   0 runner    (1001) docker     (122)    10153 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/infolm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/mer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (122)     9417 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/rouge.py
--rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/sacre_bleu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/squad.py
--rw-r--r--   0 runner    (1001) docker     (122)     6742 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/ter.py
--rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/wer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/wil.py
--rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/text/wip.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.845223 torchmetrics-1.0.2/src/torchmetrics/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34527 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/compute.py
--rw-r--r--   0 runner    (1001) docker     (122)     9412 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    12791 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/utilities/prints.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.845223 torchmetrics-1.0.2/src/torchmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8473 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/bootstrapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     9298 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/classwise.py
--rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/minmax.py
--rw-r--r--   0 runner    (1001) docker     (122)     9093 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/multioutput.py
--rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/multitask.py
--rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/running.py
--rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-08-03 19:03:52.000000 torchmetrics-1.0.2/src/torchmetrics/wrappers/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 19:03:59.809222 torchmetrics-1.0.2/src/torchmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14392 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12389 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-03 19:03:59.000000 torchmetrics-1.0.2/src/torchmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.363269 torchmetrics-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    62802 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (122)    11352 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      919 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14644 2023-08-08 15:44:56.359269 torchmetrics-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12870 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.311268 torchmetrics-1.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/audio.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/audio_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/classification_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/detection.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/detection_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/doctest.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/image.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/image_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/integrate.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/multimodal.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/nominal_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/text.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/text_test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/typing.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements/visual.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 15:44:56.363269 torchmetrics-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10482 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.303268 torchmetrics-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.311268 torchmetrics-1.0.3/src/torchmetrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8581 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27057 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.319269 torchmetrics-1.0.3/src/torchmetrics/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4127 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7054 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6930 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10350 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12742 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7472 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6510 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.323269 torchmetrics-1.0.3/src/torchmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22596 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24970 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24818 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17014 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13482 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22954 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12439 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17879 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50255 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13732 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23204 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15294 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25190 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44935 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32436 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16414 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24921 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28297 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22772 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18498 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24369 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/classification/stat_scores.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29587 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.323269 torchmetrics-1.0.3/src/torchmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42080 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/_mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7848 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7544 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13103 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35940 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/mean_ap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17512 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.323269 torchmetrics-1.0.3/src/torchmetrics/functional/
+-rw-r--r--   0 runner    (1001) docker     (122)     9467 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.327269 torchmetrics-1.0.3/src/torchmetrics/functional/audio/
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4883 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/pesq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9865 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/sdr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5036 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/snr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14322 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/srmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/audio/stoi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.331269 torchmetrics-1.0.3/src/torchmetrics/functional/classification/
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23525 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/auroc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23096 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16847 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/calibration_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11532 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27915 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/dice.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11693 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/exact_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35591 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16824 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/group_fairness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20600 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/hamming.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12281 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/hinge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16533 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/jaccard.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12258 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/matthews_corrcoef.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17938 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_fixed_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34975 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44324 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21068 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/recall_fixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26642 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/roc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18437 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/specificity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22172 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/specificity_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49470 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/classification/stat_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.331269 torchmetrics-1.0.3/src/torchmetrics/functional/detection/
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19764 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/_panoptic_quality_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/ciou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/diou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/giou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7916 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/detection/panoptic_qualities.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.335269 torchmetrics-1.0.3/src/torchmetrics/functional/image/
+-rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9224 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5675 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4544 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2899 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15747 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.335269 torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/
+-rw-r--r--   0 runner    (1001) docker     (122)     6009 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/alex.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    10811 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/squeeze.pth
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/vgg.pth
+-rw-r--r--   0 runner    (1001) docker     (122)     5948 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4527 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5515 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4322 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21491 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6425 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/image/uqi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.335269 torchmetrics-1.0.3/src/torchmetrics/functional/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.335269 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/
+-rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7377 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6924 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7151 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7676 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/nominal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.335269 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3497 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3174 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4028 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/minkowski.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.339269 torchmetrics-1.0.3/src/torchmetrics/functional/regression/
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2877 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3362 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15169 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4395 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2598 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6630 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6093 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.343269 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5408 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4043 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.347269 torchmetrics-1.0.3/src/torchmetrics/functional/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13993 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21050 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7573 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26029 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17557 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17030 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11825 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/helper_embedding_metric.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27953 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5493 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22000 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13118 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9892 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23230 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2975 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3462 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/functional/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.347269 torchmetrics-1.0.3/src/torchmetrics/image/
+-rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8783 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/d_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5822 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/ergas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18845 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9051 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14534 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/kid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8091 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/lpip.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13031 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/mifid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8492 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/psnrb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/rase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/rmse_sw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/sam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17134 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5305 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/tv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/image/uqi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51702 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.347269 torchmetrics-1.0.3/src/torchmetrics/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6649 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/multimodal/clip_score.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.351269 torchmetrics-1.0.3/src/torchmetrics/nominal/
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5928 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/cramers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5700 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/fleiss_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6228 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/theils_u.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5993 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/nominal/tschuprows.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.351269 torchmetrics-1.0.3/src/torchmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5312 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/concordance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5201 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/explained_variance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/kendall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6589 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/kl_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5406 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/log_cosh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4680 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/log_mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/mae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5063 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4574 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/minkowski.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/mse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8352 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/pearson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7330 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/r2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5440 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/rse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/spearman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/symmetric_mape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5889 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/tweedie_deviance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4857 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/regression/wmape.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.355269 torchmetrics-1.0.3/src/torchmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9210 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5938 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7461 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/fall_out.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5937 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/ndcg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16706 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/precision_recall_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/r_precision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5903 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/recall.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/retrieval/reciprocal_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.359269 torchmetrics-1.0.3/src/torchmetrics/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     1712 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8249 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14023 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/bert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5855 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5283 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/cer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10472 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/chrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6357 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/eed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10153 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/infolm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/mer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9417 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6556 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/sacre_bleu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/squad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6742 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/ter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5208 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/wer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/wil.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/text/wip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.359269 torchmetrics-1.0.3/src/torchmetrics/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      889 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34527 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/compute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9412 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12791 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/utilities/prints.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.359269 torchmetrics-1.0.3/src/torchmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8473 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/bootstrapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9298 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6027 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9093 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12082 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/running.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-08-08 15:44:53.000000 torchmetrics-1.0.3/src/torchmetrics/wrappers/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 15:44:56.315268 torchmetrics-1.0.3/src/torchmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14644 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12389 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-08 15:44:56.000000 torchmetrics-1.0.3/src/torchmetrics.egg-info/top_level.txt
```

### Comparing `torchmetrics-1.0.2/CHANGELOG.md` & `torchmetrics-1.0.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **Note: we move fast, but still we preserve 0.1 version (one feature release) back compatibility.**
 
 
+## [1.0.3] - 2023-08-08
+
+### Added
+
+- Added warning to `MeanAveragePrecision` if too many detections are observed ([#1978](https://github.com/Lightning-AI/torchmetrics/pull/1978))
+
+### Fixed
+
+- Fix support for int input for when `multidim_average="samplewise"` in classification metrics  ([#1977](https://github.com/Lightning-AI/torchmetrics/pull/1977))
+- Fixed x/y labels when plotting confusion matrices ([#1976](https://github.com/Lightning-AI/torchmetrics/pull/1976))
+- Fixed IOU compute in cuda ([#1982](https://github.com/Lightning-AI/torchmetrics/pull/1982))
+
+
 ## [1.0.2] - 2023-08-02
 
 ### Added
 
 - Added warning to `PearsonCorrCoeff` if input has a very small variance for its given dtype ([#1926](https://github.com/Lightning-AI/torchmetrics/pull/1926))
 
 ### Changed
```

### Comparing `torchmetrics-1.0.2/CITATION.cff` & `torchmetrics-1.0.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/LICENSE` & `torchmetrics-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/MANIFEST.in` & `torchmetrics-1.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/PKG-INFO` & `torchmetrics-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -37,41 +37,41 @@
 Provides-Extra: visual
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.2/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.3/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/v1.0.2">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v1.0.3">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.2)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.2)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.2/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.3)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.3)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.3/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -255,41 +255,49 @@
 ```
 
 </details>
 
 ### Implementing your own Module metric
 
 Implementing your own metric is as easy as subclassing an [`torch.nn.Module`](https://pytorch.org/docs/stable/generated/torch.nn.Module.html). Simply, subclass `torchmetrics.Metric`
-and implement the following methods:
+and just implement the `update` and `compute` methods:
 
 ```python
 import torch
 from torchmetrics import Metric
 
 
 class MyAccuracy(Metric):
     def __init__(self):
+        # remember to call super
         super().__init__()
         # call `self.add_state`for every internal state that is needed for the metrics computations
         # dist_reduce_fx indicates the function that should be used to reduce
         # state from multiple processes
         self.add_state("correct", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
-    def update(self, preds: torch.Tensor, target: torch.Tensor):
-        # update metric states
-        preds, target = self._input_format(preds, target)
+    def update(self, preds: torch.Tensor, target: torch.Tensor) -> None:
+        # extract predicted class index for computing accuracy
+        preds = preds.argmax(dim=-1)
         assert preds.shape == target.shape
-
+        # update metric states
         self.correct += torch.sum(preds == target)
         self.total += target.numel()
 
-    def compute(self):
+    def compute(self) -> torch.Tensor:
         # compute final result
         return self.correct.float() / self.total
+
+
+my_metric = MyAccuracy()
+preds = torch.randn(10, 5).softmax(dim=-1)
+target = torch.randint(5, (10,))
+
+print(my_metric(preds, target))
 ```
 
 ### Functional metrics
 
 Similar to [`torch.nn`](https://pytorch.org/docs/stable/nn.html), most metrics have both a [module-based](https://torchmetrics.readthedocs.io/en/latest/references/modules.html) and a [functional](https://torchmetrics.readthedocs.io/en/latest/references/functional.html) version.
 The functional versions are simple python functions that as input take [torch.tensors](https://pytorch.org/docs/stable/tensors.html) and return the corresponding metric as a [torch.tensor](https://pytorch.org/docs/stable/tensors.html).
 
@@ -306,15 +314,15 @@
 acc = torchmetrics.functional.classification.multiclass_accuracy(
     preds, target, num_classes=5
 )
 ```
 
 ### Covered domains and example metrics
 
-In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.2all-metrics.html), which
+In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.3all-metrics.html), which
 convers the following domains:
 
 - Audio
 - Classification
 - Detection
 - Information Retrieval
 - Image
@@ -360,15 +368,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.2/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.3/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.0.2/README.md` & `torchmetrics-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -214,41 +214,49 @@
 ```
 
 </details>
 
 ### Implementing your own Module metric
 
 Implementing your own metric is as easy as subclassing an [`torch.nn.Module`](https://pytorch.org/docs/stable/generated/torch.nn.Module.html). Simply, subclass `torchmetrics.Metric`
-and implement the following methods:
+and just implement the `update` and `compute` methods:
 
 ```python
 import torch
 from torchmetrics import Metric
 
 
 class MyAccuracy(Metric):
     def __init__(self):
+        # remember to call super
         super().__init__()
         # call `self.add_state`for every internal state that is needed for the metrics computations
         # dist_reduce_fx indicates the function that should be used to reduce
         # state from multiple processes
         self.add_state("correct", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
-    def update(self, preds: torch.Tensor, target: torch.Tensor):
-        # update metric states
-        preds, target = self._input_format(preds, target)
+    def update(self, preds: torch.Tensor, target: torch.Tensor) -> None:
+        # extract predicted class index for computing accuracy
+        preds = preds.argmax(dim=-1)
         assert preds.shape == target.shape
-
+        # update metric states
         self.correct += torch.sum(preds == target)
         self.total += target.numel()
 
-    def compute(self):
+    def compute(self) -> torch.Tensor:
         # compute final result
         return self.correct.float() / self.total
+
+
+my_metric = MyAccuracy()
+preds = torch.randn(10, 5).softmax(dim=-1)
+target = torch.randint(5, (10,))
+
+print(my_metric(preds, target))
 ```
 
 ### Functional metrics
 
 Similar to [`torch.nn`](https://pytorch.org/docs/stable/nn.html), most metrics have both a [module-based](https://torchmetrics.readthedocs.io/en/latest/references/modules.html) and a [functional](https://torchmetrics.readthedocs.io/en/latest/references/functional.html) version.
 The functional versions are simple python functions that as input take [torch.tensors](https://pytorch.org/docs/stable/tensors.html) and return the corresponding metric as a [torch.tensor](https://pytorch.org/docs/stable/tensors.html).
```

### Comparing `torchmetrics-1.0.2/requirements/audio_test.txt` & `torchmetrics-1.0.3/requirements/audio_test.txt`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/requirements/docs.txt` & `torchmetrics-1.0.3/requirements/docs.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-sphinx >5.0, <6.0
-myst-parser
-nbsphinx >=0.8
-pandoc >=1.0
-docutils >=0.16
+sphinx ==5.3.0
+myst-parser ==1.0.0
+nbsphinx ==0.9.2
+pandoc ==2.3
+docutils ==0.19
 sphinxcontrib-fulltoc >=1.0
 sphinxcontrib-mockautodoc
 pt-lightning-sphinx-theme @ https://github.com/Lightning-AI/lightning_sphinx_theme/archive/master.zip
-sphinx-autodoc-typehints >=1.0
-sphinx-paramlinks >=0.5.1
-sphinx-togglebutton >=0.2
-sphinx-copybutton >=0.3
+sphinx-autodoc-typehints ==1.23.0
+sphinx-paramlinks ==0.5.4
+sphinx-togglebutton ==0.3.2
+sphinx-copybutton ==0.5.2
 
-lightning >=1.8.0, <3.0.0
-lightning-utilities >=0.9.0
-pydantic < 2.0.0
+lightning >=1.8.0, <2.1.0
+lightning-utilities >=0.9.0, <0.10.0
+pydantic >1.0.0, < 2.0.0
 
 # integrations
 -r integrate.txt
 -r visual.txt
 -r audio.txt
 -r detection.txt
 -r image.txt
```

### Comparing `torchmetrics-1.0.2/setup.py` & `torchmetrics-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/__about__.py` & `torchmetrics-1.0.3/src/torchmetrics/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __author__ = "Lightning-AI et al."
 __author_email__ = "name@pytorchlightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2020-2023, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/torchmetrics"
 __docs__ = "PyTorch native Metrics"
 __docs_url__ = "https://torchmetrics.readthedocs.io/en/stable/"
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/aggregation.py` & `torchmetrics-1.0.3/src/torchmetrics/aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,15 @@
     ) -> None:
         super().__init__(base_metric=MeanMetric(nan_strategy=nan_strategy, **kwargs), window=window)
 
 
 class RunningSum(Running):
     """Aggregate a stream of value into their sum over a running window.
 
-    Using this metric compared to `MeanMetric` allows for calculating metrics over a running window of values, instead
+    Using this metric compared to `SumMetric` allows for calculating metrics over a running window of values, instead
     of the whole history of values. This is beneficial when you want to get a better estimate of the metric during
     training and don't want to wait for the whole training to finish to get epoch level estimates.
 
     As input to ``forward`` and ``update`` the metric accepts the following input
 
     - ``value`` (:class:`~float` or :class:`~torch.Tensor`): a single float or an tensor of float values with
       arbitary shape ``(...,)``.
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/pesq.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/pit.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/sdr.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/sdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,19 +164,19 @@
     """`Scale-invariant signal-to-distortion ratio`_ (SI-SDR).
 
     The SI-SDR value is in general considered an overall measure of how good a source sound.
 
     As input to `forward` and `update` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): float tensor with shape ``(...,time)``
-    - ``target`` (: :class:`~torch.Tensor`): float tensor with shape ``(...,time)``
+    - ``target`` (:class:`~torch.Tensor`): float tensor with shape ``(...,time)``
 
     As output of `forward` and `compute` the metric returns the following output
 
-    - ``si_sdr`` (: :class:`~torch.Tensor`): float scalar tensor with average SI-SDR value over samples
+    - ``si_sdr`` (:class:`~torch.Tensor`): float scalar tensor with average SI-SDR value over samples
 
     Args:
         zero_mean: if to zero mean target and preds or not
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Raises:
         TypeError:
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/snr.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/snr.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,19 +141,19 @@
 
 class ScaleInvariantSignalNoiseRatio(Metric):
     """Calculate `Scale-invariant signal-to-noise ratio`_ (SI-SNR) metric for evaluating quality of audio.
 
     As input to `forward` and `update` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): float tensor with shape ``(...,time)``
-    - ``target`` (: :class:`~torch.Tensor`): float tensor with shape ``(...,time)``
+    - ``target`` (:class:`~torch.Tensor`): float tensor with shape ``(...,time)``
 
     As output of `forward` and `compute` the metric returns the following output
 
-    - ``si_snr`` (: :class:`~torch.Tensor`): float scalar tensor with average SI-SNR value over samples
+    - ``si_snr`` (:class:`~torch.Tensor`): float scalar tensor with average SI-SNR value over samples
 
     Args:
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Raises:
         TypeError:
             if target and preds have a different shape
@@ -237,23 +237,23 @@
 
 
 class ComplexScaleInvariantSignalNoiseRatio(Metric):
     """Calculate `Complex scale-invariant signal-to-noise ratio`_ (C-SI-SNR) metric for evaluating quality of audio.
 
     As input to `forward` and `update` the metric accepts the following input
 
-    - ``preds`` (:class:`~torch.Tensor`): real/complex float tensor with shape ``(..., frequency, time, 2)``\
-        / ``(..., frequency, time)``
+    - ``preds`` (:class:`~torch.Tensor`): real float tensor with shape ``(...,frequency,time,2)`` or complex float
+      tensor with shape ``(..., frequency,time)``
 
-    - ``target`` (: :class:`~torch.Tensor`): real/complex float tensor with shape ``(..., frequency, time, 2)``\
-        / ``(..., frequency, time)``
+    - ``target`` (:class:`~torch.Tensor`): real float tensor with shape ``(...,frequency,time,2)`` or complex float
+      tensor with shape ``(..., frequency,time)``
 
     As output of `forward` and `compute` the metric returns the following output
 
-    - ``c_si_snr`` (: :class:`~torch.Tensor`): float scalar tensor with average C-SI-SNR value over samples
+    - ``c_si_snr`` (:class:`~torch.Tensor`): float scalar tensor with average C-SI-SNR value over samples
 
     Args:
         zero_mean: if to zero mean target and preds or not
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Raises:
         ValueError:
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/srmr.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/audio/stoi.py` & `torchmetrics-1.0.3/src/torchmetrics/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/accuracy.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/auroc.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/average_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/base.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/calibration_error.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/cohen_kappa.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/confusion_matrix.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/confusion_matrix.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,25 @@
         "MultilabelConfusionMatrix.plot",
     ]
 
 
 class BinaryConfusionMatrix(Metric):
     r"""Compute the `confusion matrix`_ for binary tasks.
 
+    The confusion matrix :math:`C` is constructed such that :math:`C_{i, j}` is equal to the number of observations
+    known to be in class :math:`i` but predicted to be in class :math:`j`. Thus row indices of the confusion matrix
+    correspond to the true class labels and column indices correspond to the predicted class labels.
+
+    For binary tasks, the confusion matrix is a 2x2 matrix with the following structure:
+
+    - :math:`C_{0, 0}`: True negatives
+    - :math:`C_{0, 1}`: False positives
+    - :math:`C_{1, 0}`: False negatives
+    - :math:`C_{1, 1}`: True positives
+
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~torch.Tensor`): An int or float tensor of shape ``(N, ...)``. If preds is a floating point
       tensor with values outside [0,1] range we consider the input to be logits and will auto apply sigmoid per
       element. Addtionally, we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (:class:`~torch.Tensor`): An int tensor of shape ``(N, ...)``.
 
@@ -168,14 +179,25 @@
         fig, ax = plot_confusion_matrix(val, ax=ax, add_text=add_text, labels=labels)
         return fig, ax
 
 
 class MulticlassConfusionMatrix(Metric):
     r"""Compute the `confusion matrix`_ for multiclass tasks.
 
+    The confusion matrix :math:`C` is constructed such that :math:`C_{i, j}` is equal to the number of observations
+    known to be in class :math:`i` but predicted to be in class :math:`j`. Thus row indices of the confusion matrix
+    correspond to the true class labels and column indices correspond to the predicted class labels.
+
+    For multiclass tasks, the confusion matrix is a NxN matrix, where:
+
+    - :math:`C_{i, i}` represents the number of true positives for class :math:`i`
+    - :math:`\sum_{j=1, j\neq i}^N C_{i, j}` represents the number of false negatives for class :math:`i`
+    - :math:`\sum_{i=1, i\neq j}^N C_{i, j}` represents the number of false positives for class :math:`i`
+    - the sum of the remaining cells in the matrix represents the number of true negatives for class :math:`i`
+
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~torch.Tensor`): An int or float tensor of shape ``(N, ...)``. If preds is a floating point
       tensor with values outside [0,1] range we consider the input to be logits and will auto apply sigmoid per
       element. Addtionally, we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (:class:`~torch.Tensor`): An int tensor of shape ``(N, ...)``.
 
@@ -293,14 +315,26 @@
         fig, ax = plot_confusion_matrix(val, ax=ax, add_text=add_text, labels=labels)
         return fig, ax
 
 
 class MultilabelConfusionMatrix(Metric):
     r"""Compute the `confusion matrix`_ for multilabel tasks.
 
+    The confusion matrix :math:`C` is constructed such that :math:`C_{i, j}` is equal to the number of observations
+    known to be in class :math:`i` but predicted to be in class :math:`j`. Thus row indices of the confusion matrix
+    correspond to the true class labels and column indices correspond to the predicted class labels.
+
+    For multilabel tasks, the confusion matrix is a Nx2x2 tensor, where each 2x2 matrix corresponds to the confusion
+    for that label. The structure of each 2x2 matrix is as follows:
+
+    - :math:`C_{0, 0}`: True negatives
+    - :math:`C_{0, 1}`: False positives
+    - :math:`C_{1, 0}`: False negatives
+    - :math:`C_{1, 1}`: True positives
+
     As input to 'update' the metric accepts the following input:
 
     - ``preds`` (int or float tensor): ``(N, C, ...)``. If preds is a floating point tensor with values outside
       [0,1] range we consider the input to be logits and will auto apply sigmoid per element. Addtionally,
       we convert to int tensor with thresholding using the value in ``threshold``.
     - ``target`` (int tensor): ``(N, C, ...)``
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/dice.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/exact_match.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/f_beta.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/f_beta.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/group_fairness.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/hamming.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/hinge.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/jaccard.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/matthews_corrcoef.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/precision_fixed_recall.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/precision_recall.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/precision_recall_curve.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/ranking.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/recall_fixed_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/roc.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/specificity.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/specificity_sensitivity.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/classification/stat_scores.py` & `torchmetrics-1.0.3/src/torchmetrics/classification/stat_scores.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/collections.py` & `torchmetrics-1.0.3/src/torchmetrics/collections.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/_mean_ap.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/_mean_ap.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,17 +206,16 @@
 
     .. note::
         ``map`` score is calculated with @[ IoU=self.iou_thresholds | area=all | max_dets=max_detection_thresholds ].
         Caution: If the initialization parameters are changed, dictionary keys for mAR can change as well.
         The default properties are also accessible via fields and will raise an ``AttributeError`` if not available.
 
     .. note::
-        This metric is following the mAP implementation of
-        `pycocotools <https://github.com/cocodataset/cocoapi/tree/master/PythonAPI/pycocotools>`_,
-        a standard implementation for the mAP metric for object detection.
+        This metric is following the mAP implementation of `pycocotools`_ a standard implementation for the mAP metric
+        for object detection.
 
     .. note::
         This metric requires you to have `torchvision` version 0.8.0 or newer installed
         (with corresponding version 1.7.0 of torch or newer). This metric requires `pycocotools`
         installed when iou_type is `segm`. Please install with ``pip install torchvision`` or
         ``pip install torchmetrics[detection]``.
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/ciou.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/ciou.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 if not _TORCHVISION_GREATER_EQUAL_0_13:
     __doctest_skip__ = ["CompleteIntersectionOverUnion", "CompleteIntersectionOverUnion.plot"]
 elif not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["CompleteIntersectionOverUnion.plot"]
 
 
 class CompleteIntersectionOverUnion(IntersectionOverUnion):
-    r"""Computes Complete Intersection Over Union (CIoU) <https://arxiv.org/abs/2005.03572>`_.
+    r"""Computes Complete Intersection Over Union (`CIoU`_).
 
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~List`): A list consisting of dictionaries each containing the key-values
       (each dictionary corresponds to a single image). Parameters that should be provided per dict:
 
         - boxes: (:class:`~torch.FloatTensor`) of shape ``(num_boxes, 4)`` containing ``num_boxes`` detection
@@ -51,15 +51,15 @@
           classes for the boxes.
 
     As output of ``forward`` and ``compute`` the metric returns the following output:
 
     - ``ciou_dict``: A dictionary containing the following key-values:
 
         - ciou: (:class:`~torch.Tensor`)
-        - ciou/cl_{cl}: (:class:`~torch.Tensor`), if argument ``class metrics=True``
+        - ciou/cl_{cl}: (:class:`~torch.Tensor`), if argument ``class_metrics=True``
 
     Args:
         box_format:
             Input format of given boxes. Supported formats are ``[`xyxy`, `xywh`, `cxcywh`]``.
         iou_thresholds:
             Optional IoU thresholds for evaluation. If set to `None` the threshold is ignored.
         class_metrics:
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/diou.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/diou.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 if not _TORCHVISION_GREATER_EQUAL_0_13:
     __doctest_skip__ = ["DistanceIntersectionOverUnion", "DistanceIntersectionOverUnion.plot"]
 elif not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["DistanceIntersectionOverUnion.plot"]
 
 
 class DistanceIntersectionOverUnion(IntersectionOverUnion):
-    r"""Computes Distance Intersection Over Union (DIoU) <https://arxiv.org/abs/1911.08287v1>`_.
+    r"""Computes Distance Intersection Over Union (`DIoU`_).
 
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~List`): A list consisting of dictionaries each containing the key-values
       (each dictionary corresponds to a single image). Parameters that should be provided per dict
 
         - boxes: (:class:`~torch.FloatTensor`) of shape ``(num_boxes, 4)`` containing ``num_boxes`` detection
@@ -51,15 +51,15 @@
           classes for the boxes.
 
     As output of ``forward`` and ``compute`` the metric returns the following output:
 
     - ``diou_dict``: A dictionary containing the following key-values:
 
         - diou: (:class:`~torch.Tensor`)
-        - diou/cl_{cl}: (:class:`~torch.Tensor`), if argument ``class metrics=True``
+        - diou/cl_{cl}: (:class:`~torch.Tensor`), if argument ``class_metrics=True``
 
     Args:
         box_format:
             Input format of given boxes. Supported formats are ``['xyxy', 'xywh', 'cxcywh']``.
         iou_thresholds:
             Optional IoU thresholds for evaluation. If set to `None` the threshold is ignored.
         class_metrics:
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/giou.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/giou.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 if not _TORCHVISION_GREATER_EQUAL_0_8:
     __doctest_skip__ = ["GeneralizedIntersectionOverUnion", "GeneralizedIntersectionOverUnion.plot"]
 elif not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["GeneralizedIntersectionOverUnion.plot"]
 
 
 class GeneralizedIntersectionOverUnion(IntersectionOverUnion):
-    r"""Compute Generalized Intersection Over Union (GIoU) <https://arxiv.org/abs/1902.09630>`_.
+    r"""Compute Generalized Intersection Over Union (`GIoU`_).
 
     As input to ``forward`` and ``update`` the metric accepts the following input:
 
     - ``preds`` (:class:`~List`): A list consisting of dictionaries each containing the key-values
       (each dictionary corresponds to a single image). Parameters that should be provided per dict
 
         - boxes: (:class:`~torch.FloatTensor`) of shape ``(num_boxes, 4)`` containing ``num_boxes`` detection
@@ -86,14 +86,15 @@
         >>> metric = GeneralizedIntersectionOverUnion()
         >>> metric(preds, target)
         {'giou': tensor(-0.0694)}
 
     Raises:
         ModuleNotFoundError:
             If torchvision is not installed with version 0.8.0 or newer.
+
     """
     _iou_type: str = "giou"
     _invalid_val: float = -1.0
 
     def __init__(
         self,
         box_format: str = "xyxy",
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/helpers.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/iou.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/iou.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/mean_ap.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/mean_ap.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import torch
 from torch import Tensor
 from torch import distributed as dist
 from typing_extensions import Literal
 
 from torchmetrics.detection.helpers import _fix_empty_tensors, _input_validator
 from torchmetrics.metric import Metric
+from torchmetrics.utilities import rank_zero_warn
 from torchmetrics.utilities.imports import (
     _MATPLOTLIB_AVAILABLE,
     _PYCOCOTOOLS_AVAILABLE,
     _TORCHVISION_GREATER_EQUAL_0_8,
 )
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
@@ -234,14 +235,16 @@
     detection_scores: List[Tensor]
     detection_labels: List[Tensor]
     groundtruths: List[Tensor]
     groundtruth_labels: List[Tensor]
     groundtruth_crowds: List[Tensor]
     groundtruth_area: List[Tensor]
 
+    warn_on_many_detections: bool = True
+
     def __init__(
         self,
         box_format: Literal["xyxy", "xywh", "cxcywh"] = "xyxy",
         iou_type: Literal["bbox", "segm"] = "bbox",
         iou_thresholds: Optional[List[float]] = None,
         rec_thresholds: Optional[List[float]] = None,
         max_detection_thresholds: Optional[List[int]] = None,
@@ -323,15 +326,15 @@
                 If any class is not type int and of length 1
             ValueError:
                 If any score is not type float and of length 1
         """
         _input_validator(preds, target, iou_type=self.iou_type)
 
         for item in preds:
-            detections = self._get_safe_item_values(item)
+            detections = self._get_safe_item_values(item, warn=self.warn_on_many_detections)
 
             self.detections.append(detections)
             self.detection_labels.append(item["labels"])
             self.detection_scores.append(item["scores"])
 
         for item in target:
             groundtruths = self._get_safe_item_values(item)
@@ -536,34 +539,39 @@
 
         with open(f"{name}_preds.json", "w") as f:
             f.write(preds_json)
 
         with open(f"{name}_target.json", "w") as f:
             f.write(target_json)
 
-    def _get_safe_item_values(self, item: Dict[str, Any]) -> Union[Tensor, Tuple]:
+    def _get_safe_item_values(self, item: Dict[str, Any], warn: bool = False) -> Union[Tensor, Tuple]:
         """Convert and return the boxes or masks from the item depending on the iou_type.
 
         Args:
             item: input dictionary containing the boxes or masks
+            warn: whether to warn if the number of boxes or masks exceeds the max_detection_thresholds
 
         Returns:
             boxes or masks depending on the iou_type
 
         """
         if self.iou_type == "bbox":
             boxes = _fix_empty_tensors(item["boxes"])
             if boxes.numel() > 0:
                 boxes = box_convert(boxes, in_fmt=self.box_format, out_fmt="xywh")
+            if warn and len(boxes) > self.max_detection_thresholds[-1]:
+                _warning_on_too_many_detections(self.max_detection_thresholds[-1])
             return boxes
         if self.iou_type == "segm":
             masks = []
             for i in item["masks"].cpu().numpy():
                 rle = mask_utils.encode(np.asfortranarray(i))
                 masks.append((tuple(rle["size"]), rle["counts"]))
+            if warn and len(masks) > self.max_detection_thresholds[-1]:
+                _warning_on_too_many_detections(self.max_detection_thresholds[-1])
             return tuple(masks)
         raise Exception(f"IOU type {self.iou_type} is not supported")
 
     def _get_classes(self) -> List:
         """Return a list of unique classes found in ground truth and detection data."""
         if len(self.detection_labels) > 0 or len(self.groundtruth_labels) > 0:
             return torch.cat(self.detection_labels + self.groundtruth_labels).unique().cpu().tolist()
@@ -737,7 +745,17 @@
         world_size = dist.get_world_size(group=process_group)
         dist.barrier(group=process_group)
 
         list_gathered = [None for _ in range(world_size)]
         dist.all_gather_object(list_gathered, list_to_gather, group=process_group)
 
         return [list_gathered[rank][idx] for idx in range(len(list_gathered[0])) for rank in range(world_size)]
+
+
+def _warning_on_too_many_detections(limit: int) -> None:
+    rank_zero_warn(
+        f"Encountered more than {limit} detections in a single image. This means that certain detections with the"
+        " lowest scores will be ignored, that may have an undesirable impact on performance. Please consider adjusting"
+        " the `max_detection_threshold` to suit your use case. To disable this warning, set attribute class"
+        " `warn_on_many_detections=False`, after initializing the metric.",
+        UserWarning,
+    )
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/detection/panoptic_qualities.py` & `torchmetrics-1.0.3/src/torchmetrics/detection/panoptic_qualities.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["PanopticQuality.plot", "ModifiedPanopticQuality.plot"]
 
 
 class PanopticQuality(Metric):
     r"""Compute the `Panoptic Quality`_ for panoptic segmentations.
 
-        .. math::
-            PQ = \frac{IOU}{TP + 0.5 FP + 0.5 FN}
+    .. math::
+        PQ = \frac{IOU}{TP + 0.5 FP + 0.5 FN}
 
-        where IOU, TP, FP and FN are respectively the sum of the intersection over union for true positives,
-        the number of true postitives, false positives and false negatives. This metric is inspired by the PQ
-        implementation of panopticapi, a standard implementation for the PQ metric for panoptic segmentation.
+    where IOU, TP, FP and FN are respectively the sum of the intersection over union for true positives,
+    the number of true postitives, false positives and false negatives. This metric is inspired by the PQ
+    implementation of panopticapi, a standard implementation for the PQ metric for panoptic segmentation.
 
     .. note:
         Points in the target tensor that do not map to a known category ID are automatically ignored in the metric
         computation.
 
     Args:
         things:
@@ -220,16 +220,16 @@
 
     The metric was introduced in `Seamless Scene Segmentation paper`_, and is an adaptation of the original
     `Panoptic Quality`_ where the metric for a stuff class is computed as
 
     .. math::
         PQ^{\dagger}_c = \frac{IOU_c}{|S_c|}
 
-    where IOU_c is the sum of the intersection over union of all matching segments for a given class, and \|S_c| is
-    the overall number of segments in the ground truth for that class.
+    where :math:`IOU_c` is the sum of the intersection over union of all matching segments for a given class, and
+    :math:`|S_c|` is the overall number of segments in the ground truth for that class.
 
     .. note:
         Points in the target tensor that do not map to a known category ID are automatically ignored in the metric
         computation.
 
     Args:
         things:
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/pesq.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/pesq.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/pit.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/pit.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/sdr.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/sdr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/snr.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/snr.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,24 +85,26 @@
     return scale_invariant_signal_distortion_ratio(preds=preds, target=target, zero_mean=True)
 
 
 def complex_scale_invariant_signal_noise_ratio(preds: Tensor, target: Tensor, zero_mean: bool = False) -> Tensor:
     """`Complex scale-invariant signal-to-noise ratio`_ (C-SI-SNR).
 
     Args:
-        preds: real/complex float tensor with shape ``(..., frequency, time, 2)``/``(..., frequency, time)``
-        target: real/complex float tensor with shape ``(..., frequency, time, 2)``/``(..., frequency, time)``
+        preds: real float tensor with shape ``(...,frequency,time,2)`` or complex float tensor with
+            shape ``(..., frequency,time)``
+        target: real float tensor with shape ``(...,frequency,time,2)`` or complex float tensor with
+            shape ``(..., frequency,time)``
         zero_mean: When set to True, the mean of all signals is subtracted prior to computation of the metrics
 
     Returns:
          Float tensor with shape ``(...,)`` of C-SI-SNR values per sample
 
     Raises:
         RuntimeError:
-            If ``preds`` is not the shape (..., frequency, time, 2) (after being converted to real if it is complex).
+            If ``preds`` is not the shape (...,frequency,time,2) (after being converted to real if it is complex).
             If ``preds`` and ``target`` does not have the same shape.
 
     Example:
         >>> import torch
         >>> from torchmetrics.functional.audio import complex_scale_invariant_signal_noise_ratio
         >>> g = torch.manual_seed(1)
         >>> preds = torch.randn((1,257,100,2))
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/srmr.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/srmr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/audio/stoi.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/audio/stoi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/accuracy.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/auroc.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/auroc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/average_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/calibration_error.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/calibration_error.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/cohen_kappa.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/confusion_matrix.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/dice.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/dice.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/exact_match.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/exact_match.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/f_beta.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/f_beta.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/group_fairness.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/group_fairness.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/hamming.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/hamming.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/hinge.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/hinge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/jaccard.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/jaccard.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/matthews_corrcoef.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/matthews_corrcoef.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_fixed_recall.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_fixed_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_recall.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/precision_recall_curve.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/ranking.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/ranking.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/recall_fixed_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/recall_fixed_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/roc.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/roc.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/specificity.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/specificity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/specificity_sensitivity.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/specificity_sensitivity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/classification/stat_scores.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/classification/stat_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,18 +362,18 @@
             idx = idx.unsqueeze(1).repeat(1, num_classes, 1) if preds.ndim > target.ndim else idx
             preds[idx] = num_classes
 
         if top_k > 1:
             preds_oh = torch.movedim(select_topk(preds, topk=top_k, dim=1), 1, -1)
         else:
             preds_oh = torch.nn.functional.one_hot(
-                preds, num_classes + 1 if ignore_index is not None and not ignore_in else num_classes
+                preds.long(), num_classes + 1 if ignore_index is not None and not ignore_in else num_classes
             )
         target_oh = torch.nn.functional.one_hot(
-            target, num_classes + 1 if ignore_index is not None and not ignore_in else num_classes
+            target.long(), num_classes + 1 if ignore_index is not None and not ignore_in else num_classes
         )
         if ignore_index is not None:
             if 0 <= ignore_index <= num_classes - 1:
                 target_oh[target == ignore_index, :] = -1
             else:
                 preds_oh = preds_oh[..., :-1] if top_k == 1 else preds_oh
                 target_oh = target_oh[..., :-1]
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/_panoptic_quality_common.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/_panoptic_quality_common.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/ciou.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/ciou.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def complete_intersection_over_union(
     preds: torch.Tensor,
     target: torch.Tensor,
     iou_threshold: Optional[float] = None,
     replacement_val: float = 0,
     aggregate: bool = True,
 ) -> torch.Tensor:
-    r"""Compute `Complete Intersection over Union <https://arxiv.org/abs/2005.03572>`_ between two sets of boxes.
+    r"""Compute Complete Intersection over Union (`CIOU`_) between two sets of boxes.
 
     Both sets of boxes are expected to be in (x1, y1, x2, y2) format with 0 <= x1 < x2 and 0 <= y1 < y2.
 
     Args:
         preds:
             The input tensor containing the predicted bounding boxes.
         target:
@@ -67,14 +67,15 @@
     Example:
         >>> import torch
         >>> from torchmetrics.functional.detection import complete_intersection_over_union
         >>> preds = torch.Tensor([[100, 100, 200, 200]])
         >>> target = torch.Tensor([[110, 110, 210, 210]])
         >>> complete_intersection_over_union(preds, target)
         tensor(0.6724)
+
     """
     if not _TORCHVISION_GREATER_EQUAL_0_13:
         raise ModuleNotFoundError(
             f"`{complete_intersection_over_union.__name__}` requires that `torchvision` version 0.13.0 or newer"
             " is installed."
             " Please install with `pip install torchvision>=0.13` or `pip install torchmetrics[detection]`."
         )
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/diou.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/diou.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def distance_intersection_over_union(
     preds: torch.Tensor,
     target: torch.Tensor,
     iou_threshold: Optional[float] = None,
     replacement_val: float = 0,
     aggregate: bool = True,
 ) -> torch.Tensor:
-    r"""Compute `Distance Intersection over Union <https://arxiv.org/abs/1911.08287v1>`_ between two sets of boxes.
+    r"""Compute Distance Intersection over Union (`DIOU`_) between two sets of boxes.
 
     Both sets of boxes are expected to be in (x1, y1, x2, y2) format with 0 <= x1 < x2 and 0 <= y1 < y2.
 
     Args:
         preds:
             The input tensor containing the predicted bounding boxes.
         target:
@@ -67,14 +67,15 @@
     Example:
         >>> import torch
         >>> from torchmetrics.functional.detection import distance_intersection_over_union
         >>> preds = torch.Tensor([[100, 100, 200, 200]])
         >>> target = torch.Tensor([[110, 110, 210, 210]])
         >>> distance_intersection_over_union(preds, target)
         tensor(0.6724)
+
     """
     if not _TORCHVISION_GREATER_EQUAL_0_13:
         raise ModuleNotFoundError(
             f"`{distance_intersection_over_union.__name__}` requires that `torchvision` version 0.13.0 or newer"
             " is installed."
             " Please install with `pip install torchvision>=0.13` or `pip install torchmetrics[detection]`."
         )
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/giou.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/giou.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def generalized_intersection_over_union(
     preds: torch.Tensor,
     target: torch.Tensor,
     iou_threshold: Optional[float] = None,
     replacement_val: float = 0,
     aggregate: bool = True,
 ) -> torch.Tensor:
-    r"""Compute `Generalized Intersection over Union <https://arxiv.org/abs/1902.09630>`_ between two sets of boxes.
+    r"""Compute Generalized Intersection over Union (`GIOU`_) between two sets of boxes.
 
     Both sets of boxes are expected to be in (x1, y1, x2, y2) format with 0 <= x1 < x2 and 0 <= y1 < y2.
 
     Args:
         preds:
             The input tensor containing the predicted bounding boxes.
         target:
@@ -67,14 +67,15 @@
     Example:
         >>> import torch
         >>> from torchmetrics.functional.detection import generalized_intersection_over_union
         >>> preds = torch.Tensor([[100, 100, 200, 200]])
         >>> target = torch.Tensor([[110, 110, 210, 210]])
         >>> generalized_intersection_over_union(preds, target)
         tensor(0.6641)
+
     """
     if not _TORCHVISION_GREATER_EQUAL_0_8:
         raise ModuleNotFoundError(
             f"`{generalized_intersection_over_union.__name__}` requires that `torchvision` version 0.8.0 or newer"
             " is installed."
             " Please install with `pip install torchvision>=0.8` or `pip install torchmetrics[detection]`."
         )
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/iou.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/iou.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         iou[iou < iou_threshold] = replacement_val
     return iou
 
 
 def _iou_compute(iou: torch.Tensor, labels_eq: bool = True) -> torch.Tensor:
     if labels_eq:
         return iou.diag().mean()
-    return iou.mean() if iou.numel() > 0 else torch.tensor(0.0)
+    return iou.mean() if iou.numel() > 0 else torch.tensor(0.0).to(iou.device)
 
 
 def intersection_over_union(
     preds: torch.Tensor,
     target: torch.Tensor,
     iou_threshold: Optional[float] = None,
     replacement_val: float = 0,
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/detection/panoptic_qualities.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/detection/panoptic_qualities.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     .. math::
         PQ = \frac{IOU}{TP + 0.5 FP + 0.5 FN}
 
     where IOU, TP, FP and FN are respectively the sum of the intersection over union for true positives, the number of
     true postitives, false positives and false negatives. This metric is inspired by the PQ implementation of
     panopticapi, a standard implementation for the PQ metric for object detection.
 
-
     .. note:
         Points in the target tensor that do not map to a known category ID are automatically ignored in the metric
         computation.
 
     Args:
         preds:
             torch tensor with panoptic detection of shape [height, width, 2] containing the pair
@@ -116,16 +115,16 @@
 
     The metric was introduced in `Seamless Scene Segmentation paper`_, and is an adaptation of the original
     `Panoptic Quality`_ where the metric for a stuff class is computed as
 
     .. math::
         PQ^{\dagger}_c = \frac{IOU_c}{|S_c|}
 
-    where IOU_c is the sum of the intersection over union of all matching segments for a given class, and \|S_c| is
-    the overall number of segments in the ground truth for that class.
+    where :math:`IOU_c` is the sum of the intersection over union of all matching segments for a given class, and
+    :math:`|S_c|` is the overall number of segments in the ground truth for that class.
 
     .. note:
         Points in the target tensor that do not map to a known category ID are automatically ignored in the metric
         computation.
 
     Args:
         preds:
@@ -147,15 +146,15 @@
         ValueError:
             If ``things``, ``stuffs`` have at least one common ``category_id``.
         TypeError:
             If ``things``, ``stuffs`` contain non-integer ``category_id``.
         TypeError:
             If ``preds`` or ``target`` is not an ``torch.Tensor``.
         ValueError:
-             If ``preds`` or ``target`` has different shape.
+            If ``preds`` or ``target`` has different shape.
         ValueError:
             If ``preds`` has less than 3 dimensions.
         ValueError:
             If the final dimension of ``preds`` has size != 2.
 
     Example:
         >>> from torch import tensor
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/d_lambda.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/ergas.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/gradients.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/gradients.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/helper.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/alex.pth` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/alex.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/squeeze.pth` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/squeeze.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/lpips_models/vgg.pth` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/lpips_models/vgg.pth`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/psnr.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/psnrb.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/rase.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/rmse_sw.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/sam.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/ssim.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/ssim.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/tv.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/image/uqi.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/multimodal/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/multimodal/clip_score.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/cramers.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/fleiss_kappa.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/pearson.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/theils_u.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/tschuprows.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/nominal/utils.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/nominal/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/cosine.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/cosine.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/euclidean.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/euclidean.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/helpers.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/helpers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/linear.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/linear.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/manhattan.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/manhattan.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/pairwise/minkowski.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/pairwise/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/concordance.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/cosine_similarity.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/explained_variance.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/kendall.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/kendall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/kl_divergence.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/log_cosh.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/log_mse.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/mae.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/mape.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/minkowski.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/minkowski.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/mse.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/pearson.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/r2.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/rse.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/rse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/spearman.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/symmetric_mape.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/tweedie_deviance.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/utils.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/utils.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/regression/wmape.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/average_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/fall_out.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/hit_rate.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/ndcg.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/precision.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/precision_recall_curve.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/r_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/recall.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/retrieval/reciprocal_rank.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/bert.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/bleu.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/cer.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/chrf.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/eed.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/helper.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/helper.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/helper_embedding_metric.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/helper_embedding_metric.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/infolm.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/mer.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/perplexity.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/rouge.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/sacre_bleu.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/squad.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/ter.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/wer.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/wil.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/functional/text/wip.py` & `torchmetrics-1.0.3/src/torchmetrics/functional/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/image/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/image/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/d_lambda.py` & `torchmetrics-1.0.3/src/torchmetrics/image/d_lambda.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/ergas.py` & `torchmetrics-1.0.3/src/torchmetrics/image/ergas.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/fid.py` & `torchmetrics-1.0.3/src/torchmetrics/image/fid.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
 
     where :math:`\mathcal{N}(\mu, \Sigma)` is the multivariate normal distribution estimated from Inception v3
     (`fid ref1`_) features calculated on real life images and :math:`\mathcal{N}(\mu_w, \Sigma_w)` is the
     multivariate normal distribution estimated from Inception v3 features calculated on generated (fake) images.
     The metric was originally proposed in `fid ref1`_.
 
     Using the default feature extraction (Inception v3 using the original weights from `fid ref2`_), the input is
-    expected to be mini-batches of 3-channel RGB images of shape ``(3 x H x W)``. If argument ``normalize``
-    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0, 1]`` range, else if
+    expected to be mini-batches of 3-channel RGB images of shape ``(3xHxW)``. If argument ``normalize``
+    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0,1]`` range, else if
     ``normalize`` is set to ``False`` images are expected to have dtype ``uint8`` and take values in the ``[0, 255]``
     range. All images will be resized to 299 x 299 which is the size of the original training data. The boolian
     flag ``real`` determines if the images should update the statistics of the real distribution or the
     fake distribution.
 
     This metric is known to be unstable in its calculatations, and we recommend for the best results using this metric
     that you calculate using `torch.float64` (default is `torch.float32`) which can be set using the `.set_dtype`
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/inception.py` & `torchmetrics-1.0.3/src/torchmetrics/image/inception.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     where :math:`KL(p(y | x) || p(y))` is the KL divergence between the conditional distribution :math:`p(y|x)`
     and the margianl distribution :math:`p(y)`. Both the conditional and marginal distribution is calculated
     from features extracted from the images. The score is calculated on random splits of the images such that
     both a mean and standard deviation of the score are returned. The metric was originally proposed in
     `inception ref1`_.
 
     Using the default feature extraction (Inception v3 using the original weights from `inception ref2`_), the input
-    is expected to be mini-batches of 3-channel RGB images of shape ``(3 x H x W)``. If argument ``normalize``
-    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0, 1]`` range, else if
+    is expected to be mini-batches of 3-channel RGB images of shape ``(3xHxW)``. If argument ``normalize``
+    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0,1]`` range, else if
     ``normalize`` is set to ``False`` images are expected to have dtype uint8 and take values in the ``[0, 255]``
     range. All images will be resized to 299 x 299 which is the size of the original training data.
 
     .. note:: using this metric with the default feature extractor requires that ``torch-fidelity``
         is installed. Either install as ``pip install torchmetrics[image]`` or
         ``pip install torch-fidelity``
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/kid.py` & `torchmetrics-1.0.3/src/torchmetrics/image/kid.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,16 @@
     .. math::
         k(x,y) = (\gamma * x^T y + coef)^{degree}
 
     which controls the distance between two features. In practise the MMD is calculated over a number of
     subsets to be able to both get the mean and standard deviation of KID.
 
     Using the default feature extraction (Inception v3 using the original weights from `kid ref2`_), the input is
-    expected to be mini-batches of 3-channel RGB images of shape ``(3 x H x W)``. If argument ``normalize``
-    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0, 1]`` range, else if
+    expected to be mini-batches of 3-channel RGB images of shape ``(3xHxW)``. If argument ``normalize``
+    is ``True`` images are expected to be dtype ``float`` and have values in the ``[0,1]`` range, else if
     ``normalize`` is set to ``False`` images are expected to have dtype ``uint8`` and take values in the ``[0, 255]``
     range. All images will be resized to 299 x 299 which is the size of the original training data. The boolian
     flag ``real`` determines if the images should update the statistics of the real distribution or the
     fake distribution.
 
     .. note:: using this metric with the default feature extractor requires that ``torch-fidelity``
         is installed. Either install as ``pip install torchmetrics[image]`` or
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/lpip.py` & `torchmetrics-1.0.3/src/torchmetrics/image/lpip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/mifid.py` & `torchmetrics-1.0.3/src/torchmetrics/image/mifid.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/psnr.py` & `torchmetrics-1.0.3/src/torchmetrics/image/psnr.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/psnrb.py` & `torchmetrics-1.0.3/src/torchmetrics/image/psnrb.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/rase.py` & `torchmetrics-1.0.3/src/torchmetrics/image/rase.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/rmse_sw.py` & `torchmetrics-1.0.3/src/torchmetrics/image/rmse_sw.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/sam.py` & `torchmetrics-1.0.3/src/torchmetrics/image/sam.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/ssim.py` & `torchmetrics-1.0.3/src/torchmetrics/image/ssim.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from torchmetrics.utilities.plot import _AX_TYPE, _PLOT_OUT_TYPE
 
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["StructuralSimilarityIndexMeasure.plot", "MultiScaleStructuralSimilarityIndexMeasure.plot"]
 
 
 class StructuralSimilarityIndexMeasure(Metric):
-    """Compute Structual Similarity Index Measure (SSIM_).
+    """Compute Structural Similarity Index Measure (SSIM_).
 
     As input to ``forward`` and ``update`` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): Predictions from model
     - ``target`` (:class:`~torch.Tensor`): Ground truth values
 
     As output of `forward` and `compute` the metric returns the following output
@@ -224,15 +224,15 @@
     As input to ``forward`` and ``update`` the metric accepts the following input
 
     - ``preds`` (:class:`~torch.Tensor`): Predictions from model
     - ``target`` (:class:`~torch.Tensor`): Ground truth values
 
     As output of `forward` and `compute` the metric returns the following output
 
-    - ``msssim`` (: :class:`~torch.Tensor`): if ``reduction!='none'`` returns float scalar tensor with average MSSSIM
+    - ``msssim`` (:class:`~torch.Tensor`): if ``reduction!='none'`` returns float scalar tensor with average MSSSIM
       value over sample else returns tensor of shape ``(N,)`` with SSIM values per sample
 
     Args:
         gaussian_kernel: If ``True`` (default), a gaussian kernel is used, if false a uniform kernel is used
         kernel_size: size of the gaussian kernel
         sigma: Standard deviation of the gaussian kernel
         reduction: a method to reduce metric score over labels.
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/tv.py` & `torchmetrics-1.0.3/src/torchmetrics/image/tv.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/image/uqi.py` & `torchmetrics-1.0.3/src/torchmetrics/image/uqi.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/metric.py` & `torchmetrics-1.0.3/src/torchmetrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/multimodal/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/multimodal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/multimodal/clip_score.py` & `torchmetrics-1.0.3/src/torchmetrics/multimodal/clip_score.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/cramers.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/cramers.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/fleiss_kappa.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/pearson.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/theils_u.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/theils_u.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/nominal/tschuprows.py` & `torchmetrics-1.0.3/src/torchmetrics/nominal/tschuprows.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/concordance.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/concordance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/cosine_similarity.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/explained_variance.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/explained_variance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/kendall.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/kendall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/kl_divergence.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/kl_divergence.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/log_cosh.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/log_cosh.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/log_mse.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/log_mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/mae.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/mae.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/mape.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/minkowski.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/minkowski.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,25 @@
 if not _MATPLOTLIB_AVAILABLE:
     __doctest_skip__ = ["MinkowskiDistance.plot"]
 
 
 class MinkowskiDistance(Metric):
     r"""Compute `Minkowski Distance`_.
 
-    .. math:: d_{\text{Minkowski}} = \\sum_{i}^N (| y_i - \\hat{y_i} |^p)^\frac{1}{p}
+    .. math::
+        d_{\text{Minkowski}} = \sum_{i}^N (| y_i - \hat{y_i} |^p)^\frac{1}{p}
+
+    where
+        :math: `y` is a tensor of target values,
+        :math: `\hat{y}` is a tensor of predictions,
+        :math: `\p` is a non-negative integer or floating-point number
 
     This metric can be seen as generalized version of the standard euclidean distance which corresponds to minkowski
     distance with p=2.
 
-    where
-        :math:`y` is a tensor of target values,
-        :math:`\\hat{y}` is a tensor of predictions,
-        :math: `\\p` is a non-negative integer or floating-point number
-
     Args:
         p: int or float larger than 1, exponent to which the difference between preds and target is to be raised
         kwargs: Additional keyword arguments, see :ref:`Metric kwargs` for more info.
 
     Example:
         >>> from torchmetrics.regression import MinkowskiDistance
         >>> target = tensor([1.0, 2.8, 3.5, 4.5])
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/mse.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/mse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/pearson.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/pearson.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/r2.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/r2.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/rse.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/rse.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/spearman.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/spearman.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/symmetric_mape.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/symmetric_mape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/tweedie_deviance.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/tweedie_deviance.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/regression/wmape.py` & `torchmetrics-1.0.3/src/torchmetrics/regression/wmape.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/average_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/average_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/base.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/fall_out.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/fall_out.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/hit_rate.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/hit_rate.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/ndcg.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/precision.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/precision_recall_curve.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/r_precision.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/r_precision.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/recall.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/retrieval/reciprocal_rank.py` & `torchmetrics-1.0.3/src/torchmetrics/retrieval/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/text/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/_deprecated.py` & `torchmetrics-1.0.3/src/torchmetrics/text/_deprecated.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/bert.py` & `torchmetrics-1.0.3/src/torchmetrics/text/bert.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/bleu.py` & `torchmetrics-1.0.3/src/torchmetrics/text/bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/cer.py` & `torchmetrics-1.0.3/src/torchmetrics/text/cer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/chrf.py` & `torchmetrics-1.0.3/src/torchmetrics/text/chrf.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/eed.py` & `torchmetrics-1.0.3/src/torchmetrics/text/eed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/infolm.py` & `torchmetrics-1.0.3/src/torchmetrics/text/infolm.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/mer.py` & `torchmetrics-1.0.3/src/torchmetrics/text/mer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/perplexity.py` & `torchmetrics-1.0.3/src/torchmetrics/text/perplexity.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/rouge.py` & `torchmetrics-1.0.3/src/torchmetrics/text/rouge.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/sacre_bleu.py` & `torchmetrics-1.0.3/src/torchmetrics/text/sacre_bleu.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/squad.py` & `torchmetrics-1.0.3/src/torchmetrics/text/squad.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/ter.py` & `torchmetrics-1.0.3/src/torchmetrics/text/ter.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/wer.py` & `torchmetrics-1.0.3/src/torchmetrics/text/wer.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/wil.py` & `torchmetrics-1.0.3/src/torchmetrics/text/wil.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/text/wip.py` & `torchmetrics-1.0.3/src/torchmetrics/text/wip.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/checks.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/checks.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/compute.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/compute.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/data.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/data.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/distributed.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/enums.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/exceptions.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/imports.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/plot.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,16 @@
     fig, axs = plt.subplots(nrows=rows, ncols=cols) if ax is None else (ax.get_figure(), ax)
     axs = trim_axs(axs, nb)
     for i in range(nb):
         ax = axs[i] if rows != 1 and cols != 1 else axs
         if fig_label is not None:
             ax.set_title(f"Label {fig_label[i]}", fontsize=15)
         ax.imshow(confmat[i].cpu().detach() if confmat.ndim == 3 else confmat.cpu().detach())
-        ax.set_xlabel("True class", fontsize=15)
-        ax.set_ylabel("Predicted class", fontsize=15)
+        ax.set_xlabel("Predicted class", fontsize=15)
+        ax.set_ylabel("True class", fontsize=15)
         ax.set_xticks(list(range(n_classes)))
         ax.set_yticks(list(range(n_classes)))
         ax.set_xticklabels(labels, rotation=45, fontsize=10)
         ax.set_yticklabels(labels, rotation=25, fontsize=10)
 
         if add_text:
             for ii, jj in product(range(n_classes), range(n_classes)):
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics/utilities/prints.py` & `torchmetrics-1.0.3/src/torchmetrics/utilities/prints.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/__init__.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/bootstrapping.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/classwise.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/classwise.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/minmax.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/minmax.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/multioutput.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/multioutput.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/multitask.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/multitask.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/running.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/running.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics/wrappers/tracker.py` & `torchmetrics-1.0.3/src/torchmetrics/wrappers/tracker.py`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics.egg-info/PKG-INFO` & `torchmetrics-1.0.3/src/torchmetrics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchmetrics
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyTorch native Metrics
 Home-page: https://github.com/Lightning-AI/torchmetrics
 Download-URL: https://github.com/Lightning-AI/torchmetrics/archive/master.zip
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/torchmetrics/issues
@@ -37,41 +37,41 @@
 Provides-Extra: visual
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
-<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.2/docs/source/_static/images/logo.png" width="400px">
+<img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.3/docs/source/_static/images/logo.png" width="400px">
 
 **Machine learning metrics for distributed, scalable PyTorch applications.**
 
 ______________________________________________________________________
 
 <p align="center">
   <a href="#what-is-torchmetrics">What is Torchmetrics</a> •
   <a href="#implementing-your-own-module-metric">Implementing a metric</a> •
   <a href="#build-in-metrics">Built-in metrics</a> •
-  <a href="https://torchmetrics.readthedocs.io/en/v1.0.2">Docs</a> •
+  <a href="https://torchmetrics.readthedocs.io/en/v1.0.3">Docs</a> •
   <a href="#community">Community</a> •
   <a href="#license">License</a>
 </p>
 
 ______________________________________________________________________
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torchmetrics)](https://pypi.org/project/torchmetrics/)
 [![PyPI Status](https://badge.fury.io/py/torchmetrics.svg)](https://badge.fury.io/py/torchmetrics)
 [![PyPI Status](https://pepy.tech/badge/torchmetrics)](https://pepy.tech/project/torchmetrics)
 [![Conda](https://img.shields.io/conda/v/conda-forge/torchmetrics?label=conda&color=success)](https://anaconda.org/conda-forge/torchmetrics)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/torchmetrics)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/torchmetrics/blob/master/LICENSE)
 
 [![CI testing - complete](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml/badge.svg?event=push)](https://github.com/Lightning-AI/torchmetrics/actions/workflows/ci-tests-full.yml)
-[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.2)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.2)
-[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.2/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
+[![Build Status](https://dev.azure.com/Lightning-AI/Metrics/_apis/build/status%2FTM.unittests?branchName=refs%2Ftags%2Fv1.0.3)](https://dev.azure.com/Lightning-AI/Metrics/_build/latest?definitionId=2&branchName=refs%2Ftags%2Fv1.0.3)
+[![codecov](https://codecov.io/gh/Lightning-AI/torchmetrics/release/v1.0.3/graph/badge.svg?token=NER6LPI3HS)](https://codecov.io/gh/Lightning-AI/torchmetrics)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Lightning-AI/torchmetrics/master.svg)](https://results.pre-commit.ci/latest/github/Lightning-AI/torchmetrics/master)
 
 [![Documentation Status](https://readthedocs.org/projects/torchmetrics/badge/?version=latest)](https://torchmetrics.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5844769.svg)](https://doi.org/10.5281/zenodo.5844769)
 [![JOSS status](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43/status.svg)](https://joss.theoj.org/papers/561d9bb59b400158bc8204e2639dca43)
 
@@ -255,41 +255,49 @@
 ```
 
 </details>
 
 ### Implementing your own Module metric
 
 Implementing your own metric is as easy as subclassing an [`torch.nn.Module`](https://pytorch.org/docs/stable/generated/torch.nn.Module.html). Simply, subclass `torchmetrics.Metric`
-and implement the following methods:
+and just implement the `update` and `compute` methods:
 
 ```python
 import torch
 from torchmetrics import Metric
 
 
 class MyAccuracy(Metric):
     def __init__(self):
+        # remember to call super
         super().__init__()
         # call `self.add_state`for every internal state that is needed for the metrics computations
         # dist_reduce_fx indicates the function that should be used to reduce
         # state from multiple processes
         self.add_state("correct", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("total", default=torch.tensor(0), dist_reduce_fx="sum")
 
-    def update(self, preds: torch.Tensor, target: torch.Tensor):
-        # update metric states
-        preds, target = self._input_format(preds, target)
+    def update(self, preds: torch.Tensor, target: torch.Tensor) -> None:
+        # extract predicted class index for computing accuracy
+        preds = preds.argmax(dim=-1)
         assert preds.shape == target.shape
-
+        # update metric states
         self.correct += torch.sum(preds == target)
         self.total += target.numel()
 
-    def compute(self):
+    def compute(self) -> torch.Tensor:
         # compute final result
         return self.correct.float() / self.total
+
+
+my_metric = MyAccuracy()
+preds = torch.randn(10, 5).softmax(dim=-1)
+target = torch.randint(5, (10,))
+
+print(my_metric(preds, target))
 ```
 
 ### Functional metrics
 
 Similar to [`torch.nn`](https://pytorch.org/docs/stable/nn.html), most metrics have both a [module-based](https://torchmetrics.readthedocs.io/en/latest/references/modules.html) and a [functional](https://torchmetrics.readthedocs.io/en/latest/references/functional.html) version.
 The functional versions are simple python functions that as input take [torch.tensors](https://pytorch.org/docs/stable/tensors.html) and return the corresponding metric as a [torch.tensor](https://pytorch.org/docs/stable/tensors.html).
 
@@ -306,15 +314,15 @@
 acc = torchmetrics.functional.classification.multiclass_accuracy(
     preds, target, num_classes=5
 )
 ```
 
 ### Covered domains and example metrics
 
-In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.2all-metrics.html), which
+In total TorchMetrics contains [100+ metrics](https://torchmetrics.readthedocs.io/en/v1.0.3all-metrics.html), which
 convers the following domains:
 
 - Audio
 - Classification
 - Detection
 - Information Retrieval
 - Image
@@ -360,15 +368,15 @@
 values = []
 for i in range(10):
     values.append(acc(preds(i), target(i)))
 fig3, ax3 = acc.plot(values)
 ```
 
 <p align="center">
-  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.2/docs/source/_static/images/plot_example.png" width="1000">
+  <img src="https://github.com/Lightning-AI/torchmetrics/raw/v1.0.3/docs/source/_static/images/plot_example.png" width="1000">
 </p>
 
 For examples of plotting different metrics try running [this example file](examples/plotting.py).
 
 ## Contribute!
 
 The lightning + TorchMetrics team is hard at work adding even more metrics.
```

### Comparing `torchmetrics-1.0.2/src/torchmetrics.egg-info/SOURCES.txt` & `torchmetrics-1.0.3/src/torchmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchmetrics-1.0.2/src/torchmetrics.egg-info/requires.txt` & `torchmetrics-1.0.3/src/torchmetrics.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -3,155 +3,155 @@
 packaging
 lightning-utilities>=0.7.0
 
 [:python_version < "3.9"]
 typing-extensions
 
 [all]
-torchaudio>=0.10.0
 pystoi>=0.3.0
-torchvision>=0.8
+torchaudio>=0.10.0
 pycocotools>2.0.0
-scipy>1.0.0
+torchvision>=0.8
 torch-fidelity<=0.3.0
 lpips<=0.1.4
+scipy>1.0.0
 transformers>=4.10.0
-nltk>=3.6
 transformers>4.4.0
 regex>=2021.9.24
 tqdm>=4.41.0
-types-requests
+nltk>=3.6
 types-PyYAML
+types-emoji
 types-protobuf
+types-six
+types-requests
 types-tabulate
 types-setuptools
 mypy==1.4.1
-types-six
-types-emoji
 matplotlib>=3.2.0
 SciencePlots>=2.0.0
 
 [audio]
-torchaudio>=0.10.0
 pystoi>=0.3.0
+torchaudio>=0.10.0
 
 [detection]
-torchvision>=0.8
 pycocotools>2.0.0
+torchvision>=0.8
 
 [dev]
-torchaudio>=0.10.0
 pystoi>=0.3.0
-torchvision>=0.8
+torchaudio>=0.10.0
 pycocotools>2.0.0
-scipy>1.0.0
+torchvision>=0.8
 torch-fidelity<=0.3.0
 lpips<=0.1.4
+scipy>1.0.0
 transformers>=4.10.0
-nltk>=3.6
 transformers>4.4.0
 regex>=2021.9.24
 tqdm>=4.41.0
-types-requests
+nltk>=3.6
 types-PyYAML
+types-emoji
 types-protobuf
+types-six
+types-requests
 types-tabulate
 types-setuptools
 mypy==1.4.1
-types-six
-types-emoji
 matplotlib>=3.2.0
 SciencePlots>=2.0.0
-scikit-learn>=1.1.1
-rouge-score>0.1.0
-dython<=0.7.4
-psutil<=5.9.5
-fast-bss-eval>=0.1.0
-jiwer>=2.3.0
+scikit-image>=0.19.0
 pytorch-msssim==1.0.0
-phmdoctest==1.4.0
-coverage==7.2.7
-bert_score==0.3.13
-numpy<1.25.0
-sacrebleu>=2.0.0
+fire<=0.5.0
 pandas>=1.4.0
+kornia>=0.6.7
+sacrebleu>=2.0.0
+pytest-cov==4.1.0
+huggingface-hub<0.16
 torch_complex<=0.4.3
-statsmodels>0.13.5
-fire<=0.5.0
-requests<=2.31.0
+rouge-score>0.1.0
+pytest==7.4.0
+fast-bss-eval>=0.1.0
+numpy<1.25.0
+coverage==7.2.7
 cloudpickle>1.3
+phmdoctest==1.4.0
 fairlearn
-huggingface-hub<0.16
-kornia>=0.6.7
-pytest-doctestplus==0.13.0
-pytest-cov==4.1.0
-pytest-rerunfailures==12.0
 pytest-timeout==2.1.0
+statsmodels>0.13.5
+jiwer>=2.3.0
+bert_score==0.3.13
+dython<=0.7.4
 netcal>1.0.0
 pandas>1.0.0
+scikit-learn>=1.1.1
+requests<=2.31.0
+pytest-rerunfailures==12.0
 sewar>=0.4.4
-pytest==7.4.0
-scikit-image>=0.19.0
 mir-eval>=0.6
+pytest-doctestplus==0.13.0
+psutil<=5.9.5
 
 [image]
-scipy>1.0.0
-torchvision>=0.8
 torch-fidelity<=0.3.0
 lpips<=0.1.4
+torchvision>=0.8
+scipy>1.0.0
 
 [multimodal]
 transformers>=4.10.0
 
 [test]
-scikit-learn>=1.1.1
-rouge-score>0.1.0
-dython<=0.7.4
-psutil<=5.9.5
-fast-bss-eval>=0.1.0
-jiwer>=2.3.0
-scipy>1.0.0
+scikit-image>=0.19.0
 pytorch-msssim==1.0.0
-phmdoctest==1.4.0
-coverage==7.2.7
-bert_score==0.3.13
-numpy<1.25.0
-sacrebleu>=2.0.0
+scipy>1.0.0
+fire<=0.5.0
 pandas>=1.4.0
+kornia>=0.6.7
+sacrebleu>=2.0.0
+pytest-cov==4.1.0
+huggingface-hub<0.16
 torch_complex<=0.4.3
-statsmodels>0.13.5
-fire<=0.5.0
-requests<=2.31.0
+rouge-score>0.1.0
+pytest==7.4.0
+fast-bss-eval>=0.1.0
+numpy<1.25.0
+coverage==7.2.7
 cloudpickle>1.3
+phmdoctest==1.4.0
 fairlearn
-huggingface-hub<0.16
-kornia>=0.6.7
-pytest-doctestplus==0.13.0
-pytest-cov==4.1.0
-pytest-rerunfailures==12.0
 pytest-timeout==2.1.0
+statsmodels>0.13.5
+jiwer>=2.3.0
+bert_score==0.3.13
+dython<=0.7.4
 netcal>1.0.0
 pandas>1.0.0
+scikit-learn>=1.1.1
+requests<=2.31.0
+pytest-rerunfailures==12.0
 sewar>=0.4.4
-pytest==7.4.0
-scikit-image>=0.19.0
 mir-eval>=0.6
+pytest-doctestplus==0.13.0
+psutil<=5.9.5
 
 [text]
-nltk>=3.6
 transformers>4.4.0
 regex>=2021.9.24
 tqdm>=4.41.0
+nltk>=3.6
 
 [typing]
-types-requests
 types-PyYAML
+types-emoji
 types-protobuf
+types-six
+types-requests
 types-tabulate
 types-setuptools
 mypy==1.4.1
-types-six
-types-emoji
 
 [visual]
 matplotlib>=3.2.0
 SciencePlots>=2.0.0
```

