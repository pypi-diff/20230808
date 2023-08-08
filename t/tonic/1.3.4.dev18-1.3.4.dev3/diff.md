# Comparing `tmp/tonic-1.3.4.dev18.tar.gz` & `tmp/tonic-1.3.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.3.4.dev18.tar", last modified: Tue Aug  8 20:23:58 2023, max compression
+gzip compressed data, was "tonic-1.3.4.dev3.tar", last modified: Tue Aug  8 12:44:44 2023, max compression
```

## Comparing `tonic-1.3.4.dev18.tar` & `tonic-1.3.4.dev3.tar`

### file list

```diff
@@ -1,191 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.090562 tonic-1.3.4.dev18/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.062562 tonic-1.3.4.dev18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.066562 tonic-1.3.4.dev18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    41044 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-08 20:23:58.090562 tonic-1.3.4.dev18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.066562 tonic-1.3.4.dev18/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.066562 tonic-1.3.4.dev18/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.070562 tonic-1.3.4.dev18/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.070562 tonic-1.3.4.dev18/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.070562 tonic-1.3.4.dev18/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.070562 tonic-1.3.4.dev18/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.070562 tonic-1.3.4.dev18/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.074562 tonic-1.3.4.dev18/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.074562 tonic-1.3.4.dev18/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_event_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.074562 tonic-1.3.4.dev18/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.074562 tonic-1.3.4.dev18/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.074562 tonic-1.3.4.dev18/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.078562 tonic-1.3.4.dev18/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.078562 tonic-1.3.4.dev18/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 20:23:58.090562 tonic-1.3.4.dev18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.078562 tonic-1.3.4.dev18/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.082562 tonic-1.3.4.dev18/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20256 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.082562 tonic-1.3.4.dev18/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.086562 tonic-1.3.4.dev18/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.086562 tonic-1.3.4.dev18/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/event_downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.086562 tonic-1.3.4.dev18/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.090562 tonic-1.3.4.dev18/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.090562 tonic-1.3.4.dev18/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    41071 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-08-08 20:23:35.000000 tonic-1.3.4.dev18/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:58.082562 tonic-1.3.4.dev18/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-08-08 20:23:58.000000 tonic-1.3.4.dev18/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 20:23:57.000000 tonic-1.3.4.dev18/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.770119 tonic-1.3.4.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.774119 tonic-1.3.4.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    40242 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.774119 tonic-1.3.4.dev3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.778119 tonic-1.3.4.dev3/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.782119 tonic-1.3.4.dev3/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.786119 tonic-1.3.4.dev3/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.786119 tonic-1.3.4.dev3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.786119 tonic-1.3.4.dev3/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.790119 tonic-1.3.4.dev3/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.790119 tonic-1.3.4.dev3/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.794119 tonic-1.3.4.dev3/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37426 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-08-08 12:44:19.000000 tonic-1.3.4.dev3/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:44:44.790119 tonic-1.3.4.dev3/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 12:44:44.000000 tonic-1.3.4.dev3/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.3.4.dev18/.github/workflows/ci-pipeline.yml` & `tonic-1.3.4.dev3/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/AUTHORS` & `tonic-1.3.4.dev3/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-Anindya Ghosh <anindya128@yahoo.com>
 Antoine Grimaldi <antoine.grimaldi@univ-amu.fr>
 AntoineGrimaldi <antoine.grimaldi@univ-amu.fr>
 Carsten Nielsen <carstenlau.nielsen@uzh.ch>
 Fabrizio Ottati <45739782+fabhertz95@users.noreply.github.com>
 Fabrizio Ottati <fabriziottati@gmail.com>
 Felix Bauer <felix.bauer@aictx.ai>
 Gregor Lenz <gregor.lenz@synsense.ai>
@@ -20,15 +19,14 @@
 Sadique Sheik <sadique.sheik@aictx.ai>
 Sadique Sheik <sadique.sheik@synsense.ai>
 Sadique Sheik <sheiksadique@gmail.com>
 Sami Barchid <sami.barchid@univ-lille.fr>
 Thomas Nowotny <t.nowotny@sussex.ac.uk>
 Tobias Fischer <info@tobiasfischer.info>
 Yalun_Hu <yalun.hu@synsense.ai>
