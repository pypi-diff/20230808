# Comparing `tmp/image2layout_computer_vision-0.1.4.tar.gz` & `tmp/image2layout_computer_vision-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.1.4.tar", last modified: Mon Aug  7 09:24:05 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.5.tar", last modified: Mon Aug  7 09:53:32 2023, max compression
```

## Comparing `image2layout_computer_vision-0.1.4.tar` & `image2layout_computer_vision-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/
--rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.4/LICENSE
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.4/README.md
--rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 09:23:41.000000 image2layout_computer_vision-0.1.4/pyproject.toml
--rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/setup.cfg
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/
--rw-rw-r--   0 test      (1001) test      (1001)      573 2023-08-07 09:23:20.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/__init__.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/
--rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/main.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/
--rw-rw-r--   0 test      (1001) test      (1001)      211 2023-08-07 07:13:29.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)    17049 2023-08-07 08:43:47.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/imagebox.py
--rw-rw-r--   0 test      (1001) test      (1001)     3080 2023-08-07 07:13:37.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/main.py
--rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
--rw-rw-r--   0 test      (1001) test      (1001)     2261 2023-08-07 07:31:11.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_paddle.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.779772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/
--rw-rw-r--   0 test      (1001) test      (1001)      333 2023-08-07 09:23:10.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/__init__.py
--rw-rw-r--   0 test      (1001) test      (1001)     7703 2023-08-07 09:06:09.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/annotation.py
--rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/color_system.py
--rw-rw-r--   0 test      (1001) test      (1001)     6603 2023-08-07 09:12:59.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/imaging.py
--rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/pixel_mask.py
--rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/timing.py
-drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:24:05.775772 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/
--rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 09:24:05.000000 image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.4/src/sandbox.py
--rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.4/src/sandbox_color.py
--rw-rw-r--   0 test      (1001) test      (1001)     1514 2023-08-07 09:18:57.000000 image2layout_computer_vision-0.1.4/src/sandbox_ocr.py
--rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.4/src/test_color.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.404372 image2layout_computer_vision-0.1.5/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.5/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:53:32.404372 image2layout_computer_vision-0.1.5/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2224 2023-08-07 06:13:00.000000 image2layout_computer_vision-0.1.5/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-07 09:53:10.000000 image2layout_computer_vision-0.1.5/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-07 09:53:32.404372 image2layout_computer_vision-0.1.5/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.400372 image2layout_computer_vision-0.1.5/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.400372 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      573 2023-08-07 09:23:20.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.400372 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.404372 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      211 2023-08-07 07:13:29.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    17572 2023-08-07 09:50:40.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3080 2023-08-07 07:13:37.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2261 2023-08-07 07:31:11.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.404372 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      333 2023-08-07 09:23:10.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7703 2023-08-07 09:06:09.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6603 2023-08-07 09:12:59.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-07 09:53:32.400372 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2794 2023-08-07 09:53:32.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-07 09:53:32.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-07 09:53:32.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-07 09:53:32.000000 image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.5/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.5/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1581 2023-08-07 09:50:48.000000 image2layout_computer_vision-0.1.5/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.5/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.1.4/LICENSE` & `image2layout_computer_vision-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/PKG-INFO` & `image2layout_computer_vision-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.1.4
+Version: 0.1.5
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.4/README.md` & `image2layout_computer_vision-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/pyproject.toml` & `image2layout_computer_vision-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/__init__.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/color_extract/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,26 +24,27 @@
                 hdist_max=hdist_max,
                 vdist_max=vdist_max,
                 height_ratio_min=height_ratio_min,
             )
         
         heights = np.array([boxb[3] - boxb[1], boxa[3] - boxa[1]])
         height_max = max(np.max(heights), 1)
