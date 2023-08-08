# Comparing `tmp/OpenGeodeWeb-Viewer-0.0.1.tar.gz` & `tmp/OpenGeodeWeb-Viewer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenGeodeWeb-Viewer-0.0.1.tar", last modified: Tue Aug  8 14:46:24 2023, max compression
+gzip compressed data, was "OpenGeodeWeb-Viewer-0.0.2.tar", last modified: Tue Aug  8 14:56:00 2023, max compression
```

## Comparing `OpenGeodeWeb-Viewer-0.0.1.tar` & `OpenGeodeWeb-Viewer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:46:24.017596 OpenGeodeWeb-Viewer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 14:46:16.000000 OpenGeodeWeb-Viewer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-08 14:46:24.017596 OpenGeodeWeb-Viewer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 14:46:16.000000 OpenGeodeWeb-Viewer-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-08 14:46:16.000000 OpenGeodeWeb-Viewer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:46:24.017596 OpenGeodeWeb-Viewer-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:46:24.017596 OpenGeodeWeb-Viewer-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:46:24.017596 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-08 14:46:24.000000 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 14:46:24.000000 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:46:24.000000 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 14:46:24.000000 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:46:24.000000 OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:56:00.982377 OpenGeodeWeb-Viewer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 14:55:53.000000 OpenGeodeWeb-Viewer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-08 14:56:00.982377 OpenGeodeWeb-Viewer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-08 14:55:53.000000 OpenGeodeWeb-Viewer-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-08 14:55:53.000000 OpenGeodeWeb-Viewer-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 14:56:00.982377 OpenGeodeWeb-Viewer-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:56:00.978377 OpenGeodeWeb-Viewer-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:56:00.982377 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-08 14:56:00.000000 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 14:56:00.000000 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:56:00.000000 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 14:56:00.000000 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:56:00.000000 OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/top_level.txt
```

### Comparing `OpenGeodeWeb-Viewer-0.0.1/LICENSE` & `OpenGeodeWeb-Viewer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Viewer-0.0.1/PKG-INFO` & `OpenGeodeWeb-Viewer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Viewer
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for vtk
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `OpenGeodeWeb-Viewer-0.0.1/pyproject.toml` & `OpenGeodeWeb-Viewer-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Viewer"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Geode-solutions", email="contact@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for vtk"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "wslink[ssl]",
     "numpy",
-    "vtk"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Geode-solutions/OpenGeodeWeb-Viewer"
 "Bug Tracker" = "https://github.com/Geode-solutions/OpenGeodeWeb-Viewer/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `OpenGeodeWeb-Viewer-0.0.1/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO` & `OpenGeodeWeb-Viewer-0.0.2/src/OpenGeodeWeb_Viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Viewer
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenGeodeWeb-Viewer is an open source framework that proposes handy python functions and wrappers for vtk
 Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

