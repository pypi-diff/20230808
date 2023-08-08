# Comparing `tmp/gocart-0.4.6.tar.gz` & `tmp/gocart-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.4.6.tar", last modified: Thu Jun  8 15:34:23 2023, max compression
+gzip compressed data, was "gocart-0.4.7.tar", last modified: Tue Aug  8 10:02:23 2023, max compression
```

## Comparing `gocart-0.4.6.tar` & `gocart-0.4.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.523552 gocart-0.4.6/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4711 2023-06-08 15:28:52.000000 gocart-0.4.6/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-06-08 15:28:52.000000 gocart-0.4.6/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-06-08 15:28:52.000000 gocart-0.4.6/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-08 15:34:23.523552 gocart-0.4.6/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5894 2023-06-08 15:28:52.000000 gocart-0.4.6/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.499551 gocart-0.4.6/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.515551 gocart-0.4.6/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      200 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.515551 gocart-0.4.6/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14497 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16347 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/resources/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6885 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/resources/package.mplstyle
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.519552 gocart-0.4.6/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-06-08 15:28:52.000000 gocart-0.4.6/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-06-08 15:34:23.507551 gocart-0.4.6/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6460 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      822 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-06-08 15:32:49.000000 gocart-0.4.6/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-06-08 15:34:23.000000 gocart-0.4.6/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-06-08 15:34:23.523552 gocart-0.4.6/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-06-08 15:28:52.000000 gocart-0.4.6/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.135371 gocart-0.4.7/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      413 2023-08-08 09:54:55.000000 gocart-0.4.7/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4867 2023-08-08 09:54:55.000000 gocart-0.4.7/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-08-08 09:54:55.000000 gocart-0.4.7/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-08-08 09:54:55.000000 gocart-0.4.7/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6926 2023-08-08 10:02:23.135371 gocart-0.4.7/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6360 2023-08-08 09:54:55.000000 gocart-0.4.7/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.115370 gocart-0.4.7/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10717 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.123370 gocart-0.4.7/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      200 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4510 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.127370 gocart-0.4.7/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14637 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.131371 gocart-0.4.7/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    16487 2023-08-08 09:54:55.000000 gocart-0.4.7/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.131371 gocart-0.4.7/gocart/resources/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6290 2023-08-08 09:54:56.000000 gocart-0.4.7/gocart/resources/package.mplstyle
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.131371 gocart-0.4.7/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-08-08 09:54:56.000000 gocart-0.4.7/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-08-08 09:54:56.000000 gocart-0.4.7/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2891 2023-08-08 09:54:56.000000 gocart-0.4.7/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-08-08 09:54:56.000000 gocart-0.4.7/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-08-08 10:02:23.119370 gocart-0.4.7/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6926 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      840 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-08-08 09:59:57.000000 gocart-0.4.7/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-08-08 10:02:22.000000 gocart-0.4.7/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-08-08 10:02:23.135371 gocart-0.4.7/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-08-08 09:54:56.000000 gocart-0.4.7/setup.py
```

### Comparing `gocart-0.4.6/CHANGES.md` & `gocart-0.4.7/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 ## Release Notes
 
+**v0.4.7 - August 8, 2023**
+
+- **FIXED**: fixing parsing issue for initial burst alerts containing image links as property and classification parameters  
+
 **v0.4.6 - June 8, 2023**
 
 - **REFACTOR**: making plots consistent across platforms by including a MPL style file
 - **FIXED**: area of contours now included in plots if generated from a plugin
 
 **v0.4.5 - June 6, 2023**