-anindyaghosh <anindya128@yahoo.com>
 bamsumit <bam_sumit@hotmail.com>
 fabrizio.ottati <fabrizio.ottati@studenti.polito.it>
 guidoz <guidoz@users.noreply.github.com>
 k-chaney <chaneyk@seas.upenn.edu>
 kai.wang <kai.wang@synsense.ai>
 neworderofjamie <J.C.Knight@sussex.ac.uk>
 neworderofjamie <neworderofjamie@gmail.com>
```

### Comparing `tonic-1.3.4.dev18/ChangeLog` & `tonic-1.3.4.dev3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 CHANGES
 =======
 
-* Fixed bug in differentiator code that resulted in improper spikes being propagated
-* Incorporated suggestion to carry out all frame histogram subtractions in single step
 * Added compatability for non-scalar targets
-* Changed numpy histogram2d to ToFrame Made docstrings more clear
-* Removed naive from event\_downsampling  Added relevant tests and changed transforms.py and \_\_init\_\_.py appropriately  Now event\_downsampling.py works for Python 3.7
-* Added gallery transform Added additional checks
-* Fixed docs
-* Fixed all bugs. All tests passed locally. Had forgotten to add functions to \_\_init\_\_.py
-* Fixed silly bug in transforms call for EventDownsampling
-* 
-* Resolved suggestions Refactored code for optimisation. Added tests
 * add ms\_to\_idx to DSEC data
-* Update transforms.py
-* Update event\_downsampling.py
-* Methods added for new event based downsampling
 
 v1.3.3
 ------
 
 * use numpy struct to unstruct function for timesurface generation
 * try/catch case where DAVIS dataset doesn't have optitrack targets
 * update plot\_animation fn
```

### Comparing `tonic-1.3.4.dev18/LICENSE.txt` & `tonic-1.3.4.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/PKG-INFO` & `tonic-1.3.4.dev3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.4.dev18
+Version: 1.3.4.dev3
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.4.dev18/README.md` & `tonic-1.3.4.dev3/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/Makefile` & `tonic-1.3.4.dev3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/event-cameras/eventstream.png` & `tonic-1.3.4.dev3/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/event-cameras/framestream.png` & `tonic-1.3.4.dev3/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.3.4.dev3/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.3.4.dev3/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/snn/neuron-models.png` & `tonic-1.3.4.dev3/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/snn/surrogates.png` & `tonic-1.3.4.dev3/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/tonic-logo-black.png` & `tonic-1.3.4.dev3/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/tonic-logo-white.png` & `tonic-1.3.4.dev3/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/_static/tonic_favicon.png` & `tonic-1.3.4.dev3/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/about/info.rst` & `tonic-1.3.4.dev3/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/about/prototype.rst` & `tonic-1.3.4.dev3/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/about/release_notes.rst` & `tonic-1.3.4.dev3/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/conf.py` & `tonic-1.3.4.dev3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/datasets.rst` & `tonic-1.3.4.dev3/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.3.4.dev3/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/representations/plot_toframe.py` & `tonic-1.3.4.dev3/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/representations/plot_toimage.py` & `tonic-1.3.4.dev3/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_decimation.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_denoise.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_downsample.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.3.4.dev3/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/getting_involved/communication_channels.rst` & `tonic-1.3.4.dev3/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/getting_involved/contribute.rst` & `tonic-1.3.4.dev3/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/getting_started/install.rst` & `tonic-1.3.4.dev3/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/getting_started/nmnist.ipynb` & `tonic-1.3.4.dev3/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.3.4.dev3/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/how-tos/visualizing-data.ipynb` & `tonic-1.3.4.dev3/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.3.4.dev3/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/index.md` & `tonic-1.3.4.dev3/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/make.bat` & `tonic-1.3.4.dev3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/reading_material/design_choices.rst` & `tonic-1.3.4.dev3/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/reading_material/intro-event-cameras.rst` & `tonic-1.3.4.dev3/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/reading_material/intro-snns.rst` & `tonic-1.3.4.dev3/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/reading_material/training-snns.rst` & `tonic-1.3.4.dev3/docs/reading_material/training-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/transformations.rst` & `tonic-1.3.4.dev3/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/tutorials/batching.ipynb` & `tonic-1.3.4.dev3/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/tutorials/davis_data.ipynb` & `tonic-1.3.4.dev3/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.3.4.dev3/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/tutorials/large_datasets.ipynb` & `tonic-1.3.4.dev3/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/docs/tutorials/slicing.ipynb` & `tonic-1.3.4.dev3/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/setup.cfg` & `tonic-1.3.4.dev3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/dataset_utils.py` & `tonic-1.3.4.dev3/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/prototype_dataset_utils.py` & `tonic-1.3.4.dev3/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_audio_transforms.py` & `tonic-1.3.4.dev3/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_caching.py` & `tonic-1.3.4.dev3/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_chained_transforms.py` & `tonic-1.3.4.dev3/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_data/sample.aedat4` & `tonic-1.3.4.dev3/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_data/sample_ncars.dat` & `tonic-1.3.4.dev3/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_data/sample_nmnist.bin` & `tonic-1.3.4.dev3/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_data/sample_stmnist.mat` & `tonic-1.3.4.dev3/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_datasets.py` & `tonic-1.3.4.dev3/test/test_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_dsec.py` & `tonic-1.3.4.dev3/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_io.py` & `tonic-1.3.4.dev3/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_prototype_datasets.py` & `tonic-1.3.4.dev3/test/test_prototype_datasets.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_representations.py` & `tonic-1.3.4.dev3/test/test_representations.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_sliced_dataset.py` & `tonic-1.3.4.dev3/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_slicers.py` & `tonic-1.3.4.dev3/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_tonic_utils.py` & `tonic-1.3.4.dev3/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/test/test_transforms.py` & `tonic-1.3.4.dev3/test/test_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -243,60 +243,31 @@
     if hot_pixel_frequency:
         merged_polarity_raster = raster.sum(0).sum(0)
         merged_polarity_frame = frame.sum(0)
         assert not merged_polarity_frame[merged_polarity_frame > 5000].sum().sum()
         assert not merged_polarity_raster[merged_polarity_raster > 5000].sum().sum()
 
 
