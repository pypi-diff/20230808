# Comparing `tmp/CalSciPy-0.3.2.tar.gz` & `tmp/CalSciPy-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalSciPy-0.3.2.tar", last modified: Thu Jun  1 22:56:41 2023, max compression
+gzip compressed data, was "CalSciPy-0.3.5.tar", last modified: Tue Aug  8 17:19:13 2023, max compression
```

## Comparing `CalSciPy-0.3.2.tar` & `CalSciPy-0.3.5.tar`

### file list

```diff
@@ -1,35 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.496893 CalSciPy-0.3.2/
--rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     4947 2023-06-01 22:56:41.493905 CalSciPy-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2840 2023-04-03 15:47:56.000000 CalSciPy-0.3.2/README.md
--rw-rw-rw-   0        0        0     2303 2023-06-01 22:55:46.000000 CalSciPy-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 22:56:41.496893 CalSciPy-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.328894 CalSciPy-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.399896 CalSciPy-0.3.2/src/CalSciPy/
--rw-rw-rw-   0        0        0      358 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/__init__.py
--rw-rw-rw-   0        0        0    15266 2023-06-01 22:35:40.000000 CalSciPy-0.3.2/src/CalSciPy/bruker.py
--rw-rw-rw-   0        0        0     3270 2023-05-24 14:25:43.000000 CalSciPy-0.3.2/src/CalSciPy/coloring.py
--rw-rw-rw-   0        0        0     8422 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/event_processing.py
--rw-rw-rw-   0        0        0     4000 2023-06-01 22:44:59.000000 CalSciPy-0.3.2/src/CalSciPy/image_processing.py
--rw-rw-rw-   0        0        0     9700 2023-06-01 22:48:52.000000 CalSciPy-0.3.2/src/CalSciPy/interactive_visuals.py
--rw-rw-rw-   0        0        0    10053 2023-06-01 22:34:13.000000 CalSciPy-0.3.2/src/CalSciPy/io_tools.py
--rw-rw-rw-   0        0        0     8733 2023-06-01 22:39:17.000000 CalSciPy-0.3.2/src/CalSciPy/misc.py
--rw-rw-rw-   0        0        0     3109 2023-06-01 22:40:45.000000 CalSciPy-0.3.2/src/CalSciPy/reorganization.py
--rw-rw-rw-   0        0        0     9604 2023-06-01 22:44:01.000000 CalSciPy-0.3.2/src/CalSciPy/trace_processing.py
--rw-rw-rw-   0        0        0      199 2023-02-20 22:24:54.000000 CalSciPy-0.3.2/src/CalSciPy/version.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.428893 CalSciPy-0.3.2/src/CalSciPy.egg-info/
--rw-rw-rw-   0        0        0     4947 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      376 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 22:56:41.000000 CalSciPy-0.3.2/src/CalSciPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 22:56:41.485893 CalSciPy-0.3.2/tests/
--rw-rw-rw-   0        0        0     1933 2023-04-03 13:04:29.000000 CalSciPy-0.3.2/tests/test_a_install.py
--rw-rw-rw-   0        0        0     3074 2023-04-05 17:07:30.000000 CalSciPy-0.3.2/tests/test_bruker.py
--rw-rw-rw-   0        0        0      492 2023-05-24 14:14:23.000000 CalSciPy-0.3.2/tests/test_coloring.py
--rw-rw-rw-   0        0        0     1218 2023-04-03 15:39:20.000000 CalSciPy-0.3.2/tests/test_event_processing.py
--rw-rw-rw-   0        0        0    12735 2023-04-05 16:39:27.000000 CalSciPy-0.3.2/tests/test_io_tools.py
--rw-rw-rw-   0        0        0     2373 2023-04-05 15:55:20.000000 CalSciPy-0.3.2/tests/test_misc.py
--rw-rw-rw-   0        0        0     5124 2023-03-29 19:08:15.000000 CalSciPy-0.3.2/tests/test_reorganization.py
--rw-rw-rw-   0        0        0     3250 2023-03-29 21:11:25.000000 CalSciPy-0.3.2/tests/test_trace_processing.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.485314 CalSciPy-0.3.5/
+-rw-rw-rw-   0        0        0     1094 2023-02-20 20:08:47.000000 CalSciPy-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0     5086 2023-08-08 17:19:13.484314 CalSciPy-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2928 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/README.md
+-rw-rw-rw-   0        0        0     2454 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-08 17:19:13.485314 CalSciPy-0.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.399315 CalSciPy-0.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.431314 CalSciPy-0.3.5/src/CalSciPy/
+-rw-rw-rw-   0        0        0      359 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/__init__.py
+-rw-rw-rw-   0        0        0     9970 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/_interactive_visuals.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/_validators.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.461314 CalSciPy-0.3.5/src/CalSciPy/bruker/
+-rw-rw-rw-   0        0        0       86 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/configuration_values.py
+-rw-rw-rw-   0        0        0    17164 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/data.py
+-rw-rw-rw-   0        0        0    14298 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/factories.py
+-rw-rw-rw-   0        0        0     6972 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/meta_objects.py
+-rw-rw-rw-   0        0        0    10498 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/prairie_link.py
+-rw-rw-rw-   0        0        0        0 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/protocols.py
+-rw-rw-rw-   0        0        0     6095 2023-08-04 16:49:38.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/validation.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.465314 CalSciPy-0.3.5/src/CalSciPy/bruker/xml_mappings/
+-rw-rw-rw-   0        0        0       35 2023-07-28 19:52:28.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/xml_mappings/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-07-28 19:52:28.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/xml_mappings/xml_mapping.py
+-rw-rw-rw-   0        0        0     9678 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/bruker/xml_objects.py
+-rw-rw-rw-   0        0        0     1776 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/color_scheme.py
+-rw-rw-rw-   0        0        0    10327 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/event_processing.py
+-rw-rw-rw-   0        0        0     4000 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/src/CalSciPy/image_processing.py
+-rw-rw-rw-   0        0        0     1723 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/interactive_visuals.py
+-rw-rw-rw-   0        0        0    11468 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/io_tools.py
+-rw-rw-rw-   0        0        0     9657 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/misc.py
+-rw-rw-rw-   0        0        0    24778 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/optogenetics.py
+-rw-rw-rw-   0        0        0     3872 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/reorganization.py
+-rw-rw-rw-   0        0        0    11120 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/src/CalSciPy/trace_processing.py
+-rw-rw-rw-   0        0        0      259 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/src/CalSciPy/version.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.442314 CalSciPy-0.3.5/src/CalSciPy.egg-info/
+-rw-rw-rw-   0        0        0     5086 2023-08-08 17:19:13.000000 CalSciPy-0.3.5/src/CalSciPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2023-08-08 17:19:13.000000 CalSciPy-0.3.5/src/CalSciPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 17:19:13.000000 CalSciPy-0.3.5/src/CalSciPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      386 2023-08-08 17:19:13.000000 CalSciPy-0.3.5/src/CalSciPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-08-08 17:19:13.000000 CalSciPy-0.3.5/src/CalSciPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-02-20 20:08:47.000000 CalSciPy-0.3.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 17:19:13.481314 CalSciPy-0.3.5/tests/
+-rw-rw-rw-   0        0        0     1933 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/tests/test_a_install.py
+-rw-rw-rw-   0        0        0     3079 2023-08-08 14:21:37.000000 CalSciPy-0.3.5/tests/test_bruker.py
+-rw-rw-rw-   0        0        0     1218 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/tests/test_event_processing.py
+-rw-rw-rw-   0        0        0    14187 2023-08-08 17:17:01.000000 CalSciPy-0.3.5/tests/test_io_tools.py
+-rw-rw-rw-   0        0        0     2373 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/tests/test_misc.py
+-rw-rw-rw-   0        0        0     5124 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/tests/test_reorganization.py
+-rw-rw-rw-   0        0        0     3250 2023-07-28 19:52:25.000000 CalSciPy-0.3.5/tests/test_trace_processing.py
```

### Comparing `CalSciPy-0.3.2/LICENSE` & `CalSciPy-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/PKG-INFO` & `CalSciPy-0.3.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.2
+Version: 0.3.5
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -30,14 +30,15 @@
 Project-URL: repository, https://github.com/darikoneil/CalSciPy
 Keywords: CalSciPy,Calcium Imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: gpu
