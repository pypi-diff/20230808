# Comparing `tmp/civilpy-0.0.47.tar.gz` & `tmp/civilpy-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civilpy-0.0.47.tar", last modified: Tue Aug  8 15:44:57 2023, max compression
+gzip compressed data, was "civilpy-0.0.48.tar", last modified: Tue Aug  8 18:43:04 2023, max compression
```

## Comparing `civilpy-0.0.47.tar` & `civilpy-0.0.48.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2023-08-08 03:31:31.000000 civilpy-0.0.47/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-08 03:31:31.000000 civilpy-0.0.47/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 03:31:31.000000 civilpy-0.0.47/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 15:44:57.191922 civilpy-0.0.47/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4148 2023-08-08 03:31:31.000000 civilpy-0.0.47/README.md
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 03:31:32.000000 civilpy-0.0.47/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-08-08 03:31:32.000000 civilpy-0.0.47/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 15:44:57.191922 civilpy-0.0.47/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-08-08 14:40:28.000000 civilpy-0.0.47/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.179921 civilpy-0.0.47/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/construction/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/construction/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/environmental/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/environmental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/general/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/database_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/gis.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/kml_tools.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/math.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/microstation.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/photos.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/physics.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/general/plan_development.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/general/pointclouds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/geotechnical/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/geotechnical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/state/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/state/ohio/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/D6_file_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42197 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/dot.py
--rw-rw-rw-   0 root         (0) root         (0)    16514 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/search_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    91957 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/state/ohio/snbi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/structural/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/structural/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20861 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/structural/beam_bending.py
--rw-rw-rw-   0 root         (0) root         (0)    14520 2023-08-08 14:40:28.000000 civilpy-0.0.47/src/civilpy/structural/steel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/transportation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/transportation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/src/civilpy/water_resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:44:34.000000 civilpy-0.0.47/src/civilpy/water_resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18085 2023-08-08 03:31:34.000000 civilpy-0.0.47/src/civilpy/water_resources/hydraulics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.187921 civilpy-0.0.47/src/civilpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1353 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 15:44:57.000000 civilpy-0.0.47/src/civilpy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:44:57.191922 civilpy-0.0.47/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13769 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     5396 2023-08-08 04:10:36.000000 civilpy-0.0.47/tests/test_ohio_dot_project.py
--rw-rw-rw-   0 root         (0) root         (0)    13098 2023-08-08 03:31:34.000000 civilpy-0.0.47/tests/test_ohio_dot_snbi_transfer.py
--rw-rw-rw-   0 root         (0) root         (0)     3371 2023-08-08 15:27:03.000000 civilpy-0.0.47/tests/test_steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.556777 civilpy-0.0.48/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2023-08-08 03:31:31.000000 civilpy-0.0.48/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-08-08 03:31:31.000000 civilpy-0.0.48/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-08-08 03:31:31.000000 civilpy-0.0.48/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 18:43:04.552777 civilpy-0.0.48/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4148 2023-08-08 03:31:31.000000 civilpy-0.0.48/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-08-08 03:31:32.000000 civilpy-0.0.48/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-08-08 03:31:32.000000 civilpy-0.0.48/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 18:43:04.556777 civilpy-0.0.48/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-08-08 18:42:44.000000 civilpy-0.0.48/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.548777 civilpy-0.0.48/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/construction/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/construction/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/environmental/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/environmental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/general/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/general/database_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/gis.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/kml_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/math.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/general/microstation.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/general/photos.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/physics.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/general/plan_development.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/general/pointclouds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/geotechnical/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/geotechnical/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/state/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/state/ohio/
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/state/ohio/D6_file_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/state/ohio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42197 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/state/ohio/dot.py
+-rw-rw-rw-   0 root         (0) root         (0)    16514 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/state/ohio/search_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    91957 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/state/ohio/snbi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/structural/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/structural/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20861 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/structural/beam_bending.py
+-rw-rw-rw-   0 root         (0) root         (0)    13959 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/structural/steel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/transportation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/transportation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy/water_resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 18:42:44.000000 civilpy-0.0.48/src/civilpy/water_resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18085 2023-08-08 03:31:34.000000 civilpy-0.0.48/src/civilpy/water_resources/hydraulics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/src/civilpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-08-08 18:43:04.000000 civilpy-0.0.48/src/civilpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-08-08 18:43:04.000000 civilpy-0.0.48/src/civilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 18:43:04.000000 civilpy-0.0.48/src/civilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      605 2023-08-08 18:43:04.000000 civilpy-0.0.48/src/civilpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-08 18:43:04.000000 civilpy-0.0.48/src/civilpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 18:43:04.552777 civilpy-0.0.48/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13769 2023-08-08 03:31:34.000000 civilpy-0.0.48/tests/test_ohio_dot_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2023-08-08 03:31:34.000000 civilpy-0.0.48/tests/test_ohio_dot_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-08-08 04:10:36.000000 civilpy-0.0.48/tests/test_ohio_dot_project.py
+-rw-rw-rw-   0 root         (0) root         (0)    13098 2023-08-08 03:31:34.000000 civilpy-0.0.48/tests/test_ohio_dot_snbi_transfer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2023-08-08 18:42:44.000000 civilpy-0.0.48/tests/test_steel.py
```

### Comparing `civilpy-0.0.47/.gitlab-ci.yml` & `civilpy-0.0.48/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/LICENSE` & `civilpy-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/PKG-INFO` & `civilpy-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.47
+Version: 0.0.48
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
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.47 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.48 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.47/README.md` & `civilpy-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/requirements.txt` & `civilpy-0.0.48/requirements.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/setup.py` & `civilpy-0.0.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='civilpy',
-    version='0.0.47',
+    version='0.0.48',
     packages=find_packages('src', exclude=['test', 'secrets', 'docs', 'res']),
     description='Civil Engineering Tools in Python',
     url="https://daneparks.com/Dane/civilpy",
     author_email="Dane@daneparks.com",
     author="Dane Parks",
     py_modules=[
         "civilpy.state.ohio.dot",
```

### Comparing `civilpy-0.0.47/src/civilpy/general/database_tools.py` & `civilpy-0.0.48/src/civilpy/general/database_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/general/microstation.py` & `civilpy-0.0.48/src/civilpy/general/microstation.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/general/photos.py` & `civilpy-0.0.48/src/civilpy/general/photos.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/state/ohio/D6_file_explorer.py` & `civilpy-0.0.48/src/civilpy/state/ohio/D6_file_explorer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/state/ohio/dot.py` & `civilpy-0.0.48/src/civilpy/state/ohio/dot.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/state/ohio/search_tools.py` & `civilpy-0.0.48/src/civilpy/state/ohio/search_tools.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/state/ohio/snbi.py` & `civilpy-0.0.48/src/civilpy/state/ohio/snbi.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/structural/beam_bending.py` & `civilpy-0.0.48/src/civilpy/structural/beam_bending.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy/structural/steel.py` & `civilpy-0.0.48/src/civilpy/structural/steel.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,42 +8,40 @@
 
 def hello_world(user_input="World"):
     return f"Hello {user_input}!"
 
 
 class SteelSection:
     """
-    Main Steel Section Class, the goal is to make the attributes of various steel
-    sections easily accessible in various python scripts.
+    Main Steel Section Class, the goal is to make the attributes of various
+    steel sections easily accessible in various python scripts.
 
     # //TODO - Add Rebar values
-    # //TODO - Integrate Units
-    # //TODO - Metric toggle
-    # //TODO - Add Definitions for members other than W-Shapes
     """
 
     def __init__(self, label):
         self.id = self.clean_user_input(label)
         self.aisc_value = self.get_shape()
 
         self.special_note = self.aisc_value['T_F'].values[0]
-        self.weight = self.W = self.aisc_value['W'].values[0] * units('lb/ft')  # lb/ft (kg/m)
-        self.area = self.A = self.aisc_value['A'].values[0] * units('in^2')  # in^2  (mm^2)
-        self.I_x = self.aisc_value['Ix'].values[0] * units('in^4')  # in^4  (mm^4 / 10^6)
-        self.Z_x = self.aisc_value['Zx'].values[0] * units('in^3')  # in^3  (mm^3 / 10^3)
-        self.S_x = self.aisc_value['Sx'].values[0] * units('in^3')  # in^3  (mm^3 / 10^3)
-        self.r_x = self.aisc_value['rx'].values[0] * units('in')  # in    (mm)
-        self.I_y = self.aisc_value['Iy'].values[0] * units('in^4')  # in^4  (mm^4/10^6)
-        self.Z_y = self.aisc_value['Zy'].values[0] * units('in^3')  # in^3  (mm^3/10^3)
-        self.S_y = self.aisc_value['Sy'].values[0] * units('in^3')  # in^3  (mm^3/10^3)
-        self.r_y = self.aisc_value['ry'].values[0] * units('in')  # in    (mm)
+        self.weight = self.W = self.aisc_value['W'].values[0] * units('lbf/ft')
+        self.area = self.A = self.aisc_value['A'].values[0] * units('in^2')
+        self.I_x = self.aisc_value['Ix'].values[0] * units('in^4')
+        self.Z_x = self.aisc_value['Zx'].values[0] * units('in^3')
+        self.S_x = self.aisc_value['Sx'].values[0] * units('in^3')
+        self.r_x = self.aisc_value['rx'].values[0] * units('in')
+        self.I_y = self.aisc_value['Iy'].values[0] * units('in^4')
+        self.Z_y = self.aisc_value['Zy'].values[0] * units('in^3')
+        self.S_y = self.aisc_value['Sy'].values[0] * units('in^3')
+        self.r_y = self.aisc_value['ry'].values[0] * units('in')
 
     def clean_user_input(self, user_input):
         """
-        Eliminates value not found errors by removing lower case letters and spaces
+        Eliminates value not found errors by removing lower case letters and
+        spaces
 
         >>> t = SteelSection("W 44X335")
         >>> print(t.clean_user_input('W 44X335'))
         W44X335
         >>> print(t.clean_user_input('w40x294'))
         W40X294
         >>> t.id
@@ -61,299 +59,339 @@
             cleaned_input = no_spaces.upper()
             self.id = cleaned_input
 
         return cleaned_input
 
     def get_shape(self):
         """
-        Searches AISC Steel database table for member label passed to it, returns values
-        from table if it finds a match, or prints an error if it doesn't
+        Searches AISC Steel database table for member label passed to it,
+        returns values from table if it finds a match, or prints an error if it
+        doesn't
 
         >>> t = SteelSection("W36X150")
         >>> t.aisc_value['Type'].values[0]
         'W'
 
         >>> t = SteelSection("2L8X4X5/8LLBB")
         >>> t.aisc_value['W'].values[0]
         48.4
 
         :param self:
         :return: dataframe of raw values from AISC Shape Table
         """
         try:
-            shape_values = steel_tables[steel_tables['EDI_Std_Nomenclature'] == self.id]
+            shape_values = steel_tables[
+                steel_tables['EDI_Std_Nomenclature'] == self.id]
             return shape_values
         except KeyError as e:
-            print("Value not found in shape table, check spelling and try again")
+            print("Value not found in shape table,"
+                  "check spelling and try again")
 
 
 class WBeam(SteelSection):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel W beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel W beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = WBeam("W36X150")
     >>> t.weight
     150.0 pound/foot
     """
 
     def __init__(self, label):
         super(WBeam, self).__init__(label)
-        self.depth = float(self.aisc_value['d'].values[0]) * units('in')  # in (mm)
-        self.detailing_depth = float(self.aisc_value['ddet'].values[0]) * units('in')  # in (mm)
-        self.flange_width = float(self.aisc_value['bf'].values[0]) * units('in')  # in (mm)
-        self.detailing_flange_width = float(self.aisc_value['bfdet'].values[0]) * units('in')  # in (mm)
-        self.web_thickness = float(self.aisc_value['tw'].values[0]) * units('in')  # in (mm)
-        self.detailing_web_thickness = float(self.aisc_value['twdet'].values[0]) * units('in')  # in (mm)
-        self.half_web_detail = float(self.aisc_value['twdet/2'].values[0]) * units('in')  # in (mm)
-        self.flange_thickness = float(self.aisc_value['tf'].values[0]) * units('in')  # in (mm)
-        self.detailing_flange_thickness = float(self.aisc_value['tfdet'].values[0]) * units('in')  # in (mm)
-        self.k_design = float(self.aisc_value['kdes'].values[0]) * units('in')  # in (mm)
-        self.k_detailing = float(self.aisc_value['kdet'].values[0]) * units('in')  # in (mm)
-        self.k1 = float(self.aisc_value['k1'].values[0]) * units('in')  # in (mm)
-        self.slenderness_ratio_flange = float(self.aisc_value['bf/2tf'].values[0])
+        self.depth = float(self.aisc_value['d'].values[0]) * units('in')
+        self.detailing_depth = (
+                float(self.aisc_value['ddet'].values[0]) * units('in')
+        )
+        self.flange_width = float(self.aisc_value['bf'].values[0]) * units('in')
+        self.detailing_flange_width = (
+                float(self.aisc_value['bfdet'].values[0]) * units('in')
+        )
+        self.web_thickness = (
+                float(self.aisc_value['tw'].values[0]) * units('in')
+        )
+        self.detailing_web_thickness = (
+                float(self.aisc_value['twdet'].values[0]) * units('in')
+        )
+        self.half_web_detail = (
+                float(self.aisc_value['twdet/2'].values[0]) * units('in')
+        )
+        self.flange_thickness = (
+                float(self.aisc_value['tf'].values[0]) * units('in')
+        )
+        self.detailing_flange_thickness = (
+                float(self.aisc_value['tfdet'].values[0]) * units('in')
+        )
+        self.k_design = float(self.aisc_value['kdes'].values[0]) * units('in')
+        self.k_detailing = (
+                float(self.aisc_value['kdet'].values[0]) * units('in')
+        )
+        self.k1 = float(self.aisc_value['k1'].values[0]) * units('in')
+        self.slenderness_ratio_flange = (
+            float(self.aisc_value['bf/2tf'].values[0])
+        )
         self.slenderness_ratio_web = float(self.aisc_value['h/tw'].values[0])
-        self.J = float(self.aisc_value['J'].values[0]) * units('in^4')  # in^4 (mm^4 / 10^3)
-        self.Cw = float(self.aisc_value['Cw'].values[0]) * units('in^6')  # in^6 (mm^6 / 10^9)
-        self.Wno = float(self.aisc_value['Wno'].values[0]) * units('in^2')  # in^2 (mm^2)
-        self.Sw1 = float(self.aisc_value['Sw1'].values[0]) * units('in^4')  # in^4 (mm^4 / 10^6)
-        self.Qf = float(self.aisc_value['Qf'].values[0]) * units('in^3')  # in^3 (mm^3 / 10^3)
-        self.Qw = float(self.aisc_value['Qw'].values[0]) * units('in^3')  # in^3 (mm^3 / 10^3)
-        self.radius_of_gyration = self.rts = float(self.aisc_value['rts'].values[0]) * units('in')  # in (mm)
-        self.flange_centroid_distance = float(self.aisc_value['ho'].values[0]) * units('in')  # in (mm)
-        self.exposed_perimeter = float(self.aisc_value['PA'].values[0]) * units('in')  # in (mm)
-        self.shape_perimeter = float(self.aisc_value['PB'].values[0]) * units('in')  # in (mm)
-        self.box_perimeter = float(self.aisc_value['PC'].values[0]) * units('in')  # in (mm)
-        self.exposed_box_perimeter = float(self.aisc_value['PD'].values[0]) * units('in')  # in (mm)
-        self.web_face_depth = self.T = float(self.aisc_value['T'].values[0]) * units('in')  # in (mm)
-        self.fastener_workable_gage = self.WGi = float(self.aisc_value['WGi'].values[0]) * units('in')  # in (mm)
+        self.J = float(self.aisc_value['J'].values[0]) * units('in^4')
+        self.Cw = float(self.aisc_value['Cw'].values[0]) * units('in^6')
+        self.Wno = float(self.aisc_value['Wno'].values[0]) * units('in^2')
+        self.Sw1 = float(self.aisc_value['Sw1'].values[0]) * units('in^4')
+        self.Qf = float(self.aisc_value['Qf'].values[0]) * units('in^3')
+        self.Qw = float(self.aisc_value['Qw'].values[0]) * units('in^3')
+        self.radius_of_gyration = self.rts = (
+                float(self.aisc_value['rts'].values[0]) * units('in')
+        )
+        self.flange_centroid_distance = (
+                float(self.aisc_value['ho'].values[0]) * units('in')
+        )
+        self.exposed_perimeter = (
+                float(self.aisc_value['PA'].values[0]) * units('in')
+        )
+        self.shape_perimeter = (
+                float(self.aisc_value['PB'].values[0]) * units('in')
+        )
+        self.box_perimeter = (
+                float(self.aisc_value['PC'].values[0]) * units('in')
+        )
+        self.exposed_box_perimeter = (
+                float(self.aisc_value['PD'].values[0]) * units('in')
+        )
+        self.web_face_depth = self.T = (
+                float(self.aisc_value['T'].values[0]) * units('in')
+        )
+        self.fastener_workable_gage = self.WGi = (
+                float(self.aisc_value['WGi'].values[0]) * units('in')
+        )
 
 
 class MBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel M beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel M beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = MBeam("M10X9")
     >>> t.weight
     9.0 pound/foot
     """
 
     def __init__(self, label):
         super(MBeam, self).__init__(label)
 
 
 class SBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel M beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel M beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = SBeam("S24X121")
     >>> t.weight
     121.0 pound/foot
     """
 
     def __init__(self, label):
         super(SBeam, self).__init__(label)
 
 
 class HPBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel M beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel M beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = HPBeam("HP18X204")
     >>> t.weight
     204.0 pound/foot
     """
 
     def __init__(self, label):
         super(HPBeam, self).__init__(label)
 
 
 class CBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel C beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel C beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = CBeam("C15X50")
     >>> t.weight
     50.0 pound/foot
     """
 
     def __init__(self, label):
         super(CBeam, self).__init__(label)
-        self.x = float(self.aisc_value['x'].values[0]) * units('in')  # in (mm)
-        self.eo = float(self.aisc_value['eo'].values[0]) * units('in')  # in (mm)
-        self.xp = float(self.aisc_value['xp'].values[0]) * units('in')  # in (mm)
+        self.x = float(self.aisc_value['x'].values[0]) * units('in')
+        self.eo = float(self.aisc_value['eo'].values[0]) * units('in')
+        self.xp = float(self.aisc_value['xp'].values[0]) * units('in')
         self.slenderness_ratio = float(self.aisc_value['b/t'].values[0])
-        self.warping_moment_2 = float(self.aisc_value['Sw2'].values[0]) * units('in^4')  # in (mm)
-        self.warping_moment_3 = float(self.aisc_value['Sw3'].values[0]) * units('in^4')  # in (mm)
-        self.ro = float(self.aisc_value['ro'].values[0]) * units('in')  # in (mm)
+        self.warping_moment_2 = (
+                float(self.aisc_value['Sw2'].values[0]) * units('in^4')
+        )
+        self.warping_moment_3 = (
+                float(self.aisc_value['Sw3'].values[0]) * units('in^4')
+        )
+        self.ro = float(self.aisc_value['ro'].values[0]) * units('in')
         self.H = float(self.aisc_value['H'].values[0])
 
 
 class MCBeam(CBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel MC beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel MC beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = MCBeam("MC18X58")
     >>> t.weight
     58.0 pound/foot
     """
 
     def __init__(self, label):
         super(MCBeam, self).__init__(label)
 
 
 class LBeam(CBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel L beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel L beams. Splitting values into multiple classes allows dropping
+    of empty vain the database.
 
     >>> t = LBeam("L12x12x1-3/8")
     >>> t.weight
     105.0 pound/foot
     """
 
     def __init__(self, label):
         super(LBeam, self).__init__(label)
-        self.b = float(self.aisc_value['b'].values[0]) * units('in')  # in (mm)
-        self.t = float(self.aisc_value['t'].values[0]) * units('in')  # in (mm)
-        self.y = float(self.aisc_value['y'].values[0]) * units('in')  # in (mm)
+        self.b = float(self.aisc_value['b'].values[0]) * units('in')
+        self.t = float(self.aisc_value['t'].values[0]) * units('in')
+        self.y = float(self.aisc_value['y'].values[0]) * units('in')
         self.yp = float(self.aisc_value['yp'].values[0])
-        self.Iz = float(self.aisc_value['Iz'].values[0]) * units('in^4')  # in^4 (mm^4/10^4)
-        self.rz = float(self.aisc_value['rz'].values[0]) * units('in')  # in (mm)
-        self.Sz = float(self.aisc_value['Sz'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
+        self.Iz = float(self.aisc_value['Iz'].values[0]) * units('in^4')
+        self.rz = float(self.aisc_value['rz'].values[0]) * units('in')
+        self.Sz = float(self.aisc_value['Sz'].values[0]) * units('in^3')
         self.tan_a = float(self.aisc_value['tan(α)'].values[0])
-        self.Iw = float(self.aisc_value['Iw'].values[0]) * units('in^4')  # in^4 (mm^4/10^4)
-        self.zA = float(self.aisc_value['zA'].values[0]) * units('in')  # in (mm)
-        self.zB = float(self.aisc_value['zB'].values[0]) * units('in')  # in (mm)
-        self.zC = float(self.aisc_value['zC'].values[0]) * units('in')  # in (mm)
-        self.wA = float(self.aisc_value['wA'].values[0]) * units('in')  # in (mm)
-        self.wB = float(self.aisc_value['wB'].values[0]) * units('in')  # in (mm)
-        self.wC = float(self.aisc_value['wC'].values[0]) * units('in')  # in (mm)
-        self.SwA = float(self.aisc_value['SwA'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.SwC = float(self.aisc_value['SwC'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.SzA = float(self.aisc_value['SzA'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.SzB = float(self.aisc_value['SzB'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.SzC = float(self.aisc_value['SzC'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.PA2 = float(self.aisc_value['PA2'].values[0]) * units('in')  # in (mm)
+        self.Iw = float(self.aisc_value['Iw'].values[0]) * units('in^4')
+        self.zA = float(self.aisc_value['zA'].values[0]) * units('in')
+        self.zB = float(self.aisc_value['zB'].values[0]) * units('in')
+        self.zC = float(self.aisc_value['zC'].values[0]) * units('in')
+        self.wA = float(self.aisc_value['wA'].values[0]) * units('in')
+        self.wB = float(self.aisc_value['wB'].values[0]) * units('in')
+        self.wC = float(self.aisc_value['wC'].values[0]) * units('in')
+        self.SwA = float(self.aisc_value['SwA'].values[0]) * units('in^3')
+        self.SwC = float(self.aisc_value['SwC'].values[0]) * units('in^3')
+        self.SzA = float(self.aisc_value['SzA'].values[0]) * units('in^3')
+        self.SzB = float(self.aisc_value['SzB'].values[0]) * units('in^3')
+        self.SzC = float(self.aisc_value['SzC'].values[0]) * units('in^3')
+        self.PA2 = float(self.aisc_value['PA2'].values[0]) * units('in')
 
 
 class WTBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel WT beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel WT beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = WTBeam("WT22x145")
     >>> t.weight
     145.0 pound/foot
     """
 
     def __init__(self, label):
         super(WTBeam, self).__init__(label)
         self.d_t = float(self.aisc_value['D/t'].values[0])
-        self.ro = float(self.aisc_value['ro'].values[0]) * units('in')  # in (mm)
-        self.y = float(self.aisc_value['y'].values[0]) * units('in')  # in (mm)
+        self.ro = float(self.aisc_value['ro'].values[0]) * units('in')
+        self.y = float(self.aisc_value['y'].values[0]) * units('in')
         self.yp = float(self.aisc_value['yp'].values[0])
         self.H = float(self.aisc_value['H'].values[0])
 
 
 class MTBeam(WTBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel WT beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel WT beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = MTBeam("MT5x4")
     >>> t.weight
     4.0 pound/foot
     """
 
     def __init__(self, label):
         super(MTBeam, self).__init__(label)
 
 
 class STBeam(WTBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel ST beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel ST beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = STBeam("ST10x48")
     >>> t.weight
     48.0 pound/foot
     """
 
     def __init__(self, label):
         super(STBeam, self).__init__(label)
 
 
 class TwoLBeam(WTBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel 2L beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel 2L beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = 2LBeam("2L10X10X1-1/4")
     >>> t.weight
     48.0 pound/foot
     """
 
     def __init__(self, label):
         super(STBeam, self).__init__(label)
-        self.b = float(self.aisc_value['b'].values[0]) * units('in')  # in (mm)
-        self.t = float(self.aisc_value['t'].values[0]) * units('in')  # in (mm)
+        self.b = float(self.aisc_value['b'].values[0]) * units('in')
+        self.t = float(self.aisc_value['t'].values[0]) * units('in')
         self.slenderness_ratio = float(self.aisc_value['b/t'].values[0])
 
 
 class HSSBeam(WBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel HSS beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel HSS beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = HSSBeam("HSS20X20X.500")
     >>> t.weight
     130.52 pound/foot
     """
 
     def __init__(self, label):
         super(HSSBeam, self).__init__(label)
-        self.tnom = float(self.aisc_value['tnom'].values[0]) * units('in')  # in (mm)
-        self.tdes = float(self.aisc_value['tdes'].values[0]) * units('in')  # in (mm)
-        self.C = float(self.aisc_value['C'].values[0]) * units('in^3')  # in^3 (mm^3/10^3)
-        self.OD = float(self.aisc_value['OD'].values[0]) * units('in')  # in (mm)
-        self.ID = float(self.aisc_value['ID'].values[0]) * units('in')  # in (mm)
+        self.tnom = float(self.aisc_value['tnom'].values[0]) * units('in')
+        self.tdes = float(self.aisc_value['tdes'].values[0]) * units('in')
+        self.C = float(self.aisc_value['C'].values[0]) * units('in^3')
+        self.OD = float(self.aisc_value['OD'].values[0]) * units('in')
+        self.ID = float(self.aisc_value['ID'].values[0]) * units('in')
 
 
 class Pipe(HSSBeam):
     """
-    Class to provide more specific attributes and functions related to designing with
-    steel HSS beams. Splitting values into multiple classes allows dropping of empty values
-    in the database.
+    Class to provide more specific attributes and functions related to designing
+    with steel HSS beams. Splitting values into multiple classes allows dropping
+    of empty values in the database.
 
     >>> t = Pipe("Pipe10SCH140")
     >>> t.weight
     104.0 pound/foot
     """
 
     def __init__(self, label):
         super(Pipe, self).__init__(label)
-        self.OD = float(self.aisc_value['OD'].values[0]) * units('in')  # in (mm)
-        self.ID = float(self.aisc_value['ID'].values[0]) * units('in')  # in (mm)
+        self.OD = float(self.aisc_value['OD'].values[0]) * units('in')
+        self.ID = float(self.aisc_value['ID'].values[0]) * units('in')
         self.D_t = float(self.aisc_value['D/t'].values[0])
 
-
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

### Comparing `civilpy-0.0.47/src/civilpy/water_resources/hydraulics.py` & `civilpy-0.0.48/src/civilpy/water_resources/hydraulics.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy.egg-info/PKG-INFO` & `civilpy-0.0.48/src/civilpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civilpy
-Version: 0.0.47
+Version: 0.0.48
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
-Metadata-Version: 2.1 Name: civilpy Version: 0.0.47 Summary: Civil Engineering
+Metadata-Version: 2.1 Name: civilpy Version: 0.0.48 Summary: Civil Engineering
 Tools in Python Home-page: https://daneparks.com/Dane/civilpy Author: Dane
 Parks Author-email: Dane@daneparks.com Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Classifier: Environment :: Console ::
 Curses Description-Content-Type: text/markdown License-File: LICENSE # CivilPy
```

### Comparing `civilpy-0.0.47/src/civilpy.egg-info/SOURCES.txt` & `civilpy-0.0.48/src/civilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/src/civilpy.egg-info/requires.txt` & `civilpy-0.0.48/src/civilpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/tests/test_ohio_dot_bridge.py` & `civilpy-0.0.48/tests/test_ohio_dot_bridge.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/tests/test_ohio_dot_functions.py` & `civilpy-0.0.48/tests/test_ohio_dot_functions.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/tests/test_ohio_dot_project.py` & `civilpy-0.0.48/tests/test_ohio_dot_project.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/tests/test_ohio_dot_snbi_transfer.py` & `civilpy-0.0.48/tests/test_ohio_dot_snbi_transfer.py`

 * *Files identical despite different names*

### Comparing `civilpy-0.0.47/tests/test_steel.py` & `civilpy-0.0.48/tests/test_steel.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         test_beam3 = SteelSection("W 44x335")  # Space in label
 
         self.assertEqual(test_beam.weight, test_beam2.weight)  # Verify all three names are imported identically
         self.assertEqual(test_beam2.weight, test_beam3.weight)
 
     def test_general_attributes(self):
         test_beam = SteelSection("W44X335")
-        self.assertEqual(test_beam.weight, 335 * units('lb/ft'))
+        self.assertEqual(test_beam.weight, 335 * units('lbf/ft'))
         self.assertEqual(test_beam.area, 98.5 * units('in^2'))
         self.assertEqual(test_beam.special_note, 'F')
         self.assertEqual(test_beam.I_x, 31100.0 * units('in^4'))
         self.assertEqual(test_beam.Z_x, 1620.0 * units('in^3'))
         self.assertEqual(test_beam.S_x, 1410.0 * units('in^3'))
         self.assertEqual(test_beam.r_x, 17.8 * units('in'))
         self.assertEqual(test_beam.I_y, 1200.0 * units('in^4'))
```

