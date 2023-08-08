# Comparing `tmp/tvdcn-0.4.1.tar.gz` & `tmp/tvdcn-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.4.1.tar", last modified: Sun Aug  6 20:35:48 2023, max compression
+gzip compressed data, was "tvdcn-0.4.2.tar", last modified: Tue Aug  8 19:21:24 2023, max compression
```

## Comparing `tvdcn-0.4.1.tar` & `tvdcn-0.4.2.tar`

### file list

```diff
@@ -1,78 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.465257 tvdcn-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-06 20:33:41.000000 tvdcn-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-06 20:33:41.000000 tvdcn-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-06 20:35:48.465257 tvdcn-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-06 20:33:41.000000 tvdcn-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-06 20:33:41.000000 tvdcn-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-06 20:33:41.000000 tvdcn-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-06 20:35:48.465257 tvdcn-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-06 20:33:41.000000 tvdcn-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.429256 tvdcn-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.437256 tvdcn-0.4.1/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.441256 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.445256 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.453256 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28031 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32013 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.457256 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28023 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.461257 tvdcn-0.4.1/tvdcn/csrc/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/ops/utils/tensor_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.461257 tvdcn-0.4.1/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.465257 tvdcn-0.4.1/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-06 20:33:41.000000 tvdcn-0.4.1/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 20:35:48.433256 tvdcn-0.4.1/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 20:35:48.000000 tvdcn-0.4.1/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.586071 tvdcn-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-08 19:19:29.000000 tvdcn-0.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 19:19:29.000000 tvdcn-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-08 19:21:24.586071 tvdcn-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-08 19:19:29.000000 tvdcn-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-08 19:19:29.000000 tvdcn-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 19:19:29.000000 tvdcn-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 19:21:24.586071 tvdcn-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-08 19:19:29.000000 tvdcn-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.566071 tvdcn-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.566071 tvdcn-0.4.2/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.566071 tvdcn-0.4.2/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.570071 tvdcn-0.4.2/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.570071 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.574071 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.578071 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23841 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27865 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31859 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24009 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28021 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32003 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.582071 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    23833 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    31851 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28013 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.582071 tvdcn-0.4.2/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.582071 tvdcn-0.4.2/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.586071 tvdcn-0.4.2/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33936 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 19:19:29.000000 tvdcn-0.4.2/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 19:21:24.566071 tvdcn-0.4.2/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 19:21:24.000000 tvdcn-0.4.2/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.4.1/LICENSE.txt` & `tvdcn-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/PKG-INFO` & `tvdcn-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.4.1
+Version: 0.4.2
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv,deform_conv_transposed,deformable_convolution,transposed_deformable_convolution
```

### Comparing `tvdcn-0.4.1/README.md` & `tvdcn-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/pyproject.toml` & `tvdcn-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/setup.cfg` & `tvdcn-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/setup.py` & `tvdcn-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.4.2/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tests/test_grad.py` & `tvdcn-0.4.2/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_w});
                 grad_input = grad_input.view_as(input_c);
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_h,
                                         in_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -457,15 +457,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_d,
                                         in_h,
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_h,
                                               out_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_d,
                                               out_h,
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_w});
                 grad_input = grad_input.view_as(input_c);
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -407,15 +407,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_h,
                                         in_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::Tensor();
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_d,
                                         in_h,
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_h,
                                               out_w});
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
                 int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
                 int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::Tensor();
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_d,
                                               out_h,
```

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/ops/utils/tensor_utils.cpp` & `tvdcn-0.4.2/tvdcn/csrc/ops/utils/tensor_utils.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.4.2/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/extension.py` & `tvdcn-0.4.2/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.4.2/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.4.2/tvdcn/ops/activations/mask_softmax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from typing import Tuple, Optional
 
 import torch
 import torch.nn as nn
 from torch import Tensor
-from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
+from torch.nn.common_types import _size_any_t, _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
-from tvdcn._types import _IntTuple
-
 __all__ = [
     'mask_softmax1d',
     'mask_softmax2d',
     'mask_softmax3d',
     'MaskSoftmax1d',
     'MaskSoftmax2d',
     'MaskSoftmax3d',
@@ -132,19 +130,19 @@
 # Modules
 ################################################################################
 class _MaskSoftmaxNd(nn.Module):
     """
     Base class for MaskSoftmax
     """
 
-    def __init__(self, kernel_size: _IntTuple):
+    def __init__(self, kernel_size: _size_any_t):
         super().__init__()
         self.kernel_size: Tuple[int, ...] = kernel_size
 
-    def forward(self, mask: Tensor, kernel_size: _IntTuple = None) -> Tensor:
+    def forward(self, mask: Tensor, kernel_size: Optional[_size_any_t] = None) -> Tensor:
         raise NotImplementedError
 
 
 class MaskSoftmax1d(_MaskSoftmaxNd):
     """
     See :func:`mask_softmax1d`
     """
```

