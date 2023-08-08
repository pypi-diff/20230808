# Comparing `tmp/saibr-0.1.4.tar.gz` & `tmp/saibr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/saibr_python/saibr_python/dist/.tmp-tzz127j1/saibr-0.1.4.tar", last modified: Thu Aug  3 11:08:39 2023, max compression
+gzip compressed data, was "/home/runner/work/saibr_python/saibr_python/dist/.tmp-ejb315w7/saibr-0.1.5.tar", last modified: Tue Aug  8 14:05:02 2023, max compression
```

## Comparing `saibr-0.1.4.tar` & `saibr-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-03 11:08:26.000000 saibr-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 11:08:39.000000 saibr-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-03 11:08:26.000000 saibr-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-08-03 11:08:26.000000 saibr-0.1.4/saibr/saibr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:08:39.000000 saibr-0.1.4/saibr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 11:08:39.000000 saibr-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-03 11:08:26.000000 saibr-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:05:02.000000 saibr-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18650 2023-08-08 14:04:49.000000 saibr-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 14:05:02.000000 saibr-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-08 14:04:49.000000 saibr-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-08 14:04:50.000000 saibr-0.1.5/saibr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 14:04:50.000000 saibr-0.1.5/saibr/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-08-08 14:04:50.000000 saibr-0.1.5/saibr/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-08-08 14:04:50.000000 saibr-0.1.5/saibr/saibr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 14:05:02.000000 saibr-0.1.5/saibr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 14:05:02.000000 saibr-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-08 14:04:50.000000 saibr-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:05:02.000000 saibr-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:04:50.000000 saibr-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-08 14:04:50.000000 saibr-0.1.5/tests/test_.py
```

### Comparing `saibr-0.1.4/LICENSE` & `saibr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `saibr-0.1.4/PKG-INFO` & `saibr-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: saibr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: https://github.com/goehringlab/saibr_python
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
 Project-URL: Source Code, https://github.com/goehringlab/saibr_python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SAIBR (python implementation)
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/saibr/)](https://pypi.org/project/saibr)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goehringlab/saibr_python/HEAD?filepath=%2Fscripts/SAIBRdemonstration.ipynb)
+[![Documentation Status](https://readthedocs.org/projects/saibr/badge/?version=latest)](https://saibr.readthedocs.io/en/latest/?badge=latest)
 
 
 Python implementation of SAIBR: a simple, platform independent protocol for spectral autofluorescence correction
 
 [Paper](https://journals.biologists.com/dev/article/149/14/dev200545/276004/SAIBR-a-simple-platform-independent-method-for)
 
 [FIJI plugin](https://github.com/goehringlab/saibr_fiji_plugin)
```

