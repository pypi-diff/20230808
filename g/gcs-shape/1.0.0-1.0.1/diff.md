# Comparing `tmp/gcs-shape-1.0.0.tar.gz` & `tmp/gcs-shape-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcs-shape-1.0.0.tar", last modified: Tue Aug  8 02:27:22 2023, max compression
+gzip compressed data, was "gcs-shape-1.0.1.tar", last modified: Tue Aug  8 03:48:22 2023, max compression
```

## Comparing `gcs-shape-1.0.0.tar` & `gcs-shape-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.695692 gcs-shape-1.0.0/
--rw-r--r--   0 sssilver   (501) staff       (20)     1084 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/LICENSE
--rw-r--r--   0 sssilver   (501) staff       (20)     4620 2023-08-08 02:27:22.695538 gcs-shape-1.0.0/PKG-INFO
--rw-r--r--   0 sssilver   (501) staff       (20)     3502 2023-08-08 02:18:47.000000 gcs-shape-1.0.0/README.md
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.692085 gcs-shape-1.0.0/gcs/
--rw-r--r--   0 sssilver   (501) staff       (20)      957 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/__init__.py
--rw-r--r--   0 sssilver   (501) staff       (20)     2831 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/discretization.py
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.692499 gcs-shape-1.0.0/gcs/io/
--rw-r--r--   0 sssilver   (501) staff       (20)      301 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/io/__init__.py
--rw-r--r--   0 sssilver   (501) staff       (20)      782 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/io/load.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1250 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/io/save.py
--rw-r--r--   0 sssilver   (501) staff       (20)     6761 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/shape.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1904 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/triangulation.py
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.693120 gcs-shape-1.0.0/gcs/utils/
--rw-r--r--   0 sssilver   (501) staff       (20)      281 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/utils/__init__.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1119 2023-07-11 13:45:31.000000 gcs-shape-1.0.0/gcs/utils/coordinates.py
--rw-r--r--   0 sssilver   (501) staff       (20)     2455 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/utils/polar_curves.py
--rw-r--r--   0 sssilver   (501) staff       (20)     3701 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/utils/summed_cosine.py
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.693714 gcs-shape-1.0.0/gcs/verify/
--rw-r--r--   0 sssilver   (501) staff       (20)      385 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/verify/__init__.py
--rw-r--r--   0 sssilver   (501) staff       (20)      995 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/verify/verify.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1097 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/verify/verify_base_perimeter.py
--rw-r--r--   0 sssilver   (501) staff       (20)     2402 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/gcs/verify/verify_radius.py
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.694480 gcs-shape-1.0.0/gcs_shape.egg-info/
--rw-r--r--   0 sssilver   (501) staff       (20)     4620 2023-08-08 02:27:22.000000 gcs-shape-1.0.0/gcs_shape.egg-info/PKG-INFO
--rw-r--r--   0 sssilver   (501) staff       (20)      646 2023-08-08 02:27:22.000000 gcs-shape-1.0.0/gcs_shape.egg-info/SOURCES.txt
--rw-r--r--   0 sssilver   (501) staff       (20)        1 2023-08-08 02:27:22.000000 gcs-shape-1.0.0/gcs_shape.egg-info/dependency_links.txt
--rw-r--r--   0 sssilver   (501) staff       (20)       82 2023-08-08 02:27:22.000000 gcs-shape-1.0.0/gcs_shape.egg-info/requires.txt
--rw-r--r--   0 sssilver   (501) staff       (20)        4 2023-08-08 02:27:22.000000 gcs-shape-1.0.0/gcs_shape.egg-info/top_level.txt
--rw-r--r--   0 sssilver   (501) staff       (20)       38 2023-08-08 02:27:22.695739 gcs-shape-1.0.0/setup.cfg
--rw-r--r--   0 sssilver   (501) staff       (20)     1582 2023-08-08 02:19:38.000000 gcs-shape-1.0.0/setup.py
-drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 02:27:22.695337 gcs-shape-1.0.0/tests/
--rw-r--r--   0 sssilver   (501) staff       (20)     1085 2023-07-11 13:45:31.000000 gcs-shape-1.0.0/tests/test_discretize.py
--rw-r--r--   0 sssilver   (501) staff       (20)     3973 2023-07-18 14:15:01.000000 gcs-shape-1.0.0/tests/test_gcs.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1046 2023-07-11 13:45:31.000000 gcs-shape-1.0.0/tests/test_io.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1039 2023-07-11 13:45:31.000000 gcs-shape-1.0.0/tests/test_triangulate.py
--rw-r--r--   0 sssilver   (501) staff       (20)     2745 2023-07-25 15:26:01.000000 gcs-shape-1.0.0/tests/test_utils.py
--rw-r--r--   0 sssilver   (501) staff       (20)     1066 2023-07-18 14:51:23.000000 gcs-shape-1.0.0/tests/test_verify.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.093779 gcs-shape-1.0.1/
+-rw-r--r--   0 sssilver   (501) staff       (20)     1084 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/LICENSE
+-rw-r--r--   0 sssilver   (501) staff       (20)     4620 2023-08-08 03:48:22.093628 gcs-shape-1.0.1/PKG-INFO
+-rw-r--r--   0 sssilver   (501) staff       (20)     3502 2023-08-08 02:18:47.000000 gcs-shape-1.0.1/README.md
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.090246 gcs-shape-1.0.1/gcs/
+-rw-r--r--   0 sssilver   (501) staff       (20)      957 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/__init__.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     2831 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/discretization.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.090680 gcs-shape-1.0.1/gcs/io/
+-rw-r--r--   0 sssilver   (501) staff       (20)      301 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/io/__init__.py
+-rw-r--r--   0 sssilver   (501) staff       (20)      782 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/io/load.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1250 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/io/save.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     6761 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/shape.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1904 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/triangulation.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.091245 gcs-shape-1.0.1/gcs/utils/
+-rw-r--r--   0 sssilver   (501) staff       (20)      281 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/utils/__init__.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1119 2023-07-11 13:45:31.000000 gcs-shape-1.0.1/gcs/utils/coordinates.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     2455 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/utils/polar_curves.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     3701 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/utils/summed_cosine.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.091859 gcs-shape-1.0.1/gcs/verify/
+-rw-r--r--   0 sssilver   (501) staff       (20)      385 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/verify/__init__.py
+-rw-r--r--   0 sssilver   (501) staff       (20)      995 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/verify/verify.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1097 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/verify/verify_base_perimeter.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     2402 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/gcs/verify/verify_radius.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.092637 gcs-shape-1.0.1/gcs_shape.egg-info/
+-rw-r--r--   0 sssilver   (501) staff       (20)     4620 2023-08-08 03:48:22.000000 gcs-shape-1.0.1/gcs_shape.egg-info/PKG-INFO
+-rw-r--r--   0 sssilver   (501) staff       (20)      646 2023-08-08 03:48:22.000000 gcs-shape-1.0.1/gcs_shape.egg-info/SOURCES.txt
+-rw-r--r--   0 sssilver   (501) staff       (20)        1 2023-08-08 03:48:22.000000 gcs-shape-1.0.1/gcs_shape.egg-info/dependency_links.txt
+-rw-r--r--   0 sssilver   (501) staff       (20)       82 2023-08-08 03:48:22.000000 gcs-shape-1.0.1/gcs_shape.egg-info/requires.txt
+-rw-r--r--   0 sssilver   (501) staff       (20)        4 2023-08-08 03:48:22.000000 gcs-shape-1.0.1/gcs_shape.egg-info/top_level.txt
+-rw-r--r--   0 sssilver   (501) staff       (20)       38 2023-08-08 03:48:22.093829 gcs-shape-1.0.1/setup.cfg
+-rw-r--r--   0 sssilver   (501) staff       (20)     1582 2023-08-08 03:46:32.000000 gcs-shape-1.0.1/setup.py
+drwxr-xr-x   0 sssilver   (501) staff       (20)        0 2023-08-08 03:48:22.093444 gcs-shape-1.0.1/tests/
+-rw-r--r--   0 sssilver   (501) staff       (20)     1085 2023-07-11 13:45:31.000000 gcs-shape-1.0.1/tests/test_discretize.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     3973 2023-07-18 14:15:01.000000 gcs-shape-1.0.1/tests/test_gcs.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1046 2023-07-11 13:45:31.000000 gcs-shape-1.0.1/tests/test_io.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1039 2023-07-11 13:45:31.000000 gcs-shape-1.0.1/tests/test_triangulate.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     2745 2023-07-25 15:26:01.000000 gcs-shape-1.0.1/tests/test_utils.py
+-rw-r--r--   0 sssilver   (501) staff       (20)     1066 2023-07-18 14:51:23.000000 gcs-shape-1.0.1/tests/test_verify.py
```

### Comparing `gcs-shape-1.0.0/LICENSE` & `gcs-shape-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/PKG-INFO` & `gcs-shape-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcs-shape
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generalized cylindrical shell library for Python.
 Home-page: https://github.com/bu-shapelab/gcs
 Download-URL: https://pypi.python.org/pypi/gcs
 Author: Kelsey L. Snapp et al.
 Maintainer: Samuel Silverman
 Maintainer-email: sssilver@bu.edu
 License: MIT