```

### Comparing `gocart-0.4.6/LICENSE` & `gocart-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/PKG-INFO` & `gocart-0.4.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gocart
-Version: 0.4.6
-Summary: Listen for, collect and convert multimessenger skymaps
-Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.6.zip
-Author: David Young
-Author-email: d.r.young@qub.ac.uk
-License: MIT
-Keywords: astronomy
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gocart
 
 [![](https://zenodo.org/badge/614846695.svg)](https://zenodo.org/badge/latestdoi/614846695)  
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/gocart)](https://pypi.org/project/gocart/)
@@ -32,26 +15,28 @@
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
 
-*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*.
+*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*
+
+[![](https://live.staticflickr.com/65535/52985431851_6a4ed02836_m.png)](https://live.staticflickr.com/65535/52985431851_6a4ed02836_o.png)
 
 Documentation for gocart is hosted by [Read the Docs](https://gocart.readthedocs.io/en/main/) ([development version](https://gocart.readthedocs.io/en/develop/) and [main version](https://gocart.readthedocs.io/en/main/)). The code lives on [github](https://github.com/thespacedoctor/gocart). Please report any issues you find [here](https://github.com/thespacedoctor/gocart/issues).
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
 - Create your own plugin scripts to run whenever an alert is parsed.
-
+- works well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag).
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
 conda create -n gocart python=3.9 pip gocart -c conda-forge
@@ -110,14 +95,18 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## SkyTag
+
+gocart works very well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag), a tool to 'annotate' transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
+
 ## How to cite gocart
 
 If you use `gocart` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_gocart,
 author = {Young, David R.},
```

### Comparing `gocart-0.4.6/README.md` & `gocart-0.4.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gocart
+Version: 0.4.7
+Summary: Listen for, collect and convert multimessenger skymaps
+Home-page: https://github.com/thespacedoctor/gocart
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.7.zip
+Author: David Young
+Author-email: d.r.young@qub.ac.uk
+License: MIT
+Keywords: astronomy
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # gocart
 
 [![](https://zenodo.org/badge/614846695.svg)](https://zenodo.org/badge/latestdoi/614846695)  
 
 <!-- INFO BADGES -->  
 
 [![](https://img.shields.io/pypi/pyversions/gocart)](https://pypi.org/project/gocart/)
@@ -15,26 +32,28 @@
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
 
-*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*.
+*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*
+
+[![](https://live.staticflickr.com/65535/52985431851_6a4ed02836_m.png)](https://live.staticflickr.com/65535/52985431851_6a4ed02836_o.png)
 
 Documentation for gocart is hosted by [Read the Docs](https://gocart.readthedocs.io/en/main/) ([development version](https://gocart.readthedocs.io/en/develop/) and [main version](https://gocart.readthedocs.io/en/main/)). The code lives on [github](https://github.com/thespacedoctor/gocart). Please report any issues you find [here](https://github.com/thespacedoctor/gocart/issues).
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
 - Create your own plugin scripts to run whenever an alert is parsed.
-
+- works well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag).
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
 conda create -n gocart python=3.9 pip gocart -c conda-forge
@@ -93,14 +112,18 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## SkyTag
+
+gocart works very well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag), a tool to 'annotate' transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
+
 ## How to cite gocart
 
 If you use `gocart` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_gocart,
 author = {Young, David R.},
```

### Comparing `gocart-0.4.6/gocart/advanced_settings.yaml` & `gocart-0.4.7/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/cl_utils.py` & `gocart-0.4.7/gocart/cl_utils.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/commonutils/flatten_healpix_map.py` & `gocart-0.4.7/gocart/commonutils/flatten_healpix_map.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.7/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/convert/aitoff.py` & `gocart-0.4.7/gocart/convert/aitoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,22 +328,28 @@
                 zlow = (ho * (self.meta['HEADER']['DISTMEAN'] - self.meta['HEADER']['DISTSTD'])) / 3e5
                 zhigh = (ho * (self.meta['HEADER']['DISTMEAN'] + self.meta['HEADER']['DISTSTD'])) / 3e5
                 if zlow < 0:
                     zlow = 0
                 data += f"Redshift: {zlow:0.2}<z<{zhigh:0.2}\n"
 
             data += "\n"
-            if "classification" in self.meta['ALERT']['event']:
-                for k, v in self.meta['ALERT']['event']['classification'].items():
-                    data += f"{k}: {v:.2f}\n"
+            try:
+                if "classification" in self.meta['ALERT']['event']:
+                    for k, v in self.meta['ALERT']['event']['classification'].items():
+                        data += f"{k}: {v:.2f}\n"
+            except:
+                pass
 
             data += "\n"
-            if "properties" in self.meta['ALERT']['event']:
-                for k, v in self.meta['ALERT']['event']['properties'].items():
-                    data += f"{k}: {v:.2f}\n"
+            try:
+                if "properties" in self.meta['ALERT']['event']:
+                    for k, v in self.meta['ALERT']['event']['properties'].items():
+                        data += f"{k}: {v:.2f}\n"
+            except:
+                pass
 
             plt.text(3.42, 0.2, data, ha='left', va='top', fontsize=5, linespacing=1.8)
 
         # this = ax.clabel(line_c, inline=True, fontsize=6, colors=['#93a1a1'], fmt='{:.0f} '.format)
 
         if self.patches:
             ax.add_collection(PatchCollection(self.patches, alpha=0.4,
```

### Comparing `gocart-0.4.6/gocart/convert/ascii.py` & `gocart-0.4.7/gocart/convert/ascii.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/convert/healpix2cart.py` & `gocart-0.4.7/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/default_settings.yaml` & `gocart-0.4.7/gocart/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/parsers/lvk.py` & `gocart-0.4.7/gocart/parsers/lvk.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,20 +148,26 @@
                 far /= 365.
                 far = f"1 per {far:0.1f} yrs"
             else:
                 far = f"1 per {far:0.1f} days"
             print(f'EVENT: {self.record["superevent_id"]} detected at {self.record["event"]["time"].replace("Z","")} UTC ({self.record["event"]["group"]})')
             print(f'ALERT: {self.record["alert_type"].replace("_"," ")} reported at {self.record["time_created"].replace("Z","")} UTC (+{timeDelta:.2f} mins)')
             print(f'FAR: {far}')
-            if "classification" in self.record['event'] and len(self.record['event']['classification']):
-                for k, v in self.record['event']['classification'].items():
-                    self.record['event']['classification'][k] = float(f'{v:.2f}')
-                print(f"CLASSIFICATION: {self.record['event']['classification']}")
-            if "properties" in self.record['event'] and len(self.record['event']['properties']):
-                print(f"PROPERTIES: {self.record['event']['properties']})")
+            try:
+                if "classification" in self.record['event'] and len(self.record['event']['classification']):
+                    for k, v in self.record['event']['classification'].items():
+                        self.record['event']['classification'][k] = float(f'{v:.2f}')
+                    print(f"CLASSIFICATION: {self.record['event']['classification']}")
+            except:
+                pass
+            try:
+                if "properties" in self.record['event'] and len(self.record['event']['properties']):
+                    print(f"PROPERTIES: {self.record['event']['properties']})")
+            except:
+                pass
         else:
             print(f'EVENT: {self.record["superevent_id"]}')
             print(f'ALERT: {self.record["alert_type"].replace("_"," ")} reported at {self.record["time_created"].replace("Z","")} UTC')
 
         # PARSE SKY MAP
         header, extras, fitsPath = {}, {}, None
         localisation = False
```

### Comparing `gocart-0.4.6/gocart/resources/package.mplstyle` & `gocart-0.4.7/gocart/resources/package.mplstyle`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 # When text.usetex is False, font.family may also be one or more concrete font names.
 font.family         : sans-serif # serif, sans-serif, cursive, fantasy, monospace
 font.style          : normal # normal, italic, oblique
 font.variant        : normal # normal, small-caps
 font.weight         : medium # normal, bold, bolder, lighter, 100, 200, 300, ..., 900
 font.stretch        : normal # ultra-condensed, extra-condensed, condensed, semi-condensed, normal, semi-expanded, expanded, extra-expanded, ultra-expanded, wider, narrower
 font.size           : 12.0
-font.serif          : Bitstream Vera Serif, New Century Schoolbook, Century Schoolbook L, Utopia, ITC Bookman, Bookman, Nimbus Roman No9 L, Times New Roman, Times, Palatino, Charter, serif
-font.sans-serif     : Bitstream Vera Sans, Lucida Grande, Verdana, Geneva, Lucid, Arial, Helvetica, Avant Garde, sans-serif
-font.cursive        : Apple Chancery, Textile, Zapf Chancery, Sand, cursive
-font.fantasy        : Comic Sans MS, Chicago, Charcoal, Impact, Western, fantasy
-font.monospace      : Bitstream Vera Sans Mono, Andale Mono, Nimbus Mono L, Courier New, Courier, Fixed, Terminal, monospace
 
 
 ### AXES
 #axes.hold           : True    # whether to clear the axes by default on
 axes.facecolor      : white   # axes background color
 axes.edgecolor      : 002b36    # axes edge color
 axes.linewidth      : 2.0     # edge linewidth
```

### Comparing `gocart-0.4.6/gocart/resources/plugins/gp_template.py` & `gocart-0.4.7/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/setup.cfg` & `gocart-0.4.7/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/test_settings.yaml` & `gocart-0.4.7/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart/utKit.py` & `gocart-0.4.7/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.4.6/gocart.egg-info/PKG-INFO` & `gocart-0.4.7/gocart.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.4.6
+Version: 0.4.7
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.6.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.7.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
@@ -32,26 +32,28 @@
 
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fmain&subject=build%20main)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=main)
 [![](https://soxs-eso-data.org/ci/buildStatus/icon?job=gocart%2Fdevelop&subject=build%20dev)](https://soxs-eso-data.org/ci/blue/organizations/jenkins/gocart/activity?branch=develop)
 [![](https://cdn.jsdelivr.net/gh/thespacedoctor/gocart@main/coverage.svg)](https://raw.githack.com/thespacedoctor/gocart/main/htmlcov/index.html)
 [![](https://readthedocs.org/projects/gocart/badge/?version=main)](https://gocart.readthedocs.io/en/main/)
 [![](https://img.shields.io/github/issues/thespacedoctor/gocart/type:%20bug?label=bug%20issues)](https://github.com/thespacedoctor/gocart/issues?q=is%3Aissue+is%3Aopen+label%3A%22type%3A+bug%22+)  
 
-*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*.
+*gocart is a python package and command-line suite used to consume [GCN Kafka streams](https://gcn.nasa.gov).*
+
+[![](https://live.staticflickr.com/65535/52985431851_6a4ed02836_m.png)](https://live.staticflickr.com/65535/52985431851_6a4ed02836_o.png)
 
 Documentation for gocart is hosted by [Read the Docs](https://gocart.readthedocs.io/en/main/) ([development version](https://gocart.readthedocs.io/en/develop/) and [main version](https://gocart.readthedocs.io/en/main/)). The code lives on [github](https://github.com/thespacedoctor/gocart). Please report any issues you find [here](https://github.com/thespacedoctor/gocart/issues).
 
 ## Features
 
 - Listen to GCN Kafka streams (currently  LIGO-Virgo-KAGRA only) and write alerts and skymaps to the local filesystem.
 - Ability to 'echo' the Kafka stream by re-listening to the last N days of alerts (provided the alerts are still hosted on the GCN Kafka cluster).
 - Alert content, FITS Header data and some extra value-added event parameters are written to a single machine-readable YAML file.
 - The healpix skymaps are optionally converted to ascii files (one row per healpix pixel) and/or rendered as aitoff plots.
 - Create your own plugin scripts to run whenever an alert is parsed.
-
+- works well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag).
 
 ## Installation
 
 The easiest way to install gocart is to use `conda`:
 
 ``` bash
 conda create -n gocart python=3.9 pip gocart -c conda-forge
@@ -110,14 +112,18 @@
 
 [![](https://live.staticflickr.com/65535/52790845580_b5a1145e13_z.png)](https://live.staticflickr.com/65535/52790845580_b5a1145e13_o.png)
 
 Don't worry about the `group_id` parameter, it's initially set to XXXX but gocart will replace this with a unique value when it's first run. It is this `group_id` that allows GCN Kafka to remember which alerts you have or have not heard before. Note the example client above has been deleted, so the credentials quoted here will not work.
 
 You are now ready to start using gocart.
 
+## SkyTag
+
+gocart works very well in conjunction with [skyTag](https://github.com/thespacedoctor/skyTag), a tool to 'annotate' transient sources or galaxies with the percentage credibility region they reside within on a given HealPix sky map.
+
 ## How to cite gocart
 
 If you use `gocart` in your work, please cite using the following BibTeX entry: 
 
 ```bibtex
 @software{Young_gocart,
 author = {Young, David R.},
```

### Comparing `gocart-0.4.6/gocart.egg-info/SOURCES.txt` & `gocart-0.4.7/gocart.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.readthedocs.yaml
 CHANGES.md
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 gocart/__init__.py
 gocart/__version__.py
```

### Comparing `gocart-0.4.6/setup.py` & `gocart-0.4.7/setup.py`

 * *Files identical despite different names*

