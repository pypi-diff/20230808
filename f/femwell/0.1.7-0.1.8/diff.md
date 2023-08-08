# Comparing `tmp/femwell-0.1.7.tar.gz` & `tmp/femwell-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.7.tar", max compression
+gzip compressed data, was "femwell-0.1.8.tar", max compression
```

## Comparing `femwell-0.1.7.tar` & `femwell-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-08-05 00:23:17.575251 femwell-0.1.7/LICENSE
--rw-r--r--   0        0        0     2480 2023-08-05 00:23:17.579251 femwell-0.1.7/README.md
--rw-r--r--   0        0        0      255 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5763 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/fefd.py
--rw-r--r--   0        0        0     3172 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/fefd_2d.py
--rw-r--r--   0        0        0     1304 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/laplace.py
--rw-r--r--   0        0        0        1 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/maxwell/__init__.py
--rw-r--r--   0        0        0    20309 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7900 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-08-05 00:23:17.579251 femwell-0.1.7/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4225 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-08-05 00:23:17.583251 femwell-0.1.7/femwell/waveguide.py
--rw-r--r--   0        0        0     1844 2023-08-05 00:23:32.191510 femwell-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 07:24:00.356309 femwell-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2480 2023-08-08 07:24:00.356309 femwell-0.1.8/README.md
+-rw-r--r--   0        0        0      255 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5763 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/fefd.py
+-rw-r--r--   0        0        0     3172 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/fefd_2d.py
+-rw-r--r--   0        0        0     1304 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/laplace.py
+-rw-r--r--   0        0        0        1 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/maxwell/__init__.py
+-rw-r--r--   0        0        0    20309 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7900 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4225 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-08-08 07:24:00.360309 femwell-0.1.8/femwell/waveguide.py
+-rw-r--r--   0        0        0     1066 2023-08-08 07:24:15.117364 femwell-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.8/PKG-INFO
```

### Comparing `femwell-0.1.7/LICENSE` & `femwell-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/README.md` & `femwell-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/culomb.py` & `femwell-0.1.8/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/eme.py.bak` & `femwell-0.1.8/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.8/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/fefd.py` & `femwell-0.1.8/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/fefd_2d.py` & `femwell-0.1.8/femwell/fefd_2d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/fiber.py` & `femwell-0.1.8/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/laplace.py` & `femwell-0.1.8/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/maxwell/waveguide.py` & `femwell-0.1.8/femwell/maxwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mesh/mesh.py` & `femwell-0.1.8/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mesh/meshtracker.py` & `femwell-0.1.8/femwell/mesh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mesh/slice.py` & `femwell-0.1.8/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mesh.py` & `femwell-0.1.8/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mode_solver_1d.py` & `femwell-0.1.8/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.8/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.8/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mode_solver_inplane.py` & `femwell-0.1.8/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/mode_solver_schrodinger.py` & `femwell-0.1.8/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/pn_analytical.py` & `femwell-0.1.8/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/solver.py` & `femwell-0.1.8/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/tcad.py` & `femwell-0.1.8/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/tests/test_mesh.py` & `femwell-0.1.8/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/thermal.py` & `femwell-0.1.8/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/thermal_transient.py` & `femwell-0.1.8/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/utils.py` & `femwell-0.1.8/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/visualization.py` & `femwell-0.1.8/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/femwell/waveguide.py` & `femwell-0.1.8/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.7/pyproject.toml` & `femwell-0.1.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "femwell"
-version = "0.0.1"
-authors = [
-    {name = "Helge Gehring"},
-]
-description = "Mode solver for photonic and electric waveguides based on FEM"
-keywords = [
-    "integrated photonics",
-    "silicon photonics",
-    "mode solving",
-    "finite element analysis"
-]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Science/Research",
-    "Programming Language :: Python :: 3",
-    "Topic :: Scientific/Engineering"
-]
-license = {file = "LICENSE"}
-readme = "README.md"
-
-requires-python = ">=3.8"
-
-dependencies = [
-    "scikit-fem>=8.1.0",
-    "gmsh",
-    "pygmsh",
-    "matplotlib",
-    "shapely>=2.0.0"
-]
-
-[project.urls]
-Homepage = "https://github.com/HelgeGehring/femwell"
-Documentation = "https://HelgeGehring.github.io/femwell/"
+requires = ["poetry-core>=1.6.0"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "femwell"
-version = "0.1.7"
+version = "0.1.8"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.7/PKG-INFO` & `femwell-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.7
+Version: 0.1.8
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