+        height_min = max(np.min(heights), 1)
         height_ratio = np.min(heights) / height_max
         
         hdists = np.abs([
             *(boxb - boxa)[[0, 2]],
             boxb[[0, 2]].mean() - boxa[[0, 2]].mean(),
         ])
         vdists = np.abs(boxb - boxa)[[1, 3]]
         # hdist, vdist, height_ratio, height_max
         
         return all([
-            np.min(hdists) / height_max < hdist_max,
-            np.min(vdists) / height_max < vdist_max,
+            np.min(hdists) / height_min < hdist_max,
+            np.min(vdists) / height_min < vdist_max,
             height_ratio > height_ratio_min,
         ])
     
     @classmethod
     def box_containing_match(cls, boxa, boxb, area_threshold=0.8):
         _boxes = np.array([boxa, boxb]).reshape(2, 2, 2)
         inter_box = np.concatenate([
@@ -54,17 +55,17 @@
         
         inter_area = np.prod(inter_wh)
         areas = np.clip(np.prod(_boxes[:, 1] - _boxes[:, 0], axis=-1), 1.0, None)
         inter_max_ratio = np.max(inter_area / areas)
         return inter_max_ratio >= area_threshold
     
     @classmethod
-    def group_texts_by_match_fn(cls, boxes: np.ndarray, fn, sort_index=None, **kwargs):
+    def group_texts_by_match_fn(cls, boxes: np.ndarray, match_fn, sort_index=None, **kwargs):
         # boxes should be sorted
-        assert callable(fn)
+        assert callable(match_fn)
         assert isinstance(boxes, np.ndarray)
         assert len(boxes.shape) == 2
         assert boxes.shape[-1] == 4
         
         count = len(boxes)
         assert count > 0
         
@@ -91,15 +92,15 @@
             
             head_index = start_index
             linked_indices = [head_index]
             
             for next_index in range(head_index+1, count):
                 if next_index in matched_indices:
                     continue
-                if fn(sorted_boxes[head_index], sorted_boxes[next_index], **kwargs):
+                if match_fn(sorted_boxes[head_index], sorted_boxes[next_index], **kwargs):
                     linked_indices.append(next_index)
                     head_index = next_index
             
             linked_groups.append(linked_indices)
             matched_indices.update(linked_indices)
             remaining_indices.difference_update(linked_indices)
         
@@ -380,41 +381,58 @@
         return img_anno
     
     def to_grouped_imageboxes(self, **kwargs):
         '''group boxes with `grouped_boxes` from self and return an ImageBoxes with grouped boxes
         '''
         
         if len(self.boxes) > 0:
-            boxes_grouped_final = self.group_boxes(self.boxes, **kwargs)
+            _, indices_original = self.group_boxes(self.boxes, **kwargs)
         else:
-            boxes_grouped_final = np.array(self.boxes)
+            _ = []
+            indices_original = []
+        
+        boxes_grouped_nested = [
+            [
+                list(self.boxes[index])
+                for index in indices
+            ]
+            for indices in indices_original
+        ]
+        boxes_grouped_flat = [
+            index
+            for indices in indices_original
+            for index in indices
+        ]
         
         imageboxes_grouped = ImageBoxes(
-            boxes=boxes_grouped_final,
+            boxes=boxes_grouped_nested,
             image=self.image.copy(),
         )
-        imageboxes_grouped.set_texts(self.texts)
+        imageboxes_grouped.set_texts([
+            self.texts[index]
+            for index in boxes_grouped_flat
+        ])
         return imageboxes_grouped
     
     @classmethod
     def group_boxes(cls,
                 boxes:Union[np.ndarray, list],
                 
                 merge_lines:bool=False,
                 line_dist_max:float=1.0,
                 line_dist_min:float=-0.1,
                 line_iou_min:float=0.4,
                 
                 merge_rows:bool=True,
-                row_hdist_max:float=0.4,
-                row_vdist_max:float=1.8,
+                row_hdist_max:float=0.5,
+                row_vdist_max:float=1.4,
                 row_height_ratio_min:float=0.8,
                 
                 merge_containing:bool=True,
-                ) -> list:
+                ) -> Tuple[List, List]:
         '''processes self.boxes and returns a new ImageBoxes object with grouped boxes
         Parameters:
             boxes
             merge_lines      (bool) False - whether to merge lines
             merge_rows       (bool) True - whether to merge rows
             merge_containing (bool) True - whether to merge overlaping boxes
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
@@ -432,53 +450,53 @@
         
         merged_dfs = []
         merged_boxes = np.array(_boxes)
         
         if merge_lines:
             _df_merged = BoxMerge.group_texts_by_match_fn(
                 merged_boxes,
-                fn=BoxMerge.same_line_match,
+                match_fn=BoxMerge.same_line_match,
                 sort_index=0,
                 dist_max=line_dist_max,
                 dist_min=line_dist_min,
                 iou_min=line_iou_min,
             )
             merged_dfs.append(_df_merged)
             merged_boxes = np.array(_df_merged['box'].tolist())
         
         if merge_rows:
             _df_merged = BoxMerge.group_texts_by_match_fn(
                 merged_boxes,
-                fn=BoxMerge.same_column_match,
+                match_fn=BoxMerge.same_column_match,
                 sort_index=1,
                 hdist_max=row_hdist_max,
                 vdist_max=row_vdist_max,
                 height_ratio_min=row_height_ratio_min,
             )
             merged_dfs.append(_df_merged)
             merged_boxes = np.array(_df_merged['box'].tolist())
         
         if merge_containing:
             _df_merged = BoxMerge.group_texts_by_match_fn(
                 merged_boxes,
-                fn=BoxMerge.box_containing_match,
+                match_fn=BoxMerge.box_containing_match,
             )
             merged_dfs.append(_df_merged)
             merged_boxes = np.array(_df_merged['box'].tolist())
         
         indices_original = cls.get_original_nested_indices(merged_dfs)
         
         boxes_nested_final = [
             [
                 _boxes[i].tolist()
                 for i in _indices
             ]
             for _indices in indices_original
         ]
-        return boxes_nested_final
+        return boxes_nested_final, indices_original
     
     @classmethod
     def get_original_nested_indices(cls, df_groups: list) -> list:
         indices_nested = [
             [
                 v.tolist()
                 for v in _df['indices']
```

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/main.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/ocr/model_paddle.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/ocr/model_paddle.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/annotation.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/imaging.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/imaging.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision/utils/timing.py` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision/utils/timing.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.1.4
+Version: 0.1.5
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `image2layout_computer_vision-0.1.4/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.5/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/sandbox.py` & `image2layout_computer_vision-0.1.5/src/sandbox.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/sandbox_color.py` & `image2layout_computer_vision-0.1.5/src/sandbox_color.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.1.4/src/sandbox_ocr.py` & `image2layout_computer_vision-0.1.5/src/sandbox_ocr.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     ImageTransform,
 )
 
 # %%
 img_fp = '/home/test/code/image2layout_computer_vision/data/inputs/Coterie benefits.png'
 img_fp = '/home/test/code/image2layout_computer_vision/data/inputs/Screenshot 2023-07-13 at 11.03.48.png'
 img = Image.open(img_fp).convert('RGB')
-img
+# img
 
 # %%
 data_merged, data_raw = detect_text_full(
     img,
-    row_hdist_max=0.15,
-    row_vdist_max=1.8,
-    row_height_ratio_min=0.85,
+#     row_hdist_max=0.6,
+#     row_vdist_max=1.4,
+#     row_height_ratio_min=0.8,
 )
 data_merged, data_raw
 
 img_anno_merged = AnnoDraw.draw_anno_text_overlay(
     img=img,
     boxes=[v['box'] for v in data_merged],
     texts=[v['text'] for v in data_merged],
@@ -48,22 +48,25 @@
     # color='#00FF88',
     color_text='#000000',
     # font='OpenSans_Condensed-Medium.ttf',
     # font='data/OpenSans_Condensed-Medium.ttf',
     opacity=0.75,
 )
 
+img_anno_merged.convert('RGB')
+
+# %%
 img_anno_dual = ImageTransform.concatenate(
+    [img_anno_merged],
     # [img_anno_merged, img_anno_raw],
     # [img, img_anno_merged],
-    [img, img_anno_raw, img_anno_merged],
+    # [img, img_anno_raw, img_anno_merged],
     columns=1,
     spacing=10,
 )
-
 img_anno_dual.convert('RGB')
 
 # %%
```

### Comparing `image2layout_computer_vision-0.1.4/src/test_color.py` & `image2layout_computer_vision-0.1.5/src/test_color.py`

 * *Files identical despite different names*

