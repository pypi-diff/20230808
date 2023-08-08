# Comparing `tmp/pygeoops-0.3.0a0.tar.gz` & `tmp/pygeoops-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.3.0a0.tar", last modified: Tue Aug  1 13:49:37 2023, max compression
+gzip compressed data, was "pygeoops-0.3.0a1.tar", last modified: Tue Aug  8 13:46:57 2023, max compression
```

## Comparing `pygeoops-0.3.0a0.tar` & `pygeoops-0.3.0a1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.987353 pygeoops-0.3.0a0/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_paramvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/_view_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pygeoops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 13:49:37.000000 pygeoops-0.3.0a0/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:49:37.991353 pygeoops-0.3.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_paramvalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_shapely.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-01 13:49:24.000000 pygeoops-0.3.0a0/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:57.598403 pygeoops-0.3.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-08 13:46:57.598403 pygeoops-0.3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:57.594404 pygeoops-0.3.0a1/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_paramvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/_view_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pygeoops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:57.594404 pygeoops-0.3.0a1/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-08 13:46:57.000000 pygeoops-0.3.0a1/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-08 13:46:57.000000 pygeoops-0.3.0a1/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:46:57.000000 pygeoops-0.3.0a1/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-08 13:46:57.000000 pygeoops-0.3.0a1/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 13:46:57.000000 pygeoops-0.3.0a1/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 13:46:57.598403 pygeoops-0.3.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:46:57.598403 pygeoops-0.3.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_paramvalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_shapely.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-08-08 13:46:47.000000 pygeoops-0.3.0a1/tests/test_view_angles.py
```

### Comparing `pygeoops-0.3.0a0/LICENSE.txt` & `pygeoops-0.3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/PKG-INFO` & `pygeoops-0.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.3.0a0/README.md` & `pygeoops-0.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/__init__.py` & `pygeoops-0.3.0a1/pygeoops/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_centerline.py` & `pygeoops-0.3.0a1/pygeoops/_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_difference.py` & `pygeoops-0.3.0a1/pygeoops/_difference.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_general.py` & `pygeoops-0.3.0a1/pygeoops/_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_grid.py` & `pygeoops-0.3.0a1/pygeoops/_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_paramvalidation.py` & `pygeoops-0.3.0a1/pygeoops/_paramvalidation.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_simplify.py` & `pygeoops-0.3.0a1/pygeoops/_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,20 @@
             geometry=geometry,
             tolerance=tolerance,
             algorithm=algorithm,
             lookahead=lookahead,
             keep_points_on=keep_points_on,
         )
 