-@pytest.mark.parametrize("time_factor, spatial_factor, target_size", [(1, 0.25, None), (1e-3, (1, 2), None), (1, 1, (5, 5))])
-def test_transform_downsample(time_factor, spatial_factor, target_size):
+@pytest.mark.parametrize("time_factor, spatial_factor", [(1, 0.25), (1e-3, 1)])
+def test_transform_downsample(time_factor, spatial_factor):
     orig_events, sensor_size = create_random_input()
 
     transform = transforms.Downsample(
-        sensor_size=sensor_size, time_factor=time_factor, spatial_factor=spatial_factor, target_size=target_size
+        time_factor=time_factor, spatial_factor=spatial_factor
     )
 
     events = transform(orig_events)
-    
-    if not isinstance(spatial_factor, tuple):
-        spatial_factor = (spatial_factor, spatial_factor)
-    
-    if target_size is None:
-        assert np.array_equal(
-            (orig_events["t"] * time_factor).astype(orig_events["t"].dtype), events["t"]
-        )
-        assert np.array_equal(np.floor(orig_events["x"] * spatial_factor[0]), events["x"])
-        assert np.array_equal(np.floor(orig_events["y"] * spatial_factor[1]), events["y"])
-    
-    else:
-        spatial_factor_test = np.asarray(target_size) / sensor_size[:-1]
-        assert np.array_equal(np.floor(orig_events["x"] * spatial_factor_test[0]), events["x"])
-        assert np.array_equal(np.floor(orig_events["y"] * spatial_factor_test[1]), events["y"])
-    
-    assert events is not orig_events
-    
-    
-@pytest.mark.parametrize("target_size, dt, downsampling_method, noise_threshold, differentiator_time_bins", 
-                         [((50, 50), 0.05, 'integrator', 1, None),
-                          ((20, 15), 5, 'differentiator', 3, 1)])
-def test_transform_event_downsampling(target_size, dt, downsampling_method, noise_threshold, 
-                                      differentiator_time_bins):
-    
-    orig_events, sensor_size = create_random_input()
-    
-    transform = transforms.EventDownsampling(sensor_size=sensor_size, target_size=target_size, dt=dt, 
-                                             downsampling_method=downsampling_method, noise_threshold=noise_threshold,
-                                             differentiator_time_bins=differentiator_time_bins)
-    
-    events = transform(orig_events)
-    
-    assert len(events) <= len(orig_events)
-    assert np.logical_and(np.all(events["x"] <= target_size[0]), np.all(events["y"] <= target_size[1]))
+
+    assert np.array_equal(
+        (orig_events["t"] * time_factor).astype(orig_events["t"].dtype), events["t"]
+    )
+    assert np.array_equal(np.floor(orig_events["x"] * spatial_factor), events["x"])
+    assert np.array_equal(np.floor(orig_events["y"] * spatial_factor), events["y"])
     assert events is not orig_events
