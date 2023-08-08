# Comparing `tmp/emtools-0.0.6.tar.gz` & `tmp/emtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emtools-0.0.6.tar", last modified: Thu Jul 13 20:58:46 2023, max compression
+gzip compressed data, was "emtools-0.0.7.tar", last modified: Tue Aug  8 14:23:55 2023, max compression
```

## Comparing `emtools-0.0.6.tar` & `emtools-0.0.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.915201 emtools-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-13 20:58:36.000000 emtools-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:58:36.000000 emtools-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-13 20:58:46.915201 emtools-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-13 20:58:36.000000 emtools-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.907201 emtools-0.0.6/emtools/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/hpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/hpc/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/image/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/epu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/starfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/metadata/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/processing/motioncor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/pwx/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/pwx/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4774 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-beamshifts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-change-optics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-epu-parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-frames.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-ps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21289 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/scripts/emt-scipion-otf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.915201 emtools-0.0.6/emtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-13 20:58:36.000000 emtools-0.0.6/emtools/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:58:46.911201 emtools-0.0.6/emtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 20:58:46.000000 emtools-0.0.6/emtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 20:58:36.000000 emtools-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:58:46.915201 emtools-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-13 20:58:36.000000 emtools-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.569957 emtools-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:43.000000 emtools-0.0.7/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-08 14:23:43.000000 emtools-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 14:23:43.000000 emtools-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 14:23:55.569957 emtools-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 14:23:43.000000 emtools-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.561957 emtools-0.0.7/emtools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.561957 emtools-0.0.7/emtools/hpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/hpc/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/hpc/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/hpc/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.561957 emtools-0.0.7/emtools/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/image/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.565957 emtools-0.0.7/emtools/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/epu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/starfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/metadata/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.565957 emtools-0.0.7/emtools/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/processing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1271 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/processing/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/processing/motioncor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.565957 emtools-0.0.7/emtools/pwx/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/pwx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/pwx/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/pwx/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.565957 emtools-0.0.7/emtools/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4774 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-beamshifts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2393 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-change-optics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1562 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-epu-parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-frames.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1888 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-ps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21289 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/scripts/emt-scipion-otf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.565957 emtools-0.0.7/emtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.569957 emtools-0.0.7/emtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1195 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-08 14:23:43.000000 emtools-0.0.7/emtools/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:23:55.561957 emtools-0.0.7/emtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 14:23:55.000000 emtools-0.0.7/emtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-08 14:23:55.000000 emtools-0.0.7/emtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:23:55.000000 emtools-0.0.7/emtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 14:23:55.000000 emtools-0.0.7/emtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 14:23:55.000000 emtools-0.0.7/emtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 14:23:43.000000 emtools-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:23:55.569957 emtools-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-08 14:23:43.000000 emtools-0.0.7/setup.py
```

### Comparing `emtools-0.0.6/LICENSE` & `emtools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/PKG-INFO` & `emtools-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: emtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utilities for CryoEM data manipulation
 Home-page: https://github.com/3dem/emtools
 Author: J.M. De la Rosa Trevin, Grigory Sharov
 Author-email: delarosatrevin@gmail.com, gsharov@mrc-lmb.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/3dem/emtools/issues
 Project-URL: Source, https://github.com/3dem/emtools
