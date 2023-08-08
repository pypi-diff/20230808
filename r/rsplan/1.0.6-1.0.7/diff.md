# Comparing `tmp/rsplan-1.0.6.tar.gz` & `tmp/rsplan-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsplan-1.0.6.tar", last modified: Mon Aug  7 19:50:27 2023, max compression
+gzip compressed data, was "rsplan-1.0.7.tar", last modified: Tue Aug  8 20:47:56 2023, max compression
```

## Comparing `rsplan-1.0.6.tar` & `rsplan-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.593753 rsplan-1.0.6/
--rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.6/LICENSE
--rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-08-07 19:50:27.589752 rsplan-1.0.6/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)     4083 2023-07-25 20:27:37.000000 rsplan-1.0.6/README.md
--rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-08-07 19:50:18.000000 rsplan-1.0.6/pyproject.toml
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.589752 rsplan-1.0.6/rsplan/
--rw-rw-r--   0 built     (1000) built     (1000)       73 2023-08-07 04:56:29.000000 rsplan-1.0.6/rsplan/__init__.py
--rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-25 20:19:49.000000 rsplan-1.0.6/rsplan/curves.py
--rw-rw-r--   0 built     (1000) built     (1000)     2552 2023-08-07 04:58:52.000000 rsplan-1.0.6/rsplan/demo.py
--rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.6/rsplan/helpers.py
--rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 20:19:52.000000 rsplan-1.0.6/rsplan/planner.py
--rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-07-25 01:56:11.000000 rsplan-1.0.6/rsplan/primitives.py
--rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.6/rsplan/py.typed
--rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.6/rsplan/unit_tests.py
-drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-07 19:50:27.589752 rsplan-1.0.6/rsplan.egg-info/
--rw-rw-r--   0 built     (1000) built     (1000)     5740 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/PKG-INFO
--rw-rw-r--   0 built     (1000) built     (1000)      335 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/SOURCES.txt
--rw-rw-r--   0 built     (1000) built     (1000)        1 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/dependency_links.txt
--rw-rw-r--   0 built     (1000) built     (1000)       39 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/requires.txt
--rw-rw-r--   0 built     (1000) built     (1000)        7 2023-08-07 19:50:27.000000 rsplan-1.0.6/rsplan.egg-info/top_level.txt
--rw-rw-r--   0 built     (1000) built     (1000)       38 2023-08-07 19:50:27.593753 rsplan-1.0.6/setup.cfg
--rw-rw-r--   0 built     (1000) built     (1000)      686 2023-08-07 19:50:11.000000 rsplan-1.0.6/setup.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-08 20:47:56.828521 rsplan-1.0.7/
+-rw-rw-r--   0 built     (1000) built     (1000)     1070 2023-07-21 19:25:35.000000 rsplan-1.0.7/LICENSE
+-rw-rw-r--   0 built     (1000) built     (1000)     5744 2023-08-08 20:47:56.824521 rsplan-1.0.7/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)     4083 2023-07-25 20:27:37.000000 rsplan-1.0.7/README.md
+-rw-rw-r--   0 built     (1000) built     (1000)     1072 2023-08-08 20:46:04.000000 rsplan-1.0.7/pyproject.toml
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-08 20:47:56.824521 rsplan-1.0.7/rsplan/
+-rw-rw-r--   0 built     (1000) built     (1000)       74 2023-08-08 17:26:29.000000 rsplan-1.0.7/rsplan/__init__.py
+-rw-rw-r--   0 built     (1000) built     (1000)    28387 2023-07-25 20:19:49.000000 rsplan-1.0.7/rsplan/curves.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2552 2023-08-07 04:58:52.000000 rsplan-1.0.7/rsplan/demo.py
+-rw-rw-r--   0 built     (1000) built     (1000)     2981 2023-07-25 02:02:07.000000 rsplan-1.0.7/rsplan/helpers.py
+-rw-rw-r--   0 built     (1000) built     (1000)     6597 2023-07-25 20:19:52.000000 rsplan-1.0.7/rsplan/planner.py
+-rw-rw-r--   0 built     (1000) built     (1000)    12043 2023-08-08 20:43:12.000000 rsplan-1.0.7/rsplan/primitives.py
+-rw-rw-r--   0 built     (1000) built     (1000)        0 2023-07-25 19:46:23.000000 rsplan-1.0.7/rsplan/py.typed
+-rw-rw-r--   0 built     (1000) built     (1000)     5121 2023-07-24 00:19:18.000000 rsplan-1.0.7/rsplan/unit_tests.py
+drwxrwxr-x   0 built     (1000) built     (1000)        0 2023-08-08 20:47:56.824521 rsplan-1.0.7/rsplan.egg-info/
+-rw-rw-r--   0 built     (1000) built     (1000)     5744 2023-08-08 20:47:56.000000 rsplan-1.0.7/rsplan.egg-info/PKG-INFO
+-rw-rw-r--   0 built     (1000) built     (1000)      335 2023-08-08 20:47:56.000000 rsplan-1.0.7/rsplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        1 2023-08-08 20:47:56.000000 rsplan-1.0.7/rsplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       39 2023-08-08 20:47:56.000000 rsplan-1.0.7/rsplan.egg-info/requires.txt
+-rw-rw-r--   0 built     (1000) built     (1000)        7 2023-08-08 20:47:56.000000 rsplan-1.0.7/rsplan.egg-info/top_level.txt
+-rw-rw-r--   0 built     (1000) built     (1000)       38 2023-08-08 20:47:56.828521 rsplan-1.0.7/setup.cfg
+-rw-rw-r--   0 built     (1000) built     (1000)      690 2023-08-08 20:46:41.000000 rsplan-1.0.7/setup.py
```

### Comparing `rsplan-1.0.6/LICENSE` & `rsplan-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/PKG-INFO` & `rsplan-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.6
+Version: 1.0.7
 Summary: Reeds-Shepp algorithm implementation in Python