```

### Comparing `gcs-shape-1.0.0/README.md` & `gcs-shape-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/__init__.py` & `gcs-shape-1.0.1/gcs/__init__.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/discretization.py` & `gcs-shape-1.0.1/gcs/discretization.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/io/load.py` & `gcs-shape-1.0.1/gcs/io/load.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/io/save.py` & `gcs-shape-1.0.1/gcs/io/save.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/shape.py` & `gcs-shape-1.0.1/gcs/shape.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/triangulation.py` & `gcs-shape-1.0.1/gcs/triangulation.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/utils/coordinates.py` & `gcs-shape-1.0.1/gcs/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/utils/polar_curves.py` & `gcs-shape-1.0.1/gcs/utils/polar_curves.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/utils/summed_cosine.py` & `gcs-shape-1.0.1/gcs/utils/summed_cosine.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/verify/verify.py` & `gcs-shape-1.0.1/gcs/verify/verify.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/verify/verify_base_perimeter.py` & `gcs-shape-1.0.1/gcs/verify/verify_base_perimeter.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs/verify/verify_radius.py` & `gcs-shape-1.0.1/gcs/verify/verify_radius.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/gcs_shape.egg-info/PKG-INFO` & `gcs-shape-1.0.1/gcs_shape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcs-shape
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generalized cylindrical shell library for Python.
 Home-page: https://github.com/bu-shapelab/gcs
 Download-URL: https://pypi.python.org/pypi/gcs
 Author: Kelsey L. Snapp et al.
 Maintainer: Samuel Silverman
 Maintainer-email: sssilver@bu.edu
 License: MIT
```

### Comparing `gcs-shape-1.0.0/gcs_shape.egg-info/SOURCES.txt` & `gcs-shape-1.0.1/gcs_shape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/setup.py` & `gcs-shape-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 
 setup(
     name='gcs-shape',
-    version='1.0.0',
+    version='1.0.1',
     description='Generalized cylindrical shell library for Python.',
     long_description=Path('README.md').read_text(encoding='utf-8'),
     long_description_content_type='text/markdown',
     author='Kelsey L. Snapp et al.',
     maintainer='Samuel Silverman',
     maintainer_email='sssilver@bu.edu',
     url='https://github.com/bu-shapelab/gcs',
```

### Comparing `gcs-shape-1.0.0/tests/test_discretize.py` & `gcs-shape-1.0.1/tests/test_discretize.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/tests/test_gcs.py` & `gcs-shape-1.0.1/tests/test_gcs.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/tests/test_io.py` & `gcs-shape-1.0.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/tests/test_triangulate.py` & `gcs-shape-1.0.1/tests/test_triangulate.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/tests/test_utils.py` & `gcs-shape-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gcs-shape-1.0.0/tests/test_verify.py` & `gcs-shape-1.0.1/tests/test_verify.py`

 * *Files identical despite different names*

