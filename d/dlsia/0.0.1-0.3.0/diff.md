# Comparing `tmp/dlsia-0.0.1.tar.gz` & `tmp/dlsia-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dlsia-0.0.1.tar", last modified: Thu Jan 26 02:35:45 2023, max compression
+gzip compressed data, was "dlsia-0.3.0.tar", last modified: Tue Aug  8 19:57:38 2023, max compression
```

## Comparing `dlsia-0.0.1.tar` & `dlsia-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,96 @@
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 02:35:45.343306 dlsia-0.0.1/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      238 2023-01-26 02:35:45.343306 dlsia-0.0.1/PKG-INFO
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 02:35:45.343306 dlsia-0.0.1/dlsia.egg-info/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      238 2023-01-26 02:35:45.000000 dlsia-0.0.1/dlsia.egg-info/PKG-INFO
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      124 2023-01-26 02:35:45.000000 dlsia-0.0.1/dlsia.egg-info/SOURCES.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-01-26 02:35:45.000000 dlsia-0.0.1/dlsia.egg-info/dependency_links.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-01-26 02:35:45.000000 dlsia-0.0.1/dlsia.egg-info/top_level.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)       38 2023-01-26 02:35:45.343306 dlsia-0.0.1/setup.cfg
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      258 2023-01-26 02:31:58.000000 dlsia-0.0.1/setup.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      137 2023-08-08 19:46:38.000000 dlsia-0.3.0/AUTHORS.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2964 2023-08-08 19:46:38.000000 dlsia-0.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      269 2023-08-08 19:46:38.000000 dlsia-0.3.0/HISTORY.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1554 2023-08-08 19:46:38.000000 dlsia-0.3.0/LICENSE
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      305 2023-08-08 19:46:38.000000 dlsia-0.3.0/MANIFEST.in
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8725 2023-08-08 19:57:38.818181 dlsia-0.3.0/PKG-INFO
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8108 2023-08-08 19:46:38.000000 dlsia-0.3.0/README.md
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.810181 dlsia-0.3.0/dlsia/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      166 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/conformalize/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/conformalize/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5950 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/conformalize/conformalize_segmentation.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      695 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/corcoef.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    17502 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/custom_losses.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16714 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/helpers.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1219 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/inference_scripts.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/networks/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      241 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2761 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/aggnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5586 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/baggins.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3670 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/graph_utils.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16443 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msae.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7937 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msd_graph_tools.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9229 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdae.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    19515 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14317 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdnet2.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5130 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/scale_up_down.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    21540 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sms1d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    23139 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sms3d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36366 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/smsnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    25596 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sparsenet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2812 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/squashnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    26668 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/tunet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    41863 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/tunet3plus.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4466 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/unet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    31241 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/train_scripts.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/utils/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3503 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/agg_utils.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3121 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/feature_extraction.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2750 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/latent_space_viewer.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2794 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/randomized_data_loader.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3201 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/simple_instance_segmenter.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/test_data/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/test_data/two_d/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    12261 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/build_test_data.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2128 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/diffusion_model.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14578 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7409 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d_time.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9088 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/random_shapes.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7450 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/torch_hdf5_loader.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      143 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/tst.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/tutorials/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/tutorials/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      615 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/tutorials/copy_all.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/viz_tools/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5874 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/draw_sparse_network.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4149 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/plot_autoencoder_image_classification.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7218 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/plots.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia.egg-info/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8725 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/PKG-INFO
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2313 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/SOURCES.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/dependency_links.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-08-08 19:47:52.000000 dlsia-0.3.0/dlsia.egg-info/not-zip-safe
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      445 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/requires.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        6 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/top_level.txt
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/docs/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      606 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/Makefile
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2672 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/conf.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/docs/images/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36602 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/Autoencoder_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    48762 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/MSDNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    42098 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/RMSNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    62953 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/UNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    47397 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/dlsia.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3417 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/index.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      772 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/make.bat
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/docs/source/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      431 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.conformalize.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2013 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.networks.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1095 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      252 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      256 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.test_data.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1652 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.test_data.two_d.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      357 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.viz_tools.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      444 2023-08-08 19:46:38.000000 dlsia-0.3.0/requirements.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      388 2023-08-08 19:57:38.818181 dlsia-0.3.0/setup.cfg
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1637 2023-08-08 19:57:24.000000 dlsia-0.3.0/setup.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/tests/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)       40 2023-08-08 19:46:38.000000 dlsia-0.3.0/tests/__init__.py
```

