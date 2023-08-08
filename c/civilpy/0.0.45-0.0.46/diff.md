# Comparing `tmp/civilpy-0.0.45.tar.gz` & `tmp/civilpy-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.45.tar", last modified: Fri Jun  2 14:28:51 2023, max compression
+gzip compressed data, was "civilpy-0.0.46.tar", last modified: Tue Aug  8 05:02:18 2023, max compression
```

## Comparing `civilpy-0.0.45.tar` & `civilpy-0.0.46.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.677655 civilpy-0.0.45/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-06-02 13:37:25.000000 civilpy-0.0.45/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-02 13:37:25.000000 civilpy-0.0.45/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-02 13:37:25.000000 civilpy-0.0.45/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4750 2023-06-02 14:28:51.673655 civilpy-0.0.45/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4148 2023-06-02 13:37:25.000000 civilpy-0.0.45/README.md
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 13:37:25.000000 civilpy-0.0.45/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-06-02 13:59:42.000000 civilpy-0.0.45/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 14:28:51.677655 civilpy-0.0.45/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2642 2023-06-02 13:59:42.000000 civilpy-0.0.45/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.669655 civilpy-0.0.45/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42197 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16514 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20861 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)     5946 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-02 14:28:31.000000 civilpy-0.0.45/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18085 2023-06-02 13:37:25.000000 civilpy-0.0.45/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4750 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 14:28:51.000000 civilpy-0.0.45/src/civilpy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:28:51.673655 civilpy-0.0.45/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13769 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     5324 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_project.py
--rw-rw-rw-   0 root         (0) root         (0)    13098 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_ohio_dot_snbi_transfer.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2023-06-02 13:37:25.000000 civilpy-0.0.45/tests/test_steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.789254 civilpy-0.0.46/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-08-08 03:31:31.000000 civilpy-0.0.46/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-08 03:31:31.000000 civilpy-0.0.46/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 03:31:31.000000 civilpy-0.0.46/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 05:02:18.785254 civilpy-0.0.46/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-08-08 03:31:31.000000 civilpy-0.0.46/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 03:31:32.000000 civilpy-0.0.46/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-08-08 03:31:32.000000 civilpy-0.0.46/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 05:02:18.789254 civilpy-0.0.46/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-08-08 04:42:27.000000 civilpy-0.0.46/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.773254 civilpy-0.0.46/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42197 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16514 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20861 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 05:01:57.000000 civilpy-0.0.46/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18085 2023-08-08 03:31:34.000000 civilpy-0.0.46/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 05:02:18.000000 civilpy-0.0.46/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 05:02:18.785254 civilpy-0.0.46/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13769 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-08-08 04:10:36.000000 civilpy-0.0.46/tests/test_ohio_dot_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    13098 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_ohio_dot_snbi_transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2023-08-08 03:31:34.000000 civilpy-0.0.46/tests/test_steel.py
```

### Comparing `civilpy-0.0.45/.gitlab-ci.yml` & `civilpy-0.0.46/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/LICENSE` & `civilpy-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/PKG-INFO` & `civilpy-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.45
+Version: 0.0.46
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
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.45 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.46 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.45/README.md` & `civilpy-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/requirements.txt` & `civilpy-0.0.46/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-beautifulsoup4==4.11.2
+beautifulsoup4~=4.11.1
 folium==0.14.0
 matplotlib==3.6.3
 numpy==1.24.1
-pandas==1.5.3
+pandas~=1.5.2
 Pillow==9.4.0
 Pint==0.20.1
 psycopg2==2.9.5
 psycopg2_binary==2.9.5
 requests==2.28.2
-setuptools==65.6.3
+setuptools~=65.5.1
 sshtunnel==0.4.0
 sympy==1.11.1
 PySimpleGUI~=4.60.4
 html5lib~=1.1
 lxml~=4.9.2
 soupsieve~=2.4.1
 defusedxml~=0.7.1
