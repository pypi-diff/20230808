# Comparing `tmp/alpaka-job-coverage-1.5.1.tar.gz` & `tmp/alpaka-job-coverage-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.5.1.tar", last modified: Fri Aug  4 14:08:02 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.5.2.tar", last modified: Tue Aug  8 11:17:25 2023, max compression
```

## Comparing `alpaka-job-coverage-1.5.1.tar` & `alpaka-job-coverage-1.5.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.456948 alpaka-job-coverage-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.456948 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12117 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_icpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:17:25.326391 alpaka-job-coverage-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-08 11:17:25.326391 alpaka-job-coverage-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:17:25.326391 alpaka-job-coverage-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:17:25.318390 alpaka-job-coverage-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:17:25.322390 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12117 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:17:25.322390 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 11:17:25.000000 alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:17:25.326391 alpaka-job-coverage-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_icpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 11:17:02.000000 alpaka-job-coverage-1.5.2/version.txt
```

### Comparing `alpaka-job-coverage-1.5.1/LICENSE` & `alpaka-job-coverage-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/PKG-INFO` & `alpaka-job-coverage-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.5.1
+Version: 1.5.2
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.5.1/README.md` & `alpaka-job-coverage-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/setup.py` & `alpaka-job-coverage-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,51 +67,70 @@
     ## gcc device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", GCC):
         if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             reason(
                 output,
-                "gcc as device compiler cannot compile with enabled alpaka_ACC_GPU_CUDA_ENABLE back-end",
+                "gcc as device compiler cannot compile with enabled "
+                "alpaka_ACC_GPU_CUDA_ENABLE back-end",
             )
             return False
 
         if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             reason(
                 output,
-                "gcc as device compiler cannot compile with enabled alpaka_ACC_GPU_HIP_ENABLE back-end",
+                "gcc as device compiler cannot compile with enabled "
+                "alpaka_ACC_GPU_HIP_ENABLE back-end",
+            )
+            return False
+        
+        if row_check_backend_version(row, ALPAKA_ACC_SYCL_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "gcc as device compiler cannot compile with enabled "
+                "alpaka_ACC_SYCL_ENABLE back-end",
             )
             return False
 
     ###########################
     ## clang device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG):
         if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
             reason(
                 output,
-                "clang as device compiler cannot compile with enabled alpaka_ACC_GPU_CUDA_ENABLE back-end (use clang-cuda instead)",
+                "clang as device compiler cannot compile with enabled "
+                "alpaka_ACC_GPU_CUDA_ENABLE back-end (use clang-cuda instead)",
             )
             return False
 
         # clang cannot compile with enabled HIP backend
         if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             reason(
                 output,
                 "clang as device compiler cannot compile with enabled "
                 "alpaka_ACC_GPU_HIP_ENABLE back-end (use hipcc instead)",
             )
             return False
+        
+        if row_check_backend_version(row, ALPAKA_ACC_SYCL_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "clang as device compiler cannot compile with enabled "
+                "alpaka_ACC_SYCL_ENABLE back-end (use icpx instead)",
+            )
+            return False
 
     ###########################
     ## nvcc device compiler
     ###########################
 
-    if row_check_name(row, DEVICE_COMPILER, "==", NVCC):
+    if row_check_name(row, DEVICE_COMPILER, "==", NVCC):       
         # the nvcc compiler needs the same version, like the backend
         if row_check_backend_version(
             row,
             ALPAKA_ACC_GPU_CUDA_ENABLE,
             "!=",
             row[param_map[DEVICE_COMPILER]][VERSION],
         ):
@@ -125,14 +144,22 @@
         if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             reason(
                 output,
                 "If nvcc is the device compiler and the CUDA back-end is enabled "
                 "it is not allowed to enable the HIP back-end",
             )
             return False
+        
+        if row_check_backend_version(row, ALPAKA_ACC_SYCL_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "If nvcc is the device compiler it is not allowed to enable "
+                "the SYCL back-end"
+            )
+            return False
 
     ###########################
     ## clang-cuda device compiler
     ###########################
 
     if row_check_name(row, DEVICE_COMPILER, "==", CLANG_CUDA):
         # the CUDA backend needs to be enabled
@@ -148,14 +175,23 @@
         if row_check_backend_version(row, ALPAKA_ACC_GPU_HIP_ENABLE, "!=", OFF_VER):
             reason(
                 output,
                 "if clang-cuda is the device compiler and the CUDA back-end is enabled "
                 "it is not allowed to enable the HIP back-end",
             )
             return False
+        
+        # clang-cuda doesn't support the SYCL back-end
+        if row_check_backend_version(row, ALPAKA_ACC_SYCL_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if clang-cuda is the device compiler it is not allowed to "
+                "enable the SYCL back-end",
+            )
+            return False
 
         # check if clang-cuda supports the CUDA SDK version
         clangcuda_cudasdk_versions = [
             ("7", "9.2"),
             ("8", "10.0"),
             ("10", "10.1"),
             ("12", "11.0"),
@@ -197,14 +233,22 @@
             reason(
                 output,
                 "if hipcc is the device compiler and the HIP back-end is enabled, "
                 "it is not allowed to enable the CUDA back-end",
             )
             return False
         
+        if row_check_backend_version(row, ALPAKA_ACC_SYCL_ENABLE, "!=", OFF_VER):
+            reason(
+                output,
+                "if hipcc is the device compiler it is not allowed to enable "
+                "the SYCL back-end",
+            )
+            return False
+        
     ###########################
     ## icpx device compiler
     ###########################
 
     # Don't use icpx for the CUDA and HIP back-ends
     if row_check_name(row, DEVICE_COMPILER, "==", ICPX):
         if row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, "!=", OFF_VER):
```

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/validate.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/validate.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/versions.py` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage/versions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.5.1
+Version: 1.5.2
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.5.2/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_compiler_names.py` & `alpaka-job-coverage-1.5.2/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.5.2/tests/test_cuda_sdk.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_hipcc.py` & `alpaka-job-coverage-1.5.2/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_icpx.py` & `alpaka-job-coverage-1.5.2/tests/test_icpx.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_single_rules.py` & `alpaka-job-coverage-1.5.2/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_util.py` & `alpaka-job-coverage-1.5.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.1/tests/test_versions.py` & `alpaka-job-coverage-1.5.2/tests/test_versions.py`

 * *Files identical despite different names*

