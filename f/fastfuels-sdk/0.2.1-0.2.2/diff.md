# Comparing `tmp/fastfuels-sdk-0.2.1.tar.gz` & `tmp/fastfuels-sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastfuels-sdk-0.2.1.tar", last modified: Mon Jul 17 16:15:55 2023, max compression
+gzip compressed data, was "fastfuels-sdk-0.2.2.tar", last modified: Mon Aug  7 23:33:15 2023, max compression
```

## Comparing `fastfuels-sdk-0.2.1.tar` & `fastfuels-sdk-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:15:55.246206 fastfuels-sdk-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-17 16:15:55.246206 fastfuels-sdk-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:15:55.246206 fastfuels-sdk-0.2.1/fastfuels_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18434 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/fuelgrids.py
--rw-r--r--   0 runner    (1001) docker     (123)    23730 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/fastfuels_sdk/treelists.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:15:55.246206 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-17 16:15:55.000000 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 16:15:55.000000 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:15:55.000000 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-17 16:15:55.000000 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 16:15:55.000000 fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 16:15:55.246206 fastfuels-sdk-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-17 16:15:43.000000 fastfuels-sdk-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/fastfuels_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/fuelgrids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/fastfuels_sdk/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/templates/duet_input.template
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/templates/fds_input.template
+-rw-r--r--   0 runner    (1001) docker     (123)    23730 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/fastfuels_sdk/treelists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-07 23:33:15.000000 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-07 23:33:15.000000 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 23:33:15.000000 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-07 23:33:15.000000 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-07 23:33:15.000000 fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 23:33:15.541533 fastfuels-sdk-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-08-07 23:33:04.000000 fastfuels-sdk-0.2.2/setup.py
```

### Comparing `fastfuels-sdk-0.2.1/LICENSE` & `fastfuels-sdk-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/PKG-INFO` & `fastfuels-sdk-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: 3D Fuels for Next Generation Fire Models
 Home-page: https://github.com/silvxlabs/fastfuels-sdk-python
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/fastfuels-sdk-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,18 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python SDK for the FastFuels API
 
+## Quick-Links
+
+[Documentation](https://silvxlabs.github.io/fastfuels-sdk-python/) - [PyPi Package](https://pypi.org/project/fastfuels-sdk/) - [Project Description](https://www.firelab.org/project/fastfuels-3d-fuels-next-generation-fire-models)
+
 ## What is FastFuels?
 
 FastFuels is an innovative solution that propels the use of advanced 3D fire 
 models into the future of fire and fuels management. It acts as a "3D fuels 
 superhighway," seamlessly merging existing data sources with cutting-edge 
 modeling to produce the detailed 3D fuel data required by these models. With 
 its unique ability to generate and manage comprehensive fuels data for large
```

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/__init__.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/_base.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/_base.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/api.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/api.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/datasets.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/exports.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/exports.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,17 @@
 
 # External imports
 import numpy as np
 import zarr.hierarchy
 from numpy import ndarray
 from scipy.io import FortranFile
 
-try:
-    # Python 3.9+
-    TEMPLATES_PATH = importlib.resources.files('fastfuels_sdk'). \
-    joinpath('templates')
-except AttributeError:
-    # Python 3.6-3.8
+try:  # Python 3.9+
+    TEMPLATES_PATH = importlib.resources.files('fastfuels_sdk').joinpath('templates')
+except AttributeError:  # Python 3.6-3.8
     from pkg_resources import resource_filename
     TEMPLATES_PATH = resource_filename('fastfuels_sdk', 'templates')
 
 
 def export_zarr_to_quicfire(zroot: zarr.hierarchy.Group,
                             output_dir: Path | str) -> None:
     """
@@ -315,17 +312,17 @@
         template = Template(fin.read())
     with open(Path(output_dir, "template.fds"), "w") as fout:
         fout.write(template.substitute(fds_attrs))
 
 
 def _get_voxel_centers(nx: int, ny: int, nz: int, dx: float, dy: float,
                        dz: float):
-    x_vec = np.linspace(dx / 2, nx*dx - dx / 2, nx)
-    y_vec = np.linspace(dy / 2, ny*dy - dy / 2, ny)
-    z_vec = np.linspace(dz / 2, nz*dz - dz / 2, nz)
+    x_vec = np.linspace(dx / 2, nx * dx - dx / 2, nx)
+    y_vec = np.linspace(dy / 2, ny * dy - dy / 2, ny)
+    z_vec = np.linspace(dz / 2, nz * dz - dz / 2, nz)
     return np.meshgrid(x_vec, y_vec, z_vec, indexing='ij')
 
 
 def _adjust_z_values_by_dem(nz: int, zz: np.array, dem_array: np.array,
                             dz: float):
     for i in range(nz):
         zval = zz[:, :, i] + dem_array
```

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/fuelgrids.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/fuelgrids.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk/treelists.py` & `fastfuels-sdk-0.2.2/fastfuels_sdk/treelists.py`

 * *Files identical despite different names*

### Comparing `fastfuels-sdk-0.2.1/fastfuels_sdk.egg-info/PKG-INFO` & `fastfuels-sdk-0.2.2/fastfuels_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastfuels-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: 3D Fuels for Next Generation Fire Models
 Home-page: https://github.com/silvxlabs/fastfuels-sdk-python
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/fastfuels-sdk-python/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,18 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python SDK for the FastFuels API
 
+## Quick-Links
+
+[Documentation](https://silvxlabs.github.io/fastfuels-sdk-python/) - [PyPi Package](https://pypi.org/project/fastfuels-sdk/) - [Project Description](https://www.firelab.org/project/fastfuels-3d-fuels-next-generation-fire-models)
+
 ## What is FastFuels?
 
 FastFuels is an innovative solution that propels the use of advanced 3D fire 
 models into the future of fire and fuels management. It acts as a "3D fuels 
 superhighway," seamlessly merging existing data sources with cutting-edge 
 modeling to produce the detailed 3D fuel data required by these models. With 
 its unique ability to generate and manage comprehensive fuels data for large
```

### Comparing `fastfuels-sdk-0.2.1/setup.py` & `fastfuels-sdk-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,10 +50,14 @@
                  "Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
                  "Programming Language :: Python :: 3.11",
                  "Topic :: Scientific/Engineering", ],
     package_dir={"": "."},
     packages=find_packages(exclude=["docs", "tests"]),
+    package_data={
+        'fastfuels_sdk': ['templates/*.template'],
+    },
+    include_package_data=True,
     install_requires=INSTALL_REQUIRES,
     python_requires=">=3.8",
 )
```

