# Comparing `tmp/blendersynth-0.0.5.tar.gz` & `tmp/blendersynth-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendersynth-0.0.5.tar", last modified: Tue Jul 25 13:12:19 2023, max compression
+gzip compressed data, was "blendersynth-0.0.6.tar", last modified: Tue Aug  8 12:54:32 2023, max compression
```

## Comparing `blendersynth-0.0.5.tar` & `blendersynth-0.0.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.699272 blendersynth-0.0.5/
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.686253 blendersynth-0.0.5/BlenderSynth.egg-info/
--rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1896 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/SOURCES.txt
--rw-r--r--   0 ollie      (501) staff       (20)        1 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/dependency_links.txt
--rw-r--r--   0 ollie      (501) staff       (20)       40 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/requires.txt
--rw-r--r--   0 ollie      (501) staff       (20)       13 2023-07-25 13:12:19.000000 blendersynth-0.0.5/BlenderSynth.egg-info/top_level.txt
--rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.5/LICENSE
--rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-07-25 13:12:19.699118 blendersynth-0.0.5/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1854 2023-07-24 10:03:26.000000 blendersynth-0.0.5/README.md
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.685681 blendersynth-0.0.5/blendersynth/
--rw-r--r--   0 ollie      (501) staff       (20)     1807 2023-07-24 20:40:32.000000 blendersynth-0.0.5/blendersynth/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.687777 blendersynth-0.0.5/blendersynth/annotations/
--rw-r--r--   0 ollie      (501) staff       (20)      133 2023-07-10 22:37:06.000000 blendersynth-0.0.5/blendersynth/annotations/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     2066 2023-07-10 22:37:46.000000 blendersynth-0.0.5/blendersynth/annotations/axes.py
--rw-r--r--   0 ollie      (501) staff       (20)     2440 2023-07-09 12:11:14.000000 blendersynth-0.0.5/blendersynth/annotations/bbox.py
--rw-r--r--   0 ollie      (501) staff       (20)      656 2023-07-09 12:11:14.000000 blendersynth-0.0.5/blendersynth/annotations/keypoints.py
--rw-r--r--   0 ollie      (501) staff       (20)     1387 2023-07-09 12:13:20.000000 blendersynth-0.0.5/blendersynth/annotations/utils.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.691050 blendersynth-0.0.5/blendersynth/blender/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-07-05 14:54:19.000000 blendersynth-0.0.5/blendersynth/blender/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     8763 2023-07-13 15:44:48.000000 blendersynth-0.0.5/blendersynth/blender/aov.py
--rw-r--r--   0 ollie      (501) staff       (20)     6498 2023-07-25 12:59:05.000000 blendersynth-0.0.5/blendersynth/blender/bsyn_object.py
--rw-r--r--   0 ollie      (501) staff       (20)     3571 2023-07-25 12:19:49.000000 blendersynth-0.0.5/blendersynth/blender/camera.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.692617 blendersynth-0.0.5/blendersynth/blender/compositor/
--rw-r--r--   0 ollie      (501) staff       (20)       34 2023-07-05 13:24:45.000000 blendersynth-0.0.5/blendersynth/blender/compositor/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)    14112 2023-07-24 12:32:58.000000 blendersynth-0.0.5/blendersynth/blender/compositor/compositor.py
--rw-r--r--   0 ollie      (501) staff       (20)     6574 2023-07-10 22:39:48.000000 blendersynth-0.0.5/blendersynth/blender/compositor/image_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.5/blendersynth/blender/compositor/mask_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)      887 2023-07-10 22:40:32.000000 blendersynth-0.0.5/blendersynth/blender/compositor/node_group.py
--rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-07-05 12:25:55.000000 blendersynth-0.0.5/blendersynth/blender/compositor/visuals.py
--rw-r--r--   0 ollie      (501) staff       (20)      726 2023-07-25 10:21:51.000000 blendersynth-0.0.5/blendersynth/blender/curve.py
--rw-r--r--   0 ollie      (501) staff       (20)     2261 2023-07-25 13:11:41.000000 blendersynth-0.0.5/blendersynth/blender/light.py
--rw-r--r--   0 ollie      (501) staff       (20)     4779 2023-07-25 08:10:33.000000 blendersynth-0.0.5/blendersynth/blender/material.py
--rw-r--r--   0 ollie      (501) staff       (20)    15416 2023-07-25 13:11:41.000000 blendersynth-0.0.5/blendersynth/blender/mesh.py
--rw-r--r--   0 ollie      (501) staff       (20)     1491 2023-07-05 15:36:05.000000 blendersynth-0.0.5/blendersynth/blender/render.py
--rw-r--r--   0 ollie      (501) staff       (20)     7380 2023-07-25 12:57:52.000000 blendersynth-0.0.5/blendersynth/blender/utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     3170 2023-07-24 14:32:46.000000 blendersynth-0.0.5/blendersynth/blender/world.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.694598 blendersynth-0.0.5/blendersynth/file/
--rw-r--r--   0 ollie      (501) staff       (20)      152 2023-07-24 12:27:08.000000 blendersynth-0.0.5/blendersynth/file/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     1165 2023-07-24 12:27:08.000000 blendersynth-0.0.5/blendersynth/file/dataset_inputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      318 2023-07-09 12:14:45.000000 blendersynth-0.0.5/blendersynth/file/dataset_outputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      497 2023-07-07 19:24:14.000000 blendersynth-0.0.5/blendersynth/file/ffmpeg_utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     3001 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/file/frames_to_video.py
--rw-r--r--   0 ollie      (501) staff       (20)      618 2023-07-05 13:54:50.000000 blendersynth-0.0.5/blendersynth/file/tempfiles.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.696211 blendersynth-0.0.5/blendersynth/run/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.5/blendersynth/run/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.5/blendersynth/run/blender_interface.py
--rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.5/blendersynth/run/blender_threading.py
--rw-r--r--   0 ollie      (501) staff       (20)     3278 2023-07-09 12:37:15.000000 blendersynth-0.0.5/blendersynth/run/run.py
--rw-r--r--   0 ollie      (501) staff       (20)      859 2023-07-12 13:54:07.000000 blendersynth-0.0.5/blendersynth/run/run_this_script.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.697611 blendersynth-0.0.5/blendersynth/utils/
--rw-r--r--   0 ollie      (501) staff       (20)       43 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      713 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/blender_importer.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-07-25 13:12:19.698670 blendersynth-0.0.5/blendersynth/utils/blender_setup/
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     4475 2023-07-07 10:33:19.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_locator.py
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_python_path.py
--rw-r--r--   0 ollie      (501) staff       (20)     3000 2023-07-24 09:59:41.000000 blendersynth-0.0.5/blendersynth/utils/blender_setup/check_blender_install.py
--rw-r--r--   0 ollie      (501) staff       (20)     3604 2023-07-09 12:37:15.000000 blendersynth-0.0.5/blendersynth/utils/node_arranger.py
--rw-r--r--   0 ollie      (501) staff       (20)      619 2023-07-25 13:01:55.000000 blendersynth-0.0.5/blendersynth/utils/types.py
--rw-r--r--   0 ollie      (501) staff       (20)      409 2023-07-25 13:12:11.000000 blendersynth-0.0.5/pyproject.toml
--rw-r--r--   0 ollie      (501) staff       (20)       38 2023-07-25 13:12:19.699322 blendersynth-0.0.5/setup.cfg
--rw-r--r--   0 ollie      (501) staff       (20)      245 2023-07-25 13:12:11.000000 blendersynth-0.0.5/setup.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.628594 blendersynth-0.0.6/
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.614698 blendersynth-0.0.6/BlenderSynth.egg-info/
+-rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-08-08 12:54:32.000000 blendersynth-0.0.6/BlenderSynth.egg-info/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1896 2023-08-08 12:54:32.000000 blendersynth-0.0.6/BlenderSynth.egg-info/SOURCES.txt
+-rw-r--r--   0 ollie      (501) staff       (20)        1 2023-08-08 12:54:32.000000 blendersynth-0.0.6/BlenderSynth.egg-info/dependency_links.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       40 2023-08-08 12:54:32.000000 blendersynth-0.0.6/BlenderSynth.egg-info/requires.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       13 2023-08-08 12:54:32.000000 blendersynth-0.0.6/BlenderSynth.egg-info/top_level.txt
+-rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.6/LICENSE
+-rw-r--r--   0 ollie      (501) staff       (20)     2129 2023-08-08 12:54:32.628421 blendersynth-0.0.6/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1854 2023-07-24 10:03:26.000000 blendersynth-0.0.6/README.md
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.614060 blendersynth-0.0.6/blendersynth/
+-rw-r--r--   0 ollie      (501) staff       (20)     1807 2023-07-24 20:40:32.000000 blendersynth-0.0.6/blendersynth/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.616152 blendersynth-0.0.6/blendersynth/annotations/
+-rw-r--r--   0 ollie      (501) staff       (20)      133 2023-07-10 22:37:06.000000 blendersynth-0.0.6/blendersynth/annotations/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2066 2023-07-10 22:37:46.000000 blendersynth-0.0.6/blendersynth/annotations/axes.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2441 2023-08-08 11:01:32.000000 blendersynth-0.0.6/blendersynth/annotations/bbox.py
+-rw-r--r--   0 ollie      (501) staff       (20)      656 2023-07-09 12:11:14.000000 blendersynth-0.0.6/blendersynth/annotations/keypoints.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1387 2023-07-09 12:13:20.000000 blendersynth-0.0.6/blendersynth/annotations/utils.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.619314 blendersynth-0.0.6/blendersynth/blender/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-07-05 14:54:19.000000 blendersynth-0.0.6/blendersynth/blender/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     8763 2023-07-13 15:44:48.000000 blendersynth-0.0.6/blendersynth/blender/aov.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6884 2023-08-08 09:20:21.000000 blendersynth-0.0.6/blendersynth/blender/bsyn_object.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3571 2023-08-08 09:19:56.000000 blendersynth-0.0.6/blendersynth/blender/camera.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.621046 blendersynth-0.0.6/blendersynth/blender/compositor/
+-rw-r--r--   0 ollie      (501) staff       (20)       34 2023-07-05 13:24:45.000000 blendersynth-0.0.6/blendersynth/blender/compositor/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)    14112 2023-07-24 12:32:58.000000 blendersynth-0.0.6/blendersynth/blender/compositor/compositor.py
+-rw-r--r--   0 ollie      (501) staff       (20)     6574 2023-07-10 22:39:48.000000 blendersynth-0.0.6/blendersynth/blender/compositor/image_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.6/blendersynth/blender/compositor/mask_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)      887 2023-07-10 22:40:32.000000 blendersynth-0.0.6/blendersynth/blender/compositor/node_group.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1103 2023-07-05 12:25:55.000000 blendersynth-0.0.6/blendersynth/blender/compositor/visuals.py
+-rw-r--r--   0 ollie      (501) staff       (20)      726 2023-07-25 10:21:51.000000 blendersynth-0.0.6/blendersynth/blender/curve.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2261 2023-07-25 13:11:41.000000 blendersynth-0.0.6/blendersynth/blender/light.py
+-rw-r--r--   0 ollie      (501) staff       (20)     5122 2023-08-08 09:34:30.000000 blendersynth-0.0.6/blendersynth/blender/material.py
+-rw-r--r--   0 ollie      (501) staff       (20)    17047 2023-08-08 11:01:32.000000 blendersynth-0.0.6/blendersynth/blender/mesh.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1491 2023-07-05 15:36:05.000000 blendersynth-0.0.6/blendersynth/blender/render.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7904 2023-08-08 09:20:21.000000 blendersynth-0.0.6/blendersynth/blender/utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3170 2023-07-24 14:32:46.000000 blendersynth-0.0.6/blendersynth/blender/world.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.623564 blendersynth-0.0.6/blendersynth/file/
+-rw-r--r--   0 ollie      (501) staff       (20)      152 2023-07-24 12:27:08.000000 blendersynth-0.0.6/blendersynth/file/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1165 2023-07-24 12:27:08.000000 blendersynth-0.0.6/blendersynth/file/dataset_inputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      318 2023-07-09 12:14:45.000000 blendersynth-0.0.6/blendersynth/file/dataset_outputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      497 2023-07-07 19:24:14.000000 blendersynth-0.0.6/blendersynth/file/ffmpeg_utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3001 2023-07-07 10:33:19.000000 blendersynth-0.0.6/blendersynth/file/frames_to_video.py
+-rw-r--r--   0 ollie      (501) staff       (20)      618 2023-07-05 13:54:50.000000 blendersynth-0.0.6/blendersynth/file/tempfiles.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.625075 blendersynth-0.0.6/blendersynth/run/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.6/blendersynth/run/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.6/blendersynth/run/blender_interface.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.6/blendersynth/run/blender_threading.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3278 2023-07-09 12:37:15.000000 blendersynth-0.0.6/blendersynth/run/run.py
+-rw-r--r--   0 ollie      (501) staff       (20)      859 2023-07-12 13:54:07.000000 blendersynth-0.0.6/blendersynth/run/run_this_script.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.626546 blendersynth-0.0.6/blendersynth/utils/
+-rw-r--r--   0 ollie      (501) staff       (20)       43 2023-07-07 10:33:19.000000 blendersynth-0.0.6/blendersynth/utils/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      713 2023-07-07 10:33:19.000000 blendersynth-0.0.6/blendersynth/utils/blender_importer.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-08-08 12:54:32.627910 blendersynth-0.0.6/blendersynth/utils/blender_setup/
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.6/blendersynth/utils/blender_setup/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4475 2023-07-07 10:33:19.000000 blendersynth-0.0.6/blendersynth/utils/blender_setup/blender_locator.py
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.6/blendersynth/utils/blender_setup/blender_python_path.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3000 2023-07-24 09:59:41.000000 blendersynth-0.0.6/blendersynth/utils/blender_setup/check_blender_install.py
+-rw-r--r--   0 ollie      (501) staff       (20)     4034 2023-08-08 09:39:16.000000 blendersynth-0.0.6/blendersynth/utils/node_arranger.py
+-rw-r--r--   0 ollie      (501) staff       (20)      619 2023-07-25 13:01:55.000000 blendersynth-0.0.6/blendersynth/utils/types.py
+-rw-r--r--   0 ollie      (501) staff       (20)      409 2023-08-08 12:54:23.000000 blendersynth-0.0.6/pyproject.toml
+-rw-r--r--   0 ollie      (501) staff       (20)       38 2023-08-08 12:54:32.628663 blendersynth-0.0.6/setup.cfg
+-rw-r--r--   0 ollie      (501) staff       (20)      245 2023-07-25 13:12:11.000000 blendersynth-0.0.6/setup.py
```

### Comparing `blendersynth-0.0.5/BlenderSynth.egg-info/PKG-INFO` & `blendersynth-0.0.6/BlenderSynth.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
```

### Comparing `blendersynth-0.0.5/BlenderSynth.egg-info/SOURCES.txt` & `blendersynth-0.0.6/BlenderSynth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/LICENSE` & `blendersynth-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/PKG-INFO` & `blendersynth-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.5
+Version: 0.0.6
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
```

### Comparing `blendersynth-0.0.5/README.md` & `blendersynth-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/__init__.py` & `blendersynth-0.0.6/blendersynth/__init__.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/annotations/axes.py` & `blendersynth-0.0.6/blendersynth/annotations/axes.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/annotations/bbox.py` & `blendersynth-0.0.6/blendersynth/annotations/bbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 	if camera is None:
 		camera = bpy.context.scene.camera
 
 	if scene is None:
 		scene = bpy.context.scene
 