@@ -51,11 +51,13 @@
 ipykernel~=6.22.0
 tornado~=6.3
 docutils~=0.20
 kiwisolver~=1.4.4
 zipp~=3.15.0
 build~=0.10.0
 wheel~=0.38.4
-civilpy~=0.0.42
-tifftools~=1.3.9
-natsort~=8.3.1
-pyntcloud~=0.3.1
+civilpy~=0.0.23
+tifftools~=1.3.7
+natsort~=8.2.0
+pyntcloud~=0.3.1
+kivymd~=1.1.1
+PyQt5~=5.15.9
```

### Comparing `civilpy-0.0.45/setup.py` & `civilpy-0.0.46/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.45',
+    version='0.0.46',
     packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     py_modules=[
         "civilpy.state.ohio.dot",
@@ -24,15 +24,16 @@
         "civilpy.general.physics",
         "civilpy.general.plan_development",
         "civilpy.general.pointclouds",
         "civilpy.structural.beam_bending",
         "civilpy.structural.search_tools",
         "civilpy.structural.steel",
         "civilpy.water_resources.hydraulics",
-        "civilpy.CLI"
+        "civilpy.CLI",
+        "civilpy.kivy"
     ],
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
@@ -73,13 +74,15 @@
         "pyntcloud>=0.3.1",
         "laspy>=2.4.1",
         "openpyxl>=3.1.2",
         "earthpy>=0.9.4",
         "pymupdf>=1.22.3",
         "tqdm>=4.65.0",
         "pyodbc>=4.0.39",
-        "pytesseract>=0.3.10"
+        "pytesseract>=0.3.10",
+        "kivymd>=1.1.1",
+        "PyQt5>=5.15.9"
     ],
 
     extras_require={
     }
 )
```

### Comparing `civilpy-0.0.45/src/civilpy/general/database_tools.py` & `civilpy-0.0.46/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/general/microstation.py` & `civilpy-0.0.46/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/general/photos.py` & `civilpy-0.0.46/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.46/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.46/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.46/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.46/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.46/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.46/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.46/src/civilpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.45
+Version: 0.0.46
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
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.45 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.46 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.45/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.46/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.46/src/civilpy.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -29,7 +29,9 @@
 laspy>=2.4.1
 openpyxl>=3.1.2
 earthpy>=0.9.4
 pymupdf>=1.22.3
 tqdm>=4.65.0
 pyodbc>=4.0.39
 pytesseract>=0.3.10
+kivymd>=1.1.1
+PyQt5>=5.15.9
```

### Comparing `civilpy-0.0.45/tests/test_ohio_dot_bridge.py` & `civilpy-0.0.46/tests/test_ohio_dot_bridge.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/tests/test_ohio_dot_functions.py` & `civilpy-0.0.46/tests/test_ohio_dot_functions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/tests/test_ohio_dot_project.py` & `civilpy-0.0.46/tests/test_ohio_dot_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,89 +3,89 @@
 
 # //TODO - Fix this test, unstable API
 
 
 class TestProject(unittest.TestCase):
     def setUp(self):
         # Creates a 'test project' and makes sure none of the attributes have changed
-        self.tp = Project(pid='96213')
+        self.tp = Project(pid='112664')
 
     def tearDown(self):
         pass
 
     def test_init(self):
         # //TODO - make tests less dependent on getting specific values from project points arrays
         self.assertIsInstance(self.tp.objectid, int)
         self.assertIsInstance(self.tp.gis_id, int)
-        self.assertEqual(self.tp.pid_nbr, 96213)
+        self.assertEqual(self.tp.pid_nbr, 112664)
         self.assertEqual(self.tp.district_nbr, 6)
