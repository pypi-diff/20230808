# Comparing `tmp/bmtrain-0.2.3.tar.gz` & `tmp/bmtrain-0.2.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./sdist/bmtrain-0.2.3.tar", last modified: Tue Jul 11 07:02:19 2023, max compression
+gzip compressed data, was "./sdist/bmtrain-0.2.3.post1.tar", last modified: Tue Aug  8 10:59:28 2023, max compression
```

## Comparing `bmtrain-0.2.3.tar` & `bmtrain-0.2.3.post1.tar`

### file list

```diff
@@ -1,74 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-11 06:56:12.000000 bmtrain-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-11 07:02:19.000000 bmtrain-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13480 2023-07-11 06:56:12.000000 bmtrain-0.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/
--rw-r--r--   0 root         (0) root         (0)      736 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/benchmark/
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/all_gather.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/reduce_scatter.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/send_recv.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/shape.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/benchmark/utils.py
--rw-r--r--   0 root         (0) root         (0)    42476 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/block_layer.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/checkpointing.py
--rw-r--r--   0 root         (0) root         (0)      708 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/distributed/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/distributed/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5283 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/distributed/ops.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/global_var.py
--rw-r--r--   0 root         (0) root         (0)     6821 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/inspect/
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1433 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/format.py
--rw-r--r--   0 root         (0) root         (0)     9983 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/model.py
--rw-r--r--   0 root         (0) root         (0)    13766 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/inspect/tensor.py
--rw-r--r--   0 root         (0) root         (0)     6825 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/layer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/loss/
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4659 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/_function.py
--rw-r--r--   0 root         (0) root         (0)     9644 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/loss/cross_entropy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/cosine.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/exponential.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/linear.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/no_decay.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/noam.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/lr_scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/nccl/
--rw-r--r--   0 root         (0) root         (0)    10248 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/nccl/__init__.py
--rw-r--r--   0 root         (0) root         (0)      437 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/nccl/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain/optim/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4448 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/_function.py
--rw-r--r--   0 root         (0) root         (0)     8169 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/adam.py
--rw-r--r--   0 root         (0) root         (0)    11534 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/adam_offload.py
--rw-r--r--   0 root         (0) root         (0)     8175 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/optim/optim_manager.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/param_init.py
--rw-r--r--   0 root         (0) root         (0)     5213 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/parameter.py
--rw-r--r--   0 root         (0) root         (0)    27322 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/pipe_layer.py
--rw-r--r--   0 root         (0) root         (0)     7916 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/store.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/synchronize.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/utils.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-07-11 06:56:12.000000 bmtrain-0.2.3/bmtrain/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1480 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-11 07:02:19.000000 bmtrain-0.2.3/bmtrain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/bind.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/cuda/
--rw-r--r--   0 root         (0) root         (0)     2199 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/adam_cuda.cu
--rw-r--r--   0 root         (0) root         (0)     7067 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/cross_entropy.cu
--rw-r--r--   0 root         (0) root         (0)     2360 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/has_inf_nan.cu
--rw-r--r--   0 root         (0) root         (0)     3206 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/cuda/reduce.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 07:02:19.000000 bmtrain-0.2.3/csrc/include/
--rw-r--r--   0 root         (0) root         (0)    10281 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/adam_cpu.hpp
--rw-r--r--   0 root         (0) root         (0)     1419 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/bind.hpp
--rw-r--r--   0 root         (0) root         (0)     4785 2023-07-11 06:56:12.000000 bmtrain-0.2.3/csrc/include/nccl.hpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 07:02:19.000000 bmtrain-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3973 2023-07-11 06:56:12.000000 bmtrain-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/cmake/
+-rw-r--r--   0 root         (0) root         (0)     3864 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/cmake/FindNCCL.cmake
+-rw-r--r--   0 root         (0) root         (0)       47 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/csrc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/csrc/include/
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/include/adam_cpu.hpp
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/include/bind.hpp
+-rw-r--r--   0 root         (0) root         (0)      874 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/include/cpu_info.h
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/include/nccl.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/csrc/cuda/
+-rw-r--r--   0 root         (0) root         (0)     3206 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/cuda/reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/cuda/cross_entropy.cu
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/cuda/adam_cuda.cu
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/cuda/has_inf_nan.cu
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/csrc/bind.cpp
+-rw-r--r--   0 root         (0) root         (0)     3833 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    13480 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)      224 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/distributed/
+-rw-r--r--   0 root         (0) root         (0)     5283 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/distributed/ops.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/distributed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/synchronize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/loss/
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/loss/cross_entropy.py
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/loss/_function.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     6964 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/reduce_scatter.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/send_recv.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/shape.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/all_gather.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/benchmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/store.py
+-rw-r--r--   0 root         (0) root         (0)    42615 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/block_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5213 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/param_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/optim/
+-rw-r--r--   0 root         (0) root         (0)    11534 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/optim/adam_offload.py
+-rw-r--r--   0 root         (0) root         (0)     8169 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/optim/adam.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/optim/_function.py
+-rw-r--r--   0 root         (0) root         (0)     8416 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/optim/optim_manager.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/init.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/global_var.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/inspect/
+-rw-r--r--   0 root         (0) root         (0)     1433 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/inspect/format.py
+-rw-r--r--   0 root         (0) root         (0)    13766 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/inspect/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     9983 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/inspect/model.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/inspect/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/nccl/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/nccl/enums.py
+-rw-r--r--   0 root         (0) root         (0)    10248 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/nccl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27322 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/pipe_layer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/
+-rw-r--r--   0 root         (0) root         (0)      777 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/exponential.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/noam.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/warmup.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/linear.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/cosine.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/no_decay.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/lr_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      708 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/debug.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/utils.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/checkpointing.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-08-08 10:52:43.000000 bmtrain-0.2.3.post1/bmtrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2023-08-08 10:59:28.000000 bmtrain-0.2.3.post1/bmtrain.egg-info/PKG-INFO
```

### Comparing `bmtrain-0.2.3/README.md` & `bmtrain-0.2.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/__init__.py` & `bmtrain-0.2.3.post1/bmtrain/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/benchmark/all_gather.py` & `bmtrain-0.2.3.post1/bmtrain/benchmark/all_gather.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/benchmark/reduce_scatter.py` & `bmtrain-0.2.3.post1/bmtrain/benchmark/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/benchmark/send_recv.py` & `bmtrain-0.2.3.post1/bmtrain/benchmark/send_recv.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/block_layer.py` & `bmtrain-0.2.3.post1/bmtrain/block_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,14 +488,16 @@
         all_keys = []
         for it in self._param_info:
             key = prefix + it["name"]
             all_keys.append(key)
             if key in state_dict:
                 # load here
                 input_param = state_dict[key]