### Comparing `tvdcn-0.4.1/tvdcn/ops/deform_conv.py` & `tvdcn-0.4.2/tvdcn/ops/deform_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Union, Optional, Tuple
+from typing import Callable, Union, Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn, Tensor
 from torch.nn import init
-from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
+from torch.nn.common_types import _size_any_t, _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.conv import _ConvNd
 from torch.nn.modules.utils import _single, _pair, _triple
 
 from .activations import (
     MaskSigmoid, MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d,
 )
-from .._types import _IntTuple, _Activation
 from ..extension import _assert_has_ops
 from ..utils import _log_api_usage_once
 
 __all__ = [
     'deform_conv1d',
     'deform_conv2d',
     'deform_conv3d',
@@ -208,20 +207,20 @@
     """
     Base class for DeformConv
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
-                 kernel_size: _IntTuple,
-                 stride: _IntTuple,
-                 padding: Union[str, _IntTuple],
-                 dilation: _IntTuple,
+                 kernel_size: _size_any_t,
+                 stride: _size_any_t,
+                 padding: Union[str, _size_any_t],
+                 dilation: _size_any_t,
                  transposed: bool,
-                 output_padding: Union[str, _IntTuple],
+                 output_padding: Union[str, _size_any_t],
                  groups: int,
                  bias: bool,
                  padding_mode: str,
                  device=None,
                  dtype=None) -> None:
         factory_kwargs = {'device': device, 'dtype': dtype}
         super().__init__(
@@ -405,16 +404,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
 
@@ -526,16 +525,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
 
@@ -647,16 +646,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             groups, bias, padding_mode, device, dtype)
```

### Comparing `tvdcn-0.4.1/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.4.2/tvdcn/ops/deform_conv_transpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from typing import List, Tuple, Optional, Union
+from typing import Callable, List, Tuple, Optional, Union
 
 import torch
 from torch import nn, Tensor
 from torch.nn import init
-from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
+from torch.nn.common_types import _size_any_t, _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
 from .activations import (
     MaskSigmoid, MaskSoftmax1d, MaskSoftmax2d, MaskSoftmax3d,
 )
 from .deform_conv import _DeformConvNd
-from .._types import _IntTuple, _Activation
 from ..extension import _assert_has_ops
 from ..utils import _log_api_usage_once
 
 __all__ = [
     'deform_conv_transpose1d',
     'deform_conv_transpose2d',
     'deform_conv_transpose3d',
@@ -205,20 +204,20 @@
     """
     Base class for DeformConvTranspose
     """
 
     def __init__(self,
                  in_channels: int,
                  out_channels: int,
-                 kernel_size: _IntTuple,
-                 stride: _IntTuple,
-                 padding: Union[str, _IntTuple],
-                 dilation: _IntTuple,
+                 kernel_size: _size_any_t,
+                 stride: _size_any_t,
+                 padding: Union[str, _size_any_t],
+                 dilation: _size_any_t,
                  transposed: bool,
-                 output_padding: Union[str, _IntTuple],
+                 output_padding: Union[str, _size_any_t],
                  groups: int,
                  bias: bool,
                  padding_mode: str,
                  device=None,
                  dtype=None) -> None:
         factory_kwargs = {'device': device, 'dtype': dtype}
         super().__init__(
@@ -460,16 +459,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
 
@@ -576,16 +575,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
 
@@ -692,16 +691,16 @@
                  groups: int = 1,
                  offset_groups: int = 1,
                  mask_groups: int = 1,
                  bias: bool = True,
                  generator_bias: bool = False,
                  deformable: bool = True,
                  modulated: bool = False,
-                 offset_activation: Union[str, _Activation] = None,
-                 mask_activation: Union[str, _Activation] = 'sigmoid',
+                 offset_activation: Optional[Union[str, Callable]] = None,
+                 mask_activation: Optional[Union[str, Callable]] = 'sigmoid',
                  padding_mode: str = 'zeros',
                  device=None,
                  dtype=None) -> None:
         super().__init__(
             in_channels, out_channels, kernel_size, stride, padding, dilation,
             output_padding, groups, bias, padding_mode, device, dtype)
```

### Comparing `tvdcn-0.4.1/tvdcn/utils.py` & `tvdcn-0.4.2/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.4.1/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.4.2/tvdcn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.4.1
+Version: 0.4.2
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv,deform_conv_transposed,deformable_convolution,transposed_deformable_convolution
```

### Comparing `tvdcn-0.4.1/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.4.2/tvdcn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tests/test_compatibility_with_torchvision.py
 tests/test_grad.py
 tvdcn/__init__.py
-tvdcn/_types.py
 tvdcn/_version.py
 tvdcn/extension.py
 tvdcn/utils.py
 tvdcn.egg-info/PKG-INFO
 tvdcn.egg-info/SOURCES.txt
 tvdcn.egg-info/dependency_links.txt
 tvdcn.egg-info/not-zip-safe
```