-    
+
 
 @pytest.mark.parametrize("target_size", [(50, 50), (10, 5)])
 def test_transform_random_crop(target_size):
     orig_events, sensor_size = create_random_input()
 
     transform = transforms.RandomCrop(sensor_size=sensor_size, target_size=target_size)
     events = transform(orig_events)
```

### Comparing `tonic-1.3.4.dev18/test/utils.py` & `tonic-1.3.4.dev3/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/audio_transforms.py` & `tonic-1.3.4.dev3/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/cached_dataset.py` & `tonic-1.3.4.dev3/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/collation.py` & `tonic-1.3.4.dev3/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/dataset.py` & `tonic-1.3.4.dev3/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/__init__.py` & `tonic-1.3.4.dev3/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/asl_dvs.py` & `tonic-1.3.4.dev3/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/cifar10dvs.py` & `tonic-1.3.4.dev3/tonic/datasets/cifar10dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/davisdataset.py` & `tonic-1.3.4.dev3/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/dsec.py` & `tonic-1.3.4.dev3/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/dvs_lips.py` & `tonic-1.3.4.dev3/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/dvsgesture.py` & `tonic-1.3.4.dev3/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/hsd.py` & `tonic-1.3.4.dev3/tonic/datasets/hsd.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/mvsec.py` & `tonic-1.3.4.dev3/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/ncaltech101.py` & `tonic-1.3.4.dev3/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/nmnist.py` & `tonic-1.3.4.dev3/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/pokerdvs.py` & `tonic-1.3.4.dev3/tonic/datasets/pokerdvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/s_mnist.py` & `tonic-1.3.4.dev3/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/tum_vie.py` & `tonic-1.3.4.dev3/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/datasets/visual_place_recognition.py` & `tonic-1.3.4.dev3/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/download_utils.py` & `tonic-1.3.4.dev3/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/__init__.py` & `tonic-1.3.4.dev3/tonic/functional/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 from .drop_event import drop_by_area_numpy, drop_by_time_numpy, drop_event_numpy
 from .drop_pixel import (
     drop_pixel_numpy,
     drop_pixel_raster,
     identify_hot_pixel,
     identify_hot_pixel_raster,
 )
-from .event_downsampling import (
-    integrator_downsample,
-    differentiator_downsample,
-)
 from .refractory_period import refractory_period_numpy
 from .spatial_jitter import spatial_jitter_numpy
 from .time_jitter import time_jitter_numpy
 from .time_skew import time_skew_numpy
 from .to_averaged_timesurface import to_averaged_timesurface_numpy
 from .to_bina_rep import to_bina_rep_numpy
 from .to_frame import to_frame_numpy
@@ -38,10 +34,8 @@
     "time_skew_numpy",
     "to_averaged_timesurface_numpy",
     "to_frame_numpy",
     "to_timesurface_numpy",
     "to_voxel_grid_numpy",
     "to_bina_rep_numpy",
     "uniform_noise_numpy",
-    "integrator_downsample",
-    "differentiator_downsample",
 ]