-Home-page: https://github.com/builtrobotics/rs
+Home-page: https://github.com/builtrobotics/rsplan
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `rsplan-1.0.6/README.md` & `rsplan-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/pyproject.toml` & `rsplan-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsplan"
-version = "1.0.6"
+version = "1.0.7"
 description = "Reeds-Shepp algorithm implementation in Python"
 readme = "README.md"
 authors = [{ name = "Built Robotics", email = "tarakapoor9@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `rsplan-1.0.6/rsplan/curves.py` & `rsplan-1.0.7/rsplan/curves.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/rsplan/demo.py` & `rsplan-1.0.7/rsplan/demo.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/rsplan/helpers.py` & `rsplan-1.0.7/rsplan/helpers.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/rsplan/planner.py` & `rsplan-1.0.7/rsplan/planner.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/rsplan/primitives.py` & `rsplan-1.0.7/rsplan/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     curvature: float
     driving_direction: Literal[-1, 1]
     is_runway: bool
 
     @property
     def turn_direction(self) -> Literal[-1, 0, 1]:
         """The direction to turn at the Waypoint defined by the right hand rule.
-        Turns either left (negative), right (positive) or straight (zero).
+        Turns either left (positive), right (negative) or straight (zero).
         """
         return helpers.sign(self.curvature)
 
     @property
     def pose_2d_tuple(self) -> Tuple[float, float, float]:
         """The X, Y, and yaw of the Waypoint as a Tuple."""
         return (self.x, self.y, self.yaw)
@@ -234,17 +234,17 @@
         ]
 
     def _curvature(self) -> float:
         """Radius of curvature for the segment. Based on segment driving direction,
         curve type, and turn radius.
         """
         if self.type == "left":
-            return -1.0 / self.turn_radius
-        elif self.type == "right":
             return 1.0 / self.turn_radius
+        elif self.type == "right":
+            return -1.0 / self.turn_radius
         return 0.0
 
     def _straight_runway_pts(
         self,
         start: Tuple[float, float, float],
         end: Tuple[float, float, float],
         step_size: float,
```

### Comparing `rsplan-1.0.6/rsplan/unit_tests.py` & `rsplan-1.0.7/rsplan/unit_tests.py`

 * *Files identical despite different names*

### Comparing `rsplan-1.0.6/rsplan.egg-info/PKG-INFO` & `rsplan-1.0.7/rsplan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rsplan
-Version: 1.0.6
+Version: 1.0.7
 Summary: Reeds-Shepp algorithm implementation in Python
-Home-page: https://github.com/builtrobotics/rs
+Home-page: https://github.com/builtrobotics/rsplan
 Author: Built Robotics
 Author-email: Built Robotics <tarakapoor9@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Built Robotics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `rsplan-1.0.6/setup.py` & `rsplan-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "rsplan",
-    version = "1.0.6",
+    version = "1.0.7",
     author = "Built Robotics",
     author_email = "tarakapoor9@gmail.com",
     description = ("Reeds-Shepp algorithm implementation in Python."),
     license = "MIT",
     keywords = "reeds-shepp path planning",
-    url = "https://github.com/builtrobotics/rs",
+    url = "https://github.com/builtrobotics/rsplan",
     packages=['rsplan'],
     package_data={"rsplan": ["py.typed"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
```