-	verts = object.get_all_vertices('WORLD')
+	verts = object._get_all_vertices('WORLD')
 	coords_2d = project_points(verts, scene, camera, invert_y=invert_y)
 
 	if normalized:
 		coords_2d[:, 0] /= scene.render.resolution_x
 		coords_2d[:, 1] /= scene.render.resolution_y
 
 	xmin, ymin = coords_2d.min(axis=0)
```

### Comparing `blendersynth-0.0.5/blendersynth/annotations/keypoints.py` & `blendersynth-0.0.6/blendersynth/annotations/keypoints.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/annotations/utils.py` & `blendersynth-0.0.6/blendersynth/annotations/utils.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/aov.py` & `blendersynth-0.0.6/blendersynth/blender/aov.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/bsyn_object.py` & `blendersynth-0.0.6/blendersynth/blender/bsyn_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base class for all BlenderSynth objects."""
-from .utils import handle_vec, SelectObjects, _euler_add, _euler_from, animatable_property
-from mathutils import Vector, Euler
+from .utils import handle_vec, SelectObjects, _euler_add, animatable_property, _euler_invert
+from mathutils import Vector, Euler, Matrix
 import numpy as np
 import bpy
 from typing import Union
 from ..utils import types
 
 class BsynObject:
 	"""Generic class for BlenderSynth objects."""
@@ -21,32 +21,36 @@
 	def object(self):
 		return self.obj
 
 	@property
 	def data(self):
 		return self.object.data
 
-	# def update(self):
+	def update(self):
 	#   ---> not currently needed, may be needed in the future
 	# 	"""On any update, run this. For most objects, this is a no-op, but for some objects,
 	# 	this is necessary to update the object's state. e.g. Camera"""