```

### Comparing `tonic-1.3.4.dev18/tonic/functional/crop.py` & `tonic-1.3.4.dev3/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/decimate.py` & `tonic-1.3.4.dev3/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/denoise.py` & `tonic-1.3.4.dev3/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/drop_event.py` & `tonic-1.3.4.dev3/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/drop_pixel.py` & `tonic-1.3.4.dev3/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/refractory_period.py` & `tonic-1.3.4.dev3/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/spatial_jitter.py` & `tonic-1.3.4.dev3/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/time_jitter.py` & `tonic-1.3.4.dev3/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/time_skew.py` & `tonic-1.3.4.dev3/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/to_averaged_timesurface.py` & `tonic-1.3.4.dev3/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/to_bina_rep.py` & `tonic-1.3.4.dev3/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/to_frame.py` & `tonic-1.3.4.dev3/tonic/functional/to_frame.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/to_timesurface.py` & `tonic-1.3.4.dev3/tonic/functional/to_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/to_voxel_grid.py` & `tonic-1.3.4.dev3/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/functional/uniform_noise.py` & `tonic-1.3.4.dev3/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/io.py` & `tonic-1.3.4.dev3/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/README.md` & `tonic-1.3.4.dev3/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/ncars.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/ncars.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/nmnist.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/prophesee.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/prophesee.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/stmnist.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/stmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/utils/_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.3.4.dev3/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/prototype/slicers.py` & `tonic-1.3.4.dev3/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/sliced_dataset.py` & `tonic-1.3.4.dev3/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/slicers.py` & `tonic-1.3.4.dev3/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic/transforms.py` & `tonic-1.3.4.dev3/tonic/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -253,55 +253,35 @@
     """Multiplies timestamps and spatial pixel coordinates with separate factors. Useful when the
     native temporal and/or spatial resolution of the original sensor is too high for downstream
     processing, notably when converting to dense representations of some sort. This transform does
     not drop any events.
 
     Parameters:
         time_factor (float): value to multiply timestamps with. Default is 1.
-        spatial_factor (float or tuple of floats): values to multiply pixel coordinates with. Default is 1.
-                                                   Note that when using subsequential transforms that require
-                                                   sensor_size, you must change the spatial values for the later
-                                                   transformation.
-        sensor_size (tuple): size of the sensor that was used [W,H,P]
-        target_size (tuple): size of the desired resolution [W,H]
+        spatial_factor (float): value to multiply pixel coordinates with. Default is 1.
+                                Note that when using subsequential transforms that require
+                                sensor_size, you must change the spatial values for the later
+                                transformation.
 
     Example:
         >>> from tonic.transforms import Downsample
         >>> transform1 = Downsample(time_factor=0.001) # change us to ms
         >>> transform2 = Downsample(spatial_factor=0.25) # reduce focal plane to 1/4.
-        >>> transform3 = Downsample(sensor_size=(40, 20, 2), target_size=(10, 5)) # reduce focal plane to 1/4.
     """
 
     time_factor: float = 1
-    spatial_factor: Union[float, Tuple[float, float]] = 1
-    sensor_size: Optional[Tuple[int, int, int]] = None
-    target_size: Optional[Tuple[int, int]] = None
-    
-    @staticmethod
-    def get_params(spatial_factor: Union[int, Tuple[int, int]]):
-        if not type(spatial_factor) == tuple:
-            spatial_factor = (spatial_factor, spatial_factor)
-        return spatial_factor
-    
+    spatial_factor: float = 1
+
     def __call__(self, events):
         events = events.copy()
-        
-        if self.target_size is not None:
-            # Ensure sensor_size is not None when target_size is not None
-            assert self.sensor_size is not None
-            # If both target_size and spatial_factor declared, override spatial_factor value in argument
-            spatial_factor = np.asarray(self.target_size) / self.sensor_size[:-1]
-        else:
-            spatial_factor = self.get_params(spatial_factor=self.spatial_factor)
-        
         events = functional.time_skew_numpy(events, coefficient=self.time_factor)
         if "x" in events.dtype.names:
-            events["x"] = events["x"] * spatial_factor[0]
+            events["x"] = events["x"] * self.spatial_factor
         if "y" in events.dtype.names:
