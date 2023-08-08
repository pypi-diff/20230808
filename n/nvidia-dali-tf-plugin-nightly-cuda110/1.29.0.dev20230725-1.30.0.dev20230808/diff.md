# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725.tar", last modified: Wed Jul 26 12:23:34 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808.tar", last modified: Tue Aug  8 12:23:30 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725.tar` & `nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 12:23:34.167813 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-18 22:18:21.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-26 12:23:34.167813 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-07-26 12:23:34.166813 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-07-26 12:23:34.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-07-26 12:23:34.167813 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-18 22:18:21.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-08 12:23:30.100104 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-08-08 12:23:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-08-08 12:23:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-08-08 12:23:30.100104 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-08-08 12:23:29.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-08-08 12:23:30.100104 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-08-08 12:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-08-08 12:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-08-08 12:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-08-08 12:23:30.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-08-08 12:23:30.100104 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-07-06 05:01:19.000000 nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/nvidia_dali_tf_plugin_nightly_cuda110.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda110
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda110-1.29.0.dev20230725/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda110-1.30.0.dev20230808/setup.py`

 * *Files identical despite different names*