-        self.assertEqual(self.tp.locale_short_nme, 'MRW')
-        self.assertEqual(self.tp.county_nme, 'Morrow')
-        self.assertEqual(self.tp.project_nme, 'MRW SR 314 (8.080) (20.57)')
+        self.assertEqual(self.tp.locale_short_nme, 'D06')
+        self.assertEqual(self.tp.county_nme, 'District 6')
+        self.assertEqual(self.tp.project_nme, 'D06-FY23 Bridge Repair')
         self.assertEqual(self.tp.contract_type, 'Standard Build')
         self.assertEqual(self.tp.primary_fund_category_txt, 'District Preservation (Pv & Br)')
-        self.assertEqual(self.tp.project_manager_nme, 'HIPP, JEFFREY P')
+        self.assertEqual(self.tp.project_manager_nme, 'PARKS, DANE RICHARD')
         self.assertEqual(self.tp.reservoir_year, None)
         self.assertEqual(self.tp.tier, None)
         self.assertEqual(self.tp.odot_letting, 'ODOT Let')
         self.assertEqual(self.tp.schedule_type_short_nme, 'Standard')
-        self.assertEqual(self.tp.env_project_manager_nme, 'TURNER, AMY S')
-        self.assertEqual(self.tp.area_engineer_nme, 'DENNIS, WADE R')
-        self.assertEqual(self.tp.project_engineer_nme, 'STOVER, DONALD L')
+        self.assertEqual(self.tp.env_project_manager_nme, 'GARTNER, JANICE M')
+        self.assertEqual(self.tp.area_engineer_nme, 'VANCE, JEFFREY A')
+        self.assertEqual(self.tp.project_engineer_nme, 'FIRIS, BENJAMIN L')
         self.assertEqual(self.tp.design_agency, 'DISTRICT 6-ENGINEERING')
-        self.assertEqual(self.tp.sponsoring_agency, 'DISTRICT 6-PLANNING')
-        self.assertEqual(self.tp.pdp_short_name, 'Path 2')
+        self.assertEqual(self.tp.sponsoring_agency, 'DISTRICT 6-BRIDGES')
+        self.assertEqual(self.tp.pdp_short_name, 'Path 1')
         self.assertEqual(self.tp.primary_work_category, 'Bridge Preservation')
-        self.assertEqual(self.tp.project_status, 'Not Filed')
-        self.assertEqual(self.tp.fiscal_year, '2024')
-        self.assertEqual(self.tp.inhouse_design_full_nme, 'HIPP, JEFFREY P')
-        self.assertEqual(self.tp.est_total_constr_cost, 650000)
-        self.assertEqual(self.tp.state_project_nbr, None)
-        self.assertEqual(self.tp.constr_vendor_nme, None)
+        self.assertEqual(self.tp.project_status, 'Awarded')
+        self.assertEqual(self.tp.fiscal_year, '2023')
+        self.assertEqual(self.tp.inhouse_design_full_nme, 'BLOOR, CLAYTON  ')
+        self.assertEqual(self.tp.est_total_constr_cost, 469316.5)
+        self.assertEqual(self.tp.state_project_nbr, '230339')
+        self.assertEqual(self.tp.constr_vendor_nme, 'EVERS STEEL CONSTRUCTION LLC')
         self.assertEqual(self.tp.stip_flag, 'N')
         self.assertEqual(self.tp.current_stip_co_amt, None)
