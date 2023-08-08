# Comparing `tmp/napari-EMD-0.0.1.tar.gz` & `tmp/napari-EMD-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-EMD-0.0.1.tar", last modified: Tue Aug  1 02:26:57 2023, max compression
+gzip compressed data, was "napari-EMD-0.1.1.tar", last modified: Tue Aug  8 03:30:42 2023, max compression
```

## Comparing `napari-EMD-0.0.1.tar` & `napari-EMD-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:57.867775 napari-EMD-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-08-01 02:26:57.867775 napari-EMD-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 02:26:57.867775 napari-EMD-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:57.859774 napari-EMD-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:57.863775 napari-EMD-0.0.1/src/napari_EMD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 02:26:57.000000 napari-EMD-0.0.1/src/napari_EMD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:57.863775 napari-EMD-0.0.1/src/napari_emd/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:57.867775 napari-EMD-0.0.1/src/napari_emd/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 02:26:39.000000 napari-EMD-0.0.1/src/napari_emd/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:42.968764 napari-EMD-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-08 03:30:42.968764 napari-EMD-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-08 03:30:42.968764 napari-EMD-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:42.964764 napari-EMD-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:42.964764 napari-EMD-0.1.1/src/napari_EMD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-08 03:30:42.000000 napari-EMD-0.1.1/src/napari_EMD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:42.968764 napari-EMD-0.1.1/src/napari_emd/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/src/napari_emd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/src/napari_emd/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:42.968764 napari-EMD-0.1.1/src/napari_emd/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 03:30:18.000000 napari-EMD-0.1.1/src/napari_emd/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-08-08 03:30:19.000000 napari-EMD-0.1.1/src/napari_emd/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-08 03:30:19.000000 napari-EMD-0.1.1/src/napari_emd/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-08-08 03:30:19.000000 napari-EMD-0.1.1/src/napari_emd/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 03:30:19.000000 napari-EMD-0.1.1/src/napari_emd/napari.yaml
```

### Comparing `napari-EMD-0.0.1/LICENSE` & `napari-EMD-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-EMD-0.0.1/PKG-INFO` & `napari-EMD-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,13 @@
-Metadata-Version: 2.1
-Name: napari-EMD
-Version: 0.0.1
-Summary: A simple plugin to view .emd files in napari (Velox files)
-Home-page: https://github.com/NickiShaw/napari-EMD.git
-Author: Nicolette Shaw
-Author-email: shaw.nicki@gmail.com
-License: BSD-3-Clause
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # napari-EMD
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-EMD.svg?color=green)](https://github.com/NickiShaw/napari-EMD/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-EMD.svg?color=green)](https://pypi.org/project/napari-EMD)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-EMD.svg?color=green)](https://python.org)
 [![tests](https://github.com/NickiShaw/napari-EMD/workflows/tests/badge.svg)](https://github.com/NickiShaw/napari-EMD/actions)
-[![codecov](https://codecov.io/gh/NickiShaw/napari-EMD/branch/main/graph/badge.svg)](https://codecov.io/gh/NickiShaw/napari-EMD)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-EMD)](https://napari-hub.org/plugins/napari-EMD)
 
 A simple plugin to view .emd files in napari (i.e. Velox files). Allows users to track metadata as it changes over the course of a video/stack, developed for analysis of in-situ microscopy data, where users may be changing magnification, focus, etc. during aquisition.
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
@@ -64,18 +38,24 @@
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-EMD" is free and open source software
 
 ## Issues and Requests
 
+> **Warning: The metadata viewer does not work in the current [Napari bundle](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-a-bundled-app) version (August 2023). Use the [python package version](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-python-package-recommended) of Napari for this feature.**
+
 If you encounter any problems or would like any functionality added, please [file an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue) along with a detailed description.
 
 Current maintainer(s): [Nicki Shaw](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)
 
+## Preview
+
+Images A and B show different frames in the same image stack, the metadata plugin on the right shows the changing focus value.
+![NapariEMD screenshots](Images/napariEMD_screenshots.jpg)
 
 ## To Do
 
 - Attatch last-opened information, so the widget does not reset when frames are changed and open toggle options are open remain.
 - Add a search bar for navigating metadata.
 - Output metadata as file option.
 - Add note to change order of open files to replacee active metadata view.
```

### Comparing `napari-EMD-0.0.1/pyproject.toml` & `napari-EMD-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-EMD-0.0.1/setup.cfg` & `napari-EMD-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-EMD-0.0.1/src/napari_EMD.egg-info/PKG-INFO` & `napari-EMD-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-EMD
-Version: 0.0.1
+Version: 0.1.1
 Summary: A simple plugin to view .emd files in napari (Velox files)
 Home-page: https://github.com/NickiShaw/napari-EMD.git
 Author: Nicolette Shaw
 Author-email: shaw.nicki@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
@@ -25,15 +25,14 @@
 
 # napari-EMD
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-EMD.svg?color=green)](https://github.com/NickiShaw/napari-EMD/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-EMD.svg?color=green)](https://pypi.org/project/napari-EMD)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-EMD.svg?color=green)](https://python.org)
 [![tests](https://github.com/NickiShaw/napari-EMD/workflows/tests/badge.svg)](https://github.com/NickiShaw/napari-EMD/actions)
-[![codecov](https://codecov.io/gh/NickiShaw/napari-EMD/branch/main/graph/badge.svg)](https://codecov.io/gh/NickiShaw/napari-EMD)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-EMD)](https://napari-hub.org/plugins/napari-EMD)
 
 A simple plugin to view .emd files in napari (i.e. Velox files). Allows users to track metadata as it changes over the course of a video/stack, developed for analysis of in-situ microscopy data, where users may be changing magnification, focus, etc. during aquisition.
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
@@ -64,18 +63,24 @@
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-EMD" is free and open source software
 
 ## Issues and Requests
 
+> **Warning: The metadata viewer does not work in the current [Napari bundle](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-a-bundled-app) version (August 2023). Use the [python package version](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-python-package-recommended) of Napari for this feature.**
+
 If you encounter any problems or would like any functionality added, please [file an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue) along with a detailed description.
 
 Current maintainer(s): [Nicki Shaw](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue)
 
+## Preview
+
+Images A and B show different frames in the same image stack, the metadata plugin on the right shows the changing focus value.
+![NapariEMD screenshots](Images/napariEMD_screenshots.jpg)
 
 ## To Do
 
 - Attatch last-opened information, so the widget does not reset when frames are changed and open toggle options are open remain.
 - Add a search bar for navigating metadata.
 - Output metadata as file option.
 - Add note to change order of open files to replacee active metadata view.
```

### Comparing `napari-EMD-0.0.1/src/napari_emd/_reader.py` & `napari-EMD-0.1.1/src/napari_emd/_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import h5py
 import ujson
 
 
 def rotateFrame(stack):
     for frame in range(len(stack)):
-        stack[frame] = np.rot90(stack[frame])
+        stack[frame] = np.flipud(np.rot90(stack[frame]))
     return stack
 
 
 class navigate:
 
     @staticmethod
     def getGroupsNames(group):
```

### Comparing `napari-EMD-0.0.1/src/napari_emd/_tests/test_reader.py` & `napari-EMD-0.1.1/src/napari_emd/_tests/test_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             self.assertIsInstance(layer_type, str)
 
 
 class TestRotateFrame(unittest.TestCase):
 
     def test_rotateFrame(self):
         # Test the rotateFrame function
-        data = np.array([[[2, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 1]],
-                         [[2, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0]]])
+        data = np.array([[[1,2,3,4], [5,6,7,8], [9,10,11,12], [13,14,15,16]],
+                         [[17,18,19,20], [21,22,23,24], [25,26,27,28], [29,30,31,32]]])
         rotated_data = rotateFrame(data)
-        self.assertEqual(rotated_data.tolist(), [[[1, 1, 1, 1], [1, 1, 1, 1], [1, 1, 1, 1], [2, 1, 1, 1]],
-                                                 [[0, 0, 0, 0], [0, 0, 0, 0], [0, 0, 0, 0], [2, 0, 0, 0]]])
+        self.assertEqual(rotated_data.tolist(), [[[1,5,9,13],[2,6,10,14],[3,7,11,15],[4,8,12,16]],
+                                                 [[17,21,25,29],[18,22,26,30],[19,23,27,31],[20,24,28,32]]])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `napari-EMD-0.0.1/src/napari_emd/_widget.py` & `napari-EMD-0.1.1/src/napari_emd/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-EMD-0.0.1/src/napari_emd/napari.yaml` & `napari-EMD-0.1.1/src/napari_emd/napari.yaml`

 * *Files identical despite different names*