+                if input_param.__class__.__name__ == "DistributedTensorWrapper":
+                    input_param = input_param.broadcast()
                 if input_param.shape != it["shape"]:
                     error_msgs.append('size mismatch for {}: copying a param with shape {} from checkpoint, '
                                       'the shape in current model is {}.'
                                       .format(key, input_param.shape, it["shape"]))
                     continue
                 param_st = it["offset"]
                 param_end = it["offset"] + it["size"]
```

### Comparing `bmtrain-0.2.3/bmtrain/checkpointing.py` & `bmtrain-0.2.3.post1/bmtrain/checkpointing.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/debug.py` & `bmtrain-0.2.3.post1/bmtrain/debug.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/distributed/ops.py` & `bmtrain-0.2.3.post1/bmtrain/distributed/ops.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/global_var.py` & `bmtrain-0.2.3.post1/bmtrain/global_var.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/init.py` & `bmtrain-0.2.3.post1/bmtrain/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import torch
 import random
 import torch.distributed as dist
 import os
 from .utils import print_dict
+import ctypes
 from .global_var import config
 from . import nccl
 from .synchronize import synchronize
 def init_distributed(
         init_method : str = "env://",
         seed : int = 0,
         zero_level: int = 3,
@@ -47,17 +48,25 @@
         os.environ["MASTER_ADDR"]="localhost"
     if "MASTER_PORT" not in os.environ:
         os.environ["MASTER_PORT"]="10010"
     addr = os.environ["MASTER_ADDR"]
     port = os.environ["MASTER_PORT"]
     master = addr+":"+port
     timeout = datetime.timedelta(seconds=1800)
-    rendezvous_iterator = dist.rendezvous(
-        init_method, rank, world_size, timeout=timeout
-    )
+    try:
+        rendezvous_iterator = dist.rendezvous(
+            init_method, rank, world_size, timeout=timeout
+        )   
+    except RuntimeError:
+        import nvidia.nccl
+        path = os.path.join(os.path.dirname(nvidia.nccl.__file__), "lib")
+        for file_so in os.listdir(path):
+            if file_so.endswith(".so"):
+                ctypes.CDLL(os.path.join(path, file_so))
+
     store, rank, world_size = next(rendezvous_iterator)
     store.set_timeout(timeout)
     store = dist.PrefixStore("bmtrain", store)
     torch.cuda.set_device(local_rank)
     config["initialized"] = True
     config["pipe_size"] = pipe_size if pipe_size > 0 else 1
     config["pipe_enabled"] = pipe_size > 0
```

### Comparing `bmtrain-0.2.3/bmtrain/inspect/format.py` & `bmtrain-0.2.3.post1/bmtrain/inspect/format.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/inspect/model.py` & `bmtrain-0.2.3.post1/bmtrain/inspect/model.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/inspect/tensor.py` & `bmtrain-0.2.3.post1/bmtrain/inspect/tensor.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/layer.py` & `bmtrain-0.2.3.post1/bmtrain/layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,16 @@
         local_name_params = itertools.chain(self._parameters.items(), persistent_buffers.items())
         local_state = {k: v for k, v in local_name_params if v is not None}
 
         for name, param in local_state.items():
             key = prefix + name
             if key in state_dict:
                 input_param = state_dict[key]
+                if input_param.__class__.__name__ == "DistributedTensorWrapper":
+                    input_param = input_param.broadcast()
                 # This is used to avoid copying uninitialized parameters into
                 # non-lazy modules, since they dont have the hook to do the checks
                 # in such case, it will error when accessing the .shape attribute.
                 is_param_lazy = torch.nn.parameter.is_lazy(param)
                 # Backward compatibility: loading 1-dim tensor from 0.3.* to version 0.4+
                 if not is_param_lazy and len(param.shape) == 0 and len(input_param.shape) == 1:
                     input_param = input_param[0]
```

### Comparing `bmtrain-0.2.3/bmtrain/loss/_function.py` & `bmtrain-0.2.3.post1/bmtrain/loss/_function.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/loss/cross_entropy.py` & `bmtrain-0.2.3.post1/bmtrain/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/lr_scheduler/cosine.py` & `bmtrain-0.2.3.post1/bmtrain/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/lr_scheduler/exponential.py` & `bmtrain-0.2.3.post1/bmtrain/lr_scheduler/exponential.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/lr_scheduler/linear.py` & `bmtrain-0.2.3.post1/bmtrain/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/lr_scheduler/noam.py` & `bmtrain-0.2.3.post1/bmtrain/lr_scheduler/noam.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/lr_scheduler/warmup.py` & `bmtrain-0.2.3.post1/bmtrain/lr_scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/nccl/__init__.py` & `bmtrain-0.2.3.post1/bmtrain/nccl/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/optim/_function.py` & `bmtrain-0.2.3.post1/bmtrain/optim/_function.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/optim/adam.py` & `bmtrain-0.2.3.post1/bmtrain/optim/adam.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/optim/adam_offload.py` & `bmtrain-0.2.3.post1/bmtrain/optim/adam_offload.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/optim/optim_manager.py` & `bmtrain-0.2.3.post1/bmtrain/optim/optim_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,28 @@
         >>>     optim_manager.clip_grad_norm(optimizer2.param_groups, max_norm=2.0, norm_type=2)
         >>>     optim_manager.step()
     """
     def __init__(self,
         loss_scale : Optional[float] = None,
         loss_scale_factor : float = 2,
         loss_scale_steps : int = 1024,
+        min_loss_scale = 1,
+        max_loss_scale = float("inf"),
     ):
         if loss_scale is not None:
             self.loss_scale = loss_scale
             self.loss_scale_enabled = True
         else:
             self.loss_scale = 1
             self.loss_scale_enabled = False
         self.steps_since_last_scale = 0
         self.loss_scale_factor = loss_scale_factor if loss_scale_factor > 1 else 1 / loss_scale_factor
         self.loss_scale_steps = loss_scale_steps
+        self.min_loss_scale = min_loss_scale
+        self.max_loss_scale = max_loss_scale
 
         self.optimizers = []
         self.lr_schedulers = []
 
     def add_optimizer(
         self,
         optimizer: torch.optim.Optimizer,
@@ -108,26 +112,27 @@
         Backward with loss scale.
         Synchronize streams before optimizer steps.
 
         This is a helper function to call optimizer.step() and lr_scheduler.step() and synchronize streams.
 
         This function can also handle gradient overflow by reducing the loss scale when it occurs.
         """
-        if self.loss_scale_enabled and self.loss_scale > 1:
+        if self.loss_scale_enabled:
             has_overflow = False
             for optimizer in self.optimizers:
                 try:
                     check_overflow(optimizer.param_groups)
                 except OverflowError:
                     has_overflow = True
                     break
             if has_overflow:
                 print_rank("Gradient overflow, change scale from %lf to %lf" % (self.loss_scale, self.loss_scale / self.loss_scale_factor))
                 with torch.no_grad():
-                    self._justify_scale(self.loss_scale / self.loss_scale_factor)
+                    if self.loss_scale > self.min_loss_scale:
+                        self._justify_scale(self.loss_scale / self.loss_scale_factor)
                     self.zero_grad()
                 return
         for optimizer, lr_scheduler in zip(self.optimizers, self.lr_schedulers):
             if hasattr(optimizer, "_bmtrain_optimizer") and optimizer._bmtrain_optimizer:
                 optimizer.step(scale=self.loss_scale)
             else:
                 if self.loss_scale_enabled:
@@ -136,15 +141,15 @@
 
             if lr_scheduler is not None:
                 lr_scheduler.step()
 
         if self.loss_scale_enabled:
             self.steps_since_last_scale += 1
 
-            if self.steps_since_last_scale >= self.loss_scale_steps:
+            if self.steps_since_last_scale >= self.loss_scale_steps and self.loss_scale < self.max_loss_scale:
                 self._justify_scale(self.loss_scale * self.loss_scale_factor)
 
         current_stream = torch.cuda.current_stream()
         config['load_stream'].wait_stream(current_stream)
 
     def clip_grad_norm(self, param_groups, max_norm, norm_type=2, eps=1e-6):
         """Clips gradient norm of an iterable of parameters.
```

### Comparing `bmtrain-0.2.3/bmtrain/param_init.py` & `bmtrain-0.2.3.post1/bmtrain/param_init.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/parameter.py` & `bmtrain-0.2.3.post1/bmtrain/parameter.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/pipe_layer.py` & `bmtrain-0.2.3.post1/bmtrain/pipe_layer.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/store.py` & `bmtrain-0.2.3.post1/bmtrain/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,59 @@
             comm
         )
         buf = byte_tensor.cpu().numpy().tobytes()
         obj = _unpickler(io.BytesIO(buf)).load()
     return obj
     
 # Must be a Mapping after pytorch 1.12.0
+class DistributedTensorWrapper:
+    def __init__(self, tensor, shape=None):
+        self._dtype = tensor.dtype
+        self._device = tensor.device
+        self.shape = shape
+        self.tensor = tensor
+        
+    def broadcast(self):
+        output_param = torch.empty(self.shape, dtype=self._dtype, device="cuda")
+        if config['rank'] == 0:
+            input_param = self.tensor
+            if input_param.is_cuda:
+                input_param = input_param.clone().contiguous()
+            else:
+                input_param = input_param.cuda().contiguous()
+
+            nccl.broadcast(
+                input_param.storage(),
+                output_param.storage(),
+                0,
+                config['comm']
+            )
+        else:
+            nccl.broadcast(
+                output_param.storage(),
+                output_param.storage(),
+                0,
+                config['comm']
+            )
+        return output_param
+    
+    def copy(self):
+        return self.tensor
+    
+    def __getattribute__(self, name):
+        if name == "tensor" or name == "shape":
+            return object.__getattribute__(self, name)
+        else:
+            try:
+                return object.__getattribute__(self, name)
+            except AttributeError:
+                pass
+
+            return getattr(self.tensor, name)
+
 class DistributedStateDictWrapper(Mapping):
     def __init__(self, state_dict : Dict) -> None:
         self._state_dict = state_dict
         self._metadata = broadcast_object(getattr(state_dict, "_metadata", None), config["comm"])
     
     def __getitem__(self, key : str):
         tmp_shape = torch.zeros(32, device="cuda", dtype=torch.int32)
@@ -161,38 +206,20 @@
             config['comm']
         )
 
         shape_list_size = tmp_shape[0].item()
         dtype_idx = tmp_shape[1].item()
         shape_list = torch.Size(tmp_shape[2: 2 + shape_list_size].tolist())
 
-        output_param = torch.empty(shape_list, dtype=DTYPE_LIST[dtype_idx], device="cuda")
-        
-        if config['rank'] == 0:
-            input_param : torch.Tensor = self._state_dict[key]
-            if input_param.is_cuda:
-                input_param = input_param.clone().contiguous()
-            else:
-                input_param = input_param.cuda().contiguous()
-
-            nccl.broadcast(
-                input_param.storage(),
-                output_param.storage(),
-                0,
-                config['comm']
-            )
+        if config['rank'] != 0:
+            return DistributedTensorWrapper(torch.tensor([], dtype=DTYPE_LIST[dtype_idx], device="cuda"), shape=shape_list)
         else:
-            nccl.broadcast(
-                output_param.storage(),
-                output_param.storage(),
-                0,
-                config['comm']
-            )
+            return DistributedTensorWrapper(self._state_dict[key], shape=shape_list)
+
         
-        return output_param
         
     def copy(self):
         return self
 
     def __len__(self):
         return broadcast_object(len(self._state_dict), config["comm"])
```

### Comparing `bmtrain-0.2.3/bmtrain/synchronize.py` & `bmtrain-0.2.3.post1/bmtrain/synchronize.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/utils.py` & `bmtrain-0.2.3.post1/bmtrain/utils.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain/wrapper.py` & `bmtrain-0.2.3.post1/bmtrain/wrapper.py`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/bmtrain.egg-info/SOURCES.txt` & `bmtrain-0.2.3.post1/bmtrain.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CMakeLists.txt
 MANIFEST.in
 README.md
 setup.py
 bmtrain/__init__.py
 bmtrain/block_layer.py
 bmtrain/checkpointing.py
 bmtrain/debug.py
@@ -45,15 +46,17 @@
 bmtrain/nccl/__init__.py
 bmtrain/nccl/enums.py
 bmtrain/optim/__init__.py
 bmtrain/optim/_function.py
 bmtrain/optim/adam.py
 bmtrain/optim/adam_offload.py
 bmtrain/optim/optim_manager.py
+cmake/FindNCCL.cmake
 csrc/bind.cpp
 csrc/cuda/adam_cuda.cu
 csrc/cuda/cross_entropy.cu
 csrc/cuda/has_inf_nan.cu
 csrc/cuda/reduce.cuh
 csrc/include/adam_cpu.hpp
 csrc/include/bind.hpp
+csrc/include/cpu_info.h
 csrc/include/nccl.hpp
```

### Comparing `bmtrain-0.2.3/csrc/bind.cpp` & `bmtrain-0.2.3.post1/csrc/bind.cpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/cuda/adam_cuda.cu` & `bmtrain-0.2.3.post1/csrc/cuda/adam_cuda.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/cuda/cross_entropy.cu` & `bmtrain-0.2.3.post1/csrc/cuda/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/cuda/has_inf_nan.cu` & `bmtrain-0.2.3.post1/csrc/cuda/has_inf_nan.cu`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/cuda/reduce.cuh` & `bmtrain-0.2.3.post1/csrc/cuda/reduce.cuh`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/include/bind.hpp` & `bmtrain-0.2.3.post1/csrc/include/bind.hpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/csrc/include/nccl.hpp` & `bmtrain-0.2.3.post1/csrc/include/nccl.hpp`

 * *Files identical despite different names*

### Comparing `bmtrain-0.2.3/setup.py` & `bmtrain-0.2.3.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import os
 from setuptools.command.build_ext import build_ext
 from setuptools import  setup, find_packages, Extension
 import setuptools
 import warnings
 import sys
 import subprocess
-COMMON_NVCC_FLAGS = [
-    '-D__CUDA_NO_HALF_OPERATORS__',
-    '-D__CUDA_NO_HALF_CONVERSIONS__',
-    '-D__CUDA_NO_HALF2_OPERATORS__',
-    '--expt-relaxed-constexpr'
-]
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=""):
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
 
 
 def is_ninja_available():
@@ -93,24 +87,25 @@
         subprocess.check_call(["cmake", "--build", "."] + build_args, cwd=build_temp)
         
 ext_modules = [
     CMakeExtension("bmtrain.C"),
 ]
 setup(
     name='bmtrain',
-    version='0.2.3',
+    version='0.2.3.post1',
     author="Guoyang Zeng",
     author_email="qbjooo@qq.com",
     description="A toolkit for training big models",
     packages=find_packages(),
     install_requires=[
         "numpy",
 		"nvidia-nccl-cu11>=2.14.3"
     ],
     setup_requires=[
+        "pybind11",
         "nvidia-nccl-cu11>=2.14.3"
     ],
     ext_modules=ext_modules,
     cmdclass={
         'build_ext': CMakeBuild
     })
```