@@ -53,46 +54,32 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
+This python packages contains a variety of useful tools for handling, processing, visualizing, & designing calcium 
+imaging experiments. I noticed I was constantly re-writing boilerplate, "one-liners", and copy/pasting code between
+environments. I wrote this so ~I don't have to~ you don't have to. It's intended to be a collection of useful, 
+well-documented functions often used in boilerplate code alongside software packages such as 
+[Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), 
+and [Suite2P](https://github.com/MouseLand/suite2p), as well as a collection of more bespoke software designed for use 
+with Bruker's PrairieView Imaging Software and MeadowLark Spatial Light Modulators. Essentially, it's a collection of 
+code written for my imaging experiments that might be considered useful to others.
 
-This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+#### Active Development
+* The current implementation is unstable and should be considered an open beta.
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
-* Methods for handling Bruker's PrairieView data
-* Interactive visualization
+* Fast, convenient functions for handling, aligning, and compiling data collected in Bruker's PrairieView software
+* Functions for generating protocols for use in Bruker's Prairieview.
+* Interactive visualization of data
 
 #### Installation
 `pip install CalSciPy`
 
-#### Subpackages
-* Bruker - MAIN
-* Coloring - TODO
-* Event Processing - DEV
-* Input/Output (I/O) - MAIN
-* Image Processing - DEV
-* Interactive Visuals - TODO
-* Reorganization - MAIN
-* Signal Processing - DEV
-* Static Visuals - TODO
-
 #### Documentation
 Hosted at [ReadtheDocs](https://calscipy.readthedocs.io/en/latest/index.html#).
 Available locally as [HTML](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/html), [LATEX](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/latex) and [PDF](https://github.com/darikoneil/CalSciPy/blob/master/docs/build/pdf/calscipy.pdf).
-
-#### Roadmap
-TODO - UNDOCUMENTED / OFFLINE     
-DEV - UNTESTED / IN DEV BRANCH      
-MAIN - COMPLETE /  IN MAIN BRANCH     
-
-Generally completing each module before the next.     
-Exceptions done last:       
-* Bruker's Prairiview XML
-* Bruker's Prairieview ENV parsing
-* Trace Processing's Diffusion
-* Event Processing's Covariance
-* Interactive's ROI methods
```

### Comparing `CalSciPy-0.3.2/README.md` & `CalSciPy-0.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,46 +8,32 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
+This python packages contains a variety of useful tools for handling, processing, visualizing, & designing calcium 
+imaging experiments. I noticed I was constantly re-writing boilerplate, "one-liners", and copy/pasting code between
+environments. I wrote this so ~I don't have to~ you don't have to. It's intended to be a collection of useful, 
+well-documented functions often used in boilerplate code alongside software packages such as 
+[Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), 
+and [Suite2P](https://github.com/MouseLand/suite2p), as well as a collection of more bespoke software designed for use 
+with Bruker's PrairieView Imaging Software and MeadowLark Spatial Light Modulators. Essentially, it's a collection of 
+code written for my imaging experiments that might be considered useful to others.
 
-This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+#### Active Development
+* The current implementation is unstable and should be considered an open beta.
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
-* Methods for handling Bruker's PrairieView data
-* Interactive visualization
+* Fast, convenient functions for handling, aligning, and compiling data collected in Bruker's PrairieView software
+* Functions for generating protocols for use in Bruker's Prairieview.
+* Interactive visualization of data
 
 #### Installation
 `pip install CalSciPy`
 
-#### Subpackages
-* Bruker - MAIN
-* Coloring - TODO
-* Event Processing - DEV
-* Input/Output (I/O) - MAIN
-* Image Processing - DEV
-* Interactive Visuals - TODO
-* Reorganization - MAIN
-* Signal Processing - DEV
-* Static Visuals - TODO
-
 #### Documentation
 Hosted at [ReadtheDocs](https://calscipy.readthedocs.io/en/latest/index.html#).
 Available locally as [HTML](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/html), [LATEX](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/latex) and [PDF](https://github.com/darikoneil/CalSciPy/blob/master/docs/build/pdf/calscipy.pdf).
-
-#### Roadmap
-TODO - UNDOCUMENTED / OFFLINE     
-DEV - UNTESTED / IN DEV BRANCH      
-MAIN - COMPLETE /  IN MAIN BRANCH     
-
-Generally completing each module before the next.     
-Exceptions done last:       
-* Bruker's Prairiview XML
-* Bruker's Prairieview ENV parsing
-* Trace Processing's Diffusion
-* Event Processing's Covariance
-* Interactive's ROI methods
```

### Comparing `CalSciPy-0.3.2/pyproject.toml` & `CalSciPy-0.3.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CalSciPy"
-version = "0.3.2"
+version = "0.3.5"
 description = "A collection"
 readme = "README.md"
 requires-python = ">=3.7, <4"
 license = {file = "LICENSE"}
 keywords = ["CalSciPy", "Calcium Imaging"]
 authors = [
   {name = "Darik A. O'Neil"}
@@ -18,27 +18,29 @@
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
+    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
+    "joblib",
     "matplotlib",
     "numpy",
     "opencv-python",
-    "pillow",
+    "pillow <= 9.4.0",
     "PPVD",
-    "prettytable",
     "PyQt5",
+    "pywin32",
     "seaborn",
     "scikit-learn",
     "scipy",
     "tqdm"
 ]
 
 [project.urls]
@@ -89,15 +91,16 @@
     "ignore::FutureWarning",
 ]
 
 [tool.coverage.run]
 branch = true
 command_line = "-m pytest"
 omit = ["*/tests*", "*tests*", "*tests/*", "tests*", "tests/*", "tests", "scratch", "htmlcov", "flake_report", "docs",
-"dist", "lib", ".pytest_cache", ".idea", ".github"]
+    "dist", "lib", ".pytest_cache", ".idea", ".github", "config-3.py", "config.py", "*CalSciPy/config-3.py",
+    "*CalSciPy/config.py"]
 dynamic_context = "test_function"
 
 
 [tool.coverage.report]
 fail_under = 10
 
 [tool.coverage.json]
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy/bruker.py` & `CalSciPy-0.3.5/src/CalSciPy/bruker/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,103 +3,78 @@
 from operator import eq
 from pathlib import Path
 from itertools import product
 from xml.etree import ElementTree
 
 import numpy as np
 import pandas as pd
-from prettytable import PrettyTable
 import cv2
 from PPVD.parsing import convert_permitted_types_to_required, find_num_unique_files_given_static_substring, \
     find_num_unique_files_containing_tag
 from PPVD.validation import validate_extension
 from tqdm import tqdm as tq
 
-
-from .misc import PatternMatching, calculate_frames_per_file, generate_blocks, generate_padded_filename
-from .io_tools import _load_single_tif, _save_single_tif
+from .configuration_values import DEFAULT_PRAIRIEVIEW_VERSION
+from .meta_objects import PhotostimulationMeta
+from .factories import BrukerElementFactory
+from ..misc import PatternMatching, calculate_frames_per_file, generate_blocks, generate_padded_filename
+from ..io_tools import _load_single_tif, _save_single_tif
 
 
 """
-These functions have been incorporated into pyPrairieView and will likely be deprecated in the future and/or
-pyPrairieView will absorbed into CalSciPy
+A collection of functions for importing / converting PrairieView collected data
 """
 
 
-def align_data(analog_data: pd.DataFrame, frame_times: pd.DataFrame, fill: bool = False) -> pd.DataFrame:
+def align_data(analog_data: pd.DataFrame,
+               frame_times: pd.DataFrame,
+               fill: bool = False,
+               method: str = "nearest"
+               ) -> pd.DataFrame:
     """
     Synchronizes analog data & imaging frames using the timestamp of each frame. Option to generate a second column
     in which the frame index is interpolated such that each analog sample matches with an associated frame.
 
     :param analog_data: analog data
     :param frame_times: frame timestamps
-    :param fill: whether to include an interpolated nearest-neighbor column so each sample has an associated frame
+    :param fill: whether to include an interpolated column so each sample has an associated frame
+    :param method: method for interpolating samples
     :returns: a dataframe containing time (index, ms) with aligned columns of voltage recordings/analog data and imaging frame
     """
     frame_times = frame_times.reindex(index=analog_data.index)
 
     # Join frames & analog (deep copy to make sure not a view)
     data = analog_data.copy(deep=True)
     data = data.join(frame_times)
 
     if fill:
         frame_times_filled = frame_times.copy(deep=True)
         frame_times_filled.columns = ["Imaging Frame (interpolated)"]
-        frame_times_filled.interpolate(method="nearest", inplace=True)
+        frame_times_filled.interpolate(method=method, inplace=True)
         # forward fill the final frame
         frame_times_filled.ffill(inplace=True)
         data = data.join(frame_times_filled)
 
     return data
 
 
-def generate_bruker_naming_convention(channel: int, plane: int, num_channels: int = 1, num_planes: int = 1) \
-        -> str:
-    """
-    Generates the expected bruker naming convention for images collected with an arbitrary number of cycles & channels
-
-    This function expects that the naming convention is _Cycle00000_Ch0_000000.ome.tiff where the channel is
-    one-indexed. The 5-digit cycle id represents the frame if using multiplane imaging and the 6-digit tag represents
-    the plane. Otherwise, the 5-digit tag is static and the 6-digit tag represents the frame.
-
-    Please note that the parameters channel and plane are *zero-indexed*.
-
-    :param channel: channel to produce name for
-    :param plane: plane to produce name for
-    :param num_channels: number of channels
-    :param num_planes: number of planes
-    :returns: proper naming convention
-    """
-    if num_channels > 1:
-        num_channels = 2
-    if num_planes > 1:
-        num_planes = 2
-    with PatternMatching([num_channels, num_planes], [eq, eq]) as case:
-        if case([1, 1]):
-            return "*.ome.tif"
-        elif case([2, 1]):
-            return "".join(["*Ch", str(channel + 1), "*"])
-        elif case([1, 2]):
-            return "".join(["*00000", str(plane + 1), ".ome.tif"])
-        elif case([2, 2]):
-            return "".join(["*Ch", str(channel + 1), "00000", str(plane + 1), ".ome.tif"])
-
-
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def determine_imaging_content(folder: Union[str, Path]) -> Tuple[int, int, int, int, int]:  # noqa: C901
     """
     This function determines the number of channels and planes within a folder containing .tif files
     exported by Bruker's Prairieview software. It also determines the size of the images (frames, y-pixels, x-pixels).
     It's a quick / fast alternative to parsing its respective xml. However, note that the function is dependent on the
     naming conventions of PrairieView and will not work on arbitrary folders.
 
     :param folder: folder containing bruker imaging data
     :returns: channels, planes, frames, height, width
     """
 
+    # TODO: I am spaghetti
+
     _files = [_file for _file in folder.glob("*.tif") if _file.is_file()]
 
     def _extract_file_identifiers(str_to_split: str) -> list:
         return str_to_split.split("_")[-3:]
 
     def _check_file_identifiers(tag_: str, str_to_split: str) -> str:
         return [_tag for _tag in _extract_file_identifiers(str_to_split) if tag_ in _tag]
@@ -180,74 +155,155 @@
     frame_times = np.round(frame_times).astype(np.int64)
     # make index
     frame_times = pd.Index(data=frame_times, name="Time (ms)")
     # make dataframe
     return pd.DataFrame(data=frames, index=frame_times, columns=["Imaging Frame"])
 
 
+def generate_bruker_naming_convention(channel: int,
+                                      plane: int,
+                                      num_channels: int = 1,
+                                      num_planes: int = 1
+                                      ) -> str:
+    """
+    Generates the expected bruker naming convention for images collected with an arbitrary number of cycles & channels
+
+    This function expects that the naming convention is _Cycle00000_Ch0_000000.ome.tiff where the channel is
+    one-indexed. The 5-digit cycle id represents the frame if using multiplane imaging and the 6-digit tag represents
+    the plane. Otherwise, the 5-digit tag is static and the 6-digit tag represents the frame.
+
+    Please note that the parameters channel and plane are *zero-indexed*.
+
+    :param channel: channel to produce name for
+    :param plane: plane to produce name for
+    :param num_channels: number of channels
+    :param num_planes: number of planes
+    :returns: proper naming convention
+    """
+    if num_channels > 1:
+        num_channels = 2
+    if num_planes > 1:
+        num_planes = 2
+    with PatternMatching([num_channels, num_planes], [eq, eq]) as case:
+        if case([1, 1]):
+            return "*.ome.tif"
+        elif case([2, 1]):
+            return "".join(["*Ch", str(channel + 1), "*"])
+        elif case([1, 2]):
+            return "".join(["*00000", str(plane + 1), ".ome.tif"])
+        elif case([2, 2]):
+            return "".join(["*Ch", str(channel + 1), "00000", str(plane + 1), ".ome.tif"])
+
+
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_bruker_tifs(folder: Union[str, Path],
-                     channel: Optional[int] = None, plane: Optional[int] = None) -> Tuple[np.ndarray]:  # noqa: C901
+                     channel: Optional[int] = None,
+                     plane: Optional[int] = None
+                     ) -> Tuple[np.ndarray]:  # noqa: C901
     """
     This function loads images collected and converted to .tif files by Bruker's Prairieview software.
     If multiple channels or multiple planes exist, each channel and plane combination is loaded to a separate
     numpy array. Identification of multiple channels / planes is dependent on :func:`determine_imaging_content`.
     Images are loaded as unsigned 16-bit (:class:`numpy.uint16`), though note that raw bruker files are
-    natively 12 or 13-bit.
+    natively could be 12 or 13-bit.
 
     :param folder: folder containing a sequence of single frame tiff files
     :param channel: specific channel to load from dataset (zero-indexed)
     :param plane: specific plane to load from dataset (zero-indexed)
     :return: a tuple of numpy arrays (frames, y-pixels, x-pixels, :class:`numpy.uint16`)
      """
     num_channels, num_planes, num_frames, y, x = determine_imaging_content(folder)
-    _pretty_print_image_description(num_channels, num_planes, num_frames, y, x)
+    _print_image_description(num_channels, num_planes, num_frames, y, x)
 
     images = []
     if channel is None and plane is None:
         for channel_, plane_ in product(range(num_channels), range(num_planes)):
             images.append(_load_bruker_tif_stack(folder, channel_, plane_, num_channels, num_planes))
     else:
         images.append(_load_bruker_tif_stack(folder, channel, plane, num_channels, num_planes))
     return tuple(images)
 
 
+@convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
+def load_mark_points(file_path: Union[str, Path], version: str = DEFAULT_PRAIRIEVIEW_VERSION) -> PhotostimulationMeta:
+    """
+
+    :param file_path: path to xml file
+    :param version: version of prairieview
+    :return: photostimulation metadata
+    """
+    # We generally expected the file to be structured such that
+    # File/
+    # ├── MarkPointSeriesElements
+    # │   └──MarkPointElement
+    # │      ├──GalvoPointElement
+    # │      |      └──Point
+    #        └──GalvoPointElement (Empty)
+    # However, by using configurable mappings we do have some wiggle room
+
+    tree = ElementTree.parse(file_path)
+    root = tree.getroot()
+
+    # if it's imaging we can grab the version directly
+    if "version" in root.attrib:
+        version = root.attrib.get("version")
+
+    bruker_element_factory = BrukerElementFactory(version)
+
+    return PhotostimulationMeta(root, factory=bruker_element_factory)
+
+
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def load_voltage_recording(path: Union[str, Path]) -> pd.DataFrame:
     """
     Import bruker analog data from an imaging folder or individual file. By PrairieView naming conventions, these
-    | files contain "VoltageRecording" in the name.
+    files contain "VoltageRecording" in the name.
 
     :param path: folder or filename containing analog data
     :returns: dataframe containing time (index, ms) x channel data
     """
     if "VoltageRecording" in path.name and path.is_file():
         return _import_csv(path)
     elif not path.is_file():
         file = [file for file in path.glob("*.csv") if "VoltageRecording" in str(file)]
-        assert (len(file) == 1), "Too many files meeting parsing requirements"
+        assert (len(file) == 1), f"Too many files meet parsing requirements: {file}"
         return _import_csv(file)
     else:
         raise FileNotFoundError
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
-def repackage_bruker_tifs(input_folder: Union[str, Path], output_folder: Union[str, Path],
-                          channel: int = 0, plane: int = 0) -> None:
+def load_voltage_output(path: Union[str, Path]) -> pd.DataFrame:
+    """
+    Import bruker analog data from an imaging folder or individual file. By PrairieView naming conventions, these
+    files contain "VoltageOutput" in the name.
+
+    :param path: folder or filename containing analog data
+    :returns: dataframe containing time (index, ms) x channel data
+    """
+    raise NotImplementedError
+
+
+@convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
+def repackage_bruker_tifs(input_folder: Union[str, Path],
+                          output_folder: Union[str, Path],
+                          channel: int = 0,
+                          plane: int = 0
+                          ) -> None:
     """
     This function repackages a folder containing .tif files exported by Bruker's Prairieview software into a sequence
     of <4 GB .tif stacks. Note that parameters channel and plane are **zero-indexed**.
 
     :param input_folder: folder containing a sequence of single frame .tif files exported by Bruker's Prairieview
     :param output_folder: empty folder where .tif stacks will be saved
     :param channel: specify channel
     :param plane: specify plane
     """
     num_channels, num_planes, num_frames, y, x = determine_imaging_content(input_folder)
-    _pretty_print_image_description(num_channels, num_planes, num_frames, y, x)
+    _print_image_description(num_channels, num_planes, num_frames, y, x)
 
     naming_convention = generate_bruker_naming_convention(channel, plane, num_channels, num_planes)
 
     files = list(input_folder.glob(naming_convention))
 
     pbar = tq(total=num_frames)
     pbar.set_description("Repackaging...")
@@ -281,26 +337,28 @@
 @convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
 @validate_extension(required_extension=".csv", pos=0)
 def _import_csv(path: Union[str, Path]) -> pd.DataFrame:
     """
     Implementation function for loading csv files. Abstracted from the upper-level functions for cleaner logic.
 
     :param path: filepath of .csv to import
-    :type path: str or Path
     :return: dataframe containing time (index) x data [0:8]
-    :rtype: pandas.DataFrame
     """
     data = pd.read_csv(path, skipinitialspace=True)
     data = data.set_index("Time(ms)")
     data.sort_index(inplace=True)
     return data
 
 
-def _load_bruker_tif_stack(input_folder: Path, channel: int, plane: int,
-                           num_channels: int, num_planes: int) -> np.ndarray:
+def _load_bruker_tif_stack(input_folder: Path,
+                           channel: int,
+                           plane: int,
+                           num_channels: int,
+                           num_planes: int
+                           ) -> np.ndarray:
     """
     Implementation function to load a single bruker tif stack
 
     :param input_folder: folder containing tif stack
     :param channel: selected channel to load
     :param plane: selected plane to load
     :param num_channels: total number of channels
@@ -312,50 +370,45 @@
     pbar = tq(total=len(files))
     pbar.set_description("".join(["Loading Channel ", str(channel), " Plane ", str(plane)]))
     images = [_verbose_load_single_tif(file, pbar) for file in files]
     pbar.close()
     return np.concatenate(images, axis=0)
 
 
-def _pretty_print_image_description(channels: int, planes: int, frames: int, height: int, width: int) -> None:
+def _print_image_description(channels: int,
+                             planes: int,
+                             frames: int,
+                             height: int,
+                             width: int
+                             ) -> None:
     """
-    Function prints the description of an imaging dataset as a table.
+    Function prints the description of an imaging dataset.
 
     :param channels: number of channels
-    :type channels: int
     :param planes: number of planes
-    :type planes: int
     :param frames: number of frames
-    :type frames: int
     :param height: y-pixels
-    :type height: int
     :param width: x-pixels
-    :type width: int
-    :rtype: None
     """
-    _table = PrettyTable()
-    _table.header = False
-    _table.add_row(["Total Images Detected", channels * planes * frames])
-    _table.add_row(["Channels", channels])
-    _table.add_row(["Planes", planes])
-    _table.add_row(["Frames", frames])
-    _table.add_row(["Height", height])
-    _table.add_row(["Width", width])
-    print("\n")
-    print(_table)
+    msg = f"\nTotal Images Detected: {channels * planes * frames}"
+    msg += f"\nChannels\t{channels}"
+    msg += f"\nPlanes\t{planes}"
+    msg += f"\nFrames\t{frames}"
+    msg += f"\nHeight\t{height}"
+    msg += f"\nWidth\t{width}"
+    msg += "\n"
+
+    print(msg)
 
 
 def _verbose_load_single_tif(file: Union[str, Path], pbar: Any) -> np.ndarray:
     """
     Verbosely loads single tif by running the io_tools load single tif function
     and updating progressbar
 
     :param file: file to load
-    :type file: str or pathlib.Path
     :param pbar: progressbar
-    :type pbar: Any
     :return: loaded image
-    :rtype: numpy.ndarray
     """
     image = _load_single_tif(file)
     pbar.update(1)
     return image
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy/event_processing.py` & `CalSciPy-0.3.5/src/CalSciPy/event_processing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
-from typing import Iterable, Callable, Tuple, List
+from typing import Iterable, Callable, Tuple, List, Union
 import numpy as np
+import pandas as pd
 from sklearn.preprocessing import StandardScaler
 from scipy.ndimage import gaussian_filter1d
 from scipy.signal import find_peaks
 
 
 def calculate_firing_rates(spike_probability_matrix: np.ndarray, frame_rate: float = 30.0, in_place: bool = False) \
         -> np.ndarray:
@@ -160,14 +161,65 @@
     :param waveforms: An Iterable of M events by N samples matrices of waveforms
     :param scaler: sklearn preprocessing object
     :returns: An Iterable of M event by N samples scaled matrices of waveforms
     """
     return tuple([_scale_waveforms(waves, scaler) for waves in waveforms])
 
 
+def bin_data(data: Union[pd.DataFrame, np.ndarray, Iterable], bin_length: int, fun: Callable) \
+        -> Union[pd.DataFrame, np.ndarray]:
+
+    # record if pd
+    if isinstance(data, (pd.DataFrame, pd.Series, pd.Index)):
+        is_pd = True
+    elif isinstance(data, (np.ndarray, Iterable)):
+        is_pd = False
+    else:
+        raise TypeError(print(f"Argument data must be DataFrame, Series, Index, numpy array, or Iterable not "
+                              f"{type(data)}"))
+
+    # convert / copy if necessary
+    if is_pd is True:
+        data_ = data.copy(deep=True)
+        index_name = data_.index.name
+    else:
+        data_ = pd.DataFrame(data=data, columns=[str(x) for x in range(data.shape[1])])
+        data_.index.name = "Index"
+        index_name = "Index"
+
+    idx = data_.index.to_numpy()
+
+    bins = np.arange(idx[0], idx[-1], bin_length)
+
+    if bins[-1] == idx[-1]:
+        bins[-1] += 1
+    else:
+        bins = np.append(bins, idx[-1] + 1)
+
+    data_.reset_index(drop=False, inplace=True)
+
+    if fun == "median":
+        data_ = data_.groupby(pd.cut(data_[index_name], bins=bins, include_lowest=True, right=False)).median()
+    elif fun == "mean":
+        data_ = data_.groupby(pd.cut(data_[index_name], bins=bins, include_lowest=True, right=False)).mean()
+    elif fun == "sum":
+        data_ = data_.groupby(pd.cut(data_[index_name], bins=bins, include_lowest=True, right=False)).sum()
+    elif fun == "std":
+        data_ = data_.groupby(pd.cut(data_[index_name], bins=bins, include_lowest=True, right=False)).std()
+    else:
+        data_ = data_.groupby(pd.cut(data_[index_name], bins=bins, include_lowest=True, right=False)).apply(fun)
+
+    data_.drop(labels=index_name, axis="columns", inplace=True)
+
+    if is_pd:
+        return data_
+    else:
+        return data_.to_numpy(copy=True)
+
+
 def _collect_waveforms(trace: np.ndarray, event_index: Iterable[int], pre: int = 150, post: int = 450) -> np.ndarray:
     """
     Collect waveforms for each event
 
     :param trace: a fluorescent trace
     :param event_index: a list of events
     :param pre: number of pre-event frames
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy/image_processing.py` & `CalSciPy-0.3.5/src/CalSciPy/image_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/src/CalSciPy/io_tools.py` & `CalSciPy-0.3.5/src/CalSciPy/io_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 from __future__ import annotations
-from typing import Union, Optional
+from typing import Union, Optional, Mapping
 from pathlib import Path
 from json import load, dump
 
-
 from PIL import Image
 import numpy as np
 import cv2
 from PPVD.validation import validate_extension, validate_filename
 from PPVD.parsing import convert_permitted_types_to_required
 
+from .misc import generate_blocks, calculate_frames_per_file, zero_pad_num_to_string
+
 
-from .misc import generate_blocks, calculate_frames_per_file
+"""
+A collection of functions for loading, saving & converting imaging files. Stable as of version 3.5
+"""
 
 
+@validate_filename(pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
-def load_binary(path: Union[str, Path], mapped: bool = False) -> Union[np.ndarray, np.memmap]:
+def load_binary(path: Union[str, Path],
+                mapped: bool = False,
+                mode: str = "r+",
+                missing_metadata: Mapping = None
+                ) -> Union[np.ndarray, np.memmap]:
     """
     This function loads images saved in language-agnostic binary format. Ideal for optimal read/write speeds and
     highly-robust to corruption. However, the downside is that the images and their metadata are split into two
     separate files. Images are saved with the *.bin* extension, while metadata is saved with extension *.json*.
     If for some reason you lose the metadata, you can still load the binary if you know three of the following:
     number of frames, y-pixels, x-pixels, and the datatype (:class:`numpy.dtype`)
 
     :param path: folder containing binary file
     :param mapped: boolean indicating whether to load image using memory-mapping
+    :param mode: indicates the level of access permitted to the original binary
+    :param missing_metadata: if you have lost the metadata or otherwise wish to manually provide it
     :returns: image (frames, y-pixels, x-pixels)
     """
-    if not path.is_file():
-        path = path.joinpath("binary_video")
+    # If path is a folder and not just the filepath without an extension
+    if not path.is_file() and not path.with_suffix(".bin").exists():
+        try:
+            path = path.joinpath("binary_video")
+            assert (path.with_suffix(".bin").exists())
+            assert (path.with_suffix(".json").exists())
+        except AssertionError:
+            raise FileNotFoundError(f"{path.parent.with_suffix('.bin')} or "
+                                    f"{path.with_suffix('.bin')}/{path.with_suffix('.json')}")
 
     # add extensions
     meta_filename = path.with_suffix(".json")
     imaging_filename = path.with_suffix(".bin")
 
-    metadata = _Metadata.decode(meta_filename)
+    if missing_metadata:
+        metadata = _Metadata(**missing_metadata)
+    else:
+        metadata = _Metadata.decode(meta_filename)
 
     if mapped:
-        return np.memmap(imaging_filename, mode="r+", dtype=metadata.dtype, shape=(metadata.frames, metadata.y,
+        return np.memmap(imaging_filename, mode=mode, dtype=metadata.dtype, shape=(metadata.frames, metadata.y,
                                                                                    metadata.x))
     else:
         images = np.fromfile(imaging_filename, dtype=metadata.dtype)
         images = np.reshape(images, (metadata.frames, metadata.y, metadata.x))
         return images
 
 
@@ -57,110 +77,91 @@
     """
     if path.is_file():
         return _load_single_tif(path)
     else:
         return _load_many_tif(path)
 
 
+@validate_filename(pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
-def save_binary(path: Union[str, Path], images: np.ndarray) -> int:
+def save_binary(path: Union[str, Path], images: np.ndarray, name: str = "binary_video") -> int:
     """
     Save images to language-agnostic binary format. Ideal for optimal read/write speeds and highly-robust to corruption.
     However, the downside is that the images and their metadata are split into two separate files. Images are saved with
     the *.bin* extension, while metadata is saved with extension *.json*. If for some reason you lose the metadata, you
     can still load the binary if you know three of the following: number of frames, y-pixels, x-pixels, and the
     datatype. The datatype is almost always unsigned 16-bit (:class:`numpy.uint16`) for all modern imaging
     systems--even if they are collected at 12 or 13-bit.
 
     :param path: path to save images to. The path stem is considered the filename if it doesn't have any extension. If
     | no filename is provided then the default filename is *binary_video*.
     :param images: images to save (frames, y-pixels, x-pixels)
+    :param name: specify filename for produced files
     :returns: 0 if successful
     """
-    # parse the desired path
-    if path.is_file():
-        name = Path.name
-        file_path = Path(path.parents)
-    else:
-        name = "binary_video"
-        file_path = path
-
-    if not file_path.exists():
-        file_path.mkdir(parents=True, exist_ok=True)
+    # make folder if it doesn't exist
+    if not path.exists():
+        path.mkdir(parents=True, exist_ok=True)
 
     # add extensions
-    imaging_filename = file_path.joinpath(name).with_suffix(".bin")
-    metadata_filename = file_path.joinpath(name).with_suffix(".json")
+    imaging_filename = path.joinpath(name).with_suffix(".bin")
+    metadata_filename = path.joinpath(name).with_suffix(".json")
 
     # save metadata
     metadata = _Metadata(images)
     metadata.encode(metadata_filename)
 
     # save images
     images.tofile(imaging_filename)
 
 
 @validate_filename(pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
-def save_images(path: Union[str, Path], images: np.ndarray, size_cap: float = 3.9) -> int:
+def save_images(path: Union[str, Path],
+                images: np.ndarray,
+                name: str = "images",
+                size_cap: float = 3.9,) -> int:
     """
     Save a numpy array to a single .tif file. If size > 4GB then saved as a series of files. If path is not a file and
     already exists the default filename will be *images*.
 
     :param path: filename or absolute path
     :param images: numpy array (frames, y pixels, x pixels)
+    :param name: filename for saving images
     :param size_cap: maximum size per file
     :returns: returns 0 if successful
     """
-    # parse desired path
-    if Path.exists(path):
-        if path.is_file():
-            name = path.name
-            file_path = path.parent
-        else:
-            name = "images"
-            file_path = path
-    else:
-        if path.is_file():
-            name = path.name
-            file_path = path.parent
-        else:
-            name = "images"
-            file_path = path
-
-    if not Path.exists(file_path):
-        Path.mkdir(file_path, parents=True, exist_ok=True)
+    if not Path.exists(path):
+        Path.mkdir(path, parents=True, exist_ok=True)
 
     file_size = images.nbytes * 1e-9  # convert to GB
     if file_size <= size_cap:  # crop at 3.9 to be saved
-        filename = file_path.joinpath(name).with_suffix(".tif")
+        filename = path.joinpath(name).with_suffix(".tif")
         _save_single_tif(filename, images)
     else:
-        filename = file_path.joinpath(name)
+        filename = path.joinpath(name)
         _save_many_tif(filename, images, size_cap)
 
 
 @validate_extension(required_extension=".tif", pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
 def _load_single_tif(file: Union[str, Path]) -> np.ndarray:
     """
-    Load a single .tif as a numpy array
+    Load a single .tif as a numpy array (implementation function)
 
     :param file: absolute filename
-    :type file: str or pathlib.Path
     :return: numpy array (frames, y-pixels, x-pixels)
-    :rtype: numpy.ndarray
     """
     return np.array(cv2.imreadmulti(file, flags=-1)[1])
 
 
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def _load_many_tif(folder: Union[str, Path]) -> np.ndarray:
     """
-    Loads all .tif's within a folder into a single numpy array.
+    Loads all .tif's within a folder into a single numpy array (implementation function)
 
     :param folder: folder containing a sequence of tiff stacks
     :returns: a numpy array containing the images (frames, y-pixels, x-pixels)
     """
     files = list(folder.glob("*tif"))
     images = [_load_single_tif(file) for file in files]
 
@@ -172,14 +173,21 @@
 
     return np.concatenate(images, axis=0)
 
 
 @validate_extension(required_extension=".tif", pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=str, pos=0)
 def _save_single_tif(path: Union[str, Path], images: np.ndarray) -> int:
+    """
+    Implementation function for saving a single tif
+
+    :param path: path to save at
+    :param images: images
+    :return: 0 if successful
+    """
     # if single page save direct
     if len(images.shape) == 2:
         images = Image.fromarray(images)
         images.save(path)
     # if multi page iterate
     else:
         images_to_save = []
@@ -188,73 +196,100 @@
         images_to_save[0].save(path, format="TIFF", save_all=True, append_images=images_to_save[1:])
     return 0
 
 
 @validate_extension(required_extension=".tif", pos=0)
 @convert_permitted_types_to_required(permitted=(str, Path), required=Path, pos=0)
 def _save_many_tif(path: Union[str, Path], images: np.ndarray, size_cap: int = 3.9) -> int:
+    """
+    Implementation function for saving many tif
+
+    :param path: path to save at
+    :param images: images
+    :return: 0 if successful
+    """
     frames_per_file = calculate_frames_per_file(*images.shape[1:], size_cap=size_cap)
     frames = list(range(images.shape[0]))
     blocks = generate_blocks(frames, frames_per_file, 0)
     idx = 0
     base_filename = path.with_suffix("")
 
     try:
         for block in blocks:
-            if idx <= 9:
-                filename = base_filename.with_name("".join([base_filename.name, "_0", str(idx)]))
-                filename = filename.with_suffix(".tif")
-            else:
-                filename = path.with_name("".join([base_filename.name, "_", str(idx)]))
-                filename = filename.with_suffix(".tif")
+            str_idx = zero_pad_num_to_string(idx, 5)
+            filename = base_filename.with_name("".join([base_filename.name, str_idx]))
+            filename = filename.with_suffix(".tif")
             _save_single_tif(filename, images[block, :, :])
             idx += 1
     except (RuntimeError, StopIteration):
         pass
     return 0
 
 
 class _Metadata:
-    def __init__(self, images: Optional[np.ndarray] = None):
+    """
+    Metadata object used for saving/loading binary images
+
+    :ivar frames: number of frames
+    :type frames: int
+    :ivar y: height of each frame
+    :type y: int
+    :ivar x: width of each frame
+    :type x: int
+    :ivar dtype: datatype of each frame
+    :type dtype: np.dtype
+    """
+    def __init__(self,
+                 images: Optional[np.ndarray] = None,
+                 frames: int = None,
+                 y: int = None,
+                 x: int = None,
+                 dtype: np.dtype = None):
         """
-        Metadata object using for saving/loading binary images
+        Metadata object used for saving/loading binary images
 
         :param images: images in numpy array (frames, y-pixels, x-pixels)
+        :param frames: number of frames
+        :param y: number of y pixels
+        :param x: number of x pixels
+        :param dtype: type of data
         """
-        self.frames, self.y, self.x, self.dtype = None, None, None, None
+        self.frames = frames
+        self.y = y
+        self.x = x
+        self.dtype = dtype
 
         if images is not None:
             self.frames, self.y, self.x = images.shape
             self.dtype = str(images.dtype)
 
+        self._validate_metadata()
+
     @classmethod
     def decode(cls: _Metadata, filename: Path) -> _Metadata:
 
         with open(str(filename), "r+") as file:
             attrs = load(file)
 
-        metadata = _Metadata()
-        for key, value in attrs.items():
-            setattr(metadata, key, value)
+        return _Metadata(**attrs)
 
-        if "dtype" not in attrs:
-            raise AttributeError("dtype not found")
+    def encode(self, filename: Path) -> int:
+        meta = vars(self)
+        with open(str(filename), "w+") as file:
+            dump(meta, file)
+        return 0
+
+    def _validate_metadata(self) -> _Metadata:
+
+        attrs = vars(self)
 
-        missing_keys = []
-        for key in ["frames", "y", "x"]:
-            if key not in attrs:
-                missing_keys.append(key)
+        missing_keys = [key for key in ["dtype", "frames", "y", "x"] if not attrs.get(key)]
+
+        if "dtype" in missing_keys:
+            raise AttributeError("dtype not found")
 
         if len(missing_keys) > 1:
             raise AttributeError("Require at least 2/3 shape keys")
 
         if len(missing_keys) == 1:
-            setattr(metadata, missing_keys[0], -1)
+            setattr(self, missing_keys[0], -1)
             # set to negative one to let numpy figure it out
-
-        return metadata
-
-    def encode(self, filename: Path) -> int:
-        meta = vars(self)
-        with open(str(filename), "w+") as file:
-            dump(meta, file)
-        return 0
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy/misc.py` & `CalSciPy-0.3.5/src/CalSciPy/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,51 @@
 from __future__ import annotations
 from typing import Iterable, Iterator, Any, Callable
 from collections import deque
 from pathlib import Path
 from numbers import Number
-from functools import wraps
-
+from functools import wraps, partial
+from joblib import Parallel, delayed
 import numpy as np
 from tqdm import tqdm
 
+
 try:
     import cupy
 except ModuleNotFoundError:
     pass
 
 
+def zero_pad_num_to_string(idx: int, num_zeros: int) -> str:
+
+    str_idx = f"{idx}"
+
+    pad_length = num_zeros - len(str_idx)
+
+    return "".join(["_", "0" * pad_length, str_idx])
+
+
+def generate_time_vector(num_samples: int, sampling_frequency: Number = 30.0, start: Number = 0.0, step: Number = None
+                         ) -> np.ndarray:
+    """
+    Generates a time vector for a number of samples collected at either
+
+    :param num_samples:
+    :param sampling_frequency:
+    :param start:
+    :param step:
+    :return:
+    """
+
+    if not step:
+        step = 1 / sampling_frequency
+
+    return np.arange(0, num_samples) * step + start
+
+
 def calculate_frames_per_file(y_pixels: int, x_pixels: int, bit_depth: np.dtype = np.uint16, size_cap: Number = 3.9) \
         -> int:
     """
     Estimates the number of image frames to allocate to each file given some maximum size.
 
     :param y_pixels: number of y_pixels in image
     :param x_pixels: number of x_pixels in image
@@ -193,25 +221,22 @@
             if not comparator(value, case):
                 return False
         return True
 
 
 def sliding_window(sequence: np.ndarray, window_length: int, function: Callable, *args, **kwargs) -> np.ndarray:
     window_gen = generate_sliding_window(range(sequence.shape[-1]), window_length, 1)
-    values = []
-    sequence_length = sequence.shape[-1] - window_length + 2
-    pbar = tqdm(total=sequence_length, desc="Calculating baselines...")
-    try:
-        for step in window_gen:
-            values.append(function(sequence[..., step], *args, **kwargs))
-            pbar.update(1)
-    except (RuntimeError, StopIteration):
-        pass
-    pbar.close()
-    return np.array(values)
+    sequence_length = sequence.shape[-1] - window_length + 1
+    slider = partial(function, *args, **kwargs)
+    values = Parallel(n_jobs=-1, backend="loky", verbose=0)(delayed(slider)(sequence[..., window])
+                                                            for window in tqdm(window_gen,
+                                                                               total=sequence_length,
+                                                                               desc="Calculating sliding windows")
+                                                            )
+    return np.asarray(values)
 
 
 def generate_sliding_window(sequence: Iterable, window_length: int, step_size: int = 1) -> np.ndarray:
 
     window = deque(maxlen=window_length)
     iterable = iter(sequence)
 
@@ -227,9 +252,9 @@
         except StopIteration:
             # noinspection PyUnboundLocalVariable
             if idx == 0:
                 pass
             elif idx == step_size:
                 pass
             else:
-                yield tuple(window)
-            raise StopIteration
+                return tuple(window)
+            return
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy/trace_processing.py` & `CalSciPy-0.3.5/src/CalSciPy/trace_processing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 from __future__ import annotations
 from typing import Optional
 
 import numpy as np
 from scipy.signal import firwin, filtfilt
+from scipy.ndimage.filters import gaussian_filter1d
 from numba import njit
 from tqdm import tqdm
+from .misc import sliding_window
 
 
-def calculate_dfof(traces: np.ndarray, frame_rate: float = 30.0, in_place: bool = False,
+def calculate_dfof(traces: np.ndarray,
+                   frame_rate: float = 30.0,
+                   in_place: bool = False,
+                   offset: float = 0.0,
+                   external_reference: Optional[np.ndarray] = None,
+                   method: str = "baseline"
+                   ) -> np.ndarray:
+    if method == "baseline":
+        return _calculate_dfof_baseline(traces, frame_rate, in_place, offset, external_reference)
+    else:
+        return _calculate_dfof_filter(traces, frame_rate, in_place, offset, external_reference)
+
+
+def _calculate_dfof_filter(traces: np.ndarray, frame_rate: float = 30.0, in_place: bool = False,
                    offset: float = 0.0, external_reference: Optional[np.ndarray] = None) \
         -> np.ndarray:
     # noinspection GrazieInspection
     """
         Calculates Δf/f0 (fold fluorescence over baseline). Baseline is defined as the 5th percentile of the signal
         after a 1Hz low-pass filter using a Hamming window. Baseline can be calculated using an external reference
         | using the raw argument or adjusted by using the offset argument. Supports in-place calculation
@@ -64,14 +79,28 @@
 
         # calculate dfof
         dfof[neuron, :] = (dfof[neuron, :] - baseline) / baseline
 
     return dfof
 
 
+def _calculate_dfof_mean_of_percentile(traces: np.ndarray,
+                                       frame_rate: float = 30.0,
+                                       in_place: bool = False,
+                                       offset: float = 0.0,
+                                       external_reference: Optional[np.ndarray] = None
+                                       ) -> np.ndarray:
+    baselines = np.nanmean(sliding_window(traces, frame_rate * 30, np.nanpercentile, q=8, axis=-1), axis=0)
+    if not in_place:
+        dfof = np.zeros_like(traces)
+    for neuron in range(dfof.shape[0]):
+        dfof[neuron, :] = (traces[neuron, :] - baseline[neuron]) / baseline[neuron]
+    return dfof
+
+
 def calculate_standardized_noise(fold_fluorescence_over_baseline: np.ndarray, frame_rate: float = 30.0) -> np.ndarray:
     """
     Calculates a frame-rate independent standardized noise as defined as:
         | :math:`v = \\frac{\sigma \\frac{\Delta F}F}\sqrt{f}`
 
     It is robust against outliers and approximates the standard deviation of Δf/f0 baseline fluctuations.
     For comparison, the more exquisite of the Allen Brain Institute's public datasets are approximately 1*%Hz^(-1/2)
@@ -101,15 +130,15 @@
 
     for _neuron in range(_neurons):
         _fit = np.polyval(np.polyfit(_samples_vector, detrended_matrix[_neuron, :], deg=4), _samples_vector)
         detrended_matrix[_neuron] -= _fit
     return detrended_matrix
 
 
-def perona_malik_diffusion(traces: np.ndarray, iters: int = 25, kappa: float = 0.15, gamma: float = 0.25,
+def perona_malik_diffusion(traces: np.ndarray, iters: int = 25, kappa: float = 0.15, gamma: float = 0.25, sigma: float = 0,
                            in_place: bool = False) -> np.ndarray:
     """
     Edge-preserving smoothing using perona malik diffusion. This is a non-linear smoothing technique that avoids the
     temporal distortion introduced onto traces by standard gaussian smoothing.
 
     The parameter `kappa` controls the level of smoothing ("diffusion") as a function of the derivative of the trace
     (or "gradient" in the case of 2D images where this algorithm is often used). This function is known as the
@@ -139,23 +168,23 @@
 
     if in_place:
         smoothed_traces = traces
     else:
         smoothed_traces = traces.copy()
 
     if traces.ndim == 1:
-        return _perona_malik_diffusion(traces, iters, kappa, gamma)
+        return _perona_malik_diffusion(traces, iters, kappa, gamma, sigma, in_place)
     else:
         for neuron in tqdm(range(traces.shape[0]), total=traces.shape[0], desc="Smoothing Traces"):
-            smoothed_traces[neuron, :] = _perona_malik_diffusion(traces[neuron, :], iters, kappa, gamma, in_place)
+            smoothed_traces[neuron, :] = _perona_malik_diffusion(traces[neuron, :], iters, kappa, gamma, sigma, in_place)
 
     return smoothed_traces
 
 
-def _perona_malik_diffusion(trace: np.ndarray, iters: int = 25, kappa: float = 0.15, gamma: float = 0.25,
+def _perona_malik_diffusion(trace: np.ndarray, iters: int = 25, kappa: float = 0.15, gamma: float = 0.25, sigma: float = 0,
                             in_place: bool = False) -> np.ndarray:
     """
     Edge-preserving smoothing using perona malik diffusion. This is a non-linear extension of gaussian smoothing
     technique that avoids the temporal distortion introduced onto traces by standard gaussian smoothing.
 
     The parameter `kappa` controls the level of smoothing ("diffusion") as a function of the derivative of the trace
     (or "gradient" in the case of 2D images where this algorithm is often used). This function is known as the
@@ -189,14 +218,16 @@
 
     # preallocate
     derivative = np.zeros_like(smoothed_trace)
 
     for _ in range(iters):
         derivative = np.zeros_like(smoothed_trace)
         derivative[:-1] = np.diff(smoothed_trace)
+        if sigma > 0:
+            derivative = gaussian_filter1d(derivative, sigma)
         diffusion = derivative * _diffusion_coefficient(derivative, kappa)
         diffusion[1:] -= diffusion[:-1]
         smoothed_trace += (gamma * diffusion)
 
     return smoothed_trace
```

### Comparing `CalSciPy-0.3.2/src/CalSciPy.egg-info/PKG-INFO` & `CalSciPy-0.3.5/src/CalSciPy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CalSciPy
-Version: 0.3.2
+Version: 0.3.5
 Summary: A collection
 Author: Darik A. O'Neil
 Maintainer: Darik A. O'Neil
 License: MIT License
         
         Copyright (c) 2023 Darik A O’Neil
         
@@ -30,14 +30,15 @@
 Project-URL: repository, https://github.com/darikoneil/CalSciPy
 Keywords: CalSciPy,Calcium Imaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: development
 Provides-Extra: gpu
@@ -53,46 +54,32 @@
 [![Documentation Status](https://readthedocs.org/projects/calscipy/badge/?version=latest)](https://calscipy.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/CalSciPy?)
 ![PyPI - Status](https://img.shields.io/pypi/status/CalSciPy)
 ![GitHub](https://img.shields.io/github/license/darikoneil/CalSciPy)
 [![Contributors](https://img.shields.io/github/contributors-anon/darikoneil/CalSciPy)](https://github.com/darikoneil/CalSciPy/graphs/contributors)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/darikoneil/CalSciPy/calscipy_lint_test_action.yml)
 
+This python packages contains a variety of useful tools for handling, processing, visualizing, & designing calcium 
+imaging experiments. I noticed I was constantly re-writing boilerplate, "one-liners", and copy/pasting code between
+environments. I wrote this so ~I don't have to~ you don't have to. It's intended to be a collection of useful, 
+well-documented functions often used in boilerplate code alongside software packages such as 
+[Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), 
+and [Suite2P](https://github.com/MouseLand/suite2p), as well as a collection of more bespoke software designed for use 
+with Bruker's PrairieView Imaging Software and MeadowLark Spatial Light Modulators. Essentially, it's a collection of 
+code written for my imaging experiments that might be considered useful to others.
 
-This python packages contains a variety of useful methods for handling, processing, and visualizing calcium imaging data. It's intended to be a collection of useful, well-documented functions often used in boilerplate code alongside software packages such as [Caiman](https://github.com/flatironinstitute/CaImAn), [SIMA](https://github.com/losonczylab/sima), and [Suite2P](https://github.com/MouseLand/suite2p).
+#### Active Development
+* The current implementation is unstable and should be considered an open beta.
 
 #### Highlights
 * Assign unique colormaps to subsets of ROIs to generate rich, informative videos
 * Perona-Malik diffusion for edge-preserving denoising
-* Methods for handling Bruker's PrairieView data
-* Interactive visualization
+* Fast, convenient functions for handling, aligning, and compiling data collected in Bruker's PrairieView software
+* Functions for generating protocols for use in Bruker's Prairieview.
+* Interactive visualization of data
 
 #### Installation
 `pip install CalSciPy`
 
-#### Subpackages
-* Bruker - MAIN
-* Coloring - TODO
-* Event Processing - DEV
-* Input/Output (I/O) - MAIN
-* Image Processing - DEV
-* Interactive Visuals - TODO
-* Reorganization - MAIN
-* Signal Processing - DEV
-* Static Visuals - TODO
-
 #### Documentation
 Hosted at [ReadtheDocs](https://calscipy.readthedocs.io/en/latest/index.html#).
 Available locally as [HTML](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/html), [LATEX](https://github.com/darikoneil/CalSciPy/tree/master/docs/build/latex) and [PDF](https://github.com/darikoneil/CalSciPy/blob/master/docs/build/pdf/calscipy.pdf).
-
-#### Roadmap
-TODO - UNDOCUMENTED / OFFLINE     
-DEV - UNTESTED / IN DEV BRANCH      
-MAIN - COMPLETE /  IN MAIN BRANCH     
-
-Generally completing each module before the next.     
-Exceptions done last:       
-* Bruker's Prairiview XML
-* Bruker's Prairieview ENV parsing
-* Trace Processing's Diffusion
-* Event Processing's Covariance
-* Interactive's ROI methods
```

### Comparing `CalSciPy-0.3.2/tests/test_a_install.py` & `CalSciPy-0.3.5/tests/test_a_install.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/tests/test_bruker.py` & `CalSciPy-0.3.5/tests/test_bruker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import numpy as np
 from pathlib import Path
 from shutil import rmtree
 from tests.helpers import BlockPrinting, read_descriptions
 from tests.conftest import SAMPLES_DATASETS_DIRECTORY
 from CalSciPy.io_tools import load_images
-from CalSciPy.bruker import determine_imaging_content, load_bruker_tifs, repackage_bruker_tifs
+from CalSciPy.bruker.data import determine_imaging_content, load_bruker_tifs, repackage_bruker_tifs
 
 
 DATASET = pytest.mark.datafiles(
     SAMPLES_DATASETS_DIRECTORY,
     keep_top_dir=False,
     on_duplicate="ignore",
 )
```

### Comparing `CalSciPy-0.3.2/tests/test_event_processing.py` & `CalSciPy-0.3.5/tests/test_event_processing.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/tests/test_io_tools.py` & `CalSciPy-0.3.5/tests/test_io_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,19 +43,26 @@
                                                                                                f"implementation and"
                                                                                                f"abstracted methods")
         # test single image saving
         save_images(output_folder, image_abstracted_method)
         _save_single_tif(output_folder, image_abstracted_method)
         image_abstracted_method_reloaded = load_images(output_folder)
         image_implement_method_reloaded = load_images(output_folder)
+        # test 2D single image
+        save_images(output_folder, image_abstracted_method.reshape(image_abstracted_method.shape[1:]))
+        images_abstracted_2d = load_images(output_folder)
         np.testing.assert_array_equal(image_abstracted_method_reloaded, image_implement_method_reloaded,
                                       err_msg=f"Image Mismatch between loading with implementation "
                                               f"and abstracted methods")
         np.testing.assert_array_equal(image_abstracted_method_reloaded, image_abstracted_method,
                                       err_msg=f"Image mismatch between saved and loaded image")
+        np.testing.assert_array_equal(
+            image_abstracted_method_reloaded,
+            images_abstracted_2d,
+            err_msg=f"Image mismatch between 3D & 2D image")
         # test exact filename
         output_file = Path(tmp_path).joinpath("exact_filename.tif")
         save_images(output_file, image_abstracted_method)
         image_reloaded = load_images(output_file)
 
     # test exceptions
     with pytest.raises(ValueError):
@@ -194,14 +201,15 @@
 
 @DATASET
 def test_binary(datafiles, tmp_path, matrix):
     for directory in datafiles.listdir():
         # Description of Expected
         descriptions = Path(directory).joinpath("description.txt")
         descriptions = read_descriptions(descriptions)
+        frames, y, x = descriptions[2:]
 
         # single image
         imaging_folder = Path(directory).joinpath("binary")
 
         # output folder
         output_folder = Path(tmp_path).joinpath("".join([Path(directory).stem, "_output_0"]))
 
@@ -218,23 +226,41 @@
         np.testing.assert_array_equal(images, images_reloaded,
                                       err_msg=f"Mismatch: failed matching original and reloaded dataset")
 
         # make sure memory map loads
         image_memory_mapped = load_binary(output_folder, mapped=True)
 
         # make sure we can save & load a non-default filename
-        output_file = Path(tmp_path).joinpath("exact_filename.bin")
-        save_binary(output_file, images)
-        images_reloaded_exact_filename = load_binary(output_file)
+        exact_output_folder = Path(tmp_path).joinpath("exact_folder")
+        save_binary(exact_output_folder, images, name="exact_filename")
+        images_reloaded_exact_filename = load_binary(exact_output_folder.joinpath("exact_filename"))
+
+        # make sure we can load with interpolated metadata
+        interp_images = load_binary(exact_output_folder.joinpath("exact_filename"),
+                                    missing_metadata={"dtype": np.uint16, "y": y, "x": x})
 
-    # test exceptions
+        np.testing.assert_array_equal(images_reloaded_exact_filename, interp_images,
+                                      err_msg=f"Mismatch: failed matching original and reloaded dataset")
+
+        # we also fail if missing sufficient metadata
+        with pytest.raises(AttributeError):
+            load_binary(exact_output_folder.joinpath("exact_filename"),
+                        missing_metadata={"frames": frames, "y": y, "x": x})
+        with pytest.raises(AttributeError):
+            load_binary(exact_output_folder.joinpath("exact_filename"),
+                        missing_metadata={"dtype": np.uint16, "x": x})
+
+    # generic test exceptions
+    with pytest.raises(FileNotFoundError):
+        load_binary(Path.cwd())
     with pytest.raises(ValueError):
-        load_images("C:\\&^6* ***%")  # FAIL PERMITTED CHARS
+        load_binary("C:\\&^6* ***%")  # FAIL PERMITTED CHARS
     with pytest.raises(TypeError):
         # noinspection PyTypeChecker
-        load_images(125.6)  # fail with bad type so we don't do anything unexpected
+        load_binary(125.6)  # fail with bad type so we don't do anything unexpected
     with pytest.raises(ValueError):
-        save_images("C:\\&^6*", matrix)  # FAIL VALIDATE PATH PERMITTED CHARS
+        save_binary("C:\\&^6*", matrix)  # FAIL VALIDATE PATH PERMITTED CHARS
     with pytest.raises(TypeError):
         # noinspection PyTypeChecker
-        save_images(125.6, matrix)  # fail with bad type so we don't do anything unexpected
+        save_binary(125.6, matrix)  # fail with bad type so we don't do anything unexpected
+
     # the rest of failures are fine being trial by forgiveness
```

### Comparing `CalSciPy-0.3.2/tests/test_misc.py` & `CalSciPy-0.3.5/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/tests/test_reorganization.py` & `CalSciPy-0.3.5/tests/test_reorganization.py`

 * *Files identical despite different names*

### Comparing `CalSciPy-0.3.2/tests/test_trace_processing.py` & `CalSciPy-0.3.5/tests/test_trace_processing.py`

 * *Files identical despite different names*