### Comparing `saibr-0.1.4/README.md` & `saibr-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SAIBR (python implementation)
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/saibr/)](https://pypi.org/project/saibr)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goehringlab/saibr_python/HEAD?filepath=%2Fscripts/SAIBRdemonstration.ipynb)
+[![Documentation Status](https://readthedocs.org/projects/saibr/badge/?version=latest)](https://saibr.readthedocs.io/en/latest/?badge=latest)
 
 
 Python implementation of SAIBR: a simple, platform independent protocol for spectral autofluorescence correction
 
 [Paper](https://journals.biologists.com/dev/article/149/14/dev200545/276004/SAIBR-a-simple-platform-independent-method-for)
 
 [FIJI plugin](https://github.com/goehringlab/saibr_fiji_plugin)
```

### Comparing `saibr-0.1.4/saibr/misc.py` & `saibr-0.1.5/saibr/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from skimage import io
 from typing import Optional
 import glob
 import matplotlib.pyplot as plt
 import copy
 
+__all__ = ['load_image', 'save_img', 'save_img_jpeg', 'direcslist']
 
 def load_image(filename: str) -> np.ndarray:
     """
     Given the filename of a TIFF, creates numpy array with pixel intensities
 
     Args:
         filename: full path to the file to import (including extension)
```

### Comparing `saibr-0.1.4/saibr/saibr.py` & `saibr-0.1.5/saibr/saibr.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,48 @@
 from sklearn.metrics import r2_score
 from sklearn.linear_model import LinearRegression
 from .misc import load_image
 from typing import Tuple, Optional, Union
 import cv2
 
 
+__all__ = ['SaibrCalibrate', 'saibr_correlation', 'saibr_correlation_3channel', 'saibr_correct', 'saibr_correct_3channel', 'make_mask', 
+           'offset_coordinates']
+
 class SaibrCalibrate:
+    """
+
+    Class for performing SAIBR calibration
+
+    Two methods of specifying data
+    - input the images directly as a list for each channel along with a list of ROIs
+    - specify a list of paths and regular expressions for image files and ROIs (easier method if files are set up appropriately)
+
+    If rfp channel is not specified, will perform the normal two channel calibration
+
+    Args:
+        gfp: list of GFP channel images
+        af: list off AF channel images
+        rfp: list of RFP channel images
+        roi: list of ROIs
+        paths: list of paths containing n2 images
+        gfp_regex: regular expression found in gfp channel image files
+        af_regex: regular expression found in af channel image files
+        rfp_regex: regular expression found in rfp channel files (optional)
+        roi_regex: regular expression found in ROI files
+        sigma: gaussian blur to apply to images prior to regression
+        intercept0: if True, force intercept of regression to go through zero. Not recommended
+        expand: expand ROIs by this many pixels (useful to include a portion of background)
+        method: fitting method, either 'OLS' for ordinary least squares or 'ODR' for orthogonal distance regression
+
+    To run regression, initialise class and run()
+    SAIBR parameters will then be found at self.params
+
+    """
+
     def __init__(self,
                  gfp: Optional[list] = None,
                  af: Optional[list] = None,
                  rfp: Optional[list] = None,
                  roi: Optional[list] = None,
                  paths: Optional[list] = None,
                  gfp_regex: Optional[str] = '*488 SP 535-50*',
@@ -23,43 +56,15 @@
                  rfp_regex: Optional[str] = None,
                  roi_regex: Optional[str] = '*ROI*',
                  sigma: float = 2.0,
                  intercept0: bool = False,
                  expand: float = 10.0,
                  method: str = 'OLS'):
 
-        """
-
-        Class for performing SAIBR calibration
-
-        Two methods of specifying data
-        - input the images directly as a list for each channel along with a list of ROIs
-        - specify a list of paths and regular expressions for image files and ROIs (easier method if files are set up appropriately)
-
-        If rfp channel is not specified, will perform the normal two channel calibration
-
-        Args:
-            gfp: list of GFP channel images
-            af: list off AF channel images
-            rfp: list of RFP channel images
-            roi: list of ROIs
-            paths: list of paths containing n2 images
-            gfp_regex: regular expression found in gfp channel image files
-            af_regex: regular expression found in af channel image files
-            rfp_regex: regular expression found in rfp channel files (optional)
-            roi_regex: regular expression found in ROI files
-            sigma: gaussian blur to apply to images prior to regression
-            intercept0: if True, force intercept of regression to go through zero. Not recommended
-            expand: expand ROIs by this many pixels (useful to include a portion of background)
-            method: fitting method, either 'OLS' for ordinary least squares or 'ODR' for orthogonal distance regression
-
-        To run regression, initialise class and run()
-        SAIBR parameters will then be found at self.params
 
-        """
 
         # Global parameters
         self.sigma = sigma
         self.intercept0 = intercept0
         self.method = method
 
         # Import method 1: if channels are given as lists of images
```

### Comparing `saibr-0.1.4/saibr.egg-info/PKG-INFO` & `saibr-0.1.5/saibr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: saibr
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python implementation of SAIBR: a tool for performing spectral autofluorescence correction on biological images
 Home-page: https://github.com/goehringlab/saibr_python
 Author: Tom Bland
 Author-email: tom_bland@hotmail.co.uk
 License: CC BY 4.0
 Project-URL: Source Code, https://github.com/goehringlab/saibr_python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SAIBR (python implementation)
 
 [![CC BY 4.0][cc-by-shield]][cc-by]
 [![PyPi version](https://badgen.net/pypi/v/saibr/)](https://pypi.org/project/saibr)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/goehringlab/saibr_python/HEAD?filepath=%2Fscripts/SAIBRdemonstration.ipynb)
+[![Documentation Status](https://readthedocs.org/projects/saibr/badge/?version=latest)](https://saibr.readthedocs.io/en/latest/?badge=latest)
 
 
 Python implementation of SAIBR: a simple, platform independent protocol for spectral autofluorescence correction
 
 [Paper](https://journals.biologists.com/dev/article/149/14/dev200545/276004/SAIBR-a-simple-platform-independent-method-for)
 
 [FIJI plugin](https://github.com/goehringlab/saibr_fiji_plugin)
```

### Comparing `saibr-0.1.4/setup.py` & `saibr-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='saibr',
-    version='0.1.4',
+    version='0.1.5',
     license="CC BY 4.0",
     author='Tom Bland',
     author_email='tom_bland@hotmail.co.uk',
     packages=find_packages(),
     url='https://github.com/goehringlab/saibr_python',
     install_requires=['numpy',
                       'matplotlib',
```

