# Comparing `tmp/xlab-util-0.7.tar.gz` & `tmp/xlab-util-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlab-util-0.7.tar", last modified: Tue Aug  8 02:40:51 2023, max compression
+gzip compressed data, was "xlab-util-0.8.tar", last modified: Tue Aug  8 03:08:18 2023, max compression
```

## Comparing `xlab-util-0.7.tar` & `xlab-util-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.318125 xlab-util-0.7/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 02:40:51.314125 xlab-util-0.7/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.7/README.md
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-08 02:40:51.318125 xlab-util-0.7/setup.cfg
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-08 02:40:43.000000 xlab-util-0.7/setup.py
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.310125 xlab-util-0.7/xlab_util.egg-info/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-08 02:40:51.000000 xlab-util-0.7/xlab_util.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 02:40:51.314125 xlab-util-0.7/xlabutil/
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      255 2023-08-08 02:40:03.000000 xlab-util-0.7/xlabutil/__init__.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.7/xlabutil/base.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.7/xlabutil/inference.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2093 2023-08-08 02:40:17.000000 xlab-util-0.7/xlabutil/result.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.7/xlabutil/type.py
--rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      967 2023-08-08 02:35:38.000000 xlab-util-0.7/xlabutil/util.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.394149 xlab-util-0.8/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:08:18.394149 xlab-util-0.8/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       11 2023-08-01 07:16:54.000000 xlab-util-0.8/README.md
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       38 2023-08-08 03:08:18.394149 xlab-util-0.8/setup.cfg
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      203 2023-08-08 03:08:06.000000 xlab-util-0.8/setup.py
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.386150 xlab-util-0.8/xlab_util.egg-info/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      149 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      263 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        1 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        9 2023-08-08 03:08:18.000000 xlab-util-0.8/xlab_util.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)        0 2023-08-08 03:08:18.390149 xlab-util-0.8/xlabutil/
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      255 2023-08-08 02:40:03.000000 xlab-util-0.8/xlabutil/__init__.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      407 2023-08-01 07:32:55.000000 xlab-util-0.8/xlabutil/base.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     1560 2023-08-07 07:01:15.000000 xlab-util-0.8/xlabutil/inference.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)     2771 2023-08-08 03:07:32.000000 xlab-util-0.8/xlabutil/result.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)       83 2023-08-04 07:12:05.000000 xlab-util-0.8/xlabutil/type.py
+-rw-r--r--   0 PJLAB\liujinyao (409470278) PJLAB\domain^users (409469441)      967 2023-08-08 02:35:38.000000 xlab-util-0.8/xlabutil/util.py
```

### Comparing `xlab-util-0.7/xlabutil/inference.py` & `xlab-util-0.8/xlabutil/inference.py`

 * *Files identical despite different names*

### Comparing `xlab-util-0.7/xlabutil/result.py` & `xlab-util-0.8/xlabutil/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,52 @@
-import numpy as np
+import base64
+import dataclasses
 
+from PIL import Image
+from io import BytesIO
 from dataclasses import dataclass, field
-from typing import Optional, List
+from typing import Optional, List, Union
+
+import numpy as np
+
+
+@dataclass
+class Visual():
+
+    # visualization
+    visualization: Optional[str] = field(default_factory=lambda: "")
+
+    def set_visual(self, input: Union[List, Image.Image]):
+        if isinstance(input, List):
+            img_byte = BytesIO()
+            img = Image.fromarray(input)
+            img.save(img_byte, format="jpeg")
+            visual = base64.b64encode(img_byte.getvalue()).decode('utf-8')
+        elif isinstance(input, Image.Image):
+            img_byte = BytesIO()
+            input.save(img_byte, format="jpeg")
+            visual = base64.b64encode(img_byte.getvalue()).decode('utf-8')
+        else:
+            visual = input if isinstance(input, str) else None
+
+        self.visualization = visual
 
 
 @dataclass
 class ClassificationResult:
     """The result of image classification."""
     # The predicted label (category index)
     label: int
     # The confidence score of the prediction
     score: Optional[float]
     # The predicted category name
     category: Optional[str]
     # The scores of all categories
     full_scores: Optional[np.ndarray]
-    # visualization
-    visualization: Optional[str]
+
 
 
 @dataclass
 class InstanceMask:
     """The dataclass of the instance segmentation mask."""
     size: List[int]  # The size of the mask
     counts: str  # The RLE-encoded mask
@@ -47,17 +73,15 @@
     # The pose estimation results of all detected objects
     poses: Optional[List[InstancePose]]
     # visualization
     visualization: Optional[str]
 
 
 @dataclass
-class PoseEstimationResult:
+class PoseEstimationResult(Visual):
     """The result of object detection."""
     # The bounding boxes of all detected objects
     bboxes: Optional[List[List[int]]] = field(default_factory=lambda: [])
     # The scores of all detected objects
     scores: Optional[List[float]] = field(default_factory=lambda: [])
     # The pose estimation results of all detected objects
-    poses: Optional[List[InstancePose]] = field(default_factory=lambda: [])
-    # visualization
-    visualization: Optional[str] = field(default_factory=lambda: "")
+    poses: Optional[List[InstancePose]] = field(default_factory=lambda: [])
```

### Comparing `xlab-util-0.7/xlabutil/util.py` & `xlab-util-0.8/xlabutil/util.py`

 * *Files identical despite different names*