-        self.assertEqual(self.tp.project_plans_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1002&PID_NUM=96213')
-        self.assertEqual(self.tp.project_addenda_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1000&PID_NUM=96213')
-        self.assertEqual(self.tp.project_proposal_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1003&PID_NUM=96213')
+        self.assertEqual(self.tp.project_plans_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1002&PID_NUM=112664')
+        self.assertEqual(self.tp.project_addenda_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1000&PID_NUM=112664')
+        self.assertEqual(self.tp.project_proposal_url, 'http://contracts.dot.state.oh.us/search.jsp?cabinetId=1003&PID_NUM=112664')
         self.assertEqual(self.tp.fmis_proj_desc, None)
-        self.assertEqual(self.tp.award_milestone_dt, 1699228800000)
-        self.assertEqual(self.tp.begin_constr_milestone_dt, 1713139200000)
-        self.assertEqual(self.tp.end_constr_milestone_dt, 1722470400000)
+        self.assertEqual(self.tp.award_milestone_dt, 1685664000000)
+        self.assertEqual(self.tp.begin_constr_milestone_dt, 1688947200000)
+        self.assertEqual(self.tp.end_constr_milestone_dt, 1697328000000)
         self.assertEqual(self.tp.open_traffic_dt, None)
         self.assertEqual(self.tp.central_office_close_dt, None)
         self.assertIsInstance(self.tp.source_last_updated, int)
         self.assertIsInstance(self.tp.cod_last_updated, int)
         self.assertEqual(self.tp.preserv_funds_ind, 'Y')
         self.assertEqual(self.tp.major_brg_funds_ind, 'N')
         self.assertEqual(self.tp.major_new_funds_ind, 'N')
         self.assertEqual(self.tp.major_rehab_funds_ind, 'N')
         self.assertEqual(self.tp.mpo_funds_ind, 'N')
         self.assertEqual(self.tp.safety_funds_ind, 'N')
         self.assertEqual(self.tp.local_funds_ind, 'N')
         self.assertEqual(self.tp.other_funds_ind, 'N')
-        self.assertEqual(self.tp.nlf_id, 'SMRWSR00314**C')
+        self.assertEqual(self.tp.nlf_id, 'SUNIUS00033**N')
         self.assertIsInstance(self.tp.ctl_begin, float)
         self.assertEqual(self.tp.ctl_end, None)
         self.assertEqual(self.tp.gis_feature_type, 'POINT')
-        self.assertEqual(self.tp.route_type, 'SR')
-        self.assertEqual(self.tp.route_id, '00314')
+        self.assertEqual(self.tp.route_type, 'US')
+        self.assertEqual(self.tp.route_id, '00033')
         self.assertIsInstance(self.tp.structure_file_nbr, str)
         self.assertIsInstance(self.tp.main_structure_type, str)
         self.assertIsInstance(self.tp.sufficiency_rating, str)
         self.assertIsInstance(self.tp.ovrl_structure_length, int)
         self.assertIsInstance(self.tp.deck_area, int)
-        self.assertIsInstance(self.tp.deck_width, int)
-        self.assertEqual(self.tp.feature_intersect, '')
+        self.assertIsInstance(self.tp.deck_width, float)
+        self.assertEqual(self.tp.feature_intersect, 'UNDER HOLYCROSS-EPPS C158')
         self.assertIsInstance(self.tp.year_built, str)
         self.assertIsInstance(self.tp.longitude_begin_nbr, float)
         self.assertIsInstance(self.tp.latitude_begin_nbr, float)
         self.assertEqual(self.tp.longitude_end_nbr, None)
         self.assertEqual(self.tp.latitude_end_nbr, None)
-        self.assertEqual(self.tp.county_cd_work_location, 'MRW')
-        self.assertEqual(self.tp.county_nme_work_location, 'MORROW')
+        self.assertEqual(self.tp.county_cd_work_location, 'UNI')
+        self.assertEqual(self.tp.county_nme_work_location, 'UNION')
         self.assertEqual(self.tp.district_work_location, '06')
         self.assertEqual(self.tp.pavement_treatment_type, None)
         self.assertEqual(self.tp.pavement_treatment_category, None)
         self.assertEqual(self.tp.created_user, 'TIMS@P31_AG')
         self.assertIsInstance(self.tp.created_date, int)
         self.assertEqual(self.tp.last_edited_user, 'TIMS@P31_AG')
         self.assertIsInstance(self.tp.last_edited_date, int)
```

### Comparing `civilpy-0.0.45/tests/test_ohio_dot_snbi_transfer.py` & `civilpy-0.0.46/tests/test_ohio_dot_snbi_transfer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.45/tests/test_steel.py` & `civilpy-0.0.46/tests/test_steel.py`

 * *Files identical despite different names*

