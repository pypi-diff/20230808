# Comparing `tmp/cardiac_geometries-0.7.0.tar.gz` & `tmp/cardiac_geometries-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-0.7.0.tar", last modified: Sat Jul 22 20:23:46 2023, max compression
+gzip compressed data, was "cardiac_geometries-0.8.0.tar", last modified: Tue Aug  8 08:16:55 2023, max compression
```

## Comparing `cardiac_geometries-0.7.0.tar` & `cardiac_geometries-0.8.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1535 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.963562 cardiac_geometries-0.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1512 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/
--rw-r--r--   0 root         (0) root         (0)      602 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12783 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     9594 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_slab.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/utils.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    21911 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mesh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/
--rw-r--r--   0 root         (0) root         (0)      260 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_biv.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_lv.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_utils.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    19764 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    16326 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)     9979 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.967562 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 20:23:33.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-22 20:23:46.000000 cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 20:23:46.971562 cardiac_geometries-0.7.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_gmsh.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-07-22 20:23:32.000000 cardiac_geometries-0.7.0/tests/test_mshr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.036463 cardiac_geometries-0.8.0/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-08-08 08:16:55.036463 cardiac_geometries-0.8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-08-08 08:16:55.036463 cardiac_geometries-0.8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.020462 cardiac_geometries-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.024463 cardiac_geometries-0.8.0/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.028463 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     9593 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/utils.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    24659 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_mesh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.028463 cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/
+-rw-r--r--   0 root         (0) root         (0)      260 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/_biv.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/_lv.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    21846 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.032463 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     6278 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9979 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.024463 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 08:16:41.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-08-08 08:16:55.000000 cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 08:16:55.036463 cardiac_geometries-0.8.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/tests/test_gmsh.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-08-08 08:16:40.000000 cardiac_geometries-0.8.0/tests/test_mshr.py
```

### Comparing `cardiac_geometries-0.7.0/LICENSE` & `cardiac_geometries-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/PKG-INFO` & `cardiac_geometries-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.7.0/setup.cfg` & `cardiac_geometries-0.8.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardiac_geometries
-version = 0.7.0
+version = 0.8.0
 description = A python library for cardiac geometries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ComputationalPhysiology/cardiac_geometries
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = MIT
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/__init__.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/__init__.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from ._biv_ellipsoid import biv_ellipsoid_torso
 from ._lv_ellipsoid import create_benchmark_geometry_land15
 from ._lv_ellipsoid import lv_ellipsoid
 from ._lv_ellipsoid import lv_ellipsoid_flat_base
 from ._lv_ellipsoid import prolate_lv_ellipsoid
 from ._lv_ellipsoid import prolate_lv_ellipsoid_flat_base
 from ._slab import slab
+from ._slab import slab_in_bath
 
 
 __all__ = [
     "lv_ellipsoid",
     "lv_ellipsoid_flat_base",
     "prolate_lv_ellipsoid_flat_base",
     "prolate_lv_ellipsoid",
     "create_benchmark_geometry_land15",
     "slab",
+    "slab_in_bath",
     "biv_ellipsoid",
     "biv_ellipsoid_torso",
 ]
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_gmsh/_lv_ellipsoid.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         Point size, by default 3.0
     ndiv : float, optional
         Number of divisions, by default 1.0
 
     Returns
     -------
     Path
