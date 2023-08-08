# Comparing `tmp/coopstructs-1.1.tar.gz` & `tmp/coopstructs-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopstructs-1.1.tar", last modified: Tue Mar  7 19:08:17 2023, max compression
+gzip compressed data, was "coopstructs-1.2.tar", last modified: Tue Aug  8 19:08:05 2023, max compression
```

## Comparing `coopstructs-1.1.tar` & `coopstructs-1.2.tar`

### file list

```diff
@@ -1,57 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.222770 coopstructs-1.1/
--rw-rw-rw-   0        0        0     1090 2021-09-13 13:50:23.000000 coopstructs-1.1/LICENSE
--rw-rw-rw-   0        0        0      816 2023-03-07 19:08:17.221771 coopstructs-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       78 2021-09-13 13:50:23.000000 coopstructs-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.083732 coopstructs-1.1/coopstructs/
--rw-rw-rw-   0        0        0        0 2021-09-13 13:50:23.000000 coopstructs-1.1/coopstructs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.114733 coopstructs-1.1/coopstructs/geometry/
--rw-rw-rw-   0        0        0      633 2023-03-07 18:48:22.000000 coopstructs-1.1/coopstructs/geometry/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.116762 coopstructs-1.1/coopstructs/geometry/circles/
--rw-rw-rw-   0        0        0        0 2022-11-10 16:03:41.000000 coopstructs-1.1/coopstructs/geometry/circles/__init__.py
--rw-rw-rw-   0        0        0     2629 2023-03-07 18:53:20.000000 coopstructs-1.1/coopstructs/geometry/circles/circle.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.148743 coopstructs-1.1/coopstructs/geometry/curves/
--rw-rw-rw-   0        0        0        0 2022-11-11 17:00:23.000000 coopstructs-1.1/coopstructs/geometry/curves/__init__.py
--rw-rw-rw-   0        0        0     3504 2023-03-07 18:53:20.000000 coopstructs-1.1/coopstructs/geometry/curves/curveBoundaryFactory.py
--rw-rw-rw-   0        0        0     4720 2023-03-07 14:53:55.000000 coopstructs-1.1/coopstructs/geometry/curves/curveBuilder.py
--rw-rw-rw-   0        0        0     5446 2023-03-07 18:53:20.000000 coopstructs-1.1/coopstructs/geometry/curves/curveTrace.py
--rw-rw-rw-   0        0        0      838 2023-03-07 18:53:19.000000 coopstructs-1.1/coopstructs/geometry/curves/curve_factory.py
--rw-rw-rw-   0        0        0    21559 2023-03-07 18:53:20.000000 coopstructs-1.1/coopstructs/geometry/curves/curves.py
--rw-rw-rw-   0        0        0     4520 2023-03-07 18:53:19.000000 coopstructs-1.1/coopstructs/geometry/curves/enums.py
--rw-rw-rw-   0        0        0      298 2023-03-07 18:53:48.000000 coopstructs-1.1/coopstructs/geometry/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.161731 coopstructs-1.1/coopstructs/geometry/lines/
--rw-rw-rw-   0        0        0       22 2022-11-10 16:00:51.000000 coopstructs-1.1/coopstructs/geometry/lines/__init__.py
--rw-rw-rw-   0        0        0     1697 2023-03-07 18:31:44.000000 coopstructs-1.1/coopstructs/geometry/lines/line.py
--rw-rw-rw-   0        0        0       72 2022-11-10 19:15:10.000000 coopstructs-1.1/coopstructs/geometry/logger.py
--rw-rw-rw-   0        0        0     6989 2023-03-07 18:53:39.000000 coopstructs-1.1/coopstructs/geometry/polygonRegion.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.163727 coopstructs-1.1/coopstructs/geometry/rectangles/
--rw-rw-rw-   0        0        0        0 2022-11-10 16:24:06.000000 coopstructs-1.1/coopstructs/geometry/rectangles/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-03-07 18:53:20.000000 coopstructs-1.1/coopstructs/geometry/rectangles/rectangle.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.165728 coopstructs-1.1/coopstructs/geometry/triangles/
--rw-rw-rw-   0        0        0        0 2022-11-10 16:13:21.000000 coopstructs-1.1/coopstructs/geometry/triangles/__init__.py
--rw-rw-rw-   0        0        0      642 2023-03-07 18:53:19.000000 coopstructs-1.1/coopstructs/geometry/triangles/triangle.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.175812 coopstructs-1.1/coopstructs/geometry/vectors/
--rw-rw-rw-   0        0        0        0 2022-11-11 17:54:51.000000 coopstructs-1.1/coopstructs/geometry/vectors/__init__.py
--rw-rw-rw-   0        0        0    13572 2023-03-07 18:44:43.000000 coopstructs-1.1/coopstructs/geometry/vectors/vectorN.py
--rw-rw-rw-   0        0        0     7746 2022-11-25 21:12:09.000000 coopstructs-1.1/coopstructs/geometry/vectors/vector_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.204772 coopstructs-1.1/coopstructs/grids/
--rw-rw-rw-   0        0        0      100 2022-10-13 15:03:52.000000 coopstructs-1.1/coopstructs/grids/__init__.py
--rw-rw-rw-   0        0        0      107 2022-09-19 22:14:23.000000 coopstructs-1.1/coopstructs/grids/enums.py
--rw-rw-rw-   0        0        0     1253 2022-09-19 21:08:23.000000 coopstructs-1.1/coopstructs/grids/gridState.py
--rw-rw-rw-   0        0        0     3333 2023-03-07 18:49:03.000000 coopstructs-1.1/coopstructs/grids/grid_base.py
--rw-rw-rw-   0        0        0     2394 2022-11-10 19:53:54.000000 coopstructs-1.1/coopstructs/grids/hexGrid.py
--rw-rw-rw-   0        0        0     3086 2023-03-07 18:22:04.000000 coopstructs-1.1/coopstructs/grids/rectGrid.py
--rw-rw-rw-   0        0        0    17685 2023-03-07 19:07:31.000000 coopstructs-1.1/coopstructs/grids/sectorTree.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.220807 coopstructs-1.1/coopstructs/zones/
--rw-rw-rw-   0        0        0       85 2022-02-21 16:55:49.000000 coopstructs-1.1/coopstructs/zones/__init__.py
--rw-rw-rw-   0        0        0      425 2022-11-10 19:51:19.000000 coopstructs-1.1/coopstructs/zones/exceptions.py
--rw-rw-rw-   0        0        0       75 2022-02-21 16:24:40.000000 coopstructs-1.1/coopstructs/zones/logger.py
--rw-rw-rw-   0        0        0     2117 2022-11-10 19:51:19.000000 coopstructs-1.1/coopstructs/zones/zoneManager.py
-drwxrwxrwx   0        0        0        0 2023-03-07 19:08:17.108757 coopstructs-1.1/coopstructs.egg-info/
--rw-rw-rw-   0        0        0      816 2023-03-07 19:08:17.000000 coopstructs-1.1/coopstructs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-03-07 19:08:17.000000 coopstructs-1.1/coopstructs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 19:08:17.000000 coopstructs-1.1/coopstructs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-09-13 13:56:55.000000 coopstructs-1.1/coopstructs.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      268 2023-03-07 19:08:17.000000 coopstructs-1.1/coopstructs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-07 19:08:17.000000 coopstructs-1.1/coopstructs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 19:08:17.222770 coopstructs-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-03-07 19:08:10.000000 coopstructs-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.221295 coopstructs-1.2/
+-rw-rw-rw-   0        0        0     1090 2021-09-13 13:50:23.000000 coopstructs-1.2/LICENSE
+-rw-rw-rw-   0        0        0      816 2023-08-08 19:08:05.220259 coopstructs-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2021-09-13 13:50:23.000000 coopstructs-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.008294 coopstructs-1.2/coopstructs/
+-rw-rw-rw-   0        0        0        0 2021-09-13 13:50:23.000000 coopstructs-1.2/coopstructs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.081258 coopstructs-1.2/coopstructs/geometry/
+-rw-rw-rw-   0        0        0      633 2023-03-07 18:48:22.000000 coopstructs-1.2/coopstructs/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.093259 coopstructs-1.2/coopstructs/geometry/circles/
+-rw-rw-rw-   0        0        0        0 2022-11-10 16:03:41.000000 coopstructs-1.2/coopstructs/geometry/circles/__init__.py
+-rw-rw-rw-   0        0        0     2629 2023-03-07 18:53:20.000000 coopstructs-1.2/coopstructs/geometry/circles/circle.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.134256 coopstructs-1.2/coopstructs/geometry/curves/
+-rw-rw-rw-   0        0        0        0 2022-11-11 17:00:23.000000 coopstructs-1.2/coopstructs/geometry/curves/__init__.py
+-rw-rw-rw-   0        0        0     3504 2023-03-07 18:53:20.000000 coopstructs-1.2/coopstructs/geometry/curves/curveBoundaryFactory.py
+-rw-rw-rw-   0        0        0     4722 2023-08-08 18:54:04.000000 coopstructs-1.2/coopstructs/geometry/curves/curveBuilder.py
+-rw-rw-rw-   0        0        0     5480 2023-08-08 16:45:45.000000 coopstructs-1.2/coopstructs/geometry/curves/curveTrace.py
+-rw-rw-rw-   0        0        0      894 2023-08-08 19:04:20.000000 coopstructs-1.2/coopstructs/geometry/curves/curve_factory.py
+-rw-rw-rw-   0        0        0    21837 2023-08-08 19:04:20.000000 coopstructs-1.2/coopstructs/geometry/curves/curves.py
+-rw-rw-rw-   0        0        0     4520 2023-03-07 18:53:19.000000 coopstructs-1.2/coopstructs/geometry/curves/enums.py
+-rw-rw-rw-   0        0        0      298 2023-03-07 18:53:48.000000 coopstructs-1.2/coopstructs/geometry/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.150256 coopstructs-1.2/coopstructs/geometry/lines/
+-rw-rw-rw-   0        0        0       22 2022-11-10 16:00:51.000000 coopstructs-1.2/coopstructs/geometry/lines/__init__.py
+-rw-rw-rw-   0        0        0     1697 2023-03-07 18:31:44.000000 coopstructs-1.2/coopstructs/geometry/lines/line.py
+-rw-rw-rw-   0        0        0       72 2022-11-10 19:15:10.000000 coopstructs-1.2/coopstructs/geometry/logger.py
+-rw-rw-rw-   0        0        0     7006 2023-03-07 19:11:57.000000 coopstructs-1.2/coopstructs/geometry/polygonRegion.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.159256 coopstructs-1.2/coopstructs/geometry/rectangles/
+-rw-rw-rw-   0        0        0        0 2022-11-10 16:24:06.000000 coopstructs-1.2/coopstructs/geometry/rectangles/__init__.py
+-rw-rw-rw-   0        0        0     3974 2023-03-12 23:24:25.000000 coopstructs-1.2/coopstructs/geometry/rectangles/rectangle.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.168256 coopstructs-1.2/coopstructs/geometry/triangles/
+-rw-rw-rw-   0        0        0        0 2022-11-10 16:13:21.000000 coopstructs-1.2/coopstructs/geometry/triangles/__init__.py
+-rw-rw-rw-   0        0        0      642 2023-03-07 18:53:19.000000 coopstructs-1.2/coopstructs/geometry/triangles/triangle.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.187260 coopstructs-1.2/coopstructs/geometry/vectors/
+-rw-rw-rw-   0        0        0        0 2022-11-11 17:54:51.000000 coopstructs-1.2/coopstructs/geometry/vectors/__init__.py
+-rw-rw-rw-   0        0        0    13624 2023-04-10 17:56:35.000000 coopstructs-1.2/coopstructs/geometry/vectors/vectorN.py
+-rw-rw-rw-   0        0        0     7746 2022-11-25 21:12:09.000000 coopstructs-1.2/coopstructs/geometry/vectors/vector_utils.py
+-rw-rw-rw-   0        0        0    17685 2023-03-07 20:36:50.000000 coopstructs-1.2/coopstructs/sectorTree.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.218256 coopstructs-1.2/coopstructs/zones/
+-rw-rw-rw-   0        0        0       85 2022-02-21 16:55:49.000000 coopstructs-1.2/coopstructs/zones/__init__.py
+-rw-rw-rw-   0        0        0      425 2022-11-10 19:51:19.000000 coopstructs-1.2/coopstructs/zones/exceptions.py
+-rw-rw-rw-   0        0        0       75 2022-02-21 16:24:40.000000 coopstructs-1.2/coopstructs/zones/logger.py
+-rw-rw-rw-   0        0        0     2151 2023-04-13 17:27:24.000000 coopstructs-1.2/coopstructs/zones/zoneManager.py
+drwxrwxrwx   0        0        0        0 2023-08-08 19:08:05.045258 coopstructs-1.2/coopstructs.egg-info/
+-rw-rw-rw-   0        0        0      816 2023-08-08 19:08:04.000000 coopstructs-1.2/coopstructs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-08-08 19:08:04.000000 coopstructs-1.2/coopstructs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 19:08:04.000000 coopstructs-1.2/coopstructs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-09-13 13:56:55.000000 coopstructs-1.2/coopstructs.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      268 2023-08-08 19:08:04.000000 coopstructs-1.2/coopstructs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-08 19:08:04.000000 coopstructs-1.2/coopstructs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 19:08:05.221295 coopstructs-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-08-08 19:06:33.000000 coopstructs-1.2/setup.py
```

### Comparing `coopstructs-1.1/LICENSE` & `coopstructs-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/PKG-INFO` & `coopstructs-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopstructs
-Version: 1.1
+Version: 1.2
 Summary: Basic data structs commonly used by various applications
 Home-page: https://github.com/tylertjburns/coopstructs
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopstructs-1.1/coopstructs/geometry/__init__.py` & `coopstructs-1.2/coopstructs/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/circles/circle.py` & `coopstructs-1.2/coopstructs/geometry/circles/circle.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/curveBoundaryFactory.py` & `coopstructs-1.2/coopstructs/geometry/curves/curveBoundaryFactory.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/curveBuilder.py` & `coopstructs-1.2/coopstructs/geometry/curves/curveBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         if close_circuit and len(leftovers) == 1:
             return curves[0].force_continuity(next_point, close_circuit)
         elif len(leftovers) != 0:
             return next_point
         else:
             return curves[-1].force_continuity(next_point)
 