-            events["y"] = events["y"] * spatial_factor[1]
+            events["y"] = events["y"] * self.spatial_factor
         return events
 
 
 @dataclass(frozen=True)
 class EventDrop:
     """Applies EventDrop transformation from the paper "EventDrop: Data Augmentation for Event-based Learning".
         Applies one of the 4 drops of event strategies between:
@@ -333,61 +313,14 @@
             return functional.drop_by_area_numpy(events, self.sensor_size, area_ratio)
         if choice == 3:
             ratio = np.random.randint(1, 10) / 10.0
             return functional.drop_event_numpy(events, ratio)
 
 
 @dataclass(frozen=True)
-class EventDownsampling:
-    """Applies EventDownsampling from the paper "Insect-inspired Spatio-temporal Downsampling of Event-based Input."
-        Allows:
-            1. Integrator based method to perform spatio-temporal event-based downsampling
-            2. Differentiator based method to perform spatio-temporal event-based downsampling
-            
-    Parameters:
-        sensor_size (Tuple): size of the sensor that was used [W,H,P]
-        target_size (Tuple): size of the desired resolution [W,H]
-        dt (float): temporal resolution of events in ms
-        downsampling_method (str): string stating downsampling method. Choose from ['naive', 'integrator', 'differentiator']
-        noise_threshold (int): set number of events in downsampled pixel required to emit spike. Zero by default.
-        differentiator_time_bins (int): number of differentiator time bins within dt. Two by default.
-        
-    Example:
-        >>> transform1 = tonic.transforms.EventDownsampling(sensor_size=(640,480,2), target_size=(20,15), dt=0.5, 
-                                                           downsampling_method='integrator')
-        >>> transform2 = tonic.transforms.EventDownsampling(sensor_size=(640,480,2), target_size=(20,15), dt=0.5, 
-                                                           downsampling_method='differentiator', noise_threshold=2,
-                                                           differentiator_time_bins=3)
-    """
-    
-    sensor_size: Tuple[int, int, int]
-    target_size: Tuple[int, int]
-    downsampling_method: str
-    dt: Optional[float] = None
-    noise_threshold: Optional[int] = None
-    differentiator_time_bins: Optional[int] = None
-    
-    def __call__(self, events):
-        assert self.downsampling_method in ['integrator', 'differentiator']
-            
-        if self.downsampling_method == 'integrator':
-            return functional.integrator_downsample(
-                events=events, sensor_size=self.sensor_size, target_size=self.target_size, 
-                dt=self.dt, noise_threshold=self.noise_threshold
-                )
-            
-        elif self.downsampling_method == 'differentiator':
-            return functional.differentiator_downsample(
-                events=events, sensor_size=self.sensor_size, target_size=self.target_size,
-                dt=self.dt, noise_threshold=self.noise_threshold,
-                differentiator_time_bins=self.differentiator_time_bins
-                )
-
-
-@dataclass(frozen=True)
 class MergePolarities:
     """Sets all polarities to zero. This transform does not have any parameters.
 
     Example:
         >>> transform = tonic.transforms.MergePolarities()
     """
```

### Comparing `tonic-1.3.4.dev18/tonic/utils.py` & `tonic-1.3.4.dev3/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic-logo-padded.png` & `tonic-1.3.4.dev3/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.3.4.dev18/tonic.egg-info/PKG-INFO` & `tonic-1.3.4.dev3/tonic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.3.4.dev18
+Version: 1.3.4.dev3
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.3.4.dev18/tonic.egg-info/SOURCES.txt` & `tonic-1.3.4.dev3/tonic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 docs/gallery/transformations/plot_decimation.py
 docs/gallery/transformations/plot_denoise.py
 docs/gallery/transformations/plot_downsample.py
 docs/gallery/transformations/plot_drop_event.py
 docs/gallery/transformations/plot_drop_event_by_area.py
 docs/gallery/transformations/plot_drop_event_by_time.py
 docs/gallery/transformations/plot_drop_pixel.py
-docs/gallery/transformations/plot_event_downsampling.py
 docs/gallery/transformations/plot_merge_polarities.py
 docs/gallery/transformations/plot_random_crop.py
 docs/gallery/transformations/plot_random_flip_lr.py
 docs/gallery/transformations/plot_random_flip_ud.py
 docs/gallery/transformations/plot_random_time_reversal.py
 docs/gallery/transformations/plot_refractory_period.py
 docs/gallery/transformations/plot_spatial_jitter.py
@@ -136,15 +135,14 @@
 tonic/datasets/visual_place_recognition.py
 tonic/functional/__init__.py
 tonic/functional/crop.py
 tonic/functional/decimate.py
 tonic/functional/denoise.py
 tonic/functional/drop_event.py
 tonic/functional/drop_pixel.py
-tonic/functional/event_downsampling.py
 tonic/functional/refractory_period.py
 tonic/functional/spatial_jitter.py
 tonic/functional/time_jitter.py
 tonic/functional/time_skew.py
 tonic/functional/to_averaged_timesurface.py
 tonic/functional/to_bina_rep.py
 tonic/functional/to_frame.py
```