-	# 	return
+		return
 
 	def _keyframe_delete(self, *args, **kwargs):
 		self._object.keyframe_delete(*args, **kwargs)
 
 	def _keyframe_insert(self, *args, **kwargs):
 		self._object.keyframe_insert(*args, **kwargs)
 
 	@property
 	def _all_objects(self):
 		"""List of all objects associated with this object."""
 		return [self.object]
 
 	@property
+	def origin(self) -> Vector:
+		return self.location
+
+	@property
 	def location(self) -> Vector:
 		"""Location of object"""
 		return self.obj.location
 
 	@location.setter
 	def location(self, value):
 		self.set_location(value)
@@ -77,29 +81,33 @@
 		:param location: Location vector to set"""
 		location = handle_vec(location, 3)
 
 		translation = location - self.location
 		with SelectObjects(self._all_objects):
 			bpy.ops.transform.translate(value=translation)
 
+	def _apply_rotation(self, rot):
+		for ax, val in zip('XYZ', rot):
+			if val != 0:
+				bpy.ops.transform.rotate(value=val, orient_axis=ax, orient_type='GLOBAL',
+										 constraint_axis=[ax == 'X', ax == 'Y', ax == 'Z'])
 
 	@animatable_property('rotation_euler')
 	def set_rotation_euler(self, rotation: types.VectorLikeAlias):
 		"""Set euler rotation of object.
 
 		:param rotation: Rotation vector"""
 
 		assert len(rotation) == 3, f"Rotation must be a tuple of length 3, got {len(rotation)}"
 		rotation = Euler(rotation, 'XYZ')
-		diff = _euler_from(self.rotation_euler, rotation)
 
+		# to avoid dealing with rotation calculations, we first rotate to the origin, then rotate to the new rotation
 		with SelectObjects(self._all_objects):
-			for ax, val in zip('XYZ', diff):
-				if val != 0:
-					bpy.ops.transform.rotate(value=val, orient_axis=ax)
+			self._apply_rotation(_euler_invert(self.rotation_euler))  # invert current rotation
+			self._apply_rotation(rotation)  # apply new rotation
 
 	@animatable_property('scale')
 	def set_scale(self, scale: types.VectorLikeOrScalarAlias):
 		"""Set scale of object.
 
 		:param scale: Scale to set. Either single value or 3 long vector"""
 		if isinstance(scale, (int, float)):
```

### Comparing `blendersynth-0.0.5/blendersynth/blender/camera.py` & `blendersynth-0.0.6/blendersynth/blender/camera.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/compositor/compositor.py` & `blendersynth-0.0.6/blendersynth/blender/compositor/compositor.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/compositor/image_overlay.py` & `blendersynth-0.0.6/blendersynth/blender/compositor/image_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/compositor/mask_overlay.py` & `blendersynth-0.0.6/blendersynth/blender/compositor/mask_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/compositor/node_group.py` & `blendersynth-0.0.6/blendersynth/blender/compositor/node_group.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/compositor/visuals.py` & `blendersynth-0.0.6/blendersynth/blender/compositor/visuals.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/curve.py` & `blendersynth-0.0.6/blendersynth/blender/curve.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/light.py` & `blendersynth-0.0.6/blendersynth/blender/light.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/material.py` & `blendersynth-0.0.6/blendersynth/blender/material.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,24 @@
 
 		mapping_node = self.nodes.new('ShaderNodeMapping')
 
 		self.links.new(self.scale_node.outputs[0], mapping_node.inputs['Scale'])
 		self.links.new(tex_coord_node.outputs['UV'], mapping_node.inputs['Vector'])
 		self._texture_scaling_socket = mapping_node.outputs['Vector']
 
+	def set_bdsf_property(self, key: str, value: float):
+		"""Set the property of the BSDF node"""
+		if self.shader.type != 'BSDF_PRINCIPLED':
+			raise ValueError("Shader is not a Principled BSDF")
+
+		if key not in self.shader.inputs:
+			raise ValueError(f"Invalid BDSF shader property `{key}`")
+
+		self.shader.inputs[key].default_value = value
+
 	@property
 	def scale(self):
 		return self._scale
 
 	@scale.setter
 	def scale(self, value):
 		self._scale = value
```

### Comparing `blendersynth-0.0.5/blendersynth/blender/mesh.py` & `blendersynth-0.0.6/blendersynth/blender/mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import bpy
 from .utils import GetNewObject, SelectObjects, handle_vec, SetMode, animatable_property
 from .bsyn_object import BsynObject
 from .material import Material
 from .aov import AOV
 import numpy as np
 import mathutils
+import bmesh
 from mathutils import Vector, Euler
 from typing import Union, List
 from copy import deepcopy
 
 _primitives = {
 	"cube": bpy.ops.mesh.primitive_cube_add,
 	"sphere": bpy.ops.mesh.primitive_uv_sphere_add,
@@ -44,15 +45,14 @@
 			child_meshes, child_other = _get_child_meshes(child)
 			meshes += child_meshes
 			other += child_other
 
 		return meshes, other
 
 
-
 class Mesh(BsynObject):
 	"""A mesh object. Can be a single mesh, or a hierarchy of meshes."""
 	primitive_list = list(_primitives.keys())
 	"""List of available primitives"""
 
 	def __init__(self, obj, material=None, scene=None, class_id=None):
 		"""
