# Comparing `tmp/element-deeplabcut-0.2.7.tar.gz` & `tmp/element-deeplabcut-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-deeplabcut-0.2.7.tar", last modified: Fri Aug  4 22:22:20 2023, max compression
+gzip compressed data, was "element-deeplabcut-0.2.8.tar", last modified: Tue Aug  8 14:45:43 2023, max compression
```

## Comparing `element-deeplabcut-0.2.7.tar` & `element-deeplabcut-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/export/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/export/nwb.py
--rw-r--r--   0 runner    (1001) docker     (123)    31536 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/readers/dlc_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/train.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/element_deeplabcut/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 22:22:20.000000 element-deeplabcut-0.2.7/element_deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:22:20.930919 element-deeplabcut-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 22:22:17.000000 element-deeplabcut-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:43.342313 element-deeplabcut-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-08 14:45:43.342313 element-deeplabcut-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:43.338313 element-deeplabcut-0.2.8/element_deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:43.338313 element-deeplabcut-0.2.8/element_deeplabcut/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/export/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31563 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:43.342313 element-deeplabcut-0.2.8/element_deeplabcut/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/readers/dlc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/element_deeplabcut/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:45:43.338313 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-08 14:45:43.000000 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 14:45:43.000000 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:45:43.000000 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-08 14:45:43.000000 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 14:45:43.000000 element-deeplabcut-0.2.8/element_deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:45:43.342313 element-deeplabcut-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-08 14:45:39.000000 element-deeplabcut-0.2.8/setup.py
```

### Comparing `element-deeplabcut-0.2.7/LICENSE` & `element-deeplabcut-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.7/element_deeplabcut/export/nwb.py` & `element-deeplabcut-0.2.8/element_deeplabcut/export/nwb.py`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.7/element_deeplabcut/model.py` & `element-deeplabcut-0.2.8/element_deeplabcut/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -626,15 +626,17 @@
             task_mode (str): Default 'trigger' computation. Or 'load' existing results.
             analyze_videos_params (dict): Optional. Parameters passed to DLC's analyze_videos:
                 videotype, gputouse, save_as_csv, batchsize, cropping, TFGPUinference,
                 dynamic, robust_nframes, allow_growth, use_shelve
         """
         processed_dir = get_dlc_processed_data_dir()
         output_dir = cls.infer_output_dir(
-            {**video_recording_key, "model_name": model_name}, relative=False, mkdir=True
+            {**video_recording_key, "model_name": model_name},
+            relative=False,
+            mkdir=True,
         )
 
         if task_mode is None:
             try:
                 _ = dlc_reader.PoseEstimation(output_dir)
             except FileNotFoundError:
                 task_mode = "trigger"
```

### Comparing `element-deeplabcut-0.2.7/element_deeplabcut/readers/dlc_reader.py` & `element-deeplabcut-0.2.8/element_deeplabcut/readers/dlc_reader.py`

 * *Files identical despite different names*

### Comparing `element-deeplabcut-0.2.7/element_deeplabcut/train.py` & `element-deeplabcut-0.2.8/element_deeplabcut/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 def activate(
     train_schema_name: str,
     *,
     create_schema: bool = True,
     create_tables: bool = True,
-    linking_module: str = None
+    linking_module: str = None,
 ):
     """Activate this schema.
 
     Args:
         train_schema_name (str): schema name on the database server
         create_schema (bool): when True (default), create schema in the database if it
                             does not yet exist.
```

### Comparing `element-deeplabcut-0.2.7/setup.py` & `element-deeplabcut-0.2.8/setup.py`

 * *Files identical despite different names*