+
 if __name__ == "__main__":
     import random as rnd
 
     builder = CurveBuilder(lambda: "1")
 
     points = []
```

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/curveTrace.py` & `coopstructs-1.2/coopstructs/geometry/curves/curveTrace.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,14 +132,15 @@
                       swim_lane: PolygonRegion,
                       ax):
     plot_series(ax=ax, points=[x.as_tuple() for x in swim_lane.boundary_points], series_type='fill')
     for ii, iter in traced_curve.items():
         plot_series(points=[x.as_tuple() for x in iter.polygon.boundary_points],
                     ax=ax,
                     series_type="scatter",
+                    point_size=1
                     )
     plot_series(ax=ax, points=[traced.anchor for ii, traced in traced_curve.items()], series_type='line', color=Color.BLACK)
 
 
 
 
 if __name__ == "__main__":
```

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/curve_factory.py` & `coopstructs-1.2/coopstructs/geometry/curves/curve_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from coopstructs.geometry.curves.curves import CubicBezier, Arc, CircularArc, LineCurve, CatmullRom
+from coopstructs.geometry.curves.curves import CubicBezier, Arc, CircularArc, LineCurve, CatmullRom, Curve
+from typing import Dict
 
 def curve_from_json(json):
     curve_type = json['type']
 
     curve_gen_switch = {
         CubicBezier.__name__: CubicBezier.from_json,
         Arc.__name__: Arc.from_json,
@@ -13,17 +14,17 @@
     gen_func = curve_gen_switch.get(curve_type, None)
 
     if gen_func is None:
         raise ValueError(f"Unsupported curve type: {curve_type}")
 
     return gen_func(json['data'])
 
-def curves_from_json(json):
+def curves_from_json(json) -> Dict[str, Curve]:
     curves_data = json['curves']
 
-    curves = []
+    curves = {}
     for data in curves_data:
         curve = curve_from_json(data)
-        curves.append(curve)
+        curves[curve.id] = curve
 
     return curves
```

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/curves.py` & `coopstructs-1.2/coopstructs/geometry/curves/curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from coopstructs.geometry.vectors.vectorN import Vector2
 from cooptools.geometry import collinear_points
-from typing import List, Callable, Tuple
+from typing import List, Callable, Tuple, Dict
 from coopstructs.geometry import Rectangle, Line, Triangle, Circle
 from uuid import uuid4
 from coopstructs.geometry.curves.enums import Orientation
 import cooptools.geometry_utils.curve_utils as utils
 import cooptools.geometry_utils.circle_utils as circ
 from cooptools.common import verify_val, bounding_box_of_points
 
@@ -316,16 +316,19 @@
     def from_points(self, points, naming_provider: Callable[[], str]) -> (List, List):
         lines = []
         for ii in range(len(points) - 1):
             lines.append(LineCurve(points[ii], points[ii + 1], id=naming_provider()))
         return lines, []
 
     @classmethod
-    def from_json(cls, json: str):
-        raise NotImplementedError()
+    def from_json(cls, json: Dict):
+        o = Vector2.from_json(json['controlPoints'][0])
+        d = Vector2.from_json(json['controlPoints'][1])
+
+        return LineCurve(origin=o, destination=d, id=json.get('id', None))
 
     def __init__(self, origin: Vector2, destination: Vector2, id: str=None):
         super().__init__(id=id, origin=origin)
         self.destination = destination
 
     def _control_points(self) -> List[Vector2]:
         return [self.origin, self.EndPoint]
@@ -336,14 +339,18 @@
     def _end_point(self):
         return self.destination
 
     @property
     def Length(self):
         return Line(self.origin, self.destination).length
 
+    @property
+    def Line(self):
+        return Line(self.origin, self.destination)
+
     def force_continuity(self, next_point: Vector2, close_circuit: bool = False) -> Vector2:
         if close_circuit:
             raise NotImplementedError(f"Close circuit not implemented for type [{type(self)}]")
         return next_point
 
     def point_at_t(self, t: float):
         if not (0 <= t <= 1):
@@ -358,21 +365,21 @@
         verify_val(t, low_inc=0, hi_inc=1)
         return (self.EndPoint - self.origin).unit()
 
 
 class CubicBezier(Curve):
 
     @classmethod
-    def from_json(cls, json: str):
+    def from_json(cls, json: Dict):
         cps = []
         for pt_data in json['controlPoints']:
             pt = Vector2.from_json(pt_data)
             cps.append(pt)
 
-        return CubicBezier(control_points=cps)
+        return CubicBezier(control_points=cps, id=json.get('id', None))
 
     def point_at_t(self, t: float):
         return Vector2.from_tuple(utils.cubic_bezier_point_at_t(t, [x.as_tuple() for x in self.ControlPoints]))
 
     def tangent_at_t(self, t: float) -> Vector2:
         return Vector2.from_tuple(utils.cubic_bezier_tangent_at_t(t, [x.as_tuple() for x in self.ControlPoints])).unit()
```

### Comparing `coopstructs-1.1/coopstructs/geometry/curves/enums.py` & `coopstructs-1.2/coopstructs/geometry/curves/enums.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/lines/line.py` & `coopstructs-1.2/coopstructs/geometry/lines/line.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/polygonRegion.py` & `coopstructs-1.2/coopstructs/geometry/polygonRegion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from coopstructs.geometry.vectors.vectorN import Vector2
 from typing import List, Tuple, Dict
-import cooptools.geometry as geo
+import cooptools.geometry_utils.line_utils as lin
 from coopstructs.geometry.lines.line import Line
 from scipy.spatial import ConvexHull
 from shapely.geometry import Polygon, Point
 from coopstructs.geometry.exceptions import DuplicatePointException
 from coopstructs.geometry.logger import geomLogger
 from cooptools.common import all_indxs_in_lst, bounding_box_of_points
 
@@ -22,15 +22,15 @@
     def from_json(cls, json):
         boundary_points = [Vector2.from_json(pt) for pt in json['boundaryPoints']]
         return PolygonRegion(boundary_points=boundary_points)
 
 
     @classmethod
     def convex_hull(self, points: List[Vector2]):
-        if not geo.collinear_points([point.as_tuple() for point in points]):
+        if not lin.collinear_points([point.as_tuple() for point in points]):
             hull = ConvexHull([point.as_tuple() for point in points])
             return PolygonRegion([points[ind] for ind in hull.vertices])
         else:
             return PolygonRegion(points)
 
     def __init__(self, boundary_points: List[Vector2] = None):
         self.boundary_points = boundary_points if boundary_points is not None else []
@@ -48,15 +48,15 @@
     @property
     def as_shapely_polygon(self) -> Polygon:
         return Polygon([p.as_tuple() for p in self.boundary_points])
 
     @property
     def valid(self):
         # valid if at least 3 points and they are not collinear
-        return len(self.boundary_points) >= 3 and not geo.collinear_points([point.as_tuple() for point in self.boundary_points])
+        return len(self.boundary_points) >= 3 and not lin.collinear_points([point.as_tuple() for point in self.boundary_points])
 
     def add_points(self, points: List[Vector2], at_idx: int = None):
         # check if the new point(s) to be added are a duplicate of the last point added
         bndry_pts_init = self.boundary_points and len(self.boundary_points) > 0
         if bndry_pts_init \
                 and at_idx \
                 and points[0] in self.boundary_points[at_idx-1: at_idx + 1]:
```

### Comparing `coopstructs-1.1/coopstructs/geometry/rectangles/rectangle.py` & `coopstructs-1.2/coopstructs/geometry/rectangles/rectangle.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,18 +102,25 @@
     def as_tuple(self):
         return (self.x, self.y, self.width, self.height)
 
     @property
     def x(self):
         return self.anchor.pt[0]
 
+    @x.setter
+    def x(self, value):
+        self.anchor = Anchor2D.from_anchor(self.anchor, pt=(value, self.anchor.pt[1]))
+
     @property
     def y(self):
         return self.anchor.pt[1]
 
+    @y.setter
+    def y(self, value):
+        self.anchor = Anchor2D.from_anchor(self.anchor, pt=(self.anchor.pt[0], value))
     @property
     def width(self):
         return self.anchor.dims[0]
 
     @property
     def height(self):
         return self.anchor.dims[1]
```

### Comparing `coopstructs-1.1/coopstructs/geometry/triangles/triangle.py` & `coopstructs-1.2/coopstructs/geometry/triangles/triangle.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/geometry/vectors/vectorN.py` & `coopstructs-1.2/coopstructs/geometry/vectors/vectorN.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,17 @@
     def from_vector3(cls, vec3):
         if not type(vec3) == Vector3:
             raise TypeError(f"input type must be {type(Vector3)} but type [{type(vec3)}] was provided")
         return Vector2(vec3.x, vec3.y)
 
     @classmethod
     def from_tuple(cls, tup: Tuple[float, float]):
+        if tup is None:
+            return None
+
         if len(tup) < 2:
             raise ValueError(f"Can only create a Vector2 from a float tuple of size 2 or more. {tup} provided")
 
         x = float(tup[0])
         y = float(tup[1])
 
         return Vector2(x, y)
```

### Comparing `coopstructs-1.1/coopstructs/geometry/vectors/vector_utils.py` & `coopstructs-1.2/coopstructs/geometry/vectors/vector_utils.py`

 * *Files identical despite different names*

### Comparing `coopstructs-1.1/coopstructs/grids/sectorTree.py` & `coopstructs-1.2/coopstructs/sectorTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from coopstructs.grids import RectGrid
+from cooptools.sectors import RectGrid
 from coopstructs.geometry import Rectangle
 from typing import Dict, Any, Tuple, List, Callable
 import cooptools.sectors.rect_utils as sec_u
 from cooptools.coopEnum import CardinalPosition
 import logging
 import matplotlib.patches as patches
 from cooptools.colors import Color
```

### Comparing `coopstructs-1.1/coopstructs/zones/zoneManager.py` & `coopstructs-1.2/coopstructs/zones/zoneManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from cooptools.geometry import Vector2
-from cooptools.geometry import PolygonRegion
+from coopstructs.geometry.vectors.vectorN import Vector2
+from coopstructs.geometry.polygonRegion import PolygonRegion
 from cooptools.zones.logger import zoneLogger
 from typing import List, Dict, Tuple
 from cooptools.zones.exceptions import ZoneDoesntExistException, ZoneAlreadyExistsException
 
 class ZoneManager:
 
     def __init__(self):
```

### Comparing `coopstructs-1.1/coopstructs.egg-info/PKG-INFO` & `coopstructs-1.2/coopstructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopstructs
-Version: 1.1
+Version: 1.2
 Summary: Basic data structs commonly used by various applications
 Home-page: https://github.com/tylertjburns/coopstructs
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopstructs-1.1/coopstructs.egg-info/SOURCES.txt` & `coopstructs-1.2/coopstructs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 coopstructs/__init__.py
+coopstructs/sectorTree.py
 coopstructs.egg-info/PKG-INFO
 coopstructs.egg-info/SOURCES.txt
 coopstructs.egg-info/dependency_links.txt
 coopstructs.egg-info/not-zip-safe
 coopstructs.egg-info/requires.txt
 coopstructs.egg-info/top_level.txt
 coopstructs/geometry/__init__.py
@@ -26,18 +27,11 @@
 coopstructs/geometry/rectangles/__init__.py
 coopstructs/geometry/rectangles/rectangle.py
 coopstructs/geometry/triangles/__init__.py
 coopstructs/geometry/triangles/triangle.py
 coopstructs/geometry/vectors/__init__.py
 coopstructs/geometry/vectors/vectorN.py
 coopstructs/geometry/vectors/vector_utils.py
-coopstructs/grids/__init__.py
-coopstructs/grids/enums.py
-coopstructs/grids/gridState.py
-coopstructs/grids/grid_base.py
-coopstructs/grids/hexGrid.py
-coopstructs/grids/rectGrid.py
-coopstructs/grids/sectorTree.py
 coopstructs/zones/__init__.py
 coopstructs/zones/exceptions.py
 coopstructs/zones/logger.py
 coopstructs/zones/zoneManager.py
```

### Comparing `coopstructs-1.1/setup.py` & `coopstructs-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopstructs',
-      version='1.01',
+      version='1.02',
       description='Basic data structs commonly used by various applications',
       url='https://github.com/tylertjburns/coopstructs',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

