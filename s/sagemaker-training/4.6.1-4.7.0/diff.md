# Comparing `tmp/sagemaker_training-4.6.1.tar.gz` & `tmp/sagemaker_training-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_training-4.6.1.tar", last modified: Mon Jun 19 16:46:04 2023, max compression
+gzip compressed data, was "dist/sagemaker_training-4.7.0.tar", last modified: Tue Aug  8 16:46:39 2023, max compression
```

## Comparing `sagemaker_training-4.6.1.tar` & `sagemaker_training-4.7.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      156 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      100 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11326 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8922 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/README.md
--rw-rw-r--   0 root         (0) root         (0)        6 2023-06-19 16:17:05.000000 sagemaker_training-4.6.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11326 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1374 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/sagemaker_training.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2902 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/src/sagemaker_training/
--rw-rw-r--   0 root         (0) root         (0)     2547 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1664 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/_entry_point_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/src/sagemaker_training/c/
--rw-rw-r--   0 root         (0) root         (0)     3533 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/c/gethostname.c
--rw-rw-r--   0 root         (0) root         (0)     7980 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/c/jsmn.c
--rw-rw-r--   0 root         (0) root         (0)     1759 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/c/jsmn.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 16:46:04.000000 sagemaker_training-4.6.1/src/sagemaker_training/cli/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/cli/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      802 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/cli/train.py
--rw-rw-r--   0 root         (0) root         (0)      781 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/content_types.py
--rw-rw-r--   0 root         (0) root         (0)     7816 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/encoders.py
--rw-rw-r--   0 root         (0) root         (0)     5806 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/entry_point.py
--rw-rw-r--   0 root         (0) root         (0)    49952 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/environment.py
--rw-rw-r--   0 root         (0) root         (0)     3645 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/errors.py
--rw-rw-r--   0 root         (0) root         (0)     5871 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/files.py
--rw-rw-r--   0 root         (0) root         (0)     3013 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/functions.py
--rw-rw-r--   0 root         (0) root         (0)     8362 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/intermediate_output.py
--rw-rw-r--   0 root         (0) root         (0)     2164 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/logging_config.py
--rw-rw-r--   0 root         (0) root         (0)     6411 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/mapping.py
--rw-rw-r--   0 root         (0) root         (0)     5569 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/modules.py
--rw-rw-r--   0 root         (0) root         (0)    20196 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/mpi.py
--rw-rw-r--   0 root         (0) root         (0)     3297 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/params.py
--rw-rw-r--   0 root         (0) root         (0)    15951 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/process.py
--rw-rw-r--   0 root         (0) root         (0)     6583 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/pytorch_xla.py
--rw-rw-r--   0 root         (0) root         (0)    25554 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/record_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     8275 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/recordio.py
--rw-rw-r--   0 root         (0) root         (0)     5574 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/runner.py
--rw-rw-r--   0 root         (0) root         (0)    15735 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/smdataparallel.py
--rw-rw-r--   0 root         (0) root         (0)     1796 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/timeout.py
--rw-rw-r--   0 root         (0) root         (0)     5938 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/torch_distributed.py
--rw-rw-r--   0 root         (0) root         (0)     4459 2023-06-16 18:59:42.000000 sagemaker_training-4.6.1/src/sagemaker_training/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      100 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8922 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-08-08 16:17:05.000000 sagemaker_training-4.7.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      274 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/sagemaker_training.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2911 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/src/sagemaker_training/
+-rw-rw-r--   0 root         (0) root         (0)     2547 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1664 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/_entry_point_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/src/sagemaker_training/c/
+-rw-rw-r--   0 root         (0) root         (0)     3533 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/c/gethostname.c
+-rw-rw-r--   0 root         (0) root         (0)     7980 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/c/jsmn.c
+-rw-rw-r--   0 root         (0) root         (0)     1759 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/c/jsmn.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 16:46:39.000000 sagemaker_training-4.7.0/src/sagemaker_training/cli/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/cli/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      802 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/cli/train.py
+-rw-rw-r--   0 root         (0) root         (0)      781 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/content_types.py
+-rw-rw-r--   0 root         (0) root         (0)     7816 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/encoders.py
+-rw-rw-r--   0 root         (0) root         (0)     5806 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/entry_point.py
+-rw-rw-r--   0 root         (0) root         (0)    49952 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     3645 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     5871 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/files.py
+-rw-rw-r--   0 root         (0) root         (0)     3013 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/functions.py
+-rw-rw-r--   0 root         (0) root         (0)     8362 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/intermediate_output.py
+-rw-rw-r--   0 root         (0) root         (0)     2164 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/logging_config.py
+-rw-rw-r--   0 root         (0) root         (0)     6411 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/mapping.py
+-rw-rw-r--   0 root         (0) root         (0)     8045 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/modules.py
+-rw-rw-r--   0 root         (0) root         (0)    20196 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/mpi.py
+-rw-rw-r--   0 root         (0) root         (0)     3297 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/params.py
+-rw-rw-r--   0 root         (0) root         (0)    15951 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/process.py
+-rw-rw-r--   0 root         (0) root         (0)     6583 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/pytorch_xla.py
+-rw-rw-r--   0 root         (0) root         (0)    25554 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/record_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     8275 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/recordio.py
+-rw-rw-r--   0 root         (0) root         (0)     5574 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/runner.py
+-rw-rw-r--   0 root         (0) root         (0)    15735 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/smdataparallel.py
+-rw-rw-r--   0 root         (0) root         (0)     1796 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/timeout.py
+-rw-rw-r--   0 root         (0) root         (0)     5938 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/torch_distributed.py
+-rw-rw-r--   0 root         (0) root         (0)     4459 2023-08-08 07:20:00.000000 sagemaker_training-4.7.0/src/sagemaker_training/trainer.py
```

### Comparing `sagemaker_training-4.6.1/LICENSE` & `sagemaker_training-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/PKG-INFO` & `sagemaker_training-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_training
-Version: 4.6.1
+Version: 4.7.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.6.1/README.md` & `sagemaker_training-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/sagemaker_training.egg-info/PKG-INFO` & `sagemaker_training-4.7.0/sagemaker_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-training
-Version: 4.6.1
+Version: 4.7.0
 Summary: Open source library for creating containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-training-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-training-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Training Toolkit
