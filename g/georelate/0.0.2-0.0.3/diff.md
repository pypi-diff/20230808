# Comparing `tmp/georelate-0.0.2.tar.gz` & `tmp/georelate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georelate-0.0.2.tar", max compression
+gzip compressed data, was "georelate-0.0.3.tar", max compression
```

## Comparing `georelate-0.0.2.tar` & `georelate-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-17 15:20:35.379129 georelate-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-17 15:20:35.379892 georelate-0.0.2/georelate/__init__.py
--rw-r--r--   0        0        0     9875 2023-05-17 22:31:48.375360 georelate-0.0.2/georelate/_distance.py
--rw-r--r--   0        0        0      189 2023-05-17 15:20:35.380043 georelate-0.0.2/georelate/demo.py
--rw-r--r--   0        0        0      451 2023-05-17 22:32:58.427091 georelate-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 georelate-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-17 15:20:35.379129 georelate-0.0.3/LICENSE
+-rw-r--r--   0        0        0      113 2023-08-08 20:35:28.419553 georelate-0.0.3/georelate/__init__.py
+-rw-r--r--   0        0        0    10679 2023-08-08 20:35:28.420145 georelate-0.0.3/georelate/_distance.py
+-rw-r--r--   0        0        0     1422 2023-08-08 20:35:28.420727 georelate-0.0.3/georelate/data.py
+-rw-r--r--   0        0        0      559 2023-08-08 20:35:28.423000 georelate-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 georelate-0.0.3/PKG-INFO
```

### Comparing `georelate-0.0.2/LICENSE` & `georelate-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `georelate-0.0.2/georelate/_distance.py` & `georelate-0.0.3/georelate/_distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -201,14 +201,16 @@
     right_id=None,
     left_lat="lat",
     left_lon="lon",
     right_lat="lat",
     right_lon="lon",
     suffixes=("_left", "_right"),
     k_closest=None,
+    include_left_coords=False,
+    include_right_coords=False,
 ):
 
     """_summary_
 
     Args:
         left (DataFrame): Left DataFrame to merge with. Assumes the index is an id.
         right (DataFrame): Right DataFrame to merge with. Assumes the index is an id.
@@ -231,14 +233,20 @@
             Pass a value of None instead of a string to indicate that the column name from
             left or right should be left as-is, with no suffix.
             At least one of the values must not be None.
             Defaults to ("_left", "_right").
         k_closest (int, optional): Specifies the number of nearest observations
             for the right DataFrame to include in the output DataFrame
             for each observations in the left DataFrame.
+        include_left_coords (bool, optional): Specifies whether to include the coordinates
+            from the left DataFrame in the results.
+            Defaults to False.
+        include_right_coords (bool, optional): Specifies whether to include the coordinates
+            from the right DataFrame in the results.
+            Defaults to False.
 
     Returns:
         DataFrame: The design matrix.
     """
 
     left_id_key, right_id_key = _get_id_keys(
         left=left, right=right, left_id=left_id, right_id=right_id
@@ -256,33 +264,35 @@
         left_lat=left_lat,
         left_lon=left_lon,
         right_lat=right_lat,
         right_lon=right_lon,
         suffixes=suffixes,
     )
 
-    left_df = left.reset_index()
-    right_df = right.reset_index()
+    left_df = left.reset_index() if left_id is None else left
+    right_df = right.reset_index() if right_id is None else right
 
     k_closest_join_df = _k_closest(
         df=distance_df,
         left_id=left_id_key_w_suffix,
         right_id=right_id_key_w_suffix,
         k=k_closest,
     )
 
     out_df = left_df.copy()
 
     if k_closest:
+
         k_closest_join_df = _k_closest(
             df=distance_df,
             left_id=left_id_key_w_suffix,
             right_id=right_id_key_w_suffix,
             k=k_closest,
         )
+
         assert set(k_closest_join_df[left_id_key_w_suffix].values) == set(
             left_df[left_id_key].values
         )
         out_df = pd.merge(
             out_df,
             k_closest_join_df,
             left_on=left_id_key,
@@ -290,16 +300,26 @@
         )
 
         for j in range(k_closest):
             # this is a false warning,
             # because I'm passing a different callback,
             # for each iteration
             # pylint:disable=cell-var-from-loop
-            right_k_df = right_df.rename(columns=lambda col: f"{col}_{j + 1}_closest")
+            right_k_df = right_df.copy()
+
+            if not include_right_coords:
+                # print(f"{k_closest_join_df.columns=}")
+                right_k_df = right_k_df.drop([right_lat, right_lon], axis="columns")
+
+            right_k_df = right_k_df.rename(columns=lambda col: f"{col}_{j + 1}_closest")
+
             out_df = pd.merge(
                 out_df,
                 right_k_df,
                 left_on=f"{right_id_key_w_suffix}_{j + 1}_closest",
                 right_on=f"{right_id_key}_{j + 1}_closest",
             )
 
+    if not include_left_coords:
+        out_df = out_df.drop([left_lat, left_lon], axis="columns")
+
     return out_df
```