@@ -95,15 +95,15 @@
 		assert isinstance(class_id, int), f"Class ID must be an integer, not {type(class_id)}"
 		assert class_id >= 0, f"Class ID must be >= 0, not {class_id}"
 
 		self._object['class_id'] = class_id
 		self.scene['MAX_CLASSES'] = max(self.scene.get('MAX_CLASSES', 0), class_id)
 
 	@classmethod
-	def from_scene(cls, key:str, class_id:int=0) -> 'Mesh':
+	def from_scene(cls, key: str, class_id: int = 0) -> 'Mesh':
 		"""Create object from named object in scene.
 
 		:param key: Name of object in scene
 		:param class_id: Class ID to assign to object
 
 		:return: Mesh loaded from scene"""
 		obj = bpy.data.objects[key]
@@ -138,31 +138,31 @@
 		if scale is not None: obj.scale = scale
 		if location is not None: obj.location = location
 		if rotation_euler is not None: obj.rotation_euler = rotation_euler
 
 		return obj
 
 	@classmethod
-	def from_obj(cls, obj_loc:str, class_id:int=None,
-				 forward_axis:str='-Z', up_axis:str='Y'):
+	def from_obj(cls, obj_loc: str, class_id: int = None,
+				 forward_axis: str = '-Z', up_axis: str = 'Y'):
 		"""Load object from .obj file.
 
 		:param obj_loc: Location of .obj file
 		:param class_id: Class ID to assign to object
 		:param forward_axis: Axis to use as forward axis
 		:param up_axis: Axis to use as up axis
 
 
 		Note: we use bpy.ops.wm.obj_import instead of bpy.ops.import_scene.obj because the latter
 		causes issues with materials & vertex ordering.
 		(Changing vertex ordering makes the use of keypoints difficult.)
 		"""
 		for axis in (forward_axis, up_axis):
 			assert axis in (
-			'X', 'Y', 'Z', '-X', '-Y', '-Z'), f"Axis `{axis}` not valid, must be one of X, Y, Z, -X, -Y, -Z"
+				'X', 'Y', 'Z', '-X', '-Y', '-Z'), f"Axis `{axis}` not valid, must be one of X, Y, Z, -X, -Y, -Z"
 
 		forward_axis = forward_axis.replace('-', 'NEGATIVE_')  # e.g. -X -> NEGATIVE_X
 		up_axis = up_axis.replace('-', 'NEGATIVE_')
 
 		assert os.path.isfile(obj_loc) and obj_loc.endswith('.obj'), f"File `{obj_loc}` not a valid .obj file"
 
 		directory, fname = os.path.split(obj_loc)