+    # If the algorithm is rdp and no keep_points_on, use the faster shapely
+    if algorithm == "rdp" and keep_points_on is None:
+        return shapely.simplify(
+            geometry, tolerance=tolerance, preserve_topology=preserve_topology
+        )
+
     # If input is arraylike, apply to all elements
     if hasattr(geometry, "__len__"):
         result = np.array(
             [
                 _simplify(
                     geometry=geom,
                     tolerance=tolerance,
@@ -123,17 +129,23 @@
     lookahead: int = 8,
     preserve_topology: bool = True,
     keep_points_on: Optional[BaseGeometry] = None,
 ) -> Optional[BaseGeometry]:
     # Init:
     if geometry is None:
         return None
+    algorithm = algorithm.lower()
+
+    # If the algorithm is rdp and no keep_points_on, use shapely
+    if algorithm == "rdp" and keep_points_on is None:
+        return shapely.simplify(
+            geometry, tolerance=tolerance, preserve_topology=preserve_topology
+        )
 
     # Check algorythm
-    algorithm = algorithm.lower()
     simplify_lookahead_points = False
     if algorithm in ["rdp", "vw"]:
         if not HAS_SIMPLIFICATION:
             raise ImportError(
                 "To use simplify_ext using rdp or vw, first install simplification "
                 "with 'pip install simplification'"
             )
```

### Comparing `pygeoops-0.3.0a0/pygeoops/_simplify_lang.py` & `pygeoops-0.3.0a1/pygeoops/_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_simplify_topo.py` & `pygeoops-0.3.0a1/pygeoops/_simplify_topo.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         The simplified geometry/geometries. If the input is a GeoSeries the result is
         returned like that, otherwise the result is returned as an ndarray.
     """
     if geometry is None:
         return None
     algorithm = algorithm.lower()
 
-    # If input isn't arraylike or if the arraylike only has one element, just apply
-    # simplify as creating a topology first is useless.
+    # If input isn't arraylike or if the arraylike only has one element, creating a
+    # topology first is useless.
     if not hasattr(geometry, "__len__") or len(geometry) <= 1:
         return pygeoops.simplify(
             geometry=geometry,
             tolerance=tolerance,
             algorithm=algorithm,
             lookahead=lookahead,
             preserve_topology=True,
@@ -81,22 +81,29 @@
             action="ignore", category=RuntimeWarning, message=message
         )
         topo = topojson.Topology(data=geometries, prequantize=False)
 
     # Simplify all arcs/vectors/boundaries of the topologies
     # ------------------------------------------------------
     topolines = shapely.MultiLineString(topo.output["arcs"])
-    topolines_simpl = pygeoops.simplify(
-        geometry=topolines,
-        tolerance=tolerance,
-        algorithm=algorithm,
-        lookahead=lookahead,
-        keep_points_on=keep_points_on,
-        preserve_topology=True,
-    )
+
+    # If the algorithm is rdp and no keep_points_on, use shapely
+    if algorithm == "rdp" and keep_points_on is None:
+        topolines_simpl = shapely.simplify(
+            geometry=topolines, tolerance=tolerance, preserve_topology=True
+        )
+    else:
+        topolines_simpl = pygeoops.simplify(
+            geometry=topolines,
+            tolerance=tolerance,
+            algorithm=algorithm,
+            lookahead=lookahead,
+            keep_points_on=keep_points_on,
+            preserve_topology=True,
+        )
     assert topolines_simpl is not None
 
     # Copy the results of the simplified lines back to the topology arcs
     if algorithm in ["lang", "lang+"]:
         # For LANG, a simple copy is OK
         assert isinstance(topolines_simpl, shapely.MultiLineString)
         topo.output["arcs"] = [list(geom.coords) for geom in topolines_simpl.geoms]
```

### Comparing `pygeoops-0.3.0a0/pygeoops/_types.py` & `pygeoops-0.3.0a1/pygeoops/_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops/_view_angles.py` & `pygeoops-0.3.0a1/pygeoops/_view_angles.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pygeoops.egg-info/PKG-INFO` & `pygeoops-0.3.0a1/pygeoops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.3.0a0/pygeoops.egg-info/SOURCES.txt` & `pygeoops-0.3.0a1/pygeoops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/pyproject.toml` & `pygeoops-0.3.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoops"
-version = "0.3.0a0"
+version = "0.3.0a1"
 authors = [
   { name="Pieter Roggemans", email="pieter.roggemans@gmail.com" },
 ]
 description = "Library with some less common or extended spatial functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pygeoops-0.3.0a0/tests/test_centerline.py` & `pygeoops-0.3.0a1/tests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_difference.py` & `pygeoops-0.3.0a1/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_general.py` & `pygeoops-0.3.0a1/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_grid.py` & `pygeoops-0.3.0a1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_helper.py` & `pygeoops-0.3.0a1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_paramvalidation.py` & `pygeoops-0.3.0a1/tests/test_paramvalidation.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_shapely.py` & `pygeoops-0.3.0a1/tests/test_shapely.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_simplify.py` & `pygeoops-0.3.0a1/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_simplify_lang.py` & `pygeoops-0.3.0a1/tests/test_simplify_lang.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_simplify_topo.py` & `pygeoops-0.3.0a1/tests/test_simplify_topo.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_types.py` & `pygeoops-0.3.0a1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.3.0a0/tests/test_view_angles.py` & `pygeoops-0.3.0a1/tests/test_view_angles.py`

 * *Files identical despite different names*