-        _description_
+        Path to file
     """
     mu_base_endo = math.acos(quota_base / r_long_endo)
     mu_base_epi = math.acos(quota_base / r_long_epi)
     mu_apex_endo = mu_apex_epi = 0
     psize_ref = psize / ndiv
     return lv_ellipsoid(
         mesh_name=mesh_name,
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -650,7 +650,113 @@
 
     geo = Geometry.from_folder(outdir)
 
     if _tmpfile is not None:
         _tmpfile.__exit__(None, None, None)
 
     return geo
+
+
+def create_slab_in_bath(
+    outdir: Optional[Union[Path, str]] = None,
+    lx: float = 1.0,
+    ly: float = 0.01,
+    lz: float = 0.5,
+    bx: float = 0.0,
+    by: float = 0.0,
+    bz: float = 0.1,
+    dx: float = 0.001,
+) -> Optional[Geometry]:
+    """Create slab geometry
+
+    Parameters
+    ----------
+    outdir : Optional[Path], optional
+        Directory where to save the results. If not provided a temporary
+        directory will be created, by default None
+    lx : float, optional
+        Length of slab the x-direction, by default 1.0
+    ly : float, optional
+        Length of slab the x-direction, by default 0.5
+    lz : float, optional
+        Length of slab the z-direction, by default 0.01
+    bx : float, optional
+        Thickness of bath the x-direction, by default 0.0
+    by : float, optional
+        Thickness of bath the x-direction, by default 0.0
+    bz : float, optional
+        Thickness of bath the z-direction, by default 0.1
+    dx : float, optional
+        Element size, by default 0.001
+
+    Returns
+    -------
+    Optional[Geometry]
+        A Geometry with the mesh, markers, markers functions and fibers.
+        Returns None if dolfin is not installed.
+
+    Raises
+    ------
+    ImportError
+        If gmsh is not installed
+    """
+
+    if not has_gmsh():
+        raise ImportError("Cannot create BiV ellipsoid. Gmsh is not installed")
+
+    _tmpfile = None
+    if outdir is None:
+        _tmpfile = tempfile.TemporaryDirectory()
+        outdir = _tmpfile.__enter__()
+
+    outdir = Path(outdir)
+    outdir.mkdir(exist_ok=True, parents=True)
+
+    with open(outdir / "info.json", "w") as f:
+        json.dump(
+            {
+                "lx": lx,
+                "ly": ly,
+                "lz": lz,
+                "bx": bx,
+                "by": by,
+                "bz": bz,
+                "dx": dx,
+                "mesh_type": MeshTypes.slab.value,
+                "cardiac_geometry_version": __version__,
+                "timestamp": datetime.datetime.now().isoformat(),
+            },
+            f,
+            indent=2,
+            default=json_serial,
+        )
+
+    from ._gmsh import slab_in_bath
+
+    mesh_name = outdir / "slab_in_bath.msh"
+    slab_in_bath(
+        mesh_name=mesh_name.as_posix(),
+        lx=lx,
+        ly=ly,
+        lz=lz,
+        bx=bx,
+        by=by,
+        bz=bz,
+        dx=dx,
+    )
+
+    if not has_dolfin():
+        return None
+
+    from .dolfin_utils import gmsh2dolfin
+
+    geometry = gmsh2dolfin(mesh_name, unlink=False)
+
+    with open(outdir / "markers.json", "w") as f:
+        json.dump(geometry.markers, f, default=json_serial)
+
+    geo = Geometry.from_folder(outdir)
+
+    if _tmpfile is not None:
+        _tmpfile.__exit__(None, None, None)
+
+    return geo
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_biv.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/_biv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/_mshr/_lv.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/_mshr/_lv.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/calculus.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/cli.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,14 +193,21 @@
     "--center-lv-y",
     default=0.0,
     type=float,
     help="Y-coordinate for the center of the lv",
     show_default=True,
 )
 @click.option(
+    "--center-lv-z",
+    default=0.0,
+    type=float,
+    help="Z-coordinate for the center of the lv",
+    show_default=True,
+)
+@click.option(
     "--a-endo-lv",
     default=2.5,
     type=float,
     help="Dilation of lv endo ellipsoid in the x-direction",
     show_default=True,
 )
 @click.option(
@@ -242,14 +249,21 @@
     "--center-rv-y",
     default=0.5,
     type=float,
     help="Y-coordinate for the center of the rv",
     show_default=True,
 )
 @click.option(
+    "--center-rv-z",
+    default=0.0,
+    type=float,
+    help="Z-coordinate for the center of the rv",
+    show_default=True,
+)
+@click.option(
     "--a-endo-rv",
     default=3.0,
     type=float,
     help="Dilation of rv endo ellipsoid in the x-direction",
     show_default=True,
 )
 @click.option(
@@ -316,21 +330,23 @@
     help="Function space for fibers of the form family_degree",
     show_default=True,
 )
 def create_biv_ellipsoid(
     outdir: Path,
     char_length: float = 0.5,
     center_lv_y: float = 0.0,
+    center_lv_z: float = 0.0,
     a_endo_lv: float = 2.5,
     b_endo_lv: float = 1.0,
     c_endo_lv: float = 1.0,
     a_epi_lv: float = 3.0,
     b_epi_lv: float = 1.5,
     c_epi_lv: float = 1.5,
     center_rv_y: float = 0.5,
+    center_rv_z: float = 0.0,
     a_endo_rv: float = 3.0,
     b_endo_rv: float = 1.5,
     c_endo_rv: float = 1.5,
     a_epi_rv: float = 4.0,
     b_epi_rv: float = 2.5,
     c_epi_rv: float = 2.0,
     create_fibers: bool = False,
@@ -343,21 +359,23 @@
 
     from ._mesh import create_biv_ellipsoid
 
     geo = create_biv_ellipsoid(
         outdir=outdir,
         char_length=char_length,
         center_lv_y=center_lv_y,
+        center_lv_z=center_lv_z,
         a_endo_lv=a_endo_lv,
         b_endo_lv=b_endo_lv,
         c_endo_lv=c_endo_lv,
         a_epi_lv=a_epi_lv,
         b_epi_lv=b_epi_lv,
         c_epi_lv=c_epi_lv,
         center_rv_y=center_rv_y,
+        center_rv_z=center_rv_z,
         a_endo_rv=a_endo_rv,
         b_endo_rv=b_endo_rv,
         c_endo_rv=c_endo_rv,
         a_epi_rv=a_epi_rv,
         b_epi_rv=b_epi_rv,
         c_epi_rv=c_epi_rv,
         create_fibers=create_fibers,
@@ -710,14 +728,103 @@
         fiber_angle_endo=fiber_angle_endo,
         fiber_angle_epi=fiber_angle_epi,
         fiber_space=fiber_space,
     )
     geo.save(outdir / "slab.h5")
 
 
+@click.command()
+@click.argument(
+    "outdir",
+    required=True,
+    type=click.Path(
+        file_okay=False,
+        dir_okay=True,
+        writable=True,
+        readable=True,
+        resolve_path=True,
+    ),
+)
+@click.option(
+    "--lx",
+    default=1.0,
+    type=float,
+    help="Length of slab in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--ly",
+    default=0.01,
+    type=float,
+    help="Length of slab in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--lz",
+    default=0.5,
+    type=float,
+    help="Length of slab in the z-direction",
+    show_default=True,
+)
+@click.option(
+    "--bx",
+    default=0.0,
+    type=float,
+    help="Thickness of bath in the x-direction",
+    show_default=True,
+)
+@click.option(
+    "--by",
+    default=0.0,
+    type=float,
+    help="Thickness of bath in the y-direction",
+    show_default=True,
+)
+@click.option(
+    "--bz",
+    default=0.1,
+    type=float,
+    help="Thickness of bath in the z-direction",
+    show_default=True,
+)
+@click.option(
+    "--dx",
+    default=0.01,
+    type=float,
+    help="Element size",
+    show_default=True,
+)
+def create_slab_in_bath(
+    outdir: Path,
+    lx: float = 1.0,
+    ly: float = 0.01,
+    lz: float = 0.5,
+    bx: float = 0.0,
+    by: float = 0.0,
+    bz: float = 0.1,
+    dx: float = 0.01,
+):
+    outdir = Path(outdir)
+    outdir.mkdir(exist_ok=True)
+
+    from ._mesh import create_slab_in_bath
+
+    geo = create_slab_in_bath(
+        outdir=outdir,
+        lx=lx,
+        ly=ly,
+        lz=lz,
+        bx=bx,
+        by=by,
+        bz=bz,
+        dx=dx,
+    )
+    geo.save(outdir / "slab_in_bath.h5")
+
+
 @click.command(
     help=(
         "Convert microstructure.h5 into separate .xdmf-files for f0, s0, and n0. "
         "Assumes a folder containing a 'mesh.xdmf' and 'microstructure.h5'."
     ),
 )
 @click.argument(
@@ -845,10 +952,11 @@
     console.print(table)
 
 
 app.add_command(create_lv_ellipsoid)
 app.add_command(create_biv_ellipsoid)
 app.add_command(create_biv_ellipsoid_torso)
 app.add_command(create_slab)
+app.add_command(create_slab_in_bath)
 app.add_command(fibers_to_xdmf)
 app.add_command(folder2h5)
 app.add_command(info)
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,22 +55,47 @@
 
 def normalize(u):
     return u / np.linalg.norm(u, axis=0)
 
 
 def compute_system(
     t_func: dolfin.Function,
-    r_short_endo,
-    r_short_epi,
-    r_long_endo,
-    r_long_epi,
+    r_short_endo: float,
+    r_short_epi: float,
+    r_long_endo: float,
+    r_long_epi: float,
     alpha_endo: float = -60,
     alpha_epi: float = 60,
     **kwargs,
-):
+) -> Microstructure:
+    """Compute ldrb system for idealized prolate
+    ellipsoid
+
+    Parameters
+    ----------
+    t_func : dolfin.Function
+        Solution to laplace equation
+    r_short_endo : float, optional
+        Shortest radius on the endocardium layer
+    r_short_epi : float, optional
+       Shortest radius on the epicardium layer
+    r_long_endo : float, optional
+        Longest radius on the endocardium layer
+    r_long_epi : float, optional
+        Longest radius on the epicardium layer
+    alpha_endo : float, optional
+        Fiber angle on endocardium, by default -60
+    alpha_epi : float, optional
+        Fiber angle on epi cardium, by default 60
+
+    Returns
+    -------
+    Microstructure
+        (fiber, sheet, sheet_normal)
+    """
 
     V = t_func.function_space()
     element = V.ufl_element()
     mesh = V.mesh()
 
     dof_coordinates = V.tabulate_dof_coordinates()
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/geometry.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries/viz.py` & `cardiac_geometries-0.8.0/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac-geometries
-Version: 0.7.0
+Version: 0.8.0
 Summary: A python library for cardiac geometries
 Home-page: https://github.com/ComputationalPhysiology/cardiac_geometries
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: MIT
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cardiac_geometries-0.7.0/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-0.8.0/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/tests/test_cli.py` & `cardiac_geometries-0.8.0/tests/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,29 @@
     res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
     assert res2.exit_code == 0
     assert outfile.is_file()
     geo = Geometry.from_file(outfile)
     assert geo.f0 is not None
 
 
+def test_create_slab_in_bath(tmp_path: Path):
+    runner = CliRunner()
+    res1 = runner.invoke(cli.create_slab_in_bath, [tmp_path.as_posix()])
+    assert res1.exit_code == 0
+    outfile = tmp_path / "geo.h5"
+    res2 = runner.invoke(cli.folder2h5, [tmp_path.as_posix(), "--outfile", outfile])
+    assert res2.exit_code == 0
+    assert outfile.is_file()
+    geo = Geometry.from_file(outfile)
+
+    assert "Bath" in geo.markers
+    bath_marker = geo.markers["Bath"][0]
+    assert bath_marker in geo.cfun.array()
+
+
 def test_create_lv_ellipsoid(tmp_path: Path):
     runner = CliRunner()
     res1 = runner.invoke(
         cli.create_lv_ellipsoid,
         ["--create-fibers", tmp_path.as_posix()],
     )
     assert res1.exit_code == 0
```

### Comparing `cardiac_geometries-0.7.0/tests/test_geometry.py` & `cardiac_geometries-0.8.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-0.7.0/tests/test_gmsh.py` & `cardiac_geometries-0.8.0/tests/test_gmsh.py`

 * *Files identical despite different names*

