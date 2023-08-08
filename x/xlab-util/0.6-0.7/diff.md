# Comparing `tmp/xlab-util-0.6.tar.gz` & `tmp/xlab-util-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlab-util-0.6.tar", last modified: Mon Aug  7 11:12:21 2023, max compression
+gzip compressed data, was "xlab-util-0.7.tar", last modified: Tue Aug  8 02:40:51 2023, max compression
```

## Comparing `xlab-util-0.6.tar` & `xlab-util-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:12:21.592330 xlab-util-0.6/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.6/README.md
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-07 11:12:21.592330 xlab-util-0.6/setup.cfg
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-07 11:12:16.000000 xlab-util-0.6/setup.py
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/xlab_util.egg-info/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-07 11:12:21.000000 xlab-util-0.6/xlab_util.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-07 11:12:21.592330 xlab-util-0.6/xlabutil/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      232 2023-08-07 11:12:10.000000 xlab-util-0.6/xlabutil/__init__.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.6/xlabutil/base.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.6/xlabutil/inference.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1870 2023-08-07 11:07:20.000000 xlab-util-0.6/xlabutil/result.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.6/xlabutil/type.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      749 2023-08-01 07:33:04.000000 xlab-util-0.6/xlabutil/util.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.318125 xlab-util-0.7/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 02:40:51.314125 xlab-util-0.7/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.7/README.md
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-08 02:40:51.318125 xlab-util-0.7/setup.cfg
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-08 02:40:43.000000 xlab-util-0.7/setup.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.310125 xlab-util-0.7/xlab_util.egg-info/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.314125 xlab-util-0.7/xlabutil/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      255 2023-08-08 02:40:03.000000 xlab-util-0.7/xlabutil/__init__.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.7/xlabutil/base.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.7/xlabutil/inference.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2093 2023-08-08 02:40:17.000000 xlab-util-0.7/xlabutil/result.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.7/xlabutil/type.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      967 2023-08-08 02:35:38.000000 xlab-util-0.7/xlabutil/util.py
```

### Comparing `xlab-util-0.6/xlabutil/inference.py` & `xlab-util-0.7/xlabutil/inference.py`

 * *Files identical despite different names*

### Comparing `xlab-util-0.6/xlabutil/result.py` & `xlab-util-0.7/xlabutil/result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional, List
 
 
 @dataclass
 class ClassificationResult:
     """The result of image classification."""
     # The predicted label (category index)
@@ -25,16 +25,16 @@
     size: List[int]  # The size of the mask
     counts: str  # The RLE-encoded mask
 
 
 @dataclass
 class InstancePose:
     """The dataclass of the pose (keypoint) information of an object."""
-    keypoints: List[List[float]]  # The coordinates of all keypoints
-    keypoint_scores: Optional[List[float]]  # The scores of all keypoints
+    keypoints: List[List[float]] = field(default_factory=lambda: [])  # The coordinates of all keypoints
+    keypoint_scores: Optional[List[float]] = field(default_factory=lambda: [])  # The scores of all keypoints
 
 
 @dataclass
 class DetectionResult:
     """The result of object detection."""
     # The bounding boxes of all detected objects
     bboxes: Optional[List[List[int]]]
@@ -50,14 +50,14 @@
     visualization: Optional[str]
 
 
 @dataclass
 class PoseEstimationResult:
     """The result of object detection."""
     # The bounding boxes of all detected objects
-    bboxes: Optional[List[List[int]]]
+    bboxes: Optional[List[List[int]]] = field(default_factory=lambda: [])
     # The scores of all detected objects
-    scores: Optional[List[float]]
+    scores: Optional[List[float]] = field(default_factory=lambda: [])
     # The pose estimation results of all detected objects
-    poses: Optional[List[InstancePose]]
+    poses: Optional[List[InstancePose]] = field(default_factory=lambda: [])
     # visualization
-    visualization: Optional[str]
+    visualization: Optional[str] = field(default_factory=lambda: "")
```