@@ -176,15 +176,15 @@
 		if class_id is None:
 			class_id = default_ids['loaded_mesh']
 
 		obj = importer.imported_obj
 		return cls(obj, class_id=class_id)
 
 	@classmethod
-	def from_glb(cls, glb_loc:str, class_id:int=None):
+	def from_glb(cls, glb_loc: str, class_id: int = None):
 		"""Load object from .glb file.
 
 		:param glb_loc: Location of .glb file
 		:param class_id: Class ID to assign to object
 		"""
 		assert os.path.isfile(glb_loc) and glb_loc.endswith(
 			('.glb', '.gtlf')), f"File `{glb_loc}` not a valid .glb file"
@@ -196,20 +196,20 @@
 
 		if class_id is None:
 			class_id = default_ids['loaded_mesh']
 
 		return cls(importer.imported_obj, class_id=class_id)
 
 	@classmethod
-	def from_gltf(cls, gltf_loc:str, class_id:int=None):
+	def from_gltf(cls, gltf_loc: str, class_id: int = None):
 		"""Alias for :meth:`~blendersynth.blender.Mesh.from_glb`"""
 		return cls.from_glb(gltf_loc, class_id=class_id)
 
 	@classmethod
-	def from_fbx(cls, fbx_loc:str, class_id:int=None):
+	def from_fbx(cls, fbx_loc: str, class_id: int = None):
 		"""Load object from .fbx file.
 
 		:param fbx_loc: Location of .fbx file
 		:param class_id: Class ID to assign to object"""
 		assert os.path.isfile(fbx_loc) and fbx_loc.endswith('.fbx'), f"File `{fbx_loc}` not a valid .fbx file"
 
 		directory, fname = os.path.split(fbx_loc)