```

### Comparing `sagemaker_training-4.6.1/sagemaker_training.egg-info/SOURCES.txt` & `sagemaker_training-4.7.0/sagemaker_training.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/setup.py` & `sagemaker_training-4.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,17 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     install_requires=required_packages,
     extras_require={
         "test": [
-            "tox==3.13.1",
+            "tox==4.6.4",
             "pytest==4.4.1",
             "pytest-cov",
             "mock",
-            "sagemaker[local]<2",
+            "sagemaker[local]>=2.172.0,<3",
             "black==22.3.0 ; python_version >= '3.7'",
         ]
     },
     entry_points={"console_scripts": ["train=sagemaker_training.cli.train:main"]},
 )
```

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/__init__.py` & `sagemaker_training-4.7.0/src/sagemaker_training/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/_entry_point_type.py` & `sagemaker_training-4.7.0/src/sagemaker_training/_entry_point_type.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/c/gethostname.c` & `sagemaker_training-4.7.0/src/sagemaker_training/c/gethostname.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/c/jsmn.c` & `sagemaker_training-4.7.0/src/sagemaker_training/c/jsmn.c`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/c/jsmn.h` & `sagemaker_training-4.7.0/src/sagemaker_training/c/jsmn.h`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/cli/train.py` & `sagemaker_training-4.7.0/src/sagemaker_training/cli/train.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/content_types.py` & `sagemaker_training-4.7.0/src/sagemaker_training/content_types.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/encoders.py` & `sagemaker_training-4.7.0/src/sagemaker_training/encoders.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/entry_point.py` & `sagemaker_training-4.7.0/src/sagemaker_training/entry_point.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/environment.py` & `sagemaker_training-4.7.0/src/sagemaker_training/environment.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/errors.py` & `sagemaker_training-4.7.0/src/sagemaker_training/errors.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/files.py` & `sagemaker_training-4.7.0/src/sagemaker_training/files.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/functions.py` & `sagemaker_training-4.7.0/src/sagemaker_training/functions.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/intermediate_output.py` & `sagemaker_training-4.7.0/src/sagemaker_training/intermediate_output.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/logging_config.py` & `sagemaker_training-4.7.0/src/sagemaker_training/logging_config.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/mapping.py` & `sagemaker_training-4.7.0/src/sagemaker_training/mapping.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/modules.py` & `sagemaker_training-4.7.0/src/sagemaker_training/modules.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 """This module contains functionality related to preparing, installing,
 and importing Python modules.
 """
 from __future__ import absolute_import
 
 import importlib
 import os
+import re
 import shlex
 import sys
 import textwrap
 
+import boto3
 import six
 
 from sagemaker_training import environment, errors, files, logging_config, process
 
 logger = logging_config.get_logger()
 
 DEFAULT_MODULE_NAME = "default_user_module_name"
+CA_REPOSITORY_ARN_ENV = "CA_REPOSITORY_ARN"
 
 
 def exists(name):  # type: (str) -> bool
     """Return True if the module exists. Return False otherwise.
 
     Args:
         name (str): Module name.
@@ -117,14 +120,17 @@
         capture_error (bool): Default false. If True, the running process captures the
             stderr, and appends it to the returned Exception message in case of errors.
     """
     cmd = "%s -m pip install . " % process.python_executable()
 
     if has_requirements(path):
         cmd += "-r requirements.txt"
+        if os.getenv(CA_REPOSITORY_ARN_ENV):
+            index = _get_codeartifact_index()
+            cmd += " -i {}".format(index)
 
     logger.info("Installing module with the following command:\n%s", cmd)
 
     process.check_error(
         shlex.split(cmd), errors.InstallModuleError, 1, cwd=path, capture_error=capture_error
     )
 
@@ -134,14 +140,17 @@
 
     Args:
         path (str):  Real path location of the requirements.txt file.
         capture_error (bool): Default false. If True, the running process captures the
             stderr, and appends it to the returned Exception message in case of errors.
     """
     cmd = "{} -m pip install -r requirements.txt".format(process.python_executable())
+    if os.getenv(CA_REPOSITORY_ARN_ENV):
+        index = _get_codeartifact_index()
+        cmd += " -i {}".format(index)
 
     logger.info("Installing dependencies from requirements.txt:\n{}".format(cmd))
 
     process.check_error(
         shlex.split(cmd), errors.InstallRequirementsError, 1, cwd=path, capture_error=capture_error
     )
 
@@ -168,7 +177,59 @@
     try:
         module = importlib.import_module(name)
         six.moves.reload_module(module)  # pylint: disable=too-many-function-args
 
         return module
     except Exception as e:  # pylint: disable=broad-except
         six.reraise(errors.ImportModuleError, errors.ImportModuleError(e), sys.exc_info()[2])
+
+
+def _get_codeartifact_index():
+    """
+    Build the authenticated codeartifact index url based on the arn provided
+    via CA_REPOSITORY_ARN environment variable following the form
+    `arn:${Partition}:codeartifact:${Region}:${Account}:repository/${DomainName}/${RepositoryName}`
+    https://docs.aws.amazon.com/codeartifact/latest/ug/python-configure-pip.html
+    https://docs.aws.amazon.com/service-authorization/latest/reference/list_awscodeartifact.html#awscodeartifact-resources-for-iam-policies
+    :return: authenticated codeartifact index url
+    """
+    repository_arn = os.getenv(CA_REPOSITORY_ARN_ENV)
+    arn_regex = (
+        "arn:(?P<partition>[^:]+):codeartifact:(?P<region>[^:]+):(?P<account>[^:]+)"
+        ":repository/(?P<domain>[^/]+)/(?P<repository>.+)"
+    )
+    m = re.match(arn_regex, repository_arn)
+    if not m:
+        raise Exception("invalid CodeArtifact repository arn {}".format(repository_arn))
+    domain = m.group("domain")
+    owner = m.group("account")
+    repository = m.group("repository")
+    region = m.group("region")
+
+    logger.info(
+        "configuring pip to use codeartifact "
+        "(domain: %s, domain owner: %s, repository: %s, region: %s)",
+        domain,
+        owner,
+        repository,
+        region,
+    )
+    try:
+        client = boto3.client("codeartifact", region_name=region)
+        auth_token_response = client.get_authorization_token(domain=domain, domainOwner=owner)
+        token = auth_token_response["authorizationToken"]
+        endpoint_response = client.get_repository_endpoint(
+            domain=domain, domainOwner=owner, repository=repository, format="pypi"
+        )
+        unauthenticated_index = endpoint_response["repositoryEndpoint"]
+        return re.sub(
+            "https://",
+            "https://aws:{}@".format(token),
+            re.sub(
+                "{}/?$".format(repository),
+                "{}/simple/".format(repository),
+                unauthenticated_index,
+            ),
+        )
+    except Exception:
+        logger.error("failed to configure pip to use codeartifact")
+        raise Exception("failed to configure pip to use codeartifact")
```

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/mpi.py` & `sagemaker_training-4.7.0/src/sagemaker_training/mpi.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/params.py` & `sagemaker_training-4.7.0/src/sagemaker_training/params.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/process.py` & `sagemaker_training-4.7.0/src/sagemaker_training/process.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/pytorch_xla.py` & `sagemaker_training-4.7.0/src/sagemaker_training/pytorch_xla.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/record_pb2.py` & `sagemaker_training-4.7.0/src/sagemaker_training/record_pb2.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/recordio.py` & `sagemaker_training-4.7.0/src/sagemaker_training/recordio.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/runner.py` & `sagemaker_training-4.7.0/src/sagemaker_training/runner.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/smdataparallel.py` & `sagemaker_training-4.7.0/src/sagemaker_training/smdataparallel.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/timeout.py` & `sagemaker_training-4.7.0/src/sagemaker_training/timeout.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/torch_distributed.py` & `sagemaker_training-4.7.0/src/sagemaker_training/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `sagemaker_training-4.6.1/src/sagemaker_training/trainer.py` & `sagemaker_training-4.7.0/src/sagemaker_training/trainer.py`

 * *Files identical despite different names*

