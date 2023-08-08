# Comparing `tmp/trianglechain-0.4.3.tar.gz` & `tmp/trianglechain-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trianglechain-0.4.3.tar", last modified: Wed Jul 12 12:14:31 2023, max compression
+gzip compressed data, was "trianglechain-0.5.0.tar", last modified: Tue Aug  8 12:16:43 2023, max compression
```

## Comparing `trianglechain-0.4.3.tar` & `trianglechain-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.481029 trianglechain-0.4.3/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-06-19 14:00:45.000000 trianglechain-0.4.3/AUTHORS.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-06-19 14:00:45.000000 trianglechain-0.4.3/CONTRIBUTING.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2034 2023-07-12 12:13:09.000000 trianglechain-0.4.3/HISTORY.rst
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-06-19 14:00:45.000000 trianglechain-0.4.3/LICENSE
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-06-19 14:00:45.000000 trianglechain-0.4.3/MANIFEST.in
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-07-12 12:14:31.481109 trianglechain-0.4.3/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1594 2023-06-19 14:00:45.000000 trianglechain-0.4.3/README.md
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      735 2023-06-19 14:00:45.000000 trianglechain-0.4.3/pyproject.toml
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1387 2023-07-12 12:14:31.481487 trianglechain-0.4.3/setup.cfg
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.472698 trianglechain-0.4.3/src/
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.477847 trianglechain-0.4.3/src/trianglechain/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     8714 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/BaseChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13478 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/LineChain.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    28284 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/TriangleChain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-07-12 12:13:52.000000 trianglechain-0.4.3/src/trianglechain/__init__.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13417 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9932 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/density_estimation.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7853 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16854 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/make_subplots.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4386 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/params.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-06-19 14:00:45.000000 trianglechain-0.4.3/src/trianglechain/utils_pj_hpd.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)    19766 2023-07-12 12:05:01.000000 trianglechain-0.4.3/src/trianglechain/utils_plots.py
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.479443 trianglechain-0.4.3/src/trianglechain.egg-info/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2427 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/PKG-INFO
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      809 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/SOURCES.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/dependency_links.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-19 14:01:00.000000 trianglechain-0.4.3/src/trianglechain.egg-info/not-zip-safe
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      310 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/requires.txt
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-07-12 12:14:31.000000 trianglechain-0.4.3/src/trianglechain.egg-info/top_level.txt
-drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-07-12 12:14:31.480821 trianglechain-0.4.3/tests/
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      674 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_bestfit.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2013 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_limits.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)      748 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_linechain.py
--rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2897 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_params.py
--rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     4006 2023-06-19 14:00:45.000000 trianglechain-0.4.3/tests/test_trianglechain.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-08-08 12:16:43.103596 trianglechain-0.5.0/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      201 2023-06-19 14:00:45.000000 trianglechain-0.5.0/AUTHORS.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1708 2023-06-19 14:00:45.000000 trianglechain-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2300 2023-08-08 12:03:53.000000 trianglechain-0.5.0/HISTORY.rst
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1116 2023-06-19 14:00:45.000000 trianglechain-0.5.0/LICENSE
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       99 2023-06-19 14:00:45.000000 trianglechain-0.5.0/MANIFEST.in
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2879 2023-08-08 12:16:43.103667 trianglechain-0.5.0/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2046 2023-08-07 21:05:41.000000 trianglechain-0.5.0/README.md
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      742 2023-08-07 21:05:41.000000 trianglechain-0.5.0/pyproject.toml
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1394 2023-08-08 12:16:43.104023 trianglechain-0.5.0/setup.cfg
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-08-08 12:16:43.098240 trianglechain-0.5.0/src/
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-08-08 12:16:43.101661 trianglechain-0.5.0/src/trianglechain/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13180 2023-08-07 21:05:41.000000 trianglechain-0.5.0/src/trianglechain/BaseChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    22995 2023-08-08 12:15:54.000000 trianglechain-0.5.0/src/trianglechain/LineChain.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)    37424 2023-08-08 12:15:54.000000 trianglechain-0.5.0/src/trianglechain/TriangleChain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      319 2023-08-08 12:04:01.000000 trianglechain-0.5.0/src/trianglechain/__init__.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    13310 2023-08-07 21:05:41.000000 trianglechain-0.5.0/src/trianglechain/bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     9930 2023-08-08 12:15:54.000000 trianglechain-0.5.0/src/trianglechain/density_estimation.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     7854 2023-08-07 21:05:41.000000 trianglechain-0.5.0/src/trianglechain/limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    16680 2023-08-08 12:15:54.000000 trianglechain-0.5.0/src/trianglechain/make_subplots.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     6729 2023-08-07 21:05:41.000000 trianglechain-0.5.0/src/trianglechain/params.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3024 2023-06-19 14:00:45.000000 trianglechain-0.5.0/src/trianglechain/utils_pj_hpd.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)    21339 2023-08-07 21:05:41.000000 trianglechain-0.5.0/src/trianglechain/utils_plots.py
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-08-08 12:16:43.102611 trianglechain-0.5.0/src/trianglechain.egg-info/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2879 2023-08-08 12:16:43.000000 trianglechain-0.5.0/src/trianglechain.egg-info/PKG-INFO
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      829 2023-08-08 12:16:43.000000 trianglechain-0.5.0/src/trianglechain.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-08-08 12:16:43.000000 trianglechain-0.5.0/src/trianglechain.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)        1 2023-06-19 14:01:00.000000 trianglechain-0.5.0/src/trianglechain.egg-info/not-zip-safe
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)      316 2023-08-08 12:16:43.000000 trianglechain-0.5.0/src/trianglechain.egg-info/requires.txt
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)       14 2023-08-08 12:16:43.000000 trianglechain-0.5.0/src/trianglechain.egg-info/top_level.txt
+drwxr-xr-x   0 silvanfischbacher   (501) staff       (20)        0 2023-08-08 12:16:43.103471 trianglechain-0.5.0/tests/
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     6907 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_bestfit.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     2961 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_limits.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     1954 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_linechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     3242 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_params.py
+-rwxr-xr-x   0 silvanfischbacher   (501) staff       (20)     9494 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_trianglechain.py
+-rw-r--r--   0 silvanfischbacher   (501) staff       (20)     4508 2023-08-08 12:15:54.000000 trianglechain-0.5.0/tests/test_utils.py
```

### Comparing `trianglechain-0.4.3/CONTRIBUTING.rst` & `trianglechain-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.3/LICENSE` & `trianglechain-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.3/PKG-INFO` & `trianglechain-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.3
+Version: 0.5.0
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -21,16 +21,19 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 trianglechain
 =============
 
 [![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/pipeline.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
-[![image](http://img.shields.io/badge/arXiv-2203.09616-orange.svg?style=flat)](https://arxiv.org/abs/2203.09616)
-[![image](http://img.shields.io/badge/arXiv-2207.01627-orange.svg?style=flat)](https://arxiv.org/abs/2207.01627)
+[![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/coverage.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
+[![Latest Release](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/badges/release.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/releases) 
+[![PyPI version](https://badge.fury.io/py/trianglechain.svg)](https://badge.fury.io/py/trianglechain)
+[![image](http://img.shields.io/badge/arXiv-2203.09616-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2203.09616)
+[![image](http://img.shields.io/badge/arXiv-2207.01627-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2207.01627)
 
 Code for plotting multidimensional marginal distributions. If you use it, please cite [arXiv-2203.09616](https://arxiv.org/abs/2203.09616) and [arXiv-2207.01627](https://arxiv.org/abs/2207.01627).
 
 [Source](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
 
 [Documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
@@ -51,15 +54,15 @@
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
 The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
-For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
+For more example plots, see the [documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
```

### Comparing `trianglechain-0.4.3/README.md` & `trianglechain-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 trianglechain
 =============
 
 [![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/pipeline.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
-[![image](http://img.shields.io/badge/arXiv-2203.09616-orange.svg?style=flat)](https://arxiv.org/abs/2203.09616)
-[![image](http://img.shields.io/badge/arXiv-2207.01627-orange.svg?style=flat)](https://arxiv.org/abs/2207.01627)
+[![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/coverage.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
+[![Latest Release](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/badges/release.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/releases) 
+[![PyPI version](https://badge.fury.io/py/trianglechain.svg)](https://badge.fury.io/py/trianglechain)
+[![image](http://img.shields.io/badge/arXiv-2203.09616-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2203.09616)
+[![image](http://img.shields.io/badge/arXiv-2207.01627-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2207.01627)
 
 Code for plotting multidimensional marginal distributions. If you use it, please cite [arXiv-2203.09616](https://arxiv.org/abs/2203.09616) and [arXiv-2207.01627](https://arxiv.org/abs/2207.01627).
 
 [Source](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
 
 [Documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
@@ -28,15 +31,15 @@
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
 The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
-For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
+For more example plots, see the [documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
```

### Comparing `trianglechain-0.4.3/pyproject.toml` & `trianglechain-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 testpaths = ["tests"]
 filterwarnings = ["ignore:invalid"]
 
 [tool.tox]
 legacy_tox_ini = '''
 [tox]
 isolated_build = true
-envlist = py38,py39,py10
+envlist = py38,py39,py310,py311
 setenv =
     PIP_EXTRA_INDEX_URL=https://cosmo-pypi.phys.ethz.ch/simple
     HTTP_PROXY=http://proxy.ethz.ch:3128
     HTTPS_PROXY=http://proxy.ethz.ch:3128
 
 [testenv]
 skip_install = false
```

### Comparing `trianglechain-0.4.3/setup.cfg` & `trianglechain-0.5.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -17,22 +17,23 @@
 	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 project_urls = 
 	Source = https://cosmo-docs.phys.ethz.ch/trianglechain
 
 [options]
 install_requires = 
-	numpy
+	arviz
+	cosmic_toolbox
+	KDEpy
 	matplotlib
+	numpy
+	pandas
 	scikit-learn
 	scipy
 	tqdm
-	arviz
-	pandas
-	cosmic_toolbox
 packages = find:
 package_dir = 
 	=src
 zip_safe = False
 python_requires = >=3.7
 
 [options.packages.find]
```

### Comparing `trianglechain-0.4.3/src/trianglechain/BaseChain.py` & `trianglechain-0.5.0/src/trianglechain/BaseChain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,147 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher, Tomasz Kacprzak
 
 
 from functools import partial
+
 import matplotlib.pyplot as plt
 
 
 class BaseChain:
-    def __init__(self, fig=None, size=4, **kwargs):
-        """
-        :param fig: matplotlib figure to use
-            default: None
-        :param size: figures size for a new figure, for a single panel.
-            All panels are square
-            default: 4
-        :param labels: labels for the parameters, default taken from columns
-            default: None
-        :param ranges: dictionary with ranges for parameters, keys correspond
-            to column names
-            default: {}
-        :param ticks: values for axis ticks, defaults taken from range with
-            equally spaced values
-            default: {}
-        :param n_ticks: number of ticks
-            default: 3
-        :param tick_length: length of the ticks
-            default: 3
-        :param n_bins: number of bins for 1d histograms
-            default: 100
-        :param fill: if to fill contours
-            default: False
-        :param grid: if to plot grid
-            default: False
-        :param add_empty_plots_like: sample with all parameters that should be
-            plotted, this should be used when plotting two data sets with
-            different numbers of parameters
-            default: None
-        :param label_fontsize: fontsize of labels in the legend and colorbar
-            default: 24
-        :param params: list of params that should be plotted, if all should be
-            plotted use "all"
-            default: "all"
-        :param normalize_prob1D: if 1D probability should be normalized
-            default: True
-        :param normalize_prob2D: if 2D probability should be normalized
-            default: True
-        :param orientation: orientation for LineChain, default: "horizontal"
-        :param density_estimation_method: method for density estimation with
-            options:
-                smoothing (default):
-                    first create a histogram of samples, and then smooth it
-                    with a Gaussian kernel corresponding to the variance of the
-                    20% of the smallest eigenvalue of the 2D distribution
-                    (smoothing scale can be adapted using the smoothing
-                    parameter in the de_kwargs)
-                gaussian_mixture:
-                    use Gaussian mixture to fit the 2D samples
-                median_filter:
-                    use median filter on the 2D histogram
-                kde:
-                    use TreeKDE, may be slow
-                hist:
-                    simple 2D histogram
-        :param line_space: space between lines in LineChain
-        :param de_kwargs: density estimation kwargs, dictionary with keys:
-            n_points:
-                number of bins for 2d histograms used to create contours, etc
-                default: n_bins
-            levels:
-                density levels for contours, the contours will enclose this
-                level of probability
-                default: [0.68, 0.95]
-            n_levels_check:
-                number of levels to check when looking for density levels
-                More levels is more accurate, but slower
-                default: 2000
-            smoothing_parameter1D:
-                smoothing scale for the 1D histograms
-                default: 0.1
-            smoothing_paramter2D:
-                smoothing scale for the 2D histograms
-                default: 0.2
-        :param grid_kwargs: kwargs for the plot grid, with keys:
-            fontsize_ticklabels:
-                font size for tick labels, default: 14
-            font_family:
-                font family for tick labels, default: sans-serif
-        :param hist_kwargs: kwargs for histograms, for plt.hist function
-        :param labels_kwargs: kwargs for xlabels and ylabels
-        :param line_kwargs: kwargs for all lines (plt.contour and plt.contourf)
-        :param scatter_kwargs: kwargs for plt.scatter
-        :param axvline_kwargs: kwargs for plt.axvline
-        :param subplots_kwargs: kwargs for plt.subplots()
-        :param grouping_kwargs: kwargs for grouping parameters in the plot with
-            options:
-                n_per_group: how many parameters are grouped together
-                    (e.g. (3, 4, 5) for grouping the parameters accordingly)
-                    default: None
-                empty_ratio: fraction of a whole plot that is left empty for
-                    separation
-                    default: 0.2
+    """
+    Base class to produce plots.
+    Parameters defined for this class are used for all plots that are added to the
+    figure. If you want to change the parameters for a specific plot, you can do so
+    by passing the parameters to the plotting function.
+
+    :param fig: matplotlib figure, default: None
+    :param size: size of the panels, default: 4
+    :param params: list of parameters to plot, default: "all"
+    :param params_from: sample or list of samples from which the parameters should
+        be taken, default: None
+    :param ranges: dictionary with the ranges for the parameters
+    :param names: list of names of the parameters, only used when input data is
+        unstructured array
+    :param labels: list of labels (e.g. latex style) for the parameters for the
+        plot
+    :param fill: if the contours should be filled, default: False
+    :param grid: if the grid should be plotted, default: False
+    :param tri: if upper or lower triangle should be plotted, default: "lower"
+    :param orientation: orientation for LineChain, default: "horizontal"
+    :param line_space: space between lines in LineChain, default: 0.5
+    :param plot_histograms_1D: if the 1D histograms should be plotted, default: True
+    :param n_ticks: number of ticks on the axes, default: 3
+    :param ticks: dict specifying the ticks for a parameter
+    :param tick_length: length of the ticks, default: 3
+    :param show_values: if best-fit and uncertainty should be given, default: False
+    :param bestfit_method: method for the best_fit,
+        options: "mode", "mean", "median", "best_sample" (requires lnprobs),
+        default: "mode"
+    :param levels_method: method to compute the uncertainty bands,
+        options: "hdi", "percentile", "PJ-HPD" (requires lnprobs),
+        default: "hdi"
+    :param credible_interval: credible interval for the uncertainty, default: 0.68
+    :param n_sigma_for_one_sided_tail: number of sigma for the one-sided tail,
+        default: 3
+    :param n_bins: number of bins for the 1D histograms, default: 100
+    :param density_estimation_method: method for density estimation. Available options:
+
+        - smoothing (default):
+            First create a histogram of samples and then smooth it with a Gaussian kernel
+            corresponding to the variance of the 20% of the smallest eigenvalue of the 2D distribution
+            (smoothing scale can be adapted using the smoothing parameter in de_kwargs).
+        - gaussian_mixture:
+            Use Gaussian mixture to fit the 2D samples.
+        - median_filter:
+            Use median filter on the 2D histogram.
+        - kde:
+            Use TreeKDE, may be slow.
+        - hist:
+            Simple 2D histogram.
+
+    :param cmap: colormap, default: "viridis"
+    :param colorbar: if a colorbar should be plotted, default: False
+    :param colorbar_label: label for the colorbar, default: None
+    :param colorbar_ax: axis for the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+    :param cmap_vmin: minimum value for the colormap, default: 0
+    :param cmap_vmax: maximum value for the colormap, default: None
+    :param show_legend: if a legend should be shown, default: False
+    :param progress_bar: if a progress bar should be shown, default: True
+    :param alpha1D: alpha for the 1D histograms, default: 1
+    :param alpha2D: alpha for the 2D histograms, default: 1
+    :param alpha: alpha for the 2D histograms in LineChain, if passed to TriangleChain,
+        overwrites the alpha1D and alpha2D value, default: 1
+    :param normalize_prob1D: if the 1D histograms should be normalized for
+        scatter_prob, default: True
+    :param normalize_prob2D: if the 2D histograms should be normalized for
+        scatter_prob, default: True
+    :param scatter_vline_1D: if a vertical line should be plotted in the 1D
+        histograms for each point when using scatter, default: False
+    :param alpha_for_low_density: if low density areas should fade to transparent
+    :param alpha_threshold: threshold from where the fading to transparent should
+        start, default: 0
+    :param n_points_scatter: number of points to use for scatter plots,
+        default: -1 (all)
+    :param label_fontsize: fontsize of the labels, default: 24
+    :param de_kwargs: density estimation kwargs, dictionary with keys:
+
+        - n_points:
+            number of bins for 2d histograms used to create contours etc., default: n_bins
+        - levels:
+            density levels for contours, the contours will enclose this
+            level of probability, default: [0.68, 0.95]
+        - n_levels_check:
+            number of levels to check when looking for density levels
+            More levels is more accurate, but slower, default: 2000
+        - smoothing_parameter1D:
+            smoothing scale for the 1D histograms, default: 0.1
+        - smoothing_parameter2D:
+            smoothing scale for the 2D histograms, default: 0.2
+
+    :param grid_kwargs: kwargs for the plot grid, with keys:
+
+        - fontsize_ticklabels:
+            font size for tick labels, default: 14
+        - font_family:
+            font family for tick labels, default: sans-serif
+
+    :param hist_kwargs: kwargs for the 1D histograms, passed to plt.hist function
+    :param labels_kwargs: kwargs for the x and y labels
+    :param line_kwargs: kwargs for the lines, passed to plt.contour and plt.contourf
+    :param scatter_kwargs: kwargs for the scatter plot, passed to plt.scatter
+    :param axvline_kwargs: kwargs for the vertical lines in the 1D histograms,
+        passed to plt.axvline
+    :param subplots_kwargs: kwargs for the subplots, passed to plt.subplots
+    :param grouping_kwargs: kwargs for grouping parameters in the plot with options:
+
+        - n_per_group:
+            how many parameters are grouped together (e.g. (3, 4, 5) for grouping the
+            parameters accordingly), default: None
+        - empty_ratio:
+            fraction of a whole plot that is left empty for separation, default: 0.2
 
-        Basic usage:
-        samples: numpy recarray containing the samples, with named columns
+    Basic usage::
 
         tri = TriangleChain()
-        tri.contour_cl(samples)  # plot contours at given confidence levels
-        tri.density_image(samples)  # plot PDF density image
-        tri.scatter(samples)  # simple scatter plot
-        tri.scatter_prob(samples)  # scatter plot
-                                   # with probability for each sample provided
-        tri.scatter_density(samples) # scatter plot
-                                     # color corresponds to probability
-        """
+        # plot contours at given confidence levels
+        tri.contour_cl(samples)
+        # plot PDF density image
+        tri.density_image(samples)
+        # simple scatter plot
+        tri.scatter(samples)
+        # scatter plot, with probability for each sample provided
+        tri.scatter_prob(samples, prob=prob)
+        # scatter plot, color corresponds to probability
+        tri.scatter_density(samples)
+
+    """
 
+    def __init__(self, fig=None, size=4, **kwargs):
         kwargs.setdefault("ticks", {})
         kwargs.setdefault("ranges", {})
         kwargs.setdefault("labels", None)
         kwargs.setdefault("n_bins", 100)
         kwargs.setdefault("de_kwargs", {})
         kwargs.setdefault("grid_kwargs", {})
         kwargs.setdefault("hist_kwargs", {})
@@ -132,19 +155,42 @@
         kwargs.setdefault("grid", False)
         kwargs.setdefault("scatter_kwargs", {})
         kwargs.setdefault("grouping_kwargs", {})
         kwargs.setdefault("subplots_kwargs", {})
         kwargs.setdefault("add_empty_plots_like", None)
         kwargs.setdefault("label_fontsize", 24)
         kwargs.setdefault("params", "all")
+        kwargs.setdefault("params_from", None)
+        kwargs.setdefault("names", None)
+        kwargs.setdefault("tri", "lower")
+        kwargs.setdefault("cmap", "viridis")
+        kwargs.setdefault("cmap_vmin", 0)
+        kwargs.setdefault("cmap_vmax", None)
+        kwargs.setdefault("colorbar", False)
+        kwargs.setdefault("colorbar_label", None)
+        kwargs.setdefault("colorbar_ax", [0.735, 0.5, 0.03, 0.25])
         kwargs.setdefault("line_space", 0.5)
         kwargs.setdefault("orientation", "horizontal")
         kwargs.setdefault("normalize_prob1D", True)
         kwargs.setdefault("normalize_prob2D", True)
         kwargs.setdefault("progress_bar", True)
+        kwargs.setdefault("plot_histograms_1D", True)
+        kwargs.setdefault("bestfit_method", "mode")
+        kwargs.setdefault("levels_method", "hdi")
+        kwargs.setdefault("show_values", False)
+        kwargs.setdefault("show_legend", False)
+        kwargs.setdefault("credible_interval", 0.68)
+        kwargs.setdefault("n_sigma_for_one_sided_tail", 3)
+        kwargs.setdefault("alpha1D", 1)
+        kwargs.setdefault("alpha2D", 1)
+        kwargs.setdefault("alpha", None)
+        kwargs.setdefault("alpha_for_low_density", False)
+        kwargs.setdefault("alpha_threshold", 0)
+        kwargs.setdefault("n_points_scatter", -1)
+        kwargs.setdefault("scatter_vline_1D", False)
         kwargs["de_kwargs"].setdefault("n_points", kwargs["n_bins"])
         kwargs["de_kwargs"].setdefault("levels", [0.68, 0.95])
         kwargs["de_kwargs"].setdefault("n_levels_check", 2000)
         kwargs["de_kwargs"].setdefault("smoothing_parameter1D", 0.1)
         kwargs["de_kwargs"].setdefault("smoothing_parameter2D", 0.2)
         kwargs["de_kwargs"]["levels"].sort()
         if kwargs["fill"]:
@@ -155,14 +201,15 @@
         kwargs["grid_kwargs"].setdefault("font_family", "sans-serif")
         kwargs["hist_kwargs"].setdefault("lw", 4)
         kwargs["labels_kwargs"].setdefault("fontsize", 24)
         kwargs["labels_kwargs"].setdefault("family", "sans-serif")
         kwargs["grouping_kwargs"].setdefault("n_per_group", None)
         kwargs["grouping_kwargs"].setdefault("empty_ratio", 0.2)
 
+        self._check_unexpected_kwargs(kwargs)
         self.fig = fig
         self.size = size
         self.kwargs = kwargs
         self.funcs = [
             "contour_cl",
             "density_image",
             "scatter",
@@ -199,7 +246,70 @@
             # find automatic next color
             pos_in_cycle = len(self.colors)
             colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
             self.colors.append(colors)
             return colors[pos_in_cycle % len(colors)]
         else:
             return color
+
+    def _check_unexpected_kwargs(self, kwargs):
+        """
+        Check for unexpected kwargs.
+
+        :param kwargs: kwargs to check
+        """
+        expected_kwargs = [
+            "ticks",
+            "ranges",
+            "labels",
+            "n_bins",
+            "de_kwargs",
+            "grid_kwargs",
+            "hist_kwargs",
+            "labels_kwargs",
+            "line_kwargs",
+            "axvline_kwargs",
+            "density_estimation_method",
+            "n_ticks",
+            "tick_length",
+            "fill",
+            "grid",
+            "scatter_kwargs",
+            "grouping_kwargs",
+            "subplots_kwargs",
+            "add_empty_plots_like",
+            "label_fontsize",
+            "params",
+            "params_from",
+            "names",
+            "tri",
+            "cmap",
+            "cmap_vmin",
+            "cmap_vmax",
+            "colorbar",
+            "colorbar_label",
+            "colorbar_ax",
+            "line_space",
+            "orientation",
+            "normalize_prob1D",
+            "normalize_prob2D",
+            "progress_bar",
+            "plot_histograms_1D",
+            "bestfit_method",
+            "levels_method",
+            "show_values",
+            "show_legend",
+            "credible_interval",
+            "n_sigma_for_one_sided_tail",
+            "alpha",
+            "alpha1D",
+            "alpha2D",
+            "alpha_for_low_density",
+            "alpha_threshold",
+            "n_points_scatter",
+            "scatter_vline_1D",
+        ]
+        unexpected_kwargs = set(kwargs.keys()) - set(expected_kwargs)
+        if len(unexpected_kwargs) > 0:
+            raise TypeError(
+                "Unexpected keyword argument: {}".format(unexpected_kwargs.pop())
+            )
```

### Comparing `trianglechain-0.4.3/src/trianglechain/LineChain.py` & `trianglechain-0.5.0/src/trianglechain/LineChain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,246 @@
 # Copyright (C) 2023 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher, Tomasz Kacprzak
 
+from copy import deepcopy
+
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
+from cosmic_toolbox import logger
+
+from trianglechain.BaseChain import BaseChain
+from trianglechain.make_subplots import contour_cl, density_image, scatter_density
+from trianglechain.params import ensure_rec
 from trianglechain.utils_plots import (
+    delete_all_ticks,
+    get_labels,
+    get_lines_and_labels,
+    get_n_points_for_scatter,
+    get_old_lims,
     prepare_columns,
-    update_current_ranges,
     set_limits,
-    get_old_lims,
+    update_current_ranges,
     update_current_ticks,
-    delete_all_ticks,
-    get_lines_and_labels,
-    get_labels,
-)
-from trianglechain.params import ensure_rec
-from trianglechain.make_subplots import (
-    contour_cl,
-    density_image,
-    scatter_density,
 )
-from trianglechain.BaseChain import BaseChain
+
+LOGGER = logger.get_logger(__file__)
 
 
 class LineChain(BaseChain):
     """
-    Class to produce line plots of chains
+    Class to produce line plots.
+    Parameters defined for this class are used for all plots that are added to the
+    figure. If you want to change the parameters for a specific plot, you can do so
+    by passing the parameters to the plotting function.
+
+    :param fig: matplotlib figure, default: None
+    :param size: size of the panels, if one number is given, the panels are rectangular
+        with the y axis being 70% of the x axis, if two numbers are given, the first
+        number is the width of the panels and the second number is the height of the
+        panels, default: 4
+    :param params: list of parameters to plot, default: "all"
+    :param params_from: sample or list of samples from which the parameters should
+        be taken, default: None
+    :param ranges: dictionary with the ranges for the parameters
+    :param names: list of names of the parameters, only used when input data is
+        unstructured array
+    :param labels: list of labels (e.g. latex style) for the parameters for the
+        plot
+    :param fill: if the contours should be filled, default: False
+    :param grid: if the grid should be plotted, default: False
+    :param n_ticks: number of ticks on the axes, default: 3
+    :param ticks: dict specifying the ticks for a parameter
+    :param tick_length: length of the ticks, default: 3
+    :param n_bins: number of bins for the 1D histograms, default: 100
+    :param density_estimation_method: method for density estimation. Available options:
+
+        - smoothing (default):
+            First create a histogram of samples and then smooth it with a Gaussian kernel
+            corresponding to the variance of the 20% of the smallest eigenvalue of the 2D distribution
+            (smoothing scale can be adapted using the smoothing parameter in de_kwargs).
+        - gaussian_mixture:
+            Use Gaussian mixture to fit the 2D samples.
+        - median_filter:
+            Use median filter on the 2D histogram.
+        - kde:
+            Use TreeKDE, may be slow.
+        - hist:
+            Simple 2D histogram.
+
+    :param cmap: colormap, default: "viridis"
+    :param colorbar: if a colorbar should be plotted, default: False
+    :param colorbar_label: label for the colorbar, default: None
+    :param colorbar_ax: axis for the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+    :param cmap_vmin: minimum value for the colormap, default: 0
+    :param cmap_vmax: maximum value for the colormap, default: None
+    :param show_legend: if a legend should be shown, default: False
+    :param alpha: alpha for the 2D histograms, default: 1
+    :param alpha_for_low_density: if low density areas should fade to transparent
+    :param alpha_threshold: threshold from where the fading to transparent should
+        start, default: 0
+    :param n_points_scatter: number of points to use for scatter plots,
+        default: -1 (all)
+    :param label_fontsize: fontsize of the labels, default: 24
+    :param de_kwargs: density estimation kwargs, dictionary with keys:
+
+        - n_points:
+            number of bins for 2d histograms used to create contours etc., default: n_bins
+        - levels:
+            density levels for contours, the contours will enclose this
+            level of probability, default: [0.68, 0.95]
+        - n_levels_check:
+            number of levels to check when looking for density levels
+            More levels is more accurate, but slower, default: 2000
+        - smoothing_parameter1D:
+            smoothing scale for the 1D histograms, default: 0.1
+        - smoothing_parameter2D:
+            smoothing scale for the 2D histograms, default: 0.2
+
+    :param grid_kwargs: kwargs for the plot grid, with keys:
+
+        - fontsize_ticklabels:
+            font size for tick labels, default: 14
+        - font_family:
+            font family for tick labels, default: sans-serif
+
+    :param labels_kwargs: kwargs for the x and y labels
+    :param line_kwargs: kwargs for the lines, passed to plt.contour and plt.contourf
+    :param scatter_kwargs: kwargs for the scatter plot, passed to plt.scatter
+    :param subplots_kwargs: kwargs for the subplots, passed to plt.subplots
+
+    Basic usage::
+
+        line = LineChain()
+        # plot contours at given confidence levels
+        line.contour_cl(samples)
+        # plot PDF density image
+        line.density_image(samples)
+        # simple scatter plot
+        line.scatter(samples)
+        # scatter plot, with probability for each sample provided
+        line.scatter_prob(samples, prob=prob)
+        # scatter plot, color corresponds to probability
+        line.scatter_density(samples)
+
     """
 
     def __init__(self, fig=None, size=4, **kwargs):
+        if "colorbar_ax" not in kwargs:
+            if "orientation" in kwargs:
+                if kwargs["orientation"] == "vertical":
+                    kwargs["colorbar_ax"] = [0.93, 0.1, 0.03, 0.3]
+                else:
+                    kwargs["colorbar_ax"] = [0.93, 0.1, 0.03, 0.8]
+            else:
+                kwargs["colorbar_ax"] = [0.93, 0.1, 0.03, 0.8]
         super().__init__(fig=fig, size=size, **kwargs)
 
         self.add_plotting_functions(self.add_plot)
 
     def add_plot(
         self,
         data,
         plottype,
         prob=None,
         color=None,
-        cmap=plt.cm.viridis,
+        label=None,
         **kwargs,
     ):
         """
-        Add a plot to the figure.
+        Plotting function for the line chain class. Parameters that are passed to
+        this function are overwriting the default parameters of the class.
+
+        :param data: data to plot, can be recarray, array, pandas dataframe or dict
+        :param prob: probability for each sample, default: None
+        :param color: color for the plot, default: None
+        :param label: label for the plot, default: None
+        :param names: list of names of the parameters, only used when input is
+            unstructured array
+        :param fill: if the contours should be filled, default: False
+        :param grid: if the grid should be plotted, default: False
+        :param n_bins: number of bins for the 1D histograms, default: 100
+        :param density_estimation_method: method for density estimation. Available
+            options:
+
+            - smoothing (default):
+                First create a histogram of samples and then smooth it with a Gaussian kernel
+                corresponding to the variance of the 20% of the smallest eigenvalue of the 2D distribution
+                (smoothing scale can be adapted using the smoothing parameter in de_kwargs).
+            - gaussian_mixture:
+                Use Gaussian mixture to fit the 2D samples.
+            - median_filter:
+                Use median filter on the 2D histogram.
+            - kde:
+                Use TreeKDE, may be slow.
+            - hist:
+                Simple 2D histogram.
+
+        :param cmap: colormap, default: "viridis"
+        :param colorbar: if a colorbar should be plotted, default: False
+        :param colorbar_label: label for the colorbar, default: None
+        :param colorbar_ax: axis for the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+        :param cmap_vmin: minimum value for the colormap, default: 0
+        :param cmap_vmax: maximum value for the colormap, default: None
+        :param show_legend: if a legend should be shown, default: False
+        :param alpha: alpha for the 2D histograms, default: 1
+        :param normalize_prob2D: if the 2D histograms should be normalized for
+            scatter_prob, default: True
+        :param alpha_for_low_density: if low density areas should fade to transparent
+        :param alpha_threshold: threshold from where the fading to transparent should
+            start, default: 0
+        :param n_points_scatter: number of points to use for scatter plots,
+            default: -1 (all)
+        :param de_kwargs: density estimation kwargs, dictionary with keys:
+
+            - n_points:
+                number of bins for 2d histograms used to create contours etc., default: n_bins
+            - levels:
+                density levels for contours, the contours will enclose this
+                level of probability, default: [0.68, 0.95]
+            - n_levels_check:
+                number of levels to check when looking for density levels
+                More levels is more accurate, but slower, default: 2000
+            - smoothing_parameter1D:
+                smoothing scale for the 1D histograms, default: 0.1
+            - smoothing_parameter2D:
+                smoothing scale for the 2D histograms, default: 0.2
+
+        :param grid_kwargs: kwargs for the plot grid, with keys:
+
+            - fontsize_ticklabels:
+                font size for tick labels, default: 14
+            - font_family:
+                font family for tick labels, default: sans-serif
+
+        :param labels_kwargs: kwargs for the x and y labels
+        :param line_kwargs: kwargs for the lines, passed to plt.contour and plt.contourf
+        :param scatter_kwargs: kwargs for the scatter plot, passed to plt.scatter
+        :param subplots_kwargs: kwargs for the subplots, passed to plt.subplots
         """
 
-        from copy import deepcopy
+        # check if all kwargs are valid trianglechain arguments
+        self._check_unexpected_kwargs(kwargs)
 
         kwargs_copy = deepcopy(self.kwargs)
         kwargs_copy.update(kwargs)
 
         if (plottype == "scatter_prob") & (prob is None):
             raise ValueError("prob needs to be defined for scatter_prob")
 
         color = self.setup_color(color)
         self.fig = plot_line_marginals(
             fig=self.fig,
             size=self.size,
             func=plottype,
-            cmap=cmap,
             data=data,
             prob=prob,
             color=color,
+            label=label,
             **kwargs_copy,
         )
 
         return self.fig
 
 
 def get_param_pairs(n_output):
@@ -83,51 +256,52 @@
             pairs += [[i, j]]
     return pairs
 
 
 def plot_line_marginals(
     data,
     prob=None,
-    params="all",
-    params_from=None,
-    names=None,
     func="contour_cl",
     orientation="horizontal",
     color="#0063B9",
+    label=None,
+    fig=None,
+    size=4,
+    line_space=0.5,
+    params="all",
+    params_from=None,
+    ranges={},
+    labels=None,
+    names=None,
+    fill=False,
+    grid=False,
+    n_ticks=3,
+    ticks={},
+    tick_length=3,
+    n_bins=100,
+    density_estimation_method="smoothing",
     cmap=plt.cm.viridis,
     cmap_vmin=0,
     cmap_vmax=None,
     colorbar=False,
     colorbar_label=None,
     colorbar_ax=[0.735, 0.5, 0.03, 0.25],
-    ranges={},
-    ticks={},
-    n_ticks=3,
-    tick_length=3,
-    n_bins=20,
-    fig=None,
-    size=4,
-    fill=True,
-    grid=False,
-    labels=None,
-    label=None,
-    label_fontsize=12,
     show_legend=False,
-    line_space=0.5,
-    density_estimation_method="smoothing",
     alpha=1,
+    normalize_prob2D=True,
     alpha_for_low_density=False,
     alpha_threshold=0,
-    subplots_kwargs={},
+    n_points_scatter=-1,
+    label_fontsize=24,
     de_kwargs={},
-    labels_kwargs={},
     grid_kwargs={},
+    labels_kwargs={},
     line_kwargs={},
     scatter_kwargs={},
-    normalize_prob2D=True,
+    subplots_kwargs={},
     **kwargs,
 ):
     """
     Plot line plots of chains.
 
     :param data: rec array, array, dict or pd dataframe
         data to plot
@@ -172,17 +346,20 @@
     :param subplots_kwargs: kwargs for plt.subplots, default: {}
     :param de_kwargs: kwargs for density estimation, default: {}
     :param labels_kwargs: kwargs for labels, default: {}
     :param grid_kwargs: kwargs for grid, default: {}
     :param line_kwargs: kwargs for line plots, default: {}
     :param scatter_kwargs: kwargs for scatter plots, default: {}
     :param normalize_prob2D: normalize probability for 2D plots, default: True
+    :param n_points_scatter: number of points for scatter plots, default: -1 (all)
     :param kwargs: additional kwargs for the plot function
     :return: fig, axes
     """
+    if alpha is None:
+        alpha = 1
     ###############################
     # prepare data and setup plot #
     ###############################
     data = ensure_rec(data, names=names)
     data, columns, _ = prepare_columns(
         data,
         params=params,
@@ -191,39 +368,49 @@
     # needed for plotting chains with different automatic limits
     current_ranges = {}
     current_ticks = {}
 
     labels = get_labels(labels, columns)
     n_dim = len(columns)
 
+    # Setup the probabilities for possible plots
     if prob is not None:
         if np.min(prob) < 0:
             prob_offset = -np.min(prob)
         else:
             prob_offset = 0
         if normalize_prob2D:
             prob2D = (prob + prob_offset) / np.sum(prob + prob_offset)
         else:
             # for example to plot an additional parameter in parameter space
             prob_label = prob
             prob2D = None
 
+    # Setup the figure orientation
     if orientation[0] == "h":
         n_rows = 1
         n_cols = (n_dim**2 - n_dim) // 2
     elif orientation[0] == "v":
         n_cols = 1
         n_rows = (n_dim**2 - n_dim) // 2
 
-    # Create figure if necessary and get axes
+    # Setup the figure size
+    if isinstance(size, (list, tuple)):
+        x_size = size[0]
+        y_size = size[1]
+    else:
+        x_size = size
+        y_size = size * 0.7
+
+    # Setup the figure
     if fig is None:
         fig, _ = plt.subplots(
             nrows=n_rows,
             ncols=n_cols,
-            figsize=(n_cols * size, n_rows * size * 0.7),
+            figsize=(n_cols * x_size, n_rows * y_size),
             **subplots_kwargs,
         )
         if orientation[0] == "h":
             fig.subplots_adjust(wspace=line_space)
         else:
             fig.subplots_adjust(hspace=line_space)
         ax = np.array(fig.get_axes()).ravel().reshape(n_rows, n_cols)
@@ -281,48 +468,56 @@
                 density_estimation_method=density_estimation_method,
                 label=label,
                 alpha_for_low_density=alpha_for_low_density,
                 alpha_threshold=alpha_threshold,
             )
 
         elif func == "scatter":
+            x, y = get_n_points_for_scatter(
+                data[columns[j]], data[columns[i]], n_points_scatter=n_points_scatter
+            )
             axc.scatter(
-                data[columns[j]],
-                data[columns[i]],
+                x,
+                y,
                 c=color,
                 label=label,
                 alpha=alpha,
                 **scatter_kwargs,
             )
 
         elif func == "scatter_prob":
             if normalize_prob2D:
                 _prob = prob2D
             else:
                 _prob = prob_label
+            x, y, _prob = get_n_points_for_scatter(
+                data[columns[j]],
+                data[columns[i]],
+                prob=_prob,
+                n_points_scatter=n_points_scatter,
+            )
             sorting = np.argsort(_prob)
             axc.scatter(
-                data[columns[j]][sorting],
-                data[columns[i]][sorting],
+                x[sorting],
+                y[sorting],
                 c=_prob[sorting],
                 label=label,
                 cmap=cmap,
                 **scatter_kwargs,
             )
 
         elif func == "scatter_density":
             scatter_density(
                 axc,
                 points1=data[columns[j]],
                 points2=data[columns[i]],
                 n_bins=n_bins,
                 lim1=current_ranges[columns[j]],
                 lim2=current_ranges[columns[i]],
-                norm_cols=False,
-                n_points_scatter=-1,
+                n_points_scatter=n_points_scatter,
                 cmap=cmap,
                 label=label,
             )
         set_limits(
             axc,
             ranges,
             current_ranges,
```

### Comparing `trianglechain-0.4.3/src/trianglechain/TriangleChain.py` & `trianglechain-0.5.0/src/trianglechain/TriangleChain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,327 +1,469 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
+from copy import deepcopy
+
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
-import matplotlib as mpl
+from cosmic_toolbox.logger import get_logger
+from tqdm.auto import tqdm, trange
+
+from trianglechain.BaseChain import BaseChain
+from trianglechain.make_subplots import (
+    contour_cl,
+    density_image,
+    plot_1d,
+    scatter_density,
+)
+from trianglechain.params import check_if_names_is_used_correctly, ensure_rec
 from trianglechain.utils_plots import (
-    prepare_columns,
-    setup_grouping,
-    get_labels,
+    add_vline,
+    delete_all_ticks,
+    find_alpha,
+    get_best_old_lims,
     get_hw_ratios,
+    get_labels,
+    get_lines_and_labels,
+    get_n_points_for_scatter,
+    get_old_lims,
+    prepare_columns,
+    set_limits,
     setup_figure,
+    setup_grouping,
     update_current_ranges,
     update_current_ticks,
-    set_limits,
-    delete_all_ticks,
-    add_vline,
-    get_old_lims,
-    get_best_old_lims,
-    find_alpha,
-    get_lines_and_labels,
-)
-from trianglechain.params import ensure_rec
-from trianglechain.make_subplots import (
-    contour_cl,
-    density_image,
-    scatter_density,
-    plot_1d,
 )
-from trianglechain.BaseChain import BaseChain
-from tqdm.auto import tqdm, trange
-
-from cosmic_toolbox.logger import get_logger
 
 LOGGER = get_logger(__file__)
 
 
 class TriangleChain(BaseChain):
     """
-    Class to produce triangle plots of chains.
+    Class to produce triangle plots.
+    Parameters defined for this class are used for all plots that are added to the
+    figure. If you want to change the parameters for a specific plot, you can do so
+    by passing the parameters to the plotting function.
+
+    :param fig: matplotlib figure, default: None
+    :param size: size of the panels, if one number is given, the panels are square,
+        if two numbers are given, the figure is rectangular, default: 4
+    :param params: list of parameters to plot, default: "all"
+    :param params_from: sample or list of samples from which the parameters should
+        be taken, default: None
+    :param ranges: dictionary with the ranges for the parameters
+    :param names: list of names of the parameters, only used when input data is
+        unstructured array
+    :param labels: list of labels (e.g. latex style) for the parameters for the
+        plot
+    :param fill: if the contours should be filled, default: False
+    :param grid: if the grid should be plotted, default: False
+    :param tri: if upper or lower triangle should be plotted, default: "lower"
+    :param plot_histograms_1D: if the 1D histograms should be plotted, default: True
+    :param n_ticks: number of ticks on the axes, default: 3
+    :param ticks: dict specifying the ticks for a parameter
+    :param tick_length: length of the ticks, default: 3
+    :param show_values: if best-fit and uncertainty should be given, default: False
+    :param bestfit_method: method for the best_fit,
+        options: "mode", "mean", "median", "best_sample" (requires lnprobs),
+        default: "mode"
+    :param levels_method: method to compute the uncertainty bands,
+        options: "hdi", "percentile", "PJ-HPD" (requires lnprobs),
+        default: "hdi"
+    :param credible_interval: credible interval for the uncertainty, default: 0.68
+    :param n_sigma_for_one_sided_tail: number of sigma for the one-sided tail,
+        default: 3
+    :param n_bins: number of bins for the 1D histograms, default: 100
+    :param density_estimation_method: method for density estimation. Available options:
+
+        - smoothing (default):
+            First create a histogram of samples and then smooth it with a Gaussian kernel
+            corresponding to the variance of the 20% of the smallest eigenvalue of the 2D distribution
+            (smoothing scale can be adapted using the smoothing parameter in de_kwargs).
+        - gaussian_mixture:
+            Use Gaussian mixture to fit the 2D samples.
+        - median_filter:
+            Use median filter on the 2D histogram.
+        - kde:
+            Use TreeKDE, may be slow.
+        - hist:
+            Simple 2D histogram.
+
+    :param cmap: colormap, default: "viridis"
+    :param colorbar: if a colorbar should be plotted, default: False
+    :param colorbar_label: label for the colorbar, default: None
+    :param colorbar_ax: axis for the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+    :param cmap_vmin: minimum value for the colormap, default: 0
+    :param cmap_vmax: maximum value for the colormap, default: None
+    :param show_legend: if a legend should be shown, default: False
+    :param progress_bar: if a progress bar should be shown, default: True
+    :param alpha: alpha for the plots, overwrite alpha1D and alpha2D, default: None
+    :param alpha1D: alpha for the 1D histograms, default: 1
+    :param alpha2D: alpha for the 2D histograms, default: 1
+    :param normalize_prob1D: if the 1D histograms should be normalized for
+        scatter_prob, default: True
+    :param normalize_prob2D: if the 2D histograms should be normalized for
+        scatter_prob, default: True
+    :param scatter_vline_1D: if a vertical line should be plotted in the 1D
+        histograms for each point when using scatter, default: False
+    :param alpha_for_low_density: if low density areas should fade to transparent
+    :param alpha_threshold: threshold from where the fading to transparent should
+        start, default: 0
+    :param n_points_scatter: number of points to use for scatter plots,
+        default: -1 (all)
+    :param label_fontsize: fontsize of the labels, default: 24
+    :param de_kwargs: density estimation kwargs, dictionary with keys:
+
+        - n_points:
+            number of bins for 2d histograms used to create contours etc., default: n_bins
+        - levels:
+            density levels for contours, the contours will enclose this
+            level of probability, default: [0.68, 0.95]
+        - n_levels_check:
+            number of levels to check when looking for density levels
+            More levels is more accurate, but slower, default: 2000
+        - smoothing_parameter1D:
+            smoothing scale for the 1D histograms, default: 0.1
+        - smoothing_parameter2D:
+            smoothing scale for the 2D histograms, default: 0.2
+
+    :param grid_kwargs: kwargs for the plot grid, with keys:
+
+        - fontsize_ticklabels:
+            font size for tick labels, default: 14
+        - font_family:
+            font family for tick labels, default: sans-serif
+
+    :param hist_kwargs: kwargs for the 1D histograms, passed to plt.hist function
+    :param labels_kwargs: kwargs for the x and y labels
+    :param line_kwargs: kwargs for the lines, passed to plt.contour and plt.contourf
+    :param scatter_kwargs: kwargs for the scatter plot, passed to plt.scatter
+    :param axvline_kwargs: kwargs for the vertical lines in the 1D histograms,
+        passed to plt.axvline
+    :param subplots_kwargs: kwargs for the subplots, passed to plt.subplots
+    :param grouping_kwargs: kwargs for grouping parameters in the plot with options:
+
+        - n_per_group:
+            how many parameters are grouped together (e.g. (3, 4, 5) for grouping the
+            parameters accordingly), default: None
+        - empty_ratio:
+            fraction of a whole plot that is left empty for separation, default: 0.2
+
+    Basic usage::
+
+        tri = TriangleChain()
+        # plot contours at given confidence levels
+        tri.contour_cl(samples)
+        # plot PDF density image
+        tri.density_image(samples)
+        # simple scatter plot
+        tri.scatter(samples)
+        # scatter plot, with probability for each sample provided
+        tri.scatter_prob(samples, prob=prob)
+        # scatter plot, color corresponds to probability
+        tri.scatter_density(samples)
+
     """
 
     def __init__(self, fig=None, size=4, **kwargs):
         super().__init__(fig=fig, size=size, **kwargs)
 
         self.add_plotting_functions(self.add_plot)
 
     def add_plot(
         self,
         data,
         plottype,
         prob=None,
         color=None,
-        cmap=plt.cm.viridis,
-        tri="lower",
-        plot_histograms_1D=True,
+        label=None,
+        lnprobs=None,
         **kwargs,
     ):
         """
-        :param data: rec array
-            the data that should be plotted with column data
-        :param plottype: {"contour_cl", "density_image", "scatter",
-            "scatter_density", "scatter_prob"}
-            type of plot that should be plotted
-        :param prob: None or array
-            if not None, then probability attached to the samples,
-            in that case samples are treated as grid not a chain
+        Plotting function for the triangle chain class. Parameters that are passed to
+        this function are overwriting the default parameters of the class.
+
+        :param data: data to plot, can be recarray, array, pandas dataframe or dict
+        :param prob: probability for each sample, default: None
+        :param color: color for the plot, default: None
+        :param label: label for the plot, default: None
+        :param lnprobs: lnprob for each sample (used for some best-fit methods),
             default: None
-        :param color: matplotlib color
-            color of the plot, default=None (automatic)
-        :param cmap: matplotlib colormap
-            colormap used for this plot, default="viridis"
-        :param tri: {"lower", "upper"}
-            if triangle should be in the upper or lower part, default="lower"
-        :param plot_histograms_1D: boolean
-            if the 1D histograms should be plotted as well, default=True
-        :param kwargs: additional arguments for the plotting functions, they include:
-        :param cmap_vmin: fixed minimum in the colormap, default: 0
-        :param cmap_vmax: fixed maximum of the colormap, default: None
-        :param colorbar: if colorbar should be plotted, default: False
-        :param colorbar_label: label of the colorbar, default: None
-        :param colorbar_ax: position of colorbar
-            default: [0.735, 0.5, 0.03, 0.25]
-        :param show_values: if best-fit and uncertainty should be plotted
-            default: False
-        :param bestfit_method: method for the best_fit
-            options: "mode", "mean", "median", "best_sample",
+        :param names: list of names of the parameters, only used when input is
+            unstructured array
+        :param fill: if the contours should be filled, default: False
+        :param grid: if the grid should be plotted, default: False
+        :param tri: if upper or lower triangle should be plotted, default: "lower"
+        :param plot_histograms_1D: if 1D histograms should be plotted, default: True
+        :param show_values: if best-fit and uncertainty should be given, default: False
+        :param bestfit_method: method for the best_fit,
+            options: "mode", "mean", "median", "best_sample" (requires lnprobs),
             default: "mode"
-        :param levels_method: method to compute the uncertainty bands
-            options: "hdi", "percentile", "PJ-HPD"
+        :param levels_method: method to compute the uncertainty bands, default:
+            options: "hdi", "percentile", "PJ-HPD" (requires lnprobs),
             default: "hdi"
-        :param credible_interval: credible interval for the uncertainty
-            default: 0.68
-        :param lnprobs: lnprobs, only needed for best_sample and PJ-HPD
-        :param scatter_vline_1D: if the scattered points should generate a
-            vertical line in the 1D histograms, default: False
-        :param label: label of the plot (for legend), default: None
-        :param alpha1D: alpha value for the 1D plot, default: 1
-        :param alpha2D: alpha value for the 2D plot, default: 1
-        :param alpha_for_low_density: if to use alpha for very low density in
-            density images. If True, alpha is 0 at the lowest density and
-            linearly increases until the defined threshold
-            default: False
-        :param alpha_threshold: threshold density where alpha value should
-            be 1 again
-            default: 0
-        :param show_legend: if legend should be shown, default: False
+        :param credible_interval: credible interval for the uncertainty, default: 0.68
+        :param n_sigma_for_one_sided_tail: number of sigma for the one-sided tail,
+            default: 3
+        :param n_bins: number of bins for the 1D histograms, default: 100
+        :param density_estimation_method: method for density estimation. Available
+            options:
+
+            - smoothing (default):
+                First create a histogram of samples and then smooth it with a Gaussian kernel
+                corresponding to the variance of the 20% of the smallest eigenvalue of the 2D distribution
+                (smoothing scale can be adapted using the smoothing parameter in de_kwargs).
+            - gaussian_mixture:
+                Use Gaussian mixture to fit the 2D samples.
+            - median_filter:
+                Use median filter on the 2D histogram.
+            - kde:
+                Use TreeKDE, may be slow.
+            - hist:
+                Simple 2D histogram.
+
+        :param cmap: colormap, default: "viridis"
+        :param colorbar: if a colorbar should be plotted, default: False
+        :param colorbar_label: label for the colorbar, default: None
+        :param colorbar_ax: axis for the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+        :param cmap_vmin: minimum value for the colormap, default: 0
+        :param cmap_vmax: maximum value for the colormap, default: None
+        :param show_legend: if a legend should be shown, default: False
+        :param progress_bar: if a progress bar should be shown, default: True
+        :param alpha: alpha for the plots, overwrite alpha1D and alpha2D, default: None
+        :param alpha1D: alpha for the 1D histograms, default: 1
+        :param alpha2D: alpha for the 2D histograms, default: 1
+        :param normalize_prob1D: if the 1D histograms should be normalized for
+            scatter_prob, default: True
+        :param normalize_prob2D: if the 2D histograms should be normalized for
+            scatter_prob, default: True
+        :param scatter_vline_1D: if a vertical line should be plotted in the 1D
+            histograms for each point when using scatter, default: False
+        :param alpha_for_low_density: if low density areas should fade to transparent
+        :param alpha_threshold: threshold from where the fading to transparent should
+            start, default: 0
+        :param n_points_scatter: number of points to use for scatter plots,
+            default: -1 (all)
+        :param de_kwargs: density estimation kwargs, dictionary with keys:
+
+            - n_points:
+                number of bins for 2d histograms used to create contours etc., default: n_bins
+            - levels:
+                density levels for contours, the contours will enclose this
+                level of probability, default: [0.68, 0.95]
+            - n_levels_check:
+                number of levels to check when looking for density levels
+                More levels is more accurate, but slower, default: 2000
+            - smoothing_parameter1D:
+                smoothing scale for the 1D histograms, default: 0.1
+            - smoothing_parameter2D:
+                smoothing scale for the 2D histograms, default: 0.2
+
+        :param grid_kwargs: kwargs for the plot grid, with keys:
+
+            - fontsize_ticklabels:
+                font size for tick labels, default: 14
+            - font_family:
+                font family for tick labels, default: sans-serif
+
+        :param hist_kwargs: kwargs for the 1D histograms, passed to plt.hist function
+        :param labels_kwargs: kwargs for the x and y labels
+        :param line_kwargs: kwargs for the lines, passed to plt.contour and plt.contourf
+        :param scatter_kwargs: kwargs for the scatter plot, passed to plt.scatter
+        :param axvline_kwargs: kwargs for the vertical lines in the 1D histograms,
+            passed to plt.axvline
+        :param subplots_kwargs: kwargs for the subplots, passed to plt.subplots
+        :param grouping_kwargs: kwargs for grouping parameters in the plot with options:
+
+            - n_per_group:
+                how many parameters are grouped together (e.g. (3, 4, 5) for grouping the
+                parameters accordingly), default: None
+            - empty_ratio:
+                fraction of a whole plot that is left empty for separation, default: 0.2
+
         """
 
-        from copy import deepcopy
+        # check if all kwargs are valid trianglechain arguments
+        self._check_unexpected_kwargs(kwargs)
 
+        # enrich kwargs with the values from the class
         kwargs_copy = deepcopy(self.kwargs)
         kwargs_copy.update(kwargs)
 
+        # get the color from color cycle if not defined
         color = self.setup_color(color)
+
         if (plottype == "scatter_prob") & (prob is None):
             raise ValueError("prob needs to be defined for scatter_prob")
 
         self.fig, self.ax = plot_triangle_marginals(
             fig=self.fig,
             size=self.size,
             func=plottype,
-            cmap=cmap,
             data=data,
             prob=prob,
-            tri=tri,
             color=color,
-            plot_histograms_1D=plot_histograms_1D,
+            label=label,
+            lnprobs=lnprobs,
             **kwargs_copy,
         )
         return self.fig, self.ax
 
 
 def plot_triangle_marginals(
     data,
     prob=None,
-    params="all",
-    params_from=None,
-    names=None,
     func="contour_cl",
-    tri="lower",
-    single_tri=True,
     color="#0063B9",
-    cmap=plt.cm.viridis,
-    cmap_vmin=0,
-    cmap_vmax=None,
-    ranges={},
-    ticks={},
-    n_bins=20,
+    label=None,
+    lnprobs=None,
     fig=None,
     size=4,
-    fill=True,
-    grid=False,
+    params="all",
+    params_from=None,
+    ranges={},
     labels=None,
+    names=None,
+    fill=False,
+    grid=False,
+    tri="lower",
     plot_histograms_1D=True,
+    n_ticks=3,
+    ticks={},
+    tick_length=3,
     show_values=False,
     bestfit_method="mode",
     levels_method="hdi",
     credible_interval=0.68,
     n_sigma_for_one_sided_tail=3,
-    lnprobs=None,
-    scatter_vline_1D=False,
-    label=None,
+    n_bins=100,
     density_estimation_method="smoothing",
-    n_ticks=3,
-    tick_length=3,
+    cmap=plt.cm.viridis,
+    cmap_vmin=0,
+    cmap_vmax=None,
+    colorbar=False,
+    colorbar_label=None,
+    colorbar_ax=[0.735, 0.5, 0.03, 0.25],
+    show_legend=False,
+    progress_bar=True,
+    alpha=None,
     alpha1D=1,
     alpha2D=1,
+    normalize_prob1D=True,
+    normalize_prob2D=True,
+    scatter_vline_1D=False,
     alpha_for_low_density=False,
     alpha_threshold=0,
-    subplots_kwargs={},
+    n_points_scatter=-1,
+    label_fontsize=24,
     de_kwargs={},
+    grid_kwargs={},
     hist_kwargs={},
-    line_kwargs={},
     labels_kwargs={},
-    grid_kwargs={},
+    line_kwargs={},
     scatter_kwargs={},
-    grouping_kwargs={},
     axvline_kwargs={},
+    subplots_kwargs={},
+    grouping_kwargs={},
     add_empty_plots_like=None,
-    label_fontsize=12,
-    show_legend=False,
-    colorbar=False,
-    colorbar_label=None,
-    colorbar_ax=[0.735, 0.5, 0.03, 0.25],
-    normalize_prob1D=True,
-    normalize_prob2D=True,
-    progress_bar=True,
     **kwargs,
 ):
     """
-    Plot a triangle plot with marginal distributions.
+    Plot triangle plot with 1D and 2D histograms, contours, scatter plots, etc.
 
-    :param data: rec array
-        the data that should be plotted with column data
-    :param prob: None or array
-        probability attached to the samples, if None, then the density is estimated
-        from the samples, default: None
-    :param params: list of strings
-        list of parameters that should be plotted, default: "all"
-    :param params_from: data like array
-        if params is "all", then the parameters are taken from this array
+    :param data: data to plot, can be a dictionary, a recarray or a pandas DataFrame
+    :param prob: probability of each point, default: None
+    :param func: function to use for plotting, default: 'contour_cl', options:
+
+        - contour_cl (default)
+        - density_image
+        - scatter_density
+        - scatter_prob
+        - scatter default
+
+    :param color: color for the plot, default: '#0063B9'
+    :param label: label for the plot, default: None
+    :param lnprobs: lnprob for each sample (used for some best-fit methods),
         default: None
-    :param names: list
-        list of names for the parameters in case data is np.ndarray, default: None
-    :param func: string
-        function that should be used for plotting,
-        options: "contour_cl", "density_image", "scatter", "scatter_prob", "scatter_density"
-        default: "contour_cl"
-    :param tri: string
-        if the upper or lower triangle should be plotted
-        options: "upper", "lower", default: "lower"
-    :param single_tri: bool
-        if only one triangle should be plotted, default: True
-    :param color: string
-        color of the plot, default: "#0063B9"
-    :param cmap: matplotlib colormap
-        colormap for the density plots, default: plt.cm.viridis
-    :param cmap_vmin: float
-        minimum value for the colormap, default: 0
-    :param cmap_vmax: float
-        maximum value for the colormap, default: None
-    :param ranges: dict
-        dictionary with ranges for the parameters, default: {}
-    :param ticks: dict
-        dictionary with ticks for the parameters, default: {}
-    :param n_bins: int
-        number of bins for the histograms, default: 20
-    :param fig: matplotlib figure
-        figure that should be used for plotting, default: None
-    :param size: float
-        size of the plot, default: 4
-    :param fill: bool
-        if the contours should be filled, default: True
-    :param grid: bool
-        if the grid should be plotted, default: False
-    :param labels: list of strings
-        labels for the parameters, default: None
-    :param plot_histograms_1D: bool
-        if the 1D histograms should be plotted, default: True
-    :param show_values: bool
-        if the values should be shown in the 1D histograms, default: False
-    :param bestfit_method: string
-        method that should be used for the bestfit value
-        options: "mode", "median", "mean", default: "mode"
-    :param levels_method: string
-        method that should be used for the levels
-        options: "hdi", "credible_interval", default: "hdi"
-    :param credible_interval: float
-        credible interval for the levels, default: 0.68
-    :param n_sigma_for_one_sided_tail: how many sigma should be used to decide if one
-        tailed credible interval should be used
-        defaults to 3
-    :param lnprobs: None or array
-        log probabilities attached to the samples for the level estimation,
-        default: None
-    :param scatter_vline_1D: bool
-        if a vertical line should be plotted at the scatter points in the 1D histograms,
-        default: False
-    :param label: string
-        label for the legend, default: None
-    :param density_estimation_method: method to use for density estimation
-        options: smoothing, histo, kde, gaussian_mixture, median_filter
-        default: smoothing
-    :param n_ticks: int
-        number of ticks for the axes, default: 3
-    :param tick_length: float
-        length of the ticks, default: 3
-    :param alpha1D: float
-        alpha value for the 1D histograms, default: 1
-    :param alpha2D: float
-        alpha value for the 2D histograms, default: 1
-    :param alpha_for_low_density: bool
-        if the alpha value should be adjusted for low density regions, default: False
-    :param alpha_threshold: float
-        threshold for the alpha value, default: 0
-    :param subplots_kwargs: dict
-        keyword arguments for the subplots function, default: {}
-    :param de_kwargs: dict
-        keyword arguments for the density estimation, default: {}
-    :param hist_kwargs: dict
-        keyword arguments for the histogram, default: {}
-    :param line_kwargs: dict
-        keyword arguments for the lines, default: {}
-    :param labels_kwargs: dict
-        keyword arguments for the labels, default: {}
-    :param grid_kwargs: dict
-        keyword arguments for the grid, default: {}
-    :param scatter_kwargs: dict
-        keyword arguments for the scatter plot, default: {}
-    :param grouping_kwargs: dict
-        keyword arguments for the grouping, default: {}
-    :param axvline_kwargs: dict
-        keyword arguments for the vertical lines, default: {}
-    :param add_empty_plots_like: string
-        DEPRECATED, default: None
-    :param label_fontsize: int
-        fontsize for the labels, default: 12
-    :param show_legend: bool
-        if the legend should be shown, default: False
-    :param colorbar: bool
-        if the colorbar should be shown, default: False
-    :param colorbar_label: string
-        label for the colorbar, default: None
-    :param colorbar_ax: list
-        position of the colorbar, default: [0.735, 0.5, 0.03, 0.25]
-    :param normalize_prob1D: bool
-        if the 1D probability should be normalized, default: True
-    :param normalize_prob2D: bool
-        if the 2D probability should be normalized, default: True
-    :param progress_bar: bool
-        if a progress bar should be shown, default: True
+    :param fig: matplotlib figure, default: None
+    :param size: size of the panels, if one number is given, the panels are square,
+        if two numbers are given, the figure is rectangular, default: 4
+    :param params: list of parameters to plot, default: 'all'
+    :param params_from: sample or list of samples from which the parameters should
+        be taken, default: None
+    :param ranges: dictionary with ranges for the parameters, default: {}
+    :param labels: list of labels (e.g. latex style) for the parameters for the
+        plot
+    :param names: list of names of the parameters, only used when input data is
+        unstructured array
+    :param fill: if the contours should be filled, default: False
+    :param grid: if the grid should be plotted, default: False
+    :param tri: if upper or lower triangle should be plotted, default: "lower"
+    :param plot_histograms_1D: if the 1D histograms should be plotted, default: True
+    :param n_ticks: number of ticks on the axes, default: 3
+    :param ticks: dict specifying the ticks for each parameter
+    :param tick_length: length of the ticks, default: 3
+    :param show_values: if best-fit and uncertainty should be given, default: False
+    :param bestfit_method: method to use for best-fit,
+        options: "mode", "mean", "median", "best_sample" (requires lnprobs),
+        default: "mode"
+    :param levels_method: method to compute the uncertainty bands,
+        options: "hdi", "percentile", "PJ-HPD" (requires lnprobs),
+        default: "hdi"
+    :param credible_interval: credible interval for the uncertainty bands, default: 0.68
+    :param n_sigma_for_one_sided_tail: number of sigma for the one-sided tail,
+        default: 3
+    :param n_bins: number of bins for the 1D histograms, default: 100
+    :param density_estimation_method: method to use for density estimation,
+        default="smoothing"
+    :param cmap: colormap, default: plt.cm.viridis
+    :param cmap_vmin: minimum value for the colormap, default: 0
+    :param cmap_vmax: maximum value for the colormap, default: None
+    :param colorbar: if a colorbar should be plotted, default: False
+    :param colorbar_label: label for the colorbar, default: None
+    :param colorbar_ax: position of the colorbar, default: [0.735, 0.5, 0.03, 0.25]
+    :param show_legend: if a legend should be plotted, default: False
+    :param progress_bar: if a progress bar should be shown, default: True
+    :param alpha: alpha for the plots, overwrite alpha1D and alpha2D, default: None
+    :param alpha1D: alpha for the 1D histograms, default: 1
+    :param alpha2D: alpha for the 2D histograms, default: 1
+    :param normalize_prob1D: if the 1D histograms should be normalized for scatter_prob,
+        default: True
+    :param normalize_prob2D: if the 2D histograms should be normalized for scatter_prob,
+        default: True
+    :param scatter_vline_1D: if a vertical line should be plotted in the 1D
+        histograms for each point when using scatter, default: False
+    :param alpha_for_low_density: if low density areas should fade to transparent
+    :param alpha_threshold: threshold for the alpha for low density areas
+    :param alpha_threshold: threshold from where the fading to transparent should
+        start, default: 0
+    :param n_points_scatter: number of points to plot when using scatter,
+        default: -1 (all)
+    :param label_fontsize: fontsize for the labels, default: 24
+    :param de_kwargs: dict with kwargs for the density estimation, default: {}
+    :param grid_kwargs: dict with kwargs for the grid, default: {}
+    :param hist_kwargs: dict with kwargs for the 1D histograms, default: {}
+    :param labels_kwargs: dict with kwargs for the labels, default: {}
+    :param line_kwargs: dict with kwargs for the lines, default: {}
+    :param scatter_kwargs: dict with kwargs for the scatter plot, default: {}
+    :param axvline_kwargs: dict with kwargs for the vertical lines, default: {}
+    :param subplots_kwargs: dict with kwargs for the subplots, default: {}
+    :param grouping_kwargs: dict with kwargs for the grouping, default: {}
+    :param add_empty_plots_like: DEPRECATED, default: None
     """
 
-    if (names is not None) and (not isinstance(data, np.ndarray)):
-        LOGGER.warning(
-            "The names argument is only used if data is a numpy array. "
-            "Probably you want to use the params argument instead."
-        )
+    check_if_names_is_used_correctly(names, data)
+
+    # overwrite alpha1D and alpha2D if alpha is given
+    if alpha is not None:
+        alpha1D = alpha
+        alpha2D = alpha
 
     ###############################
     # prepare data and setup plot #
     ###############################
     data = ensure_rec(data, names=names)
     data, columns, empty_columns = prepare_columns(
         data,
@@ -335,19 +477,16 @@
 
     # setup everything that grouping works properly
     columns, grouping_indices = setup_grouping(columns, grouping_kwargs)
     labels = get_labels(labels, columns, grouping_indices)
     hw_ratios = get_hw_ratios(columns, grouping_kwargs)
 
     n_dim = len(columns)
-    if single_tri:
-        n_box = n_dim
-    else:
-        n_box = n_dim + 1
 
+    # setup figure
     if prob is not None:
         if np.min(prob) < 0:
             prob_offset = -np.min(prob)
         else:
             prob_offset = 0
         if normalize_prob1D:
             prob1D = (prob + prob_offset) / np.sum(prob + prob_offset)
@@ -356,28 +495,28 @@
 
         if normalize_prob2D:
             prob2D = (prob + prob_offset) / np.sum(prob + prob_offset)
         else:
             # for example to plot an additional parameter in parameter space
             prob_label = prob
             prob2D = None
-
     else:
         prob1D = None
         prob2D = None
 
+    # Setup triangle (lower or upper)
     if tri[0] == "l":
         tri_indices = np.tril_indices(n_dim, k=-1)
     elif tri[0] == "u":
         tri_indices = np.triu_indices(n_dim, k=1)
     else:
-        raise Exception("tri={} should be either lower or upper".format(tri))
+        raise ValueError("tri must be 'lower' or 'upper', not {}".format(tri))
 
     # Create figure if necessary and get axes
-    fig, ax, old_tri = setup_figure(fig, n_box, hw_ratios, size, subplots_kwargs)
+    fig, ax, old_tri = setup_figure(fig, n_dim, hw_ratios, size, subplots_kwargs)
     if old_tri is not None and old_tri != tri:
         double_tri = True
     else:
         double_tri = False
     # get ranges for each parameter (if not specified, max/min of data is used)
     update_current_ranges(current_ranges, ranges, columns, data)
 
@@ -392,24 +531,18 @@
     if len(color) == len(data):
         color_hist = "k"
     else:
         color_hist = color
 
     def get_current_ax(ax, tri, i, j):
         if tri[0] == "u":
-            if single_tri:
-                axc = ax[i, j]
-            else:
-                axc = ax[i, j + 1]
-        elif tri[0] == "l":
-            if single_tri:
-                axc = ax[i, j]
-            else:
-                axc = ax[i + 1, j]
-
+            axc = ax[i, j]
+        else:
+            # lower triangle
+            axc = ax[i, j]
         if i == j and not plot_histograms_1D and not scatter_vline_1D:
             # in this case axis should not be turned on in this call
             pass
         else:
             # turn on ax sinces it is used
             axc.axis("on")
         return axc
@@ -518,17 +651,22 @@
                     prob=prob,
                     density_estimation_method=density_estimation_method,
                     label=label,
                     alpha_for_low_density=alpha_for_low_density,
                     alpha_threshold=alpha_threshold,
                 )
             elif func == "scatter":
-                axc.scatter(
+                x, y = get_n_points_for_scatter(
                     data[columns[j]],
                     data[columns[i]],
+                    n_points_scatter=n_points_scatter,
+                )
+                axc.scatter(
+                    x,
+                    y,
                     c=color,
                     label=label,
                     alpha=min(
                         (
                             find_alpha(columns[i], empty_columns, alpha2D),
                             find_alpha(columns[j], empty_columns, alpha2D),
                         )
@@ -536,33 +674,38 @@
                     **scatter_kwargs,
                 )
             elif func == "scatter_prob":
                 if normalize_prob2D:
                     _prob = prob2D
                 else:
                     _prob = prob_label
+                x, y, _prob = get_n_points_for_scatter(
+                    data[columns[j]],
+                    data[columns[i]],
+                    prob=prob,
+                    n_points_scatter=n_points_scatter,
+                )
                 sorting = np.argsort(_prob)
                 axc.scatter(
-                    data[columns[j]][sorting],
-                    data[columns[i]][sorting],
+                    x[sorting],
+                    y[sorting],
                     c=_prob[sorting],
                     label=label,
                     cmap=cmap,
                     **scatter_kwargs,
                 )
             elif func == "scatter_density":
                 scatter_density(
                     axc,
                     points1=data[columns[j]],
                     points2=data[columns[i]],
                     n_bins=n_bins,
                     lim1=current_ranges[columns[j]],
                     lim2=current_ranges[columns[i]],
-                    norm_cols=False,
-                    n_points_scatter=-1,
+                    n_points_scatter=n_points_scatter,
                     cmap=cmap,
                     label=label,
                     **scatter_kwargs,
                 )
             set_limits(
                 axc,
                 ranges,
```

### Comparing `trianglechain-0.4.3/src/trianglechain/bestfit.py` & `trianglechain-0.5.0/src/trianglechain/bestfit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher
 
 import numpy as np
+from cosmic_toolbox import logger
 from scipy.optimize import minimize
 from scipy.stats import gaussian_kde
 from tqdm.auto import trange
-from cosmic_toolbox import logger
 
 LOGGER = logger.get_logger(__name__)
 
 
 def get_bestfit(samples, lnprobs=None, bestfit_method="mode"):
     """
     Get the best fit value each parameter of the sample.
@@ -101,15 +101,15 @@
     :param inv_C: inverse covariance matrix
     :param ells: ell values
     :param lims: limits of the parameters
     :param prior_ind: indices of the parameters with a gaussian prior
     :param gauss_mean: mean of the gaussian prior
     :param gauss_sigma: sigma of the gaussian prior
     :param use_best_n: number of best samples to use for the minimization
-    :return: best likelihood value
+    :return: bool if successful minimization, best likelihood value and best lnprob
     """
     if use_best_n == 1:
         bl = params_chain[np.argmax(lnprobs)]
     else:
         sorted_indices = np.unique(-lnprobs, return_index=True)[1][:use_best_n]
         bl = params_chain[sorted_indices]
 
@@ -147,14 +147,15 @@
             for i, p in enumerate(params_chain.dtype.names):
                 best_l[p] = res.x[i]
             return True, best_l, -res.fun
         else:
             best_l[0] = params_chain[np.argmax(lnprobs)]
             return False, best_l, np.max(lnprobs)
     else:
+        success = True
         best_l = np.empty(use_best_n, dtype=params_chain.dtype)
         for ii in trange(use_best_n):
             x0 = np.zeros(len(bl[ii]))
             for i, p in enumerate(bl[ii]):
                 x0[i] = p
             res = minimize(
                 chi2,
@@ -162,16 +163,17 @@
                 args=(cl_fid, inv_C, ells, lims),
                 method="Nelder-Mead",
             )  # options={'maxiter':5000})
             if res.success:
                 for i, p in enumerate(params_chain.dtype.names):
                     best_l[ii][p] = res.x[i]
             else:
+                success = False
                 best_l[ii] = params_chain[np.argmax(lnprobs)]
-        return True, get_mode(best_l, lims), np.max(lnprobs)
+        return success, get_means_and_medians(best_l)[1], np.max(lnprobs)
 
 
 def get_best_likelihood_from_MCMC(params_chain, lnprobs):
     """
     Get the best likelihood value of the chain by maximizing the log probability.
 
     :param params_chain: rec array with samples
@@ -187,22 +189,20 @@
     """
     Get the mode of a sample.
 
     :param sample: 1D array with samples
     :param lim: limits of the parameter
     :return: mode of the sample
     """
-    x = np.linspace(lim[0], lim[1], 100)
+    x = np.linspace(lim[0], lim[1])
     kde = gaussian_kde(sample)
     func = lambda x: -kde(x)  # noqa
     res = minimize(func, x[np.argmax(kde(x))])
-    if -res.fun > np.max(kde(x)):
-        return res.x[0]
-    else:
-        return x[np.argmax(kde(x))]
+    assert -res.fun >= np.max(kde(x)), "Finding mode failed"
+    return res.x[0]
 
 
 def get_mode(samples, lims):
     """
     Get the mode of the sample for each parameter.
 
     :param samples: rec array with samples
@@ -231,15 +231,14 @@
 
 def get_all_bl_estimates(
     params_chain,
     lnprobs,
     emu,
     cl_fid,
     inv_C,
-    n_bin,
     ells,
     lims,
     prior_ind=[],
     gauss_mean=[],
     gauss_sigma=[],
     just_names=False,
     use_best_n=1,
@@ -247,18 +246,17 @@
     flat_chi2minimization=False,
 ):
     """
     Get all the best likelihood estimates.
 
     :param params_chain: rec array with samples
     :param lnprobs: array with log probabilities of the samples
-    :param emu: emulator
+    :param emu: emulator (or any function that returns the observable)
     :param cl_fid: fiducial power spectrum
     :param inv_C: inverse covariance matrix
-    :param n_bin: number of tomographic bins
     :param ells: array with multipoles
     :param lims: limits of the parameters
     :param prior_ind: indices of the parameters with priors
     :param gauss_mean: mean of the Gaussian priors
     :param gauss_sigma: standard deviation of the Gaussian priors
     :param just_names: if True, only return the names of the best likelihood estimates
     :param use_best_n: number of best likelihood samples to use
@@ -299,15 +297,14 @@
         bl.append(
             get_best_likelihood(
                 params_chain,
                 lnprobs,
                 emu,
                 cl_fid,
                 inv_C,
-                n_bin,
                 ells,
                 lims,
                 prior_ind,
                 gauss_mean,
                 gauss_sigma,
                 use_best_n=1,
             )[1]
@@ -315,15 +312,14 @@
     bl.append(
         get_best_likelihood(
             params_chain,
             lnprobs,
             emu,
             cl_fid,
             inv_C,
-            n_bin,
             ells,
             lims,
             prior_ind,
             gauss_mean,
             gauss_sigma,
             use_best_n=use_best_n,
         )[1]
@@ -332,30 +328,28 @@
         bl.append(
             get_best_likelihood(
                 params_chain,
                 lnprobs,
                 emu,
                 cl_fid,
                 inv_C,
-                n_bin,
                 ells,
                 lims,
                 prior_ind=[],
             )[1]
         )
     return bl, names
 
 
 def get_all_bl_estimates_except_mode(
     params_chain,
     lnprobs,
     emu,
     cl_fid,
     inv_C,
-    n_bin,
     ells,
     lims,
     prior_ind=[],
     gauss_mean=[],
     gauss_sigma=[],
     just_names=False,
     use_best_n=1,
@@ -366,15 +360,14 @@
     Get all the best likelihood estimates except the mode.
 
     :param params_chain: rec array with samples
     :param lnprobs: array with log probabilities of the samples
     :param emu: emulator
     :param cl_fid: fiducial power spectrum
     :param inv_C: inverse covariance matrix
-    :param n_bin: number of tomographic bins
     :param ells: array with multipoles
     :param lims: limits of the parameters
     :param prior_ind: indices of the parameters with priors
     :param gauss_mean: mean of the Gaussian priors
     :param gauss_sigma: standard deviation of the Gaussian priors
     :param just_names: if True, only return the names of the best likelihood estimates
     :param use_best_n: number of best likelihood samples to use
@@ -412,15 +405,14 @@
         bl.append(
             get_best_likelihood(
                 params_chain,
                 lnprobs,
                 emu,
                 cl_fid,
                 inv_C,
-                n_bin,
                 ells,
                 lims,
                 prior_ind,
                 gauss_mean,
                 gauss_sigma,
                 use_best_n=1,
             )[1]
@@ -428,15 +420,14 @@
     bl.append(
         get_best_likelihood(
             params_chain,
             lnprobs,
             emu,
             cl_fid,
             inv_C,
-            n_bin,
             ells,
             lims,
             prior_ind,
             gauss_mean,
             gauss_sigma,
             use_best_n=use_best_n,
         )[1]
@@ -445,14 +436,13 @@
         bl.append(
             get_best_likelihood(
                 params_chain,
                 lnprobs,
                 emu,
                 cl_fid,
                 inv_C,
-                n_bin,
                 ells,
                 lims,
                 prior_ind=[],
             )[1]
         )
     return bl, names
```

### Comparing `trianglechain-0.4.3/src/trianglechain/density_estimation.py` & `trianglechain-0.5.0/src/trianglechain/density_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
 
 import numpy as np
 import scipy
+
 from trianglechain.utils_plots import (
-    safe_normalise,
+    get_smoothing_sigma,
     normalise,
     pixel_coords,
-    get_smoothing_sigma,
+    safe_normalise,
 )
 
 
 def get_density_grid_1D(
     data,
     binedges,
     bincenters,
@@ -48,45 +49,42 @@
             ind = np.random.choice(
                 a=len(prob), size=10000, p=safe_normalise(prob), replace=True
             )
             data_ = data[ind][:, np.newaxis]
         else:
             data_ = data[:, np.newaxis]
 
-        from cosmic_toolbox.TransformedGaussianMixture import (
-            TransformedGaussianMixture,
-        )
+        from cosmic_toolbox.TransformedGaussianMixture import TransformedGaussianMixture
 
         clf = TransformedGaussianMixture(
             param_bounds=[lims], n_components=20, covariance_type="full"
         )
         clf.fit(data_)
         logL = clf.score_samples(bincenters[:, np.newaxis])
 
         de = np.exp(logL - np.max(logL))
         de = normalise(de, bincenters)
 
     elif method == "smoothing":
-        from scipy import signal
-        from scipy import ndimage
+        from scipy import ndimage, signal
 
         prob1D = histogram_1D(data=data, prob=prob, binedges=binedges)
         data_pixel = pixel_coords(
             data, [[binedges[0], binedges[-1]]], n_pix_img=len(bincenters)
         )
         if prob is not None:
             ind = np.random.choice(prob.shape[0], p=prob, size=1000)
             data_pixel = data_pixel[0, ind]
 
         sig_pix = (
             get_smoothing_sigma(data_pixel, prob1D.shape[0])
             * de_kwargs["smoothing_parameter1D"]
         )
         n_pix = max(3, int(np.ceil(sig_pix * 10)))  # 10 sigma smoothing
-        kernel = signal.gaussian(n_pix, sig_pix)
+        kernel = signal.windows.gaussian(n_pix, sig_pix)
         de = scipy.ndimage.convolve(prob1D, kernel, mode="reflect")
         de = normalise(de, bincenters)
 
         # de = np.convolve(a=prob1D, v=np.ones(5), mode='same')
         # de = signal.convolve2d(prob2d, kernel, mode='same', boundary='wrap')
 
     elif method == "median_filter":
@@ -94,15 +92,19 @@
 
         prob1D = histogram_1D(data=data, prob=prob, binedges=binedges)
         de = ndimage.median_filter(prob1D, int(prob1D.shape[0] / 10))
 
     elif method == "kde":
         from KDEpy import TreeKDE
 
-        de = TreeKDE(kernel="gaussian", bw="ISJ").fit(data).evaluate(bincenters)
+        de = (
+            TreeKDE(kernel="gaussian", bw="ISJ")
+            .fit(data, weights=prob)
+            .evaluate(bincenters)
+        )
 
     elif method == "hist":
         de = histogram_1D(data=data, prob=prob, binedges=binedges)
 
     else:
         raise Exception("unknown density estimation method {}".format(method))
 
@@ -172,17 +174,15 @@
             ind = np.random.choice(
                 a=len(prob), size=10000, p=safe_normalise(prob), replace=True
             )
             data_panel = data_panel[:, ind]
 
         bounds = [ranges[columns[j]], ranges[columns[i]]]
 
-        from cosmic_toolbox.TransformedGaussianMixture import (
-            TransformedGaussianMixture,
-        )
+        from cosmic_toolbox.TransformedGaussianMixture import TransformedGaussianMixture
 
         clf = TransformedGaussianMixture(
             param_bounds=bounds, n_components=10, covariance_type="full"
         )
         clf.fit(data_panel.T)
         logL = clf.score_samples(gridpoints.T)
```

### Comparing `trianglechain-0.4.3/src/trianglechain/limits.py` & `trianglechain-0.5.0/src/trianglechain/limits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher
 
 
-import numpy as np
 import arviz
+import numpy as np
+from cosmic_toolbox.logger import get_logger
 from scipy.stats import norm
+
 from trianglechain import utils_pj_hpd
-from cosmic_toolbox.logger import get_logger
 
 LOGGER = get_logger(__file__)
 
 
 def get_levels(
     samples, lnprob=None, levels_method="hdi", credible_interval=0.68, sigma_one_tail=3
 ):
```

### Comparing `trianglechain-0.4.3/src/trianglechain/make_subplots.py` & `trianglechain-0.5.0/src/trianglechain/make_subplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
+import warnings
+
+import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib.colors import ListedColormap
+from scipy.interpolate import griddata
+
 from trianglechain.density_estimation import (
+    get_confidence_levels,
     get_density_grid_1D,
     get_density_grid_2D,
-    get_confidence_levels,
 )
 from trianglechain.utils_plots import (
-    get_old_lims,
+    compute_plot_limits,
     find_alpha,
-    get_values,
     get_best_lims,
-    compute_plot_limits,
+    get_old_lims,
+    get_values,
 )
-from matplotlib.colors import ListedColormap
-import matplotlib
-import warnings
 
 
 def plot_1d(
     axc,
     column,
     param_label,
     data,
@@ -455,15 +458,14 @@
 def scatter_density(
     axc,
     points1,
     points2,
     n_bins=50,
     lim1=None,
     lim2=None,
-    norm_cols=False,
     n_points_scatter=-1,
     label=None,
     **kwargs,
 ):
     """
     Plot the density of the data in the given axis as a scatter plot. The color of
     the scatter points is determined by the density of the points.
@@ -476,16 +478,14 @@
         array of the second parameter
     :param n_bins: int
         number of bins
     :param lim1: tuple
         limits of the first parameter
     :param lim2: tuple
         limits of the second parameter
-    :param norm_cols: bool
-        if the columns should be normalized
     :param n_points_scatter: int
         number of points to plot
     :param label: str
         label of the plot
     :param kwargs: dict
         dict with kwargs for the scatter plot
     """
@@ -504,22 +504,17 @@
         max2 = lim2[1]
 
     bins_edges1 = np.linspace(min1, max1, n_bins)
     bins_edges2 = np.linspace(min2, max2, n_bins)
 
     hv, _, _ = np.histogram2d(points1, points2, bins=[bins_edges1, bins_edges2])
 
-    if norm_cols is True:
-        hv = hv / np.sum(hv, axis=0)[:, np.newaxis]
-
     bins_centers1 = (bins_edges1 - (bins_edges1[1] - bins_edges1[0]) / 2)[1:]
     bins_centers2 = (bins_edges2 - (bins_edges2[1] - bins_edges2[0]) / 2)[1:]
 
-    from scipy.interpolate import griddata
-
     select_box = (
         (points1 < max1) & (points1 > min1) & (points2 < max2) & (points2 > min2)
     )
     points1_box, points2_box = points1[select_box], points2[select_box]
 
     x1, x2 = np.meshgrid(bins_centers1, bins_centers2)
     points = np.concatenate(
```

### Comparing `trianglechain-0.4.3/src/trianglechain/params.py` & `trianglechain-0.5.0/src/trianglechain/params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Copyright (C) 2023 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
 import numpy as np
 import pandas as pd
 from cosmic_toolbox import arraytools as at
+from cosmic_toolbox import logger
+
+LOGGER = logger.get_logger(__file__)
 
 
 def ensure_rec(data, names=None, column_prefix=""):
     """
     Ensure that the input data is a numpy record array (recarray).
     If the input is already a recarray, it is returned as-is.
     If it is a 2D numpy array, a pandas dataframe, or a dictionary of arrays,
@@ -121,7 +124,71 @@
     # Add new column to data
     data = at.add_cols(data, [new_param])
 
     # Set values of new column to the derived value
     data[new_param] = derived
 
     return data
+
+
+def check_if_names_is_used_correctly(names, data):
+    """
+    Check if the names argument is used correctly.
+
+    :param names: A list of field names to use if the input data is a 2D numpy array.
+    :param data: The input data to check.
+    :return: corrected names
+    """
+
+    is_ndarray = isinstance(data, np.ndarray) and not isinstance(data, np.recarray)
+    if (names is not None) and (not is_ndarray):
+        LOGGER.warning(
+            "The names argument is only used if data is a non-structured numpy array. "
+            "Probably you want to use the params argument instead. "
+            "The names argument will be ignored."
+        )
+        names = None
+    return names
+
+
+def get_samples(
+    n_samples=100000,
+    n_dims=None,
+    names=None,
+    column_prefix="col",
+    covmat=None,
+    mean=None,
+):
+    """
+    Get a random set of samples from a multivariate Gaussian distribution.
+
+    :param n_samples: The number of samples to generate.
+    :param n_dims: The number of dimensions of the samples.
+    :param names: A list of field names to use if the input data is a 2D numpy array.
+        The length of this list should match the number of columns in the array.
+        If not provided, field names will be automatically generated.
+    :param column_prefix: A prefix to add to the automatically generated field names
+        for the input data.
+    :param covmat: The covariance matrix of the distribution.
+    :param mean: The mean of of each parameter in the distribution.
+    :return: The samples.
+    """
+    # Get dimension from default or from input data
+    if n_dims is None:
+        if (names is None) & (covmat is None) & (mean is None):
+            n_dims = 4
+        else:
+            if names is not None:
+                n_dims = len(names)
+            elif mean is not None:
+                n_dims = len(mean)
+            else:
+                n_dims = np.shape(covmat)[0]
+
+    if covmat is None:
+        covmat = np.random.normal(size=(n_dims, n_dims))
+        covmat = np.dot(covmat.T, covmat)
+    if mean is None:
+        mean = np.random.uniform(size=(n_dims))
+    samples = np.random.multivariate_normal(mean=mean, cov=covmat, size=(n_samples))
+    samples = ensure_rec(samples, names, column_prefix)
+    return samples
```

### Comparing `trianglechain-0.4.3/src/trianglechain/utils_pj_hpd.py` & `trianglechain-0.5.0/src/trianglechain/utils_pj_hpd.py`

 * *Files identical despite different names*

### Comparing `trianglechain-0.4.3/src/trianglechain/utils_plots.py` & `trianglechain-0.5.0/src/trianglechain/utils_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Tomasz Kacprzak, Silvan Fischbacher
 
-import numpy as np
 import math
-from scipy.stats import median_abs_deviation
-from sklearn.decomposition import PCA
+
 import matplotlib.pyplot as plt
-from matplotlib.ticker import FormatStrFormatter
-from trianglechain import limits, bestfit
-from trianglechain.params import ensure_rec
+import numpy as np
 from cosmic_toolbox import arraytools as at
 from cosmic_toolbox import logger
+from matplotlib.ticker import FormatStrFormatter
+from scipy.stats import median_abs_deviation
+from sklearn.decomposition import PCA
 
+from trianglechain import bestfit, limits
+from trianglechain.params import ensure_rec
 
 LOGGER = logger.get_logger(__file__)
 
 
 def prepare_columns(data, params="all", params_from=None, add_empty_plots_like=None):
     """
     Prepare the columns of the data to be plotted.
@@ -29,15 +30,15 @@
     :param add_empty_plots_like: DEPRECATED: data to get the parameters from.
     :return: The data with only the columns to be plotted, the list of column names
         and the list of empty columns.
     """
     empty_columns = []
     if params_from is not None:
         par = []
-        if not (isinstance(params_from, list) or isinstance(params_from, np.ndarray)):
+        if not isinstance(params_from, (list, tuple)):
             # make a list out of single samples
             params_from = [params_from]
 
         for p in params_from:
             # add all the parameters of the samples
             par.append(ensure_rec(p).dtype.names)
         if params == "all":
@@ -161,33 +162,41 @@
     :param fig: The figure to be used.
     :param n_box: The number of boxes.
     :param hw_ratios: The height/width ratios.
     :param size: The size of the figure.
     :param subplots_kwargs: The keyword arguments for the subplots.
     :return: The figure and the axes.
     """
+    # Setup the figure size
+    if isinstance(size, (list, tuple)):
+        x_size = size[0]
+        y_size = size[1]
+    else:
+        x_size = size
+        y_size = size
+
     if fig is None:
         fig, _ = plt.subplots(
             nrows=n_box,
             ncols=n_box,
-            figsize=(sum(hw_ratios) * size, sum(hw_ratios) * size),
+            figsize=(sum(hw_ratios) * x_size, sum(hw_ratios) * y_size),
             gridspec_kw={
                 "height_ratios": hw_ratios,
                 "width_ratios": hw_ratios,
             },
             **subplots_kwargs,
         )
         ax = np.array(fig.get_axes()).reshape(n_box, n_box)
         for axc in ax.ravel():
             # remove all unused axs
             axc.axis("off")
         old_tri = None
     else:
         ax = np.array(fig.get_axes())
-        if len(ax) != n_box * n_box:
+        while len(ax) != n_box * n_box:
             # remove colorbar from before
             ax = ax[:-1]
         ax = ax.reshape(n_box, n_box)
         old_tri = check_orientation(ax)
     return fig, ax, old_tri
 
 
@@ -325,50 +334,51 @@
         bf = bestfit.get_bestfit(data[column], lnprobs, bestfit_method)
         uncertainty = (upper - lower) / 2
         rounding_digit, frmt = get_rounding_digit(uncertainty)
         str_bf = f"{frmt}".format(np.around(bf, rounding_digit))
 
         if np.around(bf - lower, rounding_digit) < 0:
             # special case where the bestfit is not in the interval
-            low = f"{frmt}".format(np.around(bf - lower, rounding_digit))
+            low = f"+{frmt}".format(abs(np.around(bf - lower, rounding_digit)))
         else:
-            # take abs for the special case -0.
             low = f"-{frmt}".format(abs(np.around(bf - lower, rounding_digit)))
 
         if np.around(upper - bf, rounding_digit) < 0:
             # special case where the bestfit is not in the interval
-            up = f"{frmt}".format(np.around(upper - bf, rounding_digit))
+            up = f"-{frmt}".format(abs(np.around(upper - bf, rounding_digit)))
         else:
-            # take abs for the special case -0.
             up = f"+{frmt}".format(abs(np.around(upper - bf, rounding_digit)))
 
         return two_tail, str_bf, up, low
     else:
         uncertainty_estimate = np.std(data[column])
         rounding_digit, frmt = get_rounding_digit(uncertainty_estimate)
         return two_tail, side, f"{frmt}".format(np.around(lim, rounding_digit)), None
 
 
 def get_rounding_digit(uncertainty):
     """
-    Get the rounding digit and the format.
+    Get the rounding digit and the format from PDG conventions.
 
     :param uncertainty: The uncertainty.
     :return: The rounding digit and the format.
     """
     first_significant_digit = math.floor(np.log10(uncertainty))
     u = round_to_significant_digits(uncertainty, 3) * 10 ** (
         -first_significant_digit + 2
     )
     if u > 100 and u < 354:
         significant_digits_to_round = 2
     elif u < 949:
         significant_digits_to_round = 1
     else:
-        significant_digits_to_round = 2
+        # technically, u should be rounded up to 1000 and two significant digits
+        # should be used, but keeping u as is and using one significant digit
+        # is more equivalent to that.
+        significant_digits_to_round = 1
     uncertainty = 1000 / 10 ** (-first_significant_digit + 2)
     rounding_digit = -(math.floor(np.log10(uncertainty)) - significant_digits_to_round)
     if rounding_digit > 0:
         frmt = "{{:.{}f}}".format(rounding_digit)
     else:
         frmt = "{:.0f}"
     return rounding_digit, frmt
@@ -437,49 +447,65 @@
     :param n_ticks: The number of ticks.
     :return: The ticks.
     """
     diff = range_of_param[1] - range_of_param[0]
     ticks = np.zeros(n_ticks)
 
     # mathematical center and tick interval
-    diff_range = diff / (n_ticks + 1)
+    tick_interval = diff / (n_ticks + 1)
     center = range_of_param[0] + diff / 2
 
     # first significant digit for rounding
-    significant_digit = math.floor(np.log10(diff_range))
+    significant_digit = math.floor(np.log10(tick_interval))
 
     for i in range(10 * n_ticks):
         rounded_center = np.around(center, -significant_digit + i)
-        if abs(rounded_center - center) / diff_range < 0.05:
+        if abs(rounded_center - center) / tick_interval < 0.05:
             break
     for i in range(10 * n_ticks):
-        rounded_diff_range = np.around(diff_range, -significant_digit)
-        start = rounded_center - (n_ticks - 1) / 2 * rounded_diff_range
-        for i in range(n_ticks):
-            if n_ticks % 2 == 0:
-                ticks[i] = np.around(
-                    start + i * rounded_diff_range, -significant_digit + 1
+        # determine tick_interval when rounding to significant digit
+        rounded_tick_interval = np.around(tick_interval, -significant_digit)
+        start = np.around(
+            rounded_center - (n_ticks - 1) / 2 * rounded_tick_interval,
+            -significant_digit,
+        )
+
+        for j in range(n_ticks):
+            if n_ticks % 2 != 0:
+                ticks[j] = np.around(
+                    start + j * rounded_tick_interval, -significant_digit
                 )
             else:
-                ticks[i] = np.around(start + i * rounded_diff_range, -significant_digit)
+                ticks[j] = np.around(
+                    start + j * rounded_tick_interval, -significant_digit + 1
+                )
+
         # check if ticks are inside parameter space and
         # not too close to each other
         if (
             (ticks[0] < range_of_param[0])
             or (ticks[-1] > range_of_param[1])
-            or ((ticks[0] - range_of_param[0]) > 1.2 * rounded_diff_range)
-            or ((range_of_param[1] - ticks[-1]) > 1.2 * rounded_diff_range)
+            or ((ticks[0] - range_of_param[0]) > 1.2 * rounded_tick_interval)
+            or ((range_of_param[1] - ticks[-1]) > 1.2 * rounded_tick_interval)
         ):
             significant_digit -= 1
         else:
             break
-    if significant_digit == math.floor(np.log10(diff_range)) - 10 * n_ticks:
+    if (
+        significant_digit == math.floor(np.log10(tick_interval)) - 10 * n_ticks
+    ):  # pragma: no cover
+        LOGGER.warning(
+            "Could not find optimal ticks, please report this to the developer."
+        )
+        LOGGER.warning("Send the following information:")
+        LOGGER.warning(f"range_of_param: {range_of_param}, n_ticks: {n_ticks}")
+        LOGGER.warning("to silvanf@phys.ethz")
         for i in range(n_ticks):
-            start = center - (n_ticks - 1) / 2 * diff_range
-            ticks[i] = np.around(start + i * diff_range, -significant_digit)
+            start = center - (n_ticks - 1) / 2 * tick_interval
+            ticks[i] = np.around(start + i * tick_interval, -significant_digit)
     return ticks
 
 
 def get_best_lims(new_xlims, new_ylims, old_xlims, old_ylims):
     """
     Get the best limits for the axes.
 
@@ -636,7 +662,31 @@
     """
     min_x = np.nanmin(x)
     max_x = np.nanmax(x)
     diff_x = max_x - min_x
     min_x -= diff_x * margin
     max_x += diff_x * margin
     return min_x, max_x
+
+
+def get_n_points_for_scatter(x, y, n_points_scatter=-1, prob=None):
+    """
+    Get the number of points to use for the scatter plot.
+
+    :param x: The x data.
+    :param y: The y data.
+    :param n_points_scatter: The number of points to use for the scatter plot.
+        If -1, all points are used.
+    :param prob: The probability to use for the scatter plot.
+    :return: The x, y and prob data.
+    """
+    if n_points_scatter > 0:
+        select = np.random.choice(x.shape[0], n_points_scatter)
+        if prob is None:
+            return x[select], y[select]
+        else:
+            return x[select], y[select], prob[select]
+    else:
+        if prob is None:
+            return x, y
+        else:
+            return x, y, prob
```

### Comparing `trianglechain-0.4.3/src/trianglechain.egg-info/PKG-INFO` & `trianglechain-0.5.0/src/trianglechain.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trianglechain
-Version: 0.4.3
+Version: 0.5.0
 Summary: Code to plot multidimensional distributions
 Author: Silvan Fischbacher, Tomasz Kacprzak
 Author-email: silvanf@phys.ethz.ch, tomaszk@phys.ethz.ch
 License: MIT License
 Project-URL: Source, https://cosmo-docs.phys.ethz.ch/trianglechain
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -21,16 +21,19 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 trianglechain
 =============
 
 [![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/pipeline.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
-[![image](http://img.shields.io/badge/arXiv-2203.09616-orange.svg?style=flat)](https://arxiv.org/abs/2203.09616)
-[![image](http://img.shields.io/badge/arXiv-2207.01627-orange.svg?style=flat)](https://arxiv.org/abs/2207.01627)
+[![image](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/badges/main/coverage.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
+[![Latest Release](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/badges/release.svg)](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/-/releases) 
+[![PyPI version](https://badge.fury.io/py/trianglechain.svg)](https://badge.fury.io/py/trianglechain)
+[![image](http://img.shields.io/badge/arXiv-2203.09616-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2203.09616)
+[![image](http://img.shields.io/badge/arXiv-2207.01627-B31B1B.svg?logo=arxiv&style=flat)](https://arxiv.org/abs/2207.01627)
 
 Code for plotting multidimensional marginal distributions. If you use it, please cite [arXiv-2203.09616](https://arxiv.org/abs/2203.09616) and [arXiv-2207.01627](https://arxiv.org/abs/2207.01627).
 
 [Source](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain)
 
 [Documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
@@ -51,15 +54,15 @@
     size=(10000)
 )
 
 tri = TriangleChain()
 tri.contour_cl(samples);
 ```
 The input data can be rec arrays, numpy array, pandas dataframes or dictionaries.
-For more example plots, see [demos](https://cosmo-gitlab.phys.ethz.ch/cosmo_public/trianglechain/demo)
+For more example plots, see the [documentation](http://cosmo-docs.phys.ethz.ch/trianglechain)
 
 Credits
 -------
 
 This package was created by Tomasz Kacprzak and further developed and extended by Silvan Fischbacher.
 The package is maintained by Silvan Fischbacher: silvanf@phys.ethz.ch.
```

### Comparing `trianglechain-0.4.3/src/trianglechain.egg-info/SOURCES.txt` & `trianglechain-0.5.0/src/trianglechain.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/trianglechain.egg-info/not-zip-safe
 src/trianglechain.egg-info/requires.txt
 src/trianglechain.egg-info/top_level.txt
 tests/test_bestfit.py
 tests/test_limits.py
 tests/test_linechain.py
 tests/test_params.py
-tests/test_trianglechain.py
+tests/test_trianglechain.py
+tests/test_utils.py
```

### Comparing `trianglechain-0.4.3/tests/test_limits.py` & `trianglechain-0.5.0/tests/test_limits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # Copyright (C) 2022 ETH Zurich
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher
 
 import numpy as np
+import pytest
+
 from trianglechain.limits import (
-    percentile,
-    hdi,
     PJ_HPD,
     get_levels,
+    get_one_tailed_levels,
     get_uncertainty_band,
+    hdi,
+    percentile,
+    sigma_to_cdf,
     uncertainty,
 )
 
+np.random.seed(0)
+
 
 def test_percentile():
     samples = np.random.normal(0, 1, 1000)
     lower, upper = percentile(samples, credible_interval=0.68)
     assert lower < 0
     assert upper > 0
 
@@ -30,20 +36,24 @@
     samples = np.random.normal(0, 1, 1000)
     lower, upper = hdi(samples, credible_interval=0.68)
     assert lower < 0
     assert upper > 0
 
 
 def test_PJ_HPD():
-    samples = np.random.normal(0, 1, 1000)
-    lnprobs = np.random.uniform(0, 1, 1000)
+    samples = np.random.uniform(-10, 10, 1000)
+    lnprobs = samples**2
     lower, upper = PJ_HPD(samples, lnprobs, credible_interval=0.68)
     assert lower < 0
     assert upper > 0
 
+    lower, upper = PJ_HPD(samples, lnprobs, credible_interval=0.95)
+    assert lower < 0
+    assert upper > 0
+
 
 def test_get_levels():
     samples = np.random.normal(0, 1, 1000)
     (lower, upper), _, _ = get_levels(
         samples, levels_method="hdi", credible_interval=0.68
     )
     assert lower < 0
@@ -69,10 +79,35 @@
 
 
 def test_one_sided_tail():
     samples = np.random.normal(0, 1, 100000)
     _, two_tail, _ = get_levels(samples, levels_method="hdi", credible_interval=0.68)
     assert two_tail
 
-    samples = samples[samples < 0]
-    _, two_tail, _ = get_levels(samples, levels_method="hdi", credible_interval=0.68)
+    samp = samples[samples < 0]
+    _, two_tail, _ = get_levels(samp, levels_method="hdi", credible_interval=0.68)
     assert not two_tail
+
+    samp = samples[samples > 0]
+    _, two_tail, _ = get_levels(samp, levels_method="hdi", credible_interval=0.68)
+    assert not two_tail
+
+
+def test_errors():
+    with pytest.raises(ValueError):
+        sigma_to_cdf(0.68, side="middle")
+
+    with pytest.raises(ValueError):
+        get_one_tailed_levels(np.random.rand(100), side="middle")
+
+    samples = np.random.normal(0, 1, 100000)
+    (lower, upper), _, _ = get_levels(samples)
+
+    # PJ_HPD without lnprob
+    (lower_test, upper_test), _, _ = get_levels(samples, levels_method="PJ_HPD")
+    assert lower_test == lower
+    assert upper_test == upper
+
+    # Unknown levels_method
+    (lower_test, upper_test), _, _ = get_levels(samples, levels_method="by_eye")
+    assert lower_test == lower
+    assert upper_test == upper
```

### Comparing `trianglechain-0.4.3/tests/test_params.py` & `trianglechain-0.5.0/tests/test_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 # Institute for Particle Physics and Astrophysics
 # Author: Silvan Fischbacher
 
 import numpy as np
 import pandas as pd
 import pytest
 from numpy.testing import assert_array_equal
-from trianglechain.params import ensure_rec, add_derived
+
+from trianglechain.params import (
+    add_derived,
+    check_if_names_is_used_correctly,
+    ensure_rec,
+)
 
 
 @pytest.fixture
 def data():
     return np.array([[1, 2], [3, 4]])
 
 
@@ -101,7 +106,14 @@
     # Test adding derived parameter to numpy rarray
     data = np.array([[1, 2], [3, 4]])
     new_param = "z"
     derived = np.array([3, 7])
     result = add_derived(data, new_param, derived, names=["x", "y"])
     assert np.array_equal(result[new_param], np.array([3, 7]))
     assert np.array_equal(result["x"], np.array([1, 3]))
+
+
+def test_check_names(data, data_dict, expected_rec):
+    names = ["col0", "col1"]
+    assert check_if_names_is_used_correctly(names, data) == names
+    assert check_if_names_is_used_correctly(names, data_dict) is None
+    assert check_if_names_is_used_correctly(names, expected_rec) is None
```