@@ -252,22 +252,36 @@
 				try:
 					vec = handle_vec(origin[i])
 					self._meshes[i].location = vec
 				except:
 					raise ValueError(
 						f"Error with setting origin. Expects a list of {len(self._meshes)} 3-long Vector. Received: {origin}")
 
-	def get_all_vertices(self, ref_frame='WORLD'):
+	def _get_all_vertices(self, ref_frame='WORLD') -> np.ndarray:
+		"""
+		Get all vertices of object, taking into account deformations.
+		:param ref_frame: LOCAL or WORLD
+		:return: Nx3 array of vertices
+		"""
+
+		depsgraph = bpy.context.evaluated_depsgraph_get()  # to account for deformations
+
 		if ref_frame not in {'LOCAL', 'WORLD'}:
 			raise ValueError(f"Invalid ref_frame: {ref_frame}. Must be one of ['LOCAL', 'WORLD']")
 
 		verts = []
 
 		for mesh in self._meshes:
-			mesh_verts = np.array([vert.co for vert in mesh.data.vertices])
+
+			# use bmesh to get vertices - this accounts for deformations in depsgraph
+			bm = bmesh.new()
+			bm.from_object(mesh, depsgraph)
+			bm.verts.ensure_lookup_table()
+			mesh_verts = np.array([x.co for x in bm.verts])
+			bm.free()
 
 			if ref_frame == 'WORLD':
 				mesh_verts = np.dot(mesh.matrix_world, np.vstack((mesh_verts.T, np.ones(mesh_verts.shape[0]))))
 
 			verts.append(mesh_verts)
 
 		verts = np.concatenate(verts, axis=1)
@@ -275,36 +289,71 @@
 		return verts[:3].T
 
 	@property
 	def materials(self):
 		return {m for mesh in self._meshes for m in mesh.data.materials}
 
 	def assign_pass_index(self, index: int):
-		"""Assign pass index to object. This can be used when mask rendering."""
+		"""Assign pass index to object. This can be used when mask rendering.
+
+		:param index: Pass index to assign"""
 		for mesh in self._meshes:
 			mesh.pass_index = index
 		return index
 
 	def assign_aov(self, aov: AOV):
