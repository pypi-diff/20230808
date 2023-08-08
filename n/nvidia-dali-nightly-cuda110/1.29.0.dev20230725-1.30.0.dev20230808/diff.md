# Comparing `tmp/nvidia-dali-nightly-cuda110-1.29.0.dev20230725.tar.gz` & `tmp/nvidia-dali-nightly-cuda110-1.30.0.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda110-1.29.0.dev20230725.tar", last modified: Wed Jul 26 12:24:53 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda110-1.30.0.dev20230808.tar", last modified: Tue Aug  8 12:24:50 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230725.tar` & `nvidia-dali-nightly-cuda110-1.30.0.dev20230808.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 12:24:53.159606 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-26 12:24:53.159606 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 12:24:53.159606 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-26 12:24:53.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-26 12:24:53.159606 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.29.0.dev20230725/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-08 12:24:50.075340 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-08-08 12:24:50.075340 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-08 12:24:50.075340 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-08 12:24:50.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-08 12:24:50.075340 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-nightly-cuda110-1.30.0.dev20230808/setup.py
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230725/LICENSE.md` & `nvidia-dali-nightly-cuda110-1.30.0.dev20230808/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230725/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.30.0.dev20230808/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230725
+Version: 1.30.0.dev20230808
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.29.0.dev20230725
+Version: 1.30.0.dev20230808
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda110-1.29.0.dev20230725/setup.py` & `nvidia-dali-nightly-cuda110-1.30.0.dev20230808/setup.py`

 * *Files identical despite different names*