```

### Comparing `emtools-0.0.6/README.rst` & `emtools-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/__init__.py` & `emtools-0.0.7/emtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'delarosatrevin@scilifelab.se'
 # *
 # **************************************************************************
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
```

### Comparing `emtools-0.0.6/emtools/hpc/__main__.py` & `emtools-0.0.7/emtools/hpc/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/hpc/lsf.py` & `emtools-0.0.7/emtools/hpc/lsf.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/hpc/submit.py` & `emtools-0.0.7/emtools/hpc/submit.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/image/__init__.py` & `emtools-0.0.7/emtools/image/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/image/thumbnail.py` & `emtools-0.0.7/emtools/image/thumbnail.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/__init__.py` & `emtools-0.0.7/emtools/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/epu.py` & `emtools-0.0.7/emtools/metadata/epu.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/misc.py` & `emtools-0.0.7/emtools/metadata/misc.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/sqlite.py` & `emtools-0.0.7/emtools/metadata/sqlite.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/starfile.py` & `emtools-0.0.7/emtools/metadata/starfile.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/metadata/table.py` & `emtools-0.0.7/emtools/metadata/table.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/processing/__init__.py` & `emtools-0.0.7/emtools/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/processing/__main__.py` & `emtools-0.0.7/emtools/processing/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/processing/motioncor.py` & `emtools-0.0.7/emtools/processing/motioncor.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/pwx/__init__.py` & `emtools-0.0.7/emtools/pwx/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/pwx/monitors.py` & `emtools-0.0.7/emtools/pwx/monitors.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/pwx/workflow.py` & `emtools-0.0.7/emtools/pwx/workflow.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-beamshifts.py` & `emtools-0.0.7/emtools/scripts/emt-beamshifts.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-change-optics.py` & `emtools-0.0.7/emtools/scripts/emt-change-optics.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-epu-parse.py` & `emtools-0.0.7/emtools/scripts/emt-epu-parse.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-files.py` & `emtools-0.0.7/emtools/scripts/emt-files.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-frames.py` & `emtools-0.0.7/emtools/scripts/emt-frames.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-ps.py` & `emtools-0.0.7/emtools/scripts/emt-ps.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/scripts/emt-scipion-otf.py` & `emtools-0.0.7/emtools/scripts/emt-scipion-otf.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/tests/test_metadata.py` & `emtools-0.0.7/emtools/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/tests/test_pipeline.py` & `emtools-0.0.7/emtools/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/tests/test_utils.py` & `emtools-0.0.7/emtools/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/__init__.py` & `emtools-0.0.7/emtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/__main__.py` & `emtools-0.0.7/emtools/utils/__main__.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/color.py` & `emtools-0.0.7/emtools/utils/color.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/path.py` & `emtools-0.0.7/emtools/utils/path.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/pipeline.py` & `emtools-0.0.7/emtools/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/pretty.py` & `emtools-0.0.7/emtools/utils/pretty.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/process.py` & `emtools-0.0.7/emtools/utils/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,17 @@
     def print(self, args=True, stdout=False):
         if args:
             print(">>> ", *self.args)
         if stdout:
             print(self.stdout)
 
     @staticmethod
-    def system(cmd, only_print=False):
-        print(cmd)
+    def system(cmd, only_print=False, color=None):
+        printCmd = cmd if color is None else color(cmd)
+        print(printCmd)
         if not only_print:
             return os.system(cmd)
 
     @staticmethod
     def ps(program, workingDir=None):
         """ Inspect processes matching a given program name.
         Args:
```

### Comparing `emtools-0.0.6/emtools/utils/server.py` & `emtools-0.0.7/emtools/utils/server.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/system.py` & `emtools-0.0.7/emtools/utils/system.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools/utils/time.py` & `emtools-0.0.7/emtools/utils/time.py`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/emtools.egg-info/PKG-INFO` & `emtools-0.0.7/emtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: emtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: Utilities for CryoEM data manipulation
 Home-page: https://github.com/3dem/emtools
 Author: J.M. De la Rosa Trevin, Grigory Sharov
 Author-email: delarosatrevin@gmail.com, gsharov@mrc-lmb.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/3dem/emtools/issues
 Project-URL: Source, https://github.com/3dem/emtools
```

### Comparing `emtools-0.0.6/emtools.egg-info/SOURCES.txt` & `emtools-0.0.7/emtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emtools-0.0.6/setup.py` & `emtools-0.0.7/setup.py`

 * *Files identical despite different names*