-		"""Assign AOV to object. Applies to all materials"""
+		"""Assign AOV to object. Applies to all materials.
+
+		:param aov: AOV to assign"""
 		if aov not in self.assigned_aovs:
 			for material in self.materials:
 				shader_node_tree = material.node_tree
 				assert shader_node_tree is not None, "Material must have a node tree"
 				aov.add_to_shader(shader_node_tree)
 
 		self.assigned_aovs.append(aov)
 
-	def set_minimum_to(self, axis='Z', pos=0):
-		"""Set minimum of object to a given position"""
-		min_pos = self.get_all_vertices('WORLD')[:, 'XYZ'.index(axis)].min()
+	def set_minimum_to(self, axis: str = 'Z', pos: float = 0):
+		"""Set minimum of object to a given position in a given axis.
+
+		:param axis: Axis to set minimum in
+		:param pos: Position to set minimum to
+		"""
+		min_pos = self._get_all_vertices('WORLD')[:, 'XYZ'.index(axis)].min()
 		trans_vec = np.zeros(3)
 		trans_vec['XYZ'.index(axis)] = pos - min_pos
 		self.translate(trans_vec)
 
+	def clamp_in_axis(self, axis: str = 'Z', mode: str = 'min', value: float = 0):
+		"""Clamp object in a given axis to a given value - ensure that, in this axis,
+		the object never goes below (mode='min') or above (mode='max') the given value.
+
+		This can be used to ensure that an object never goes below the ground plane, for example.
+
+		:param axis: Axis to clamp in
+		:param mode: 'min' or 'max'
+		:param value: Value to clamp to
+		"""
+
+		axis = axis.upper()
+		assert axis in 'XYZ', f"Invalid axis: {axis}"
+		assert mode in {'min', 'max'}, f"Invalid mode: {mode}"
+
+		verts = self._get_all_vertices('WORLD')
+		axis_idx = 'XYZ'.index(axis)
+
+		translation = 0
+		if mode == 'min':
+			translation = max(value - verts[:, axis_idx].min(), 0)  # can only be positive
+		elif mode == 'max':
+			translation = min(value - verts[:, axis_idx].max(), 0)  # can only be negative
+
+		trans_vec = np.zeros(3)
+		trans_vec['XYZ'.index(axis)] = translation
+		self.translate(trans_vec)
 
 	def delete(self, delete_materials: bool = True):
 		"""Clear mesh from scene & mesh data.
 
 		:param delete_materials: Also delete object materials from scene"""
 		mesh_names = [m.name for m in self._meshes]
 		for mesh in self._meshes:
@@ -421,17 +470,18 @@
 				raise ValueError("No armatures found.")
 
 			return armatures[0]
 
 	def get_bone(self, bone_name: str, armature_name: str = None) -> bpy.types.PoseBone:
 		"""
 		Get bone from armature.
-		:param bone_name:
+
+		:param bone_name: Name of bone to get
 		:param armature_name: If not given, will load first available armature found
-		:return:
+		:return: PoseBone object
 		"""
 
 		armature = self.get_armature(armature_name)
 		try:
 			bone = armature.pose.bones[bone_name]
 		except KeyError:
 			raise KeyError(f"Bone `{bone_name}` not found in armature `{armature.name}`")
@@ -444,18 +494,17 @@
 		:param bone: Name of bone to pose, or PoseBone object
 		:param rotation: Euler XYZ rotation in radians
 		:param location: Location in object space
 		:param armature_name: Name of armature to use. If not given, will use first armature found.
 		:param frame: Frame to set pose on. If given, will insert keyframe here.
 		"""
 
-
 		with SelectObjects(self._meshes + self._other_objects):
 			armature = self.get_armature(armature_name)
-			with SetMode('POSE', object = armature):
+			with SetMode('POSE', object=armature):
 				if isinstance(bone, str):
 					bone = self.get_bone(bone, armature_name)
 
 				bone.rotation_mode = 'XYZ'
 				if rotation is not None:
 					bone.rotation_euler = rotation
 					if frame is not None:
```

### Comparing `blendersynth-0.0.5/blendersynth/blender/render.py` & `blendersynth-0.0.6/blendersynth/blender/render.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/blender/utils.py` & `blendersynth-0.0.6/blendersynth/blender/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,34 @@
 import mathutils
 from typing import Union, List, Tuple
 
 # define Blender Array type
 blender_array_type = Union[List[float], mathutils.Vector, np.ndarray, Tuple[float, ...], Tuple[int, ...]]
 blender_array_or_scalar = Union[blender_array_type, int, float]
 
+def _quaternion_equal(a: mathutils.Quaternion, b: mathutils.Quaternion, tol=1e-6):
+	"""Check if two quaternion rotations are functionally equal"""
+	return abs(a.dot(b)) > 1 - tol
+
+def _euler_equal(a: mathutils.Euler, b: mathutils.Euler, tol=1e-6):
+	"""Check if two euler rotations are equal"""
+	return _quaternion_equal(a.to_quaternion(), b.to_quaternion(), tol=tol)
+
 def _euler_from(a: mathutils.Euler, b: mathutils.Euler):
 	"""Get euler rotation from a to b"""
-	return (b.to_matrix() @ a.to_matrix().inverted()).to_euler()
+	return (a.to_quaternion().rotation_difference(b.to_quaternion())).to_euler('XYZ')
 
 
 def _euler_add(a: mathutils.Euler, b: mathutils.Euler):
 	"""Compute euler rotation of a, followed by b"""
-	return (a.to_matrix() @ b.to_matrix()).to_euler()
+	return (a.to_quaternion() @ b.to_quaternion()).to_euler('XYZ')
+
+def _euler_invert(a: mathutils.Euler):
+	"""Invert euler rotation"""
+	return a.to_quaternion().inverted().to_euler('XYZ')
 
 
 class GetNewObject():
 	"""Context manager for getting the newly imported object(s) to the scene.
 
 	On exit, will return the newly imported object(s).
