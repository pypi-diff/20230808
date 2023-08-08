# Comparing `tmp/quicfire-tools-0.1.1.tar.gz` & `tmp/quicfire-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quicfire-tools-0.1.1.tar", last modified: Tue Aug  8 18:30:52 2023, max compression
+gzip compressed data, was "quicfire-tools-0.1.2.tar", last modified: Tue Aug  8 18:39:19 2023, max compression
```

## Comparing `quicfire-tools-0.1.1.tar` & `quicfire-tools-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/quicfire_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/quicfire_tools/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/quicfire_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 18:30:52.000000 quicfire-tools-0.1.1/quicfire_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:30:52.086427 quicfire-tools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 18:30:41.000000 quicfire-tools-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.119680 quicfire-tools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:39:19.119680 quicfire-tools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.107679 quicfire-tools-0.1.2/quicfire_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.103680 quicfire-tools-0.1.2/quicfire_tools/input-templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.111680 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QFire_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QFire_Bldg_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QFire_Plume_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QFire_Pyvista.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QP_buildout.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QUIC_fire.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_TopoInputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_buildings.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_fileoptions.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_landuse.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_metparams.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_movingcoords.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/QU_simparams.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/Runtime_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/gridlist
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/rasterorigin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/latest/sensor1.inp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.111680 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QFire_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QFire_Bldg_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QFire_Plume_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QP_buildout.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QUIC_fire.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_TopoInputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_buildings.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_fileoptions.inp
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_landuse.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_metparams.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_movingcoords.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/QU_simparams.inp
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/Runtime_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/gridlist
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/rasterorigin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.1.1/sensor1.inp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.115680 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QFire_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QFire_Bldg_Advanced_User_Inputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QFire_Plume_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QFire_Pyvista.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QP_buildout.inp
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QUIC_fire.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_TopoInputs.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_buildings.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      441 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_fileoptions.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)       20 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_landuse.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_metparams.inp
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_movingcoords.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/QU_simparams.inp
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/Runtime_Advanced_User_Inputs.inp
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/gridlist
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/rasterorigin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/input-templates/v5.2.3/sensor1.inp
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/quicfire_tools/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:39:19.119680 quicfire-tools-0.1.2/quicfire_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-08-08 18:39:19.000000 quicfire-tools-0.1.2/quicfire_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-08 18:39:19.000000 quicfire-tools-0.1.2/quicfire_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:39:19.000000 quicfire-tools-0.1.2/quicfire_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-08 18:39:19.000000 quicfire-tools-0.1.2/quicfire_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 18:39:19.000000 quicfire-tools-0.1.2/quicfire_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:39:19.119680 quicfire-tools-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-08 18:39:00.000000 quicfire-tools-0.1.2/setup.py
```

### Comparing `quicfire-tools-0.1.1/LICENSE` & `quicfire-tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.1/PKG-INFO` & `quicfire-tools-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.1.1/quicfire_tools/inputs.py` & `quicfire-tools-0.1.2/quicfire_tools/inputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.1/quicfire_tools/outputs.py` & `quicfire-tools-0.1.2/quicfire_tools/outputs.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.1/quicfire_tools/parameters.py` & `quicfire-tools-0.1.2/quicfire_tools/parameters.py`

 * *Files identical despite different names*

### Comparing `quicfire-tools-0.1.1/quicfire_tools.egg-info/PKG-INFO` & `quicfire-tools-0.1.2/quicfire_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quicfire-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Input and output management tools for the QUIC-Fire fire model
 Home-page: https://github.com/silvxlabs/quicfire-tools
 License: MIT
 Project-URL: Bug Tracker, https://github.com/silvxlabs/quicfire-tools/issues
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quicfire-tools-0.1.1/setup.py` & `quicfire-tools-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                  "Programming Language :: Python :: 3.9",
                  "Programming Language :: Python :: 3.10",
                  "Programming Language :: Python :: 3.11",
                  "Topic :: Scientific/Engineering", ],
     package_dir={"": "."},
     packages=find_packages(exclude=["docs", "tests"]),
     package_data={
-        'quicfire_tools': ['input-templates/'],
+        'quicfire_tools': ['input-templates/*/*'],
     },
     include_package_data=True,
     install_requires=[
         "numpy",
         "pydantic>=2",
         "zarr>=2",
     ],
```

