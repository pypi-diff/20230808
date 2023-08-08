# Comparing `tmp/civilpy-0.0.46.tar.gz` & `tmp/civilpy-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.46.tar", last modified: Tue Aug  8 05:02:18 2023, max compression
+gzip compressed data, was "civilpy-0.0.47.tar", last modified: Tue Aug  8 15:44:57 2023, max compression
```

## Comparing `civilpy-0.0.46.tar` & `civilpy-0.0.47.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.789254 civilpy-0.0.46/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-08-08 03:31:31.000000 civilpy-0.0.46/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-08 03:31:31.000000 civilpy-0.0.46/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 03:31:31.000000 civilpy-0.0.46/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 05:02:18.785254 civilpy-0.0.46/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4148 2023-08-08 03:31:31.000000 civilpy-0.0.46/README.md
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 03:31:32.000000 civilpy-0.0.46/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-08-08 03:31:32.000000 civilpy-0.0.46/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 05:02:18.789254 civilpy-0.0.46/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-08-08 04:42:27.000000 civilpy-0.0.46/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.773254 civilpy-0.0.46/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42197 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16514 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20861 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18085 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1353 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13769 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-08-08 04:10:36.000000 civilpy-0.0.46/tests/test_ohio_dot_project.py
--rw-rw-rw-   0 root         (0) root         (0)    13098 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_snbi_transfer.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-08-08 03:31:31.000000 civilpy-0.0.47/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-08 03:31:31.000000 civilpy-0.0.47/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 03:31:31.000000 civilpy-0.0.47/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 15:44:57.191922 civilpy-0.0.47/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-08-08 03:31:31.000000 civilpy-0.0.47/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 03:31:32.000000 civilpy-0.0.47/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-08-08 03:31:32.000000 civilpy-0.0.47/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 15:44:57.191922 civilpy-0.0.47/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-08-08 14:40:28.000000 civilpy-0.0.47/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.179921 civilpy-0.0.47/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42197 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16514 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20861 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2023-08-08 14:40:28.000000 civilpy-0.0.47/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18085 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13769 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-08-08 04:10:36.000000 civilpy-0.0.47/tests/test_ohio_dot_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    13098 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_snbi_transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3371 2023-08-08 15:27:03.000000 civilpy-0.0.47/tests/test_steel.py
```

### Comparing `civilpy-0.0.46/.gitlab-ci.yml` & `civilpy-0.0.47/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/LICENSE` & `civilpy-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/PKG-INFO` & `civilpy-0.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.46
+Version: 0.0.47
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.46 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.47 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.46/README.md` & `civilpy-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/requirements.txt` & `civilpy-0.0.47/requirements.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/setup.py` & `civilpy-0.0.47/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.46',
+    version='0.0.47',
     packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     py_modules=[
         "civilpy.state.ohio.dot",
```

### Comparing `civilpy-0.0.46/src/civilpy/general/database_tools.py` & `civilpy-0.0.47/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/general/microstation.py` & `civilpy-0.0.47/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/general/photos.py` & `civilpy-0.0.47/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.47/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.47/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.47/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.47/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.47/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy/structural/steel.py` & `civilpy-0.0.47/src/civilpy/structural/steel.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,30 +107,30 @@
         self.detailing_web_thickness = float(self.aisc_value['twdet'].values[0]) * units('in')  # in (mm)
         self.half_web_detail = float(self.aisc_value['twdet/2'].values[0]) * units('in')  # in (mm)
         self.flange_thickness = float(self.aisc_value['tf'].values[0]) * units('in')  # in (mm)
         self.detailing_flange_thickness = float(self.aisc_value['tfdet'].values[0]) * units('in')  # in (mm)
         self.k_design = float(self.aisc_value['kdes'].values[0]) * units('in')  # in (mm)
         self.k_detailing = float(self.aisc_value['kdet'].values[0]) * units('in')  # in (mm)
         self.k1 = float(self.aisc_value['k1'].values[0]) * units('in')  # in (mm)
-        self.slenderness_ratio_flange = float(self.aisc_value['bf/2tf'])
-        self.slenderness_ratio_web = float(self.aisc_value['h/tw'])
-        self.J = float(self.aisc_value['J']) * units('in^4')  # in^4 (mm^4 / 10^3)
-        self.Cw = float(self.aisc_value['Cw']) * units('in^6')  # in^6 (mm^6 / 10^9)
-        self.Wno = float(self.aisc_value['Wno']) * units('in^2')  # in^2 (mm^2)
-        self.Sw1 = float(self.aisc_value['Sw1']) * units('in^4')  # in^4 (mm^4 / 10^6)
-        self.Qf = float(self.aisc_value['Qf']) * units('in^3')  # in^3 (mm^3 / 10^3)
-        self.Qw = float(self.aisc_value['Qw']) * units('in^3')  # in^3 (mm^3 / 10^3)
-        self.radius_of_gyration = self.rts = float(self.aisc_value['rts']) * units('in')  # in (mm)
-        self.flange_centroid_distance = float(self.aisc_value['ho']) * units('in')  # in (mm)
-        self.exposed_perimeter = float(self.aisc_value['PA']) * units('in')  # in (mm)
-        self.shape_perimeter = float(self.aisc_value['PB']) * units('in')  # in (mm)
-        self.box_perimeter = float(self.aisc_value['PC']) * units('in')  # in (mm)
-        self.exposed_box_perimeter = float(self.aisc_value['PD']) * units('in')  # in (mm)
-        self.web_face_depth = self.T = float(self.aisc_value['T']) * units('in')  # in (mm)
-        self.fastener_workable_gage = self.WGi = float(self.aisc_value['WGi']) * units('in')  # in (mm)
+        self.slenderness_ratio_flange = float(self.aisc_value['bf/2tf'].values[0])
+        self.slenderness_ratio_web = float(self.aisc_value['h/tw'].values[0])
+        self.J = float(self.aisc_value['J'].values[0]) * units('in^4')  # in^4 (mm^4 / 10^3)
+        self.Cw = float(self.aisc_value['Cw'].values[0]) * units('in^6')  # in^6 (mm^6 / 10^9)
+        self.Wno = float(self.aisc_value['Wno'].values[0]) * units('in^2')  # in^2 (mm^2)
+        self.Sw1 = float(self.aisc_value['Sw1'].values[0]) * units('in^4')  # in^4 (mm^4 / 10^6)
+        self.Qf = float(self.aisc_value['Qf'].values[0]) * units('in^3')  # in^3 (mm^3 / 10^3)
+        self.Qw = float(self.aisc_value['Qw'].values[0]) * units('in^3')  # in^3 (mm^3 / 10^3)
+        self.radius_of_gyration = self.rts = float(self.aisc_value['rts'].values[0]) * units('in')  # in (mm)
+        self.flange_centroid_distance = float(self.aisc_value['ho'].values[0]) * units('in')  # in (mm)
+        self.exposed_perimeter = float(self.aisc_value['PA'].values[0]) * units('in')  # in (mm)
+        self.shape_perimeter = float(self.aisc_value['PB'].values[0]) * units('in')  # in (mm)
+        self.box_perimeter = float(self.aisc_value['PC'].values[0]) * units('in')  # in (mm)
+        self.exposed_box_perimeter = float(self.aisc_value['PD'].values[0]) * units('in')  # in (mm)
+        self.web_face_depth = self.T = float(self.aisc_value['T'].values[0]) * units('in')  # in (mm)
+        self.fastener_workable_gage = self.WGi = float(self.aisc_value['WGi'].values[0]) * units('in')  # in (mm)
 
 
 class MBeam(WBeam):
     """
     Class to provide more specific attributes and functions related to designing with
     steel M beams. Splitting values into multiple classes allows dropping of empty values
     in the database.
```

### Comparing `civilpy-0.0.46/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.47/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.47/src/civilpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.46
+Version: 0.0.47
 Summary: Civil Engineering Tools in Python
 Home-page: https://daneparks.com/Dane/civilpy
 Author: Dane Parks
 Author-email: Dane@daneparks.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.46 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.47 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.46/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.47/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.47/src/civilpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/tests/test_ohio_dot_bridge.py` & `civilpy-0.0.47/tests/test_ohio_dot_bridge.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/tests/test_ohio_dot_functions.py` & `civilpy-0.0.47/tests/test_ohio_dot_functions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/tests/test_ohio_dot_project.py` & `civilpy-0.0.47/tests/test_ohio_dot_project.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.46/tests/test_ohio_dot_snbi_transfer.py` & `civilpy-0.0.47/tests/test_ohio_dot_snbi_transfer.py`

 * *Files identical despite different names*