```

### Comparing `blendersynth-0.0.5/blendersynth/blender/world.py` & `blendersynth-0.0.6/blendersynth/blender/world.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/file/dataset_inputs.py` & `blendersynth-0.0.6/blendersynth/file/dataset_inputs.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/file/frames_to_video.py` & `blendersynth-0.0.6/blendersynth/file/frames_to_video.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/file/tempfiles.py` & `blendersynth-0.0.6/blendersynth/file/tempfiles.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/run/blender_threading.py` & `blendersynth-0.0.6/blendersynth/run/blender_threading.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/run/run.py` & `blendersynth-0.0.6/blendersynth/run/run.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/run/run_this_script.py` & `blendersynth-0.0.6/blendersynth/run/run_this_script.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/utils/blender_importer.py` & `blendersynth-0.0.6/blendersynth/utils/blender_importer.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/utils/blender_setup/blender_locator.py` & `blendersynth-0.0.6/blendersynth/utils/blender_setup/blender_locator.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/utils/blender_setup/check_blender_install.py` & `blendersynth-0.0.6/blendersynth/utils/blender_setup/check_blender_install.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.5/blendersynth/utils/node_arranger.py` & `blendersynth-0.0.6/blendersynth/utils/node_arranger.py`

 * *Files 16% similar despite different names*

```diff
@@ -95,31 +95,35 @@
 	for node in node_island:
 		node['depth'] -= min_depth
 
 	return node_island
 
 
 def tidy_tree(node_tree: bpy.types.NodeTree, dX: int = 400, dY: int = 200):
-	"""Search through tree, positioning nodes in a grid based on their depth and connectivity.
+    """Search through tree, positioning nodes in a grid based on their depth and connectivity.
 
-	:param node_tree: node tree to tidy
-	:param dX: horizontal distance between nodes
-	:param dY: vertical distance between nodes"""
+    :param node_tree: node tree to tidy
+    :param dX: horizontal distance between nodes
+    :param dY: vertical distance between nodes"""
+
+    nodes = node_tree.nodes
+    islands = split_to_islands(nodes)
+
+    y = 0  # track running height to manage multiple islands
+
+    height = defaultdict(int)  # track height of each depth level
+    for island in islands:
+        island = calc_depth(island)
+
+        # want to center each depth level, so set heights accordingly
+        for i in range(max(node['depth'] for node in island) + 1):
+            # Adjusting the initial height calculation to account for node sizes.
+            depth_nodes = [node for node in island if node['depth'] == i]
+            total_height_for_depth = sum(node.dimensions.y for node in depth_nodes)
+            spacing_needed = dY * (len(depth_nodes) - 1)
+            height[i] = -(total_height_for_depth + spacing_needed) / 2
+
+        for node in island:
+            node.location = (node['depth'] * dX, y + height[node['depth']])
+            height[node['depth']] += node.dimensions.y + dY  # Incrementing by the node's height
 
-	nodes = node_tree.nodes
-	islands = split_to_islands(nodes)
-
-	y = 0  # track running height to manage multiple islands
-
-	height = defaultdict(int)  # track height of each depth level
-	for island in islands:
-		island = calc_depth(island)
-
-		# want to centre each depth level, so set heights accordingly
-		for i in range(max(node['depth'] for node in island) + 1):
-			height[i] = - dY * sum(node['depth'] == i for node in island) / 2
-
-		for node in island:
-			node.location = (node['depth'] * dX, y + height[node['depth']])
-			height[node['depth']] += dY
-
-		y += max(height.values()) + dY
+        y += max(height.values()) + dY
```

### Comparing `blendersynth-0.0.5/blendersynth/utils/types.py` & `blendersynth-0.0.6/blendersynth/utils/types.py`

 * *Files identical despite different names*

