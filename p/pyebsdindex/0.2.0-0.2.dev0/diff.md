# Comparing `tmp/pyebsdindex-0.2.0.tar.gz` & `tmp/pyebsdindex-0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyebsdindex-0.2.0.tar", last modified: Tue Aug  8 20:23:29 2023, max compression
+gzip compressed data, was "pyebsdindex-0.2.dev0.tar", last modified: Sat May  6 11:03:22 2023, max compression
```

## Comparing `pyebsdindex-0.2.0.tar` & `pyebsdindex-0.2.dev0.tar`

### file list

```diff
@@ -1,95 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.818707 pyebsdindex-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)   368506 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/IPFCubic.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   147377 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/IPFCubic.png
--rw-r--r--   0 runner    (1001) docker     (123)   197654 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/IPFHex.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    82053 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/IPFHex.png
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/License
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-08 20:23:29.818707 pyebsdindex-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.806707 pyebsdindex-0.2.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.806707 pyebsdindex-0.2.0/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/_static/colormap_banners/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_static/colormap_banners/banner0.png
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_static/colormap_banners/banner1.png
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_static/colormap_banners/create_colormap_banners.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/custom-attribute-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/custom-function-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/custom-method-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/tutorials/NLPAR_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1570100 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/tutorials/ebsd_index_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.810706 pyebsdindex-0.2.0/doc/user/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/doc/user/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.814707 pyebsdindex-0.2.0/pyebsdindex/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.814707 pyebsdindex-0.2.0/pyebsdindex/EBSDImage/
--rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/EBSDImage/IPFcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/EBSDImage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30986 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/_ebsd_index_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    28589 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/_ebsd_index_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/band_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    34271 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/band_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)    17076 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/crystal_sym.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/crystallometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    50585 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/ebsd_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/ebsdfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/misorientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25488 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/nlpar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.814707 pyebsdindex-0.2.0/pyebsdindex/opencl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/opencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26857 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/opencl/band_detect_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23342 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/opencl/clkernels.cl
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/opencl/openclparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/opencl/radon_fast_cl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/pairlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19414 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/pcopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/radon_fast.py
--rw-r--r--   0 runner    (1001) docker     (123)    22234 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/rotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/rotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.818707 pyebsdindex-0.2.0/pyebsdindex/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.806707 pyebsdindex-0.2.0/pyebsdindex/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.818707 pyebsdindex-0.2.0/pyebsdindex/tests/data/al_sim_20kv/
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/numbatest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/raytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/rotlibunittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/test_ebsd_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/test_pcopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tests/test_tripletvote.py
--rw-r--r--   0 runner    (1001) docker     (123)    58613 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/pyebsdindex/tripletvote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:23:29.814707 pyebsdindex-0.2.0/pyebsdindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:23:29.000000 pyebsdindex-0.2.0/pyebsdindex.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-08 20:23:29.818707 pyebsdindex-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-08-08 20:23:20.000000 pyebsdindex-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    48700 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    49952 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/IPFCubic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/License
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.488583 pyebsdindex-0.2.dev0/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner0.png
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/colormap_banners/create_colormap_banners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-function-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-method-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.492583 pyebsdindex-0.2.dev0/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/NLPAR_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   634518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/ebsd_index_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.496583 pyebsdindex-0.2.dev0/doc/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/doc/user/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/IPFcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/EBSDImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21731 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/band_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystal_sym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/ebsdfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex/opencl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21518 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/clkernels.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/openclparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22234 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51672 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11739 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/spherical_radon_fast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.484583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_ebsd_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/pyebsdindex/tripletlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 11:03:22.500583 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 11:03:22.000000 pyebsdindex-0.2.dev0/pyebsdindex.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-06 11:03:22.504583 pyebsdindex-0.2.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-06 11:03:07.000000 pyebsdindex-0.2.dev0/setup.py
```

### Comparing `pyebsdindex-0.2.0/.readthedocs.yaml` & `pyebsdindex-0.2.dev0/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# .readthedocs.yaml
+# ..readthedocs.yaml
 # Read the Docs configuration file
 # See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
 
 # Required
 version: 2
 
 # Build documentation in the doc/ directory with Sphinx
 sphinx:
   configuration: doc/conf.py
 
 # Set the version of Python and other tools you might need
 build:
-  os: ubuntu-22.04
+  os: ubuntu-20.04
   tools:
-    python: "3.11"
+    python: "3.9"
 
 # Build doc in all formats (HTML, PDF and ePub)
 formats:
   - htmlzip
   - pdf
 
 # Python environment for building the docs
```

### Comparing `pyebsdindex-0.2.0/License` & `pyebsdindex-0.2.dev0/License`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/PKG-INFO` & `pyebsdindex-0.2.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pyebsdindex
-Version: 0.2.0
+Version: 0.2.dev0
 Summary: Python based tool for Hough/Radon based EBSD indexing
 Home-page: https://pyebsdindex.readthedocs.io
 Download-URL: https://pypi.python.org/pypi/pyebsdindex
 Author: ['Dave Rowenhorst', 'Håkon Wiik Ånes']
 Maintainer: Dave Rowenhorst
 Maintainer-email: 
 License: Custom
 Project-URL: Bug Tracker, https://github.com/USNavalResearchLaboratory/PyEBSDIndex/issues
 Project-URL: Documentation, https://pyebsdindex.readthedocs.io
 Project-URL: Source Code, https://github.com/USNavalResearchLaboratory/PyEBSDIndex
-Keywords: EBSD,electron backscatter diffraction,HI,Radon indexing,NLPAR
+Keywords: EBSD,electron backscatter diffraction,HI,Hough indexing,NLPAR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -33,15 +32,15 @@
 Provides-Extra: parallel
 Provides-Extra: dev
 Provides-Extra: all
 License-File: License
 
 # PyEBSDIndex
 
-Python based tool for Radon based EBSD orientation indexing.
+Python based tool for Hough/Radon based EBSD orientation indexing.
 
 [![Build status](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml/badge.svg)](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml)
 [![Documentation status](https://readthedocs.org/projects/pyebsdindex/badge/?version=latest)](https://pyebsdindex.readthedocs.io/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/pyebsdindex.svg)](https://pypi.python.org/pypi/pyebsdindex)
 
 The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
 Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
```

### Comparing `pyebsdindex-0.2.0/README.md` & `pyebsdindex-0.2.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PyEBSDIndex
 
-Python based tool for Radon based EBSD orientation indexing.
+Python based tool for Hough/Radon based EBSD orientation indexing.
 
 [![Build status](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml/badge.svg)](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml)
 [![Documentation status](https://readthedocs.org/projects/pyebsdindex/badge/?version=latest)](https://pyebsdindex.readthedocs.io/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/pyebsdindex.svg)](https://pypi.python.org/pypi/pyebsdindex)
 
 The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
 Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
```

### Comparing `pyebsdindex-0.2.0/RELEASE.rst` & `pyebsdindex-0.2.dev0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/Makefile` & `pyebsdindex-0.2.dev0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_static/colormap_banners/banner0.png` & `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner0.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_static/colormap_banners/banner1.png` & `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/banner1.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_static/colormap_banners/create_colormap_banners.py` & `pyebsdindex-0.2.dev0/doc/_static/colormap_banners/create_colormap_banners.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_static/custom.css` & `pyebsdindex-0.2.dev0/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_templates/custom-class-template.rst` & `pyebsdindex-0.2.dev0/doc/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/_templates/custom-module-template.rst` & `pyebsdindex-0.2.dev0/doc/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/conf.py` & `pyebsdindex-0.2.dev0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/dev/index.rst` & `pyebsdindex-0.2.dev0/doc/dev/index.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/index.rst` & `pyebsdindex-0.2.dev0/doc/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===================================
 PyEBSDIndex |release| documentation
 ===================================
 
-Python based tool for Radon based EBSD orientation indexing.
+Python based tool for Hough/Radon based EBSD orientation indexing.
 
 The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
 Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
 Science, 23(3):759–767, 1992, and N. C. Krieger Lassen. Automated Determination of
 Crystal Orientations from Electron Backscattering Patterns. PhD thesis, The Technical
 University of Denmark, 1994.
```

### Comparing `pyebsdindex-0.2.0/doc/make.bat` & `pyebsdindex-0.2.dev0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/reference/index.rst` & `pyebsdindex-0.2.dev0/doc/reference/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -28,8 +28,7 @@
 .. autosummary::
     :toctree: generated
     :template: custom-module-template.rst
 
     ebsd_index
     nlpar
     pcopt
-    tripletvote
```

### Comparing `pyebsdindex-0.2.0/doc/tutorials/NLPAR_demo.ipynb` & `pyebsdindex-0.2.dev0/doc/tutorials/NLPAR_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/doc/user/installation.rst` & `pyebsdindex-0.2.dev0/doc/user/installation.rst`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/__init__.py` & `pyebsdindex-0.2.dev0/pyebsdindex/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Initial committer first, then sorted by line contributions
 __credits__ = [
     "Dave Rowenhorst",
     "Håkon Wiik Ånes",
 ]
 __description__ = "Python based tool for Hough/Radon based EBSD indexing"
 __name__ = "pyebsdindex"
-__version__ = "0.2.0"
+__version__ = "0.2.dev0"
 
 
 # Try to import only once
 try:
     import pyopencl
     _pyopencl_installed = True
 except ImportError:
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/_ebsd_index_single.py` & `pyebsdindex-0.2.dev0/pyebsdindex/_ebsd_index_single.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-"""Setup and handling of Radon indexing runs of EBSD patterns on a
+"""Setup and handling of Hough indexing runs of EBSD patterns on a
 single thread.
 """
 
 from timeit import default_timer as timer
 
 import numpy as np
 import h5py
 
-from pyebsdindex import tripletvote as bandindexer  # use triplet voting as the default indexer.
-from pyebsdindex.tripletvote import BandIndexer
 from pyebsdindex import (
+    band_vote,
     ebsd_pattern,
     rotlib,
+    tripletlib,
     _pyopencl_installed,
 )
 
 if _pyopencl_installed:
     from pyebsdindex.opencl import band_detect_cl as band_detect
 else:
     from pyebsdindex import band_detect as band_detect
@@ -135,15 +135,15 @@
         EBSD indexer. If not given, many of the above parameters must be
         passed. Otherwise, these parameters are retrieved from this
         indexer.
     clparams : list, optional
         OpenCL parameters passed to :mod:`pyopencl` if the package is
         installed.
     verbose : int, optional
-        0 - no output (default), 1 - timings, 2 - timings and the Radon
+        0 - no output (default), 1 - timings, 2 - timings and the Hough
         transform of the first pattern with detected bands highlighted.
     chunksize : int, optional
         Default is 528.
     gpu_id : int, optional
         ID of GPU to use if :mod:`pyopencl` is installed.
 
     Returns
@@ -156,30 +156,15 @@
         of bands matched for each phase. Each data entry contains the
         orientation expressed as a quaternion (quat) (using the
         convention of ``vendor`` or :attr:`indexer.vendor`), Pattern
         Quality (pq), Confidence Metric (cm), Phase ID (phase), Fit
         (fit) and Number of Bands Matched (nmatch). There are some other
         metrics reported, but these are mostly for debugging purposes.
     bandData : numpy.ndarray
-        Band identification data from the Radon transform. Stored
-        as a structured numpy array, of dimensions [npoints, nbands].
-
-        With fields that include:
-            - id: band ID
-            - max: peak max intesensity (used to calculate pattern quality)
-            - maxloc: nearest integer location of the Radon peak
-            - avemax: nearest neighbor average of the max peak intensity
-            - aveloc: sub-pixel location of the Radon peak
-            - width: a metric of the band width
-            - theta: the theta value of the sub-pixel location on the Radon (lower-left origin)
-            - rho: the rho value of the sub-pixel location on the Radon (lower-left origin)
-            - valid: was the peak detected
-            - band_match_index: index for phase number and pole number that indexed to this band
-              (use :meth:`~EBSDIndexer.getmatchedpole`)
-
+        Band identification data from the Radon transform.
     indexer : EBSDIndexer
         EBSD indexer, returned if ``return_indexer_obj=True``.
     """
     pats = None
     if patsin is None:
         pdim = None
     else:
@@ -242,15 +227,15 @@
     if not return_indexer_obj:
         return dataout, banddata
     else:
         return dataout, banddata, indexer
 
 
 class EBSDIndexer:
-    """Setup of Radon indexing of EBSD patterns.
+    """Setup of Hough indexing of EBSD patterns.
 
     Parameters
     ----------
     filename : str, optional
         Name of file with EBSD patterns.
     phaselist : list of str, optional
         Options are ``"FCC"`` and ``"BCC"``. Default is ``["FCC"]``.
@@ -309,33 +294,27 @@
         nRho=90,
         nTheta=180,
         tSigma=1.0,
         rSigma=1.2,
         rhoMaskFrac=0.15,
         nBands=9,
         patDim=None,
-        nband_earlyexit=None,
         **kwargs
     ):
         """Create an EBSD indexer."""
         self.filein = filename
         if self.filein is not None:
             self.fID = ebsd_pattern.get_pattern_file_obj(self.filein)
         else:
             self.fID = None
 
         self.phaselist = phaselist
         self.phaseLib = []
         for ph in self.phaselist:
-            if ph is None:
-                self.phaseLib.append(None)
-            if isinstance(ph, str):
-                self.phaseLib.append(bandindexer.addphase(libtype=ph))
-            if isinstance(ph, BandIndexer):
-                self.phaseLib.append(ph)
+            self.phaseLib.append(band_vote.BandVote(tripletlib.triplib(libType=ph)))
 
         self.vendor = "EDAX"
         if vendor is None:
             if self.fID is not None:
                 self.vendor = self.fID.vendor
         else:
             self.vendor = vendor
@@ -367,25 +346,24 @@
         if self.fID is not None:
             self.bandDetectPlan.band_detect_setup(
                 patDim=[self.fID.patternW, self.fID.patternH]
             )
         elif patDim is not None:
             self.bandDetectPlan.band_detect_setup(patDim=patDim)
 
-        self.nband_earlyexit = nband_earlyexit
         self.dataTemplate = np.dtype(
             [
                 ("quat", np.float64, 4),
                 ("iq", np.float32),
                 ("pq", np.float32),
                 ("cm", np.float32),
                 ("phase", np.int32),
                 ("fit", np.float32),
                 ("nmatch", np.int32),
-                ("matchattempts", np.int32, 4),
+                ("matchattempts", np.int32, 2),
                 ("totvotes", np.int32),
             ]
         )
 
     def update_file(self, filename=None, patDim=np.array([120, 120], dtype=np.int32)):
         """Update file with patterns to index.
 
@@ -407,19 +385,18 @@
             )
 
     def index_pats(
         self,
         patsin=None,
         patstart=0,
         npats=-1,
-        xyloc=None,
         clparams=None,
         PC=None,
         verbose=0,
-        chunksize=512,
+        chunksize=528,
     ):
         """Index EBSD patterns.
 
         Parameters
         ----------
         patsin : numpy.ndarray, optional
             EBSD patterns in an array of shape (n points, n pattern
@@ -437,267 +414,146 @@
             convention. For EDAX TSL, this is (x*, y*, z*), defined in
             fractions of pattern width with respect to the lower left
             corner of the detector. If not given, this is read from
             :attr:`self.PC`. If :attr:`vendor` is ``"EMSOFT"``, the PC
             must be four numbers, the final number being the pixel size.
         verbose : int, optional
             0 - no output (default), 1 - timings, 2 - timings and the
-            Radon transform of the first pattern with detected bands
+            Hough transform of the first pattern with detected bands
             highlighted.
         chunksize : int, optional
-            Default is 512.
+            Default is 528.
 
         Returns
         -------
         indxData : numpy.ndarray
-            Structured numpy array, that is
-            [nphases + 1, npoints]. The data is stored for each phase used
-            in indexing and the ``indxData[-1]`` layer uses the best guess
-            on which is the most likely phase, based on the fit, and number
-            of bands matched for each phase. Each data entry contains the
-            orientation expressed as a quaternion ('quat') (using the
-            convention of ``vendor`` or :attr:`indexer.vendor`), Pattern
-            Quality ('pq'), Confidence Metric ('cm'), Phase ID ('phase'), Fit
-            ('fit') and Number of Bands Matched ('nmatch'). There are some other
-            metrics reported, but these are mostly for debugging purposes.
-            The number and order of fields are not guaranteed to remain the same, but
-            fields listed here are stable.
-            (phase) parameter will be set to -1 for any no-solution point.
+            Complex numpy array (or array of structured data), that is
+            [nphases + 1, npoints]. The data is stored for each phase
+            used in indexing and the `indxData[-1]` layer uses the best
+            guess on which is the most likely phase, based on the fit,
+            and number of bands matched for each phase. Each data entry
+            contains the orientation expressed as a quaternion (quat)
+            (using `self.vendor`'s convention), Pattern Quality (pq),
+            Confidence Metric (cm), Phase ID (phase), Fit (fit) and
+            Number of Bands Matched (nmatch). There are some other
+            metrics reported, but these are mostly for debugging
+            purposes.
         bandData : numpy.ndarray
-            Band identification data from the Radon transform. Stored
-            as a structured numpy array, of dimensions [npoints, nbands].
-
-            With fields that include:
-                - id: band ID
-                - max: peak max intesensity (used to calculate pattern quality)
-                - maxloc: nearest integer location of the Radon peak
-                - avemax: nearest neighbor average of the max peak intensity
-                - aveloc: sub-pixel location of the Radon peak
-                - width: a metric of the band width
-                - theta: the theta value of the sub-pixel location on the Radon (lower-left origin)
-                - rho: the rho value of the sub-pixel location on the Radon (lower-left origin)
-                - valid: was the peak detected
-                - band_match_index: index for phase number and pole number that indexed to this band
-                  (use :meth:`~EBSDIndexer.getmatchedpole`)
-
+            Band identification data from the Radon transform.
         patstart : int
             Starting index of the indexed patterns.
         npats : int
             Number of patterns indexed. This and `patstart` are useful
             for the distributed indexing procedures.
         """
-
-        pats, xyloc = self._getpats(patsin=patsin, patstart=patstart, npats=npats, xyloc=xyloc)
-        # just a check that the band_detect is ready for this size pattern.
-        if self.bandDetectPlan.patDim is None:
-            self.bandDetectPlan.band_detect_setup(patterns=pats)
-
-        npoints = pats.shape[0]
-        if npats == -1:
-            npats = npoints
-
-        banddata, bandnorm = self._detectbands(pats, PC, xyloc=xyloc, clparams=clparams, verbose=verbose,
-                                               chunksize=chunksize)
-        tic = timer()
-
-        indxData, banddata = self._indexbandsphase(banddata, bandnorm, verbose=verbose)
-
-        if verbose > 0:
-            print("Band Vote Time: ", timer() - tic)
-
-        return indxData, banddata, patstart, npats
-
-    def getmatchedpole(self, banddata, float_out=False):
-        """Return the pole from the library that was matched to the
-        detected band.
-
-        Parameters
-        ----------
-        banddata : numpy.ndarray
-            Output structured band data array from
-            :meth:`~pyebsdindex.ebsd_index.index_pats` or
-            :meth:`~pyebsdindex.ebsd_index.index_pats_distributed`.
-        float_out : bool, optional
-            Default (False) is to return an array of ints with Miller
-            indices. If set to True, then floats, with unit length, will
-            be returned in the sample Cartesian reference frame.
-            (Length is only valid for cubic systems).
-
-        Returns
-        -------
-        numpy.ndarray
-            The default is an array [npoints, nbands, 3] that contains
-            the Miller indices (as ints) of the matching pole (note that
-            hexagonal will also return only three-index notation). If
-            the float_out is set to True, then the output will be
-            floating point vectors of length one, within the sample
-            Cartesian reference frame.
-        """
-        nphases = len(self.phaseLib)
-
-        bnddat = banddata
-        shpbdndat = bnddat.shape
-        if len(shpbdndat) == 0:
-            bnddat = np.array(bnddat).reshape(1)
-        shpbdndat = bnddat.shape
-        nbands = shpbdndat[-1]
-        if len(shpbdndat) == 1:
-            bnddat = bnddat.reshape(1, nbands)
-        shpbdndat = bnddat.shape
-        npoints = shpbdndat[0]
-
-        polesout = np.zeros((npoints,nbands,3))
-        if float_out is False:
-            polekey = 'poles'
-        else:
-            polekey = 'polesCart'
-
-        for ph in range(nphases):
-            wh = np.nonzero(bnddat['band_match_index'][:,0,0] == ph)[0]
-            if len(wh) == 0:
-                continue
-            pindex = bnddat['band_match_index'][wh,:, 1]
-            poles = self.phaseLib[ph].completelib[polekey][pindex,:]
-            polesout[wh, :, :] = poles
-
-        if float_out is False:
-            polesout = np.round(polesout).astype(int)
-
-        return polesout
-
-    def _getpats(self, patsin=None, patstart=0, npats=-1, xyloc=None):
         if patsin is None:
-            pats, xylocin = self.fID.read_data(
+            pats = self.fID.read_data(
                 returnArrayOnly=True,
                 patStartCount=[patstart, npats],
                 convertToFloat=True,
             )
-            if xyloc is None:
-                xyloc = xylocin
         else:
             pshape = patsin.shape
             if len(pshape) == 2:
                 pats = np.reshape(patsin, (1, pshape[0], pshape[1]))
             else:
                 pats = patsin  # [patStart:patEnd, :,:]
             pshape = pats.shape
 
             if self.bandDetectPlan.patDim is None:
                 self.bandDetectPlan.band_detect_setup(patDim=pshape[1:3])
             else:
                 if np.all((np.array(pshape[1:3]) - self.bandDetectPlan.patDim) == 0):
                     self.bandDetectPlan.band_detect_setup(patDim=pshape[1:3])
-        return pats, xyloc
 
-    def _detectbands(self, pats, PC, xyloc=None, clparams=None, verbose=0, chunksize=528):
-        banddata = self.bandDetectPlan.find_bands(
+        if self.bandDetectPlan.patDim is None:
+            self.bandDetectPlan.band_detect_setup(patterns=pats)
+
+        npoints = pats.shape[0]
+        if npats == -1:
+            npats = npoints
+
+        bandData = self.bandDetectPlan.find_bands(
             pats, clparams=clparams, verbose=verbose, chunksize=chunksize
         )
-        #  shpBandDat = banddata.shape
+        shpBandDat = bandData.shape
         if PC is None:
             PC_0 = self.PC
         else:
             PC_0 = PC
-        bandnorm = self.bandDetectPlan.radonPlan.radon2pole(
-            banddata, PC=PC_0, vendor=self.vendor
+        bandNorm = self.bandDetectPlan.radonPlan.radon2pole(
+            bandData, PC=PC_0, vendor=self.vendor
         )
-        return banddata, bandnorm
 
-    def _indexbandsphase(self, banddata, bandnorm, verbose=0):
-
-#        rhomax = 1.0e12
-        rhomax = self.bandDetectPlan.rhoMax * (1-self.bandDetectPlan.rhoMaskFrac)
-        shpBandDat = banddata.shape
-        npoints = int(banddata.size/(shpBandDat[-1])+0.1)
+        # Return bandNorm, patStart, patEnd
+        tic = timer()
         nPhases = len(self.phaseLib)
         q = np.zeros((nPhases, npoints, 4))
         indxData = np.zeros((nPhases + 1, npoints), dtype=self.dataTemplate)
-        bandmatchindex = np.zeros((nPhases, npoints,shpBandDat[-1],2), dtype=np.int32)-100
-        banddataout = banddata.copy()
 
         indxData["phase"] = -1
         indxData["fit"] = 180.0
         indxData["totvotes"] = 0
-        if self.phaseLib[0] is None:
-            return indxData, banddata
-
-        if self.nband_earlyexit is None:
-            earlyexit = -1
-            for ph in self.phaselist:
-                if hasattr(ph, 'nband_earlyexit'):
-                    earlyexit = max(earlyexit, ph.nband_earlyexit)
-            if earlyexit < 0:
-                earlyexit = shpBandDat[1]  # default to all the poles.
-            self.nband_earlyexit = earlyexit
-        else:
-            earlyexit = self.nband_earlyexit
-
+        earlyexit = max(7, shpBandDat[1])
         for i in range(npoints):
-            bandNorm1 = bandnorm[i, :, :]
-            bDat1 = banddata[i, :]
+            bandNorm1 = bandNorm[i, :, :]
+            bDat1 = bandData[i, :]
             whgood = np.nonzero(bDat1["max"] > -1.0e6)[0]
             if whgood.size >= 3:
                 bDat1 = bDat1[whgood]
                 bandNorm1 = bandNorm1[whgood, :]
                 indxData["pq"][0:nPhases, i] = np.sum(bDat1["max"], axis=0)
-                adj_intensity = (-1*np.abs(bDat1["rho"]) * 0.5 / rhomax + 1) * bDat1["max"]
-                #adj_intensity = bDat1["avemax"]
-                #print(bDat1["max"])
-                #print(adj_intensity)
-                for j in range(len(self.phaseLib)):
-                    bandmatchindex[j,i, :, 0] = j
 
+                for j in range(len(self.phaseLib)):
                     (
                         avequat,
                         fit,
                         cm,
                         bandmatch,
                         nMatch,
                         matchAttempts,
                         totvotes,
-                    ) = self.phaseLib[j].bandindex(
-                        bandNorm1, band_intensity=adj_intensity, band_widths=bDat1["width"], verbose=verbose,
+                    ) = self.phaseLib[j].tripvote(
+                        bandNorm1, band_intensity=bDat1["avemax"], verbose=verbose,
                     )
                     # avequat,fit,cm,bandmatch,nMatch, matchAttempts = self.phaseLib[j].pairVoteOrientation(bandNorm1,goNumba=True)
                     if nMatch >= 3:
                         q[j, i, :] = avequat
                         indxData["fit"][j, i] = fit
                         indxData["cm"][j, i] = cm
                         indxData["phase"][j, i] = j
                         indxData["nmatch"][j, i] = nMatch
                         indxData["matchattempts"][j, i] = matchAttempts
                         indxData["totvotes"][j, i] = totvotes
-                        bandmatchindex[j,i, whgood, 1] = bandmatch
-
                     if nMatch >= earlyexit:
                         break
 
-        qref2detect = self._detector2refframe()
+        qref2detect = self._refframe2detector()
         q = q.reshape(nPhases * npoints, 4)
         q = rotlib.quat_multiply(q, qref2detect)
         q = rotlib.quatnorm(q)
         q = q.reshape(nPhases, npoints, 4)
         indxData["quat"][0:nPhases, :, :] = q
-        indxData[-1, :] = indxData[0, :]
-        banddataout['band_match_index'][:,:,:] = bandmatchindex[0,:,:,:].squeeze()
         if nPhases > 1:
-            for j in range(1, nPhases):
-                # indxData[-1, :] = np.where(
-                #    (indxData[j, :]["cm"] * indxData[j, :]["nmatch"])
-                #    > (indxData[j + 1, :]["cm"] * indxData[j + 1, :]["nmatch"]),
-                #    indxData[j, :],
-                #    indxData[j + 1, :],
-                phasetest = ((3.0 - indxData[j, :]["fit"]) * indxData[j, :]["nmatch"]) \
-                            > ((3.0 - indxData[-1, :]["fit"]) * indxData[-1, :]["nmatch"])
-                whbetter = np.nonzero(phasetest)
-                indxData[-1, whbetter] = indxData[j, whbetter]
-                banddataout['band_match_index'][whbetter,:] =  bandmatchindex[j,whbetter,:,:].squeeze()
-        return indxData, banddataout
+            for j in range(nPhases - 1):
+                indxData[-1, :] = np.where(
+                    (indxData[j, :]["cm"] * indxData[j, :]["nmatch"])
+                    > (indxData[j + 1, :]["cm"] * indxData[j + 1, :]["nmatch"]),
+                    indxData[j, :],
+                    indxData[j + 1, :],
+                )
+        else:
+            indxData[-1, :] = indxData[0, :]
+
+        if verbose > 0:
+            print("Band Vote Time: ", timer() - tic)
+
+        return indxData, bandData, patstart, npats
 
-    def _detector2refframe(self):
+    def _refframe2detector(self):
         ven = str.upper(self.vendor)
         if ven in ["EDAX", "EMSOFT", "KIKUCHIPY"]:
             q0 = np.array([np.sqrt(2.0) * 0.5, 0.0, 0.0, -1.0 * np.sqrt(2.0) * 0.5])
             tiltang = -1.0 * (90.0 - self.sampleTilt + self.camElev) / RADEG
             q1 = np.array([np.cos(tiltang * 0.5), np.sin(tiltang * 0.5), 0.0, 0.0])
             quatref2detect = rotlib.quat_multiply(q1, q0)
         elif ven in ["OXFORD", "BRUKER"]:
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/band_detect.py` & `pyebsdindex-0.2.dev0/pyebsdindex/band_detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,29 @@
 import platform
 import tempfile
 from timeit import default_timer as timer
 
 import matplotlib.pyplot as plt
 import numba
 import numpy as np
-import scipy.ndimage as scipyndim #import gaussian_filter
-#from scipy.ndimage #import grey_dilation as scipy_grey_dilation
-#from scipy.ndimage #import median_filter
-import scipy.optimize as scipyopt
+from scipy.ndimage import gaussian_filter
+from scipy.ndimage import grey_dilation as scipy_grey_dilation
+import scipy.optimize as opt
 
 from pyebsdindex import radon_fast
 
 
 tempdir = PurePath("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
 tempdir = tempdir.joinpath('numba')
 environ["NUMBA_CACHE_DIR"] = str(tempdir)
 
 RADEG = 180.0/np.pi
 
 
-class BandDetect():
+class BandDetect:
   def __init__(
     self,
     patterns=None,
     patDim=None,
     nTheta=180,
     nRho=90,
     tSigma=None,
@@ -75,15 +74,15 @@
     self.nBands = nBands
     self.EDAXIQ = False
     self.backgroundsub = None
 
     self.dataType = np.dtype([('id', np.int32), ('max', np.float32), \
                     ('maxloc', np.float32, (2)), ('avemax', np.float32), ('aveloc', np.float32, (2)),\
                     ('pqmax', np.float32), ('width', np.float32), ('theta', np.float32), ('rho', np.float32),
-                    ('valid', np.int8),('band_match_index', np.int32, (2))])
+                    ('valid', np.int8)])
 
 
     if (patterns is None) and (patDim is None):
       pass
     else:
       if (patterns is not None):
         self.patDim = np.asarray(patterns.shape[-2:])
@@ -160,18 +159,18 @@
       recalc_masks = True
 
     if recalc_masks == True:
       ksz = np.array([np.max([np.int64(4*self.rSigma), 5]), np.max([np.int64(4*self.tSigma), 5])])
       ksz = ksz + ((ksz % 2) == 0)
       kernel = np.zeros(ksz, dtype=np.float32)
       kernel[(ksz[0]/2).astype(int),(ksz[1]/2).astype(int) ] = 1
-      kernel = -1.0*scipyndim.gaussian_filter(kernel, [self.rSigma, self.tSigma], order=[2,0])
+      kernel = -1.0*gaussian_filter(kernel, [self.rSigma, self.tSigma], order=[2,0])
       self.kernel = kernel.reshape((1,ksz[0], ksz[1]))
       #self.peakPad = np.array(np.around([ 4*ksz[0], 20.0/self.dTheta]), dtype=np.int64)
-      self.peakPad = np.array(np.around([2 * ksz[0], 2 * ksz[1]]), dtype=np.int64)
+      self.peakPad = np.array(np.around([3 * ksz[0], 4 * ksz[1]]), dtype=np.int64)
       self.peakPad += 1 - np.mod(self.peakPad, 2)  # make sure we have it as odd.
 
     self.padding = np.array([np.max( [self.peakPad[0], self.padding[0]] ), np.max([self.peakPad[1], self.padding[1]])])
 
     if nBands is not None:
       self.nBands = nBands
 
@@ -213,26 +212,29 @@
 
       if method.upper() == 'RANDOMSTRIDE':
         stride = np.random.choice(npats, size = nsample, replace = False )
         stride = np.sort(stride)
       elif method.upper() == 'EVENSTRIDE':
         step = int(npats / nsample) # not great, but maybe good enough.
         stride = np.arange(0,npats, step, dypte = np.uint64)
-      pat1 = fileobj.read_data(convertToFloat=True,patStartCount=[stride[0], 1],returnArrayOnly=True)[0]
+      pat1 = fileobj.read_data(convertToFloat=True,patStartCount=[stride[0], 1],returnArrayOnly=True)
       for i in stride[1:]:
-        pat1 += fileobj.read_data(convertToFloat=True,patStartCount=[i, 1],returnArrayOnly=True)[0]
+        pat1 += fileobj.read_data(convertToFloat=True,patStartCount=[i, 1],returnArrayOnly=True)
       back = pat1 / float(len(stride))
       #pshape = pat1.shape
     # a bit of image processing.
     if back is not None:
-      back = np.squeeze(back)
+      #if sigma is None:
+       #sigma = 2.0 * float(pshape[-1]) / 80.0
+      #back[0,:,:] = gaussian_filter(back[0,:,:], sigma = sigma )
       back = self.backsub_fit(back)
+      #back -= np.mean(back)
     self.backgroundsub = back
 
-  def backsub_fit(self, back, mask = None):
+  def backsub_fit(self, back):
     # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
     # It will automatically use whatever mask is defined for valid data.
     # If the gaussian fit fails to converge, it will fall back to just using the mean set of patterns for the background
     # with a warning.
     def gaussian_surf(x, y, a, x0, y0, sigx, sigy, c, d, e):
     # equation for 2D gaussian on top of a plane.
       return a * np.exp(- ((x - x0) ** 2) / (2.0 * sigx ** 2) - ((y - y0) ** 2) / (2.0 * sigy ** 2)) + c + d * x + e * y
@@ -248,34 +250,32 @@
     nx = back.shape[-1]
     ny = back.shape[-2]
     #plt.imshow(back)
     x = np.arange(nx, dtype=float)
     x = (np.broadcast_to(x.reshape(1,nx), (ny, nx))).ravel()
     y = np.arange(ny, dtype=float)
     y = (np.broadcast_to(y, (nx, ny)).T).ravel()
-    if mask is None:
-      # make a circular mask - even if not EDAX, this should work OK.
-      cx = (np.arange(nx) - nx*0.5)**2
-      cy = (np.arange(ny) - ny*0.5)**2
-      cmask = np.sqrt(np.broadcast_to(cx.reshape(1,nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) < (ny*0.49)
-    else:
-      cmask = mask
+    # make a circular mask - even if not EDAX, this should work OK.
+    cx = (np.arange(nx) - nx*0.5)**2
+    cy = (np.arange(ny) - ny*0.5)**2
+    cmask = np.sqrt(np.broadcast_to(cx.reshape(1,nx), (ny, nx)) + np.broadcast_to(cy, (nx, ny)).T) < (ny*0.49)
+
     # need to grab only the values that are in the mask.
     wh = np.nonzero(cmask.ravel())[0]
     xwh = x[wh]
     ywh = y[wh]
     xywh = np.vstack((xwh, ywh))
-    zwh = (scipyndim.median_filter(np.squeeze(back),3).ravel())[wh]
+    zwh = (back.ravel())[wh]
     whmx = np.unravel_index(back.argmax(), back.shape)
     minz = zwh.min()
     # initialize a guess for the parameters.
     # [gauss amplitude, max loc x, max loc y, sigx, sigy, const offset, slope x, slope y]
     p0 = [(zwh.max() - zwh.min())*0.1, whmx[1], whmx[0], nx/2.355, ny/2.355, minz, 0, 0]
     try:
-      popt, pcov = scipyopt.curve_fit(fit_gauss, xywh, zwh, p0)
+      popt, pcov = opt.curve_fit(fit_gauss, xywh, zwh, p0)
       backfit = (gaussian_surf(x, y, *popt)).reshape(ny, nx)
       #print(p0, popt)
     except RuntimeError:
       print('Warning: no convergence on back subtract ... using mean of the patterns.')
       print('This may not be ideal for scans with few grains across the width of the scan.')
       backfit = back
     backfit -= np.mean(backfit)
@@ -298,15 +298,14 @@
     else:
       patterns = patternsIn
 
     shape = patterns.shape
     nPats = shape[0]
 
     bandData = np.zeros((nPats,self.nBands),dtype=self.dataType)
-    bandData['band_match_index'] = -100
     if chunksize < 0:
       nchunks = 1
       chunksize = nPats
       chunk_start_end = [[0,nPats]]
     else:
       nchunks = (np.ceil(nPats / chunksize)).astype(np.compat.long)
       chunk_start_end = [[i * chunksize, (i + 1) * chunksize] for i in range(nchunks)]
@@ -341,14 +340,15 @@
     if verbose > 0:
       print('Radon Time:',rdntime)
       print('Convolution Time:', convtime)
       print('Peak ID Time:', lmaxtime)
       print('Band Label Time:', blabeltime)
       print('Total Band Find Time:',tottime)
     if verbose > 1:
+      plt.clf()
 
       if len(rdnConv.shape) == 3:
         im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
       else:
         im2show = rdnConv[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
 
       rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
@@ -367,22 +367,22 @@
       plt.imshow(im2show, cmap='gray', extent=[self.radonPlan.theta.min(), self.radonPlan.theta.max(),
                                                self.radonPlan.rho.min(), self.radonPlan.rho.max()],
                  interpolation='none', zorder=1, aspect='auto')
       width = bandData['width'][-1, :]
       width /= width.min()
       width *= 2
       xplt = np.squeeze(
-        180.0 - np.interp(bandData['aveloc'][-1, :, 1]+0.5, np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
+        180.0 - np.interp(bandData['aveloc'][-1, :, 1], np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
       yplt = np.squeeze(
-        -1.0 * np.interp(bandData['aveloc'][-1, :, 0]-0.5, np.arange(self.radonPlan.nRho), self.radonPlan.rho))
+        -1.0 * np.interp(bandData['aveloc'][-1, :, 0], np.arange(self.radonPlan.nRho), self.radonPlan.rho))
 
       plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
 
       for pt in range(self.nBands):
-        plt.annotate(str(pt + 1), np.squeeze([xplt[pt]+4, yplt[pt]]), color='yellow')
+        plt.annotate(str(pt + 1), np.squeeze([xplt[pt], yplt[pt]]), color='yellow')
       plt.xlim(0,180)
       plt.ylim(-self.rhoMax, self.rhoMax)
 
 
     return bandData
 
   def radonPad(self,radon,rPad=0,tPad = 0, mirrorTheta = True):
@@ -438,15 +438,15 @@
       radon[0:self.padding[0], :,:] = radon[self.padding[0],:,:].reshape(1,shp[1], shp[2])
       radon[-self.padding[0]:, :,:] = radon[-self.padding[0]-1, :,:].reshape(1, shp[1],shp[2])
 
 
     rdnConv = np.zeros_like(radon)
 
     for i in range(shp[2]):
-      rdnConv[:,:,i] = -1.0 * scipyndim.gaussian_filter(np.squeeze(radon[:,:,i]),[self.rSigma,self.tSigma],order=[2,0])
+      rdnConv[:,:,i] = -1.0 * gaussian_filter(np.squeeze(radon[:,:,i]),[self.rSigma,self.tSigma],order=[2,0])
 
     #print(rdnConv.min(),rdnConv.max())
     mns = (rdnConv[self.padding[0]:shprdn[1]-self.padding[0],self.padding[1]:shprdn[1]-self.padding[1],:]).min(axis=0).min(axis=0)
 
     rdnConv -= mns.reshape((1,1, shp[2]))
     rdnConv = rdnConv.clip(min=0.0)
 
@@ -454,15 +454,15 @@
 
   def rdn_local_max(self, rdn, clparams=None, rdn_gpu=None, use_gpu=False):
 
     shp = rdn.shape
     # find the local max
     lMaxK = (self.peakPad[0],self.peakPad[1],1)
 
-    lMaxRdn = scipyndim.grey_dilation(rdn,size=lMaxK)
+    lMaxRdn = scipy_grey_dilation(rdn,size=lMaxK)
     #lMaxRdn[:,:,0:self.peakPad[1]] = 0
     #lMaxRdn[:,:,-self.peakPad[1]:] = 0
     #location of the max is where the local max is equal to the original.
     lMaxRdn = lMaxRdn == rdn
 
     rhoMaskTrim = np.int32((shp[0] - 2 * self.padding[0]) * self.rhoMaskFrac + self.padding[0])
     lMaxRdn[0:rhoMaskTrim,:,:] = 0
@@ -558,20 +558,16 @@
         dxx = nn[1,2] + nn[1,0] - 2 * nn[1,1]
         dyy = nn[2,1] + nn[0,1] - 2 * nn[1,1]
         dxy = 0.25*(nn[2,2] - nn [0,2] - nn[2,0] + nn[0,0])
         #det = 1.0 / (dxx * dyy - dxy * dxy)
         det = (dxx * dyy - dxy * dxy)
         det = det if np.fabs(det) > 1e-12 else 1.0e-12
         det = 1.0/det
-        dc =  (dyy * dx - dxy * dy) * det
-        rc = (dxx * dy - dxy * dx) * det
-        dc = max(-1.0, dc) ; rc = max(-1.0, rc)
-        dc = min(1.0, dc) ;  rc = min(1.0, rc)
-        cnn = c - dc
-        rnn = r - rc
+        cnn = c - (dyy * dx - dxy * dy) * det
+        rnn = r - (dxx * dy - dxy * dx) * det
         bandData_aveloc[q,i,:] = np.array([rnn,cnn])
         bandData_valid[q,i] = 1
 
     return bandData_max,bandData_avemax,bandData_maxloc,bandData_aveloc, bandData_valid, bandData_width
 
 def getopenclparam(**kwargs): # dummy function to maintain compatability with openCL version
   return None
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/band_vote.py` & `pyebsdindex-0.2.dev0/pyebsdindex/band_vote.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 environ["NUMBA_CACHE_DIR"] = str(tempdir)
 
 
 class BandVote:
   def __init__(self, tripLib, angTol=3.0, high_fidelity=True):
     self.tripLib = tripLib
     self.phase_name = self.tripLib.phaseName
-    self.phase_sym = self.tripLib.pointgroup
+    self.phase_sym = self.tripLib.symmetry_pg
     self.lattice_param = self.tripLib.latticeParameter
     self.angTol = angTol
     self.n_band_early_exit = 8
     self.high_fidelity = high_fidelity
     # these lookup tables are used to order the index for the pole-family when
     # sorting triplet angles from low to high.
     LUTA = np.array([[0,1,2],[0,2,1],[1,0,2],[1,2,0],[2,0,1],[2,1,0]],dtype=np.int64)
@@ -56,15 +56,15 @@
     LUT = np.zeros((3,3,3,3),dtype=np.int64)
     for i in range(6):
       LUT[:,LUTA[i,0],LUTA[i,1],LUTA[i,2]] = LUTB[i,:]
     self.LUT = np.asarray(LUT).copy()
 
   def tripvote(self, band_norms, band_intensity = None, goNumba = True, verbose=0):
     tic0 = timer()
-    nfam = self.tripLib.polefamilies.shape[0]
+    nfam = self.tripLib.family.shape[0]
     bandnorms = np.squeeze(band_norms)
     n_bands = np.int64(bandnorms.size/3)
     if band_intensity is None:
       band_intensity = np.ones((n_bands))
     tic = timer()
     bandangs = np.abs(bandnorms.dot(bandnorms.T))
     bandangs = np.clip(bandangs, -1.0, 1.0)
@@ -139,35 +139,35 @@
     polematch = np.array([-1])
     whGood = -1
 
     angTable = self.tripLib.completelib['angTable']
     sztable = angTable.shape
     famIndx = self.tripLib.completelib['famIndex']
     nFam = self.tripLib.completelib['nFamily']
-    polesCart = self.tripLib.completelib['polesCart']
+    poles = self.tripLib.completelib['polesCart']
     angTol = self.angTol
     n_band_early = np.int64(self.n_band_early_exit)
 
     # this will check the vote, and return the exact band matching to specific poles of the best fitting solution.
     fit, polematch, nMatch, whGood, ij, R, fitb = \
-      self.band_index_nb(polesCart, bandRank_arg, bandFam, famIndx, nFam, angTable, bandnorms, angTol, n_band_early)
+      self.band_index_nb(poles, bandRank_arg, bandFam,  famIndx, nFam, angTable, bandnorms, angTol, n_band_early)
 
     if verbose > 2:
       print('band index: ',timer() - tic)
     tic = timer()
 
     cm2 = 0.0
     if nMatch >=2:
       if self.high_fidelity == True:
 
         srt = np.argsort(fitb[whGood])
         whgood6 = whGood[srt[0:np.min([8, whGood.shape[0]])]]
 
         weights6 = band_intensity[whgood6]
-        pflt6 = (np.asarray(polesCart[polematch[whgood6], :], dtype=np.float64))
+        pflt6 = (np.asarray(poles[polematch[whgood6], :], dtype=np.float64))
         bndnorm6 = (np.asarray(bandnorms[whgood6, :], dtype=np.float64))
 
         avequat, fit = self.refine_orientation_quest(bndnorm6, pflt6 , weights=weights6)
         fit = np.arccos(np.clip(fit, -1.0, 1.0))*RADEG
         #avequat, fit = self.refine_orientation(bandnorms,whGood,polematch)
       else:
         avequat = rotlib.om2qu(R)
@@ -275,27 +275,27 @@
 
 
     fit = np.mean(test)
 
     #print('fitting: ',timer() - tic)
     return avequat, fit
 
-  def refine_orientation_quest(self, bandnorms, polecartmatch, weights = None):
+  def refine_orientation_quest(self,bandnorms, polematch, weights = None):
     tic = timer()
 
 
     if weights is None:
       weights = np.ones((bandnorms.shape[0]), dtype=np.float64)
     weightsn = np.asarray(weights, dtype=np.float64)
     weightsn /= np.sum(weightsn)
     #print(weightsn)
-    pflt = np.asarray(polecartmatch, dtype=np.float64)
+    pflt = np.asarray(polematch, dtype=np.float64)
     bndnorm = np.asarray(bandnorms, dtype=np.float64)
 
-    avequat, fit = self.orientation_quest_nb(pflt, bndnorm, weightsn)
+    avequat, fit = self.orientation_quest(pflt, bndnorm, weightsn)
 
     return avequat, fit
 
 
   @staticmethod
   @numba.jit(nopython=True, cache=True,fastmath=True,parallel=False)
   def tripvote_numba( bandangs, LUT, angTol, tripAngles, tripID, nfam, n_bands):
@@ -369,26 +369,26 @@
       bandFam[q] = np.argmax(accumulator[:,q])
     bandRank = (n_bands - np.arange(n_bands)) / n_bands * band_cm * mxvote
 
     return accumulator, bandFam, bandRank, band_cm
 
   @staticmethod
   @numba.jit(nopython=True, cache=True, fastmath=True,parallel=False)
-  def band_index_nb(polesCart, bandRank_arg, familyLabel, famIndx, nFam, angTable, bandnorms, angTol, n_band_early):
+  def band_index_nb(poles, bandRank_arg, familyLabel,  famIndx, nFam, angTable, bandnorms, angTol, n_band_early):
     eps = np.float32(1.0e-12)
     nBnds = bandnorms.shape[0]
 
     whGood_out = np.zeros(nBnds, dtype=np.int64)-1
 
 
     nMatch = np.int64(-1)
     Rout = np.zeros((1,3,3), dtype=np.float32)
     #Rout[0,0,0] = 1.0; Rout[0,1,1] = 1.0; Rout[0,2,2] = 1.0
     polematch_out = np.zeros((nBnds),dtype=np.int64) - 1
-    pflt = np.asarray(polesCart, dtype=np.float32)
+    pflt = np.asarray(poles, dtype=np.float32)
     bndnorm = np.transpose(np.asarray(bandnorms, dtype=np.float32))
 
     fit = np.float32(360.0)
     fitout = np.float32(360.0)
     fitbout = np.zeros((nBnds))
     R = np.zeros((1, 3, 3), dtype=np.float32)
     #fit = np.float32(360.0)
@@ -422,15 +422,15 @@
         wh01 = np.nonzero(np.abs(angTable[famIndx[f0],famIndx[f1]:np.int64(famIndx[f1] + nFam[f1])] - ang01) < angTol)[0]
 
         n01 = wh01.size
         if n01 == 0:
           continue
 
         wh01 += famIndx[f1]
-        p0 = polesCart[famIndx[f0], :]
+        p0 = poles[famIndx[f0],:]
 
         n01 = wh01.size
         v0v1c = np.cross(v0,v1)
         v0v1c /= np.linalg.norm(v0v1c)
         # attempt to see which solution gives the best match to all the poles
         # best is measured as the number of poles that are within tolerance,
         # divided by the angular deviation.
@@ -446,15 +446,15 @@
         B[0,:] = v0
         B[1,:] = v0v1c
         B[2,:] = b2
         A[:,0] = p0
         score = -1.0
 
         for i in range(n01):
-          p1 = polesCart[wh01[i], :]
+          p1 = poles[wh01[i],:]
           ntemp = np.linalg.norm(p1) + 1.0e-35
           p1 = p1 / ntemp
           p0p1c = np.cross(p0,p1)
           ntemp = np.linalg.norm(p0p1c) + 1.0e-35
           p0p1c = p0p1c / ntemp
           A[:,1] = p0p1c
           A[:,2] = np.cross(p0,p0p1c)
@@ -686,18 +686,20 @@
         else:  # the two are parallel - throwout the result.
           whgood2[counter] = np.float32(360.0)
           counter += 1
     return AB,whgood2
 
   @staticmethod
   @numba.jit(nopython=True, cache=True, fastmath=True, parallel=False)
-  def orientation_quest_nb(polescart, bandnorms, weights):
+  def orientation_quest(poles, bandnorms, weights):
     # this uses the Quaternion Estimator AKA quest algorithm.
 
-    pflt = np.asarray(polescart, dtype=np.float64)
+    #pflt = (np.asarray(poles[polematch[whGood], :], dtype=np.float32))
+    #bndnorm = (np.asarray(bandnorms[whGood, :], dtype=np.float32))
+    pflt = np.asarray(poles, dtype=np.float64)
     bndnorm = np.asarray(bandnorms, dtype=np.float64)
     npoles = pflt.shape[0]
     wn = (np.asarray(weights, dtype=np.float64)).reshape(npoles, 1)
 
     #wn = np.ones((nGood,1), dtype=np.float32)/np.float32(nGood)  #(weights[whGood]).reshape(nGood,1)
     wn /= np.sum(wn)
 
@@ -744,15 +746,15 @@
 
     #polesrot = rotlib.quat_vectorL1N(q, pflt, npoles, np.float64, p=1)
     #pdot = np.sum(polesrot*bndnorm, axis = 1, dtype=np.float64)
     return q, lam#, pdot
 
   def pairVoteOrientation(self,bandnormsIN,goNumba=True):
     tic0 = timer()
-    nfam = self.tripLib.polefamilies.shape[0]
+    nfam = self.tripLib.family.shape[0]
     bandnorms = np.squeeze(bandnormsIN)
     n_bands = np.int64(bandnorms.size / 3)
 
     bandangs = np.abs(bandnorms.dot(bandnorms.T))
     bandangs = np.clip(bandangs,-1.0,1.0)
     bandangs = np.arccos(bandangs) * RADEG
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/crystallometry.py` & `pyebsdindex-0.2.dev0/pyebsdindex/crystallometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,16 +78,14 @@
         ca = np.cos(alpha*np.pi/180)
         cb = np.cos( beta*np.pi/180)
         cg = np.cos(gamma*np.pi/180)
         sa = np.sin(alpha*np.pi/180)
         sb = np.sin( beta*np.pi/180)
         sg = np.sin(gamma*np.pi/180)
         tg = np.tan(gamma*np.pi/180)
-        fabg = ca*cb-cg
-
 
         #compute the real space metric tensor
         self.metricTensor = np.zeros([3,3])
         self.metricTensor[0,0] = a**2.0
         self.metricTensor[1,1] = b**2.0
         self.metricTensor[2,2] = c**2.0
         self.metricTensor[1,0] = a*b*cg
@@ -125,28 +123,14 @@
         self.directStructureMatrix[1,1] = b*sg
         self.directStructureMatrix[2,1] = -c*(cb*cg-ca)/sg
         self.directStructureMatrix[0,2] = 0.0
         self.directStructureMatrix[1,2] = 0.0
         self.directStructureMatrix[2,2] = self.volume/(a*b*sg)
         self.directStructureMatrix = self.directStructureMatrix.transpose()
         self.directStructureMatrix[np.abs(self.directStructureMatrix) < smallThreshold] = 0
-
-        # Compute inverse direct stucture matrix
-        self.invDirectStructureMatrix = np.zeros([3, 3])
-        self.invDirectStructureMatrix[0, 0] = 1.0/a
-        self.invDirectStructureMatrix[1, 0] = -1.0/(a * tg)
-        self.invDirectStructureMatrix[2, 0] = b*c * (cg*ca-cb)/(self.volume * sg)
-        self.invDirectStructureMatrix[0, 1] = 0.0
-        self.invDirectStructureMatrix[1, 1] = 1.0/(b * sg)
-        self.invDirectStructureMatrix[2, 1] = a*c*(cb*cg-ca)/(self.volume*sg)
-        self.invDirectStructureMatrix[0, 2] = 0.0
-        self.invDirectStructureMatrix[1, 2] = 0.0
-        self.invDirectStructureMatrix[2, 2] = a*b*sg/(self.volume)
-        self.invDirectStructureMatrix = self.invDirectStructureMatrix.transpose()
-        self.invDirectStructureMatrix[np.abs(self.invDirectStructureMatrix) < smallThreshold] = 0
         
         #compute reciprocal structure matrix
         self.reciprocalStructureMatrix = np.zeros([3,3])
         self.reciprocalStructureMatrix[0,0] = 1.0/a
         self.reciprocalStructureMatrix[1,0] = 0.0
         self.reciprocalStructureMatrix[2,0] = 0.0
         self.reciprocalStructureMatrix[0,1] = -1.0/(a*tg)
@@ -154,18 +138,14 @@
         self.reciprocalStructureMatrix[2,1] = 0.0
         self.reciprocalStructureMatrix[0,2] = b*c*(cg*ca-cb)/(self.volume*sg)
         self.reciprocalStructureMatrix[1,2] = a*c*(cb*cg-ca)/(self.volume*sg)
         self.reciprocalStructureMatrix[2,2] = (a*b*sg)/self.volume
         self.reciprocalStructureMatrix = self.reciprocalStructureMatrix.transpose()
         self.reciprocalStructureMatrix[np.abs(self.reciprocalStructureMatrix) < smallThreshold] = 0
 
-        # Compute inverse reciprocal stucture matrix
-        self.invReciprocalStructureMatrix = np.zeros([3, 3])
-        self.invReciprocalStructureMatrix = np.transpose(self.directStructureMatrix)
-
     # def get_lattice_centering(self):
     #     self.latticeCentering = self.spaceGroup[0]
 
     # def is_g_allowed(self,g):
     #     get_lattice_centering()
     #     allowed = True
     #     if lattice_centering == 'F':
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/ebsd_index.py` & `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-"""Setup and handling of Radon indexing runs of EBSD patterns."""
+"""Setup and handling of Hough indexing runs of EBSD patterns."""
 
 from pyebsdindex import _ray_installed
 from pyebsdindex._ebsd_index_single import EBSDIndexer, index_pats
 
 if _ray_installed:
-    from pyebsdindex._ebsd_index_parallel import index_pats_distributed
+    from pyebsdindex._ebsd_index_parallel import index_pats_distributed, IndexerRay
 
 
 __all__ = [
     "EBSDIndexer",
+    "IndexerRay",
     "index_pats",
     "index_pats_distributed",
 ]
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/ebsd_pattern.py` & `pyebsdindex-0.2.dev0/pyebsdindex/ebsd_pattern.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,39 +43,28 @@
   ftype = file_type
   if ftype == str(''):
     extension = str.lower(Path(filepath).suffix)
     if (extension == '.up1'):
       ftype = 'UP1'
     elif (extension == '.up2'):
       ftype = 'UP2'
-    elif (extension == '.ebsp'):
-      ftype = 'EBSP'
     elif (extension == '.oh5'):
       ftype = 'OH5'
     elif (extension == '.h5'):
       ftype = 'H5'
-    elif (extension == '.h5oina'):
-      ftype = 'H5OINA'
     else:
       raise ValueError('Error: extension not recognized')
 
   if (ftype.upper() == 'UP1') or (ftype.upper() == 'UP2'):
     ebsdfileobj = UPFile(path)
-  if (ftype.upper() == 'EBSP'):
-    ebsdfileobj = EBSPFile(path)
   if (ftype.upper() == 'OH5'):
     ebsdfileobj = EDAXOH5(path)
     if hdf5path is None: #automatically chose the first data group
       ebsdfileobj.get_data_paths()
       ebsdfileobj.set_data_path(pathindex=0)
-  if (ftype.upper() == 'H5OINA'):
-    ebsdfileobj = OXFORDOINA(path)
-    if hdf5path is None: #automatically chose the first data group
-      ebsdfileobj.get_data_paths()
-      ebsdfileobj.set_data_path(pathindex=0)
   if (ftype.upper() == 'H5'):
     ebsdfileobj = HDF5PatFile(path) # if the path variable is a list,
     # the second item is set to be the hdf5 path to the patterns.
     try:
       f = h5py.File(Path(pathtemp[0]).expanduser(),'r+')
     except:
       print("File Not Found:",str(Path(pathtemp[0])))
@@ -167,22 +156,20 @@
     self.filepath = None
     self.filetype = None
     self.patternW = None
     self.patternH = None
     self.nFileCols = None
     self.nFileRows = None
     self.nPatterns = None
-    self.hexflag = None
+    self.hexFlag = None
     self.xStep = None
     self.yStep = None
     self.patStart = [0,0] #starting point of the pattern location in the file. len==1
     # if 2D, then it is the row/column starting points
     self.patterns = None
-    self.xyLocations = None
-    # The x,y locations of the pattern collection relative to the center of the SEM field-of-view.
 
 
 
 
 # a class template for any EBSD pattern file type.
 # Any EBSD file class should inheret this class.
 class EBSDPatternFile():
@@ -191,18 +178,16 @@
     self.vendor = None
     self.version = None
     self.nCols = None
     self.nRows = None
     self.nPatterns = None
     self.patternW = None
     self.patternH = None
-    self.xStep = None  # assumming square grid data, with constant step size
+    self.xStep = None
     self.yStep = None
-    self.xyCenter = np.array([0.0, 0.0])
-    # This is the location of the center of the scan relative to center of SEM field-of-view
     self.hexflag = False
     self.filetype = filetype
     self.filedatatype = np.uint8  # the data type of the patterns within the file
 
   def set_filepath(self, path=None):
     if path is not None:
       ptemp = np.atleast_1d(path)
@@ -213,15 +198,15 @@
 
   def read_data(self,path=None,convertToFloat=False,patStartCount = [0,-1],returnArrayOnly=False):
     if path is not None:
       self.set_filepath(path)
       self.read_header()
     if self.version is None:
       self.read_header()
-    patStartCount = np.array(patStartCount, dtype=np.int64)
+
     # bitD = 8 * (self.bitdepth == 8) + 16 * (self.bitdepth == 16)
 
     # # this will allow for overriding the original file spec -- not sure why would want to but ...
     # if (bitdepth == 8):
     #   bitD = 8
     # if (bitdepth == 16):
     #   bitD = 16
@@ -235,84 +220,80 @@
     if convertToFloat == True:
       typeout = np.float32
     else:
       typeout = self.filedatatype
 
     pStartEnd = np.asarray(patStartCount, dtype=np.int64)
     if pStartEnd.ndim == 1: # read a continuous set of patterns.
-      patStart = int(patStartCount[0])
-      nPatToRead = int(patStartCount[-1])
+      patStart = patStartCount[0]
+      nPatToRead = patStartCount[-1]
       if nPatToRead == -1:
-        nPatToRead = int(self.nPatterns - patStart)
+        nPatToRead = self.nPatterns - patStart
       if nPatToRead == 0:
         nPatToRead = 1
       if (patStart + nPatToRead) > self.nPatterns:
-        nPatToRead = int(self.nPatterns - patStart)
+        nPatToRead = self.nPatterns - patStart
 
 
       # this function does the actual reading from the file.
-      readpats, xyloc = self.pat_reader(patStart, nPatToRead)
+      readpats = self.pat_reader(patStart, nPatToRead)
       patterns = readpats.astype(typeout)
 
 
 
     elif pStartEnd.ndim == 2: # read a slab of patterns.
-        colstart = int(pStartEnd[0,0])
-        ncolread = int(pStartEnd[1,0])
-        rowstart = int(pStartEnd[0,1])
-        nrowread = int(pStartEnd[1,1])
+        colstart = pStartEnd[0,0]
+        ncolread = pStartEnd[1,0]
+        rowstart = pStartEnd[0,1]
+        nrowread = pStartEnd[1,1]
 
         patStart = [colstart, rowstart]
         if ncolread < 0:
-          ncolread = int(self.nCols - colstart)
+          ncolread = self.nCols - colstart
         if nrowread < 0:
-          nrowread = int(self.nRows - rowstart)
+          nrowread = self.nRows - rowstart
 
         if (colstart+ncolread) > self.nCols:
-          ncolread = int(self.nCols - colstart)
+          ncolread = self.nCols - colstart
 
         if (rowstart+nrowread) > self.nRows:
-          nrowread = int(self.nRows - rowstart)
+          nrowread = self.nRows - rowstart
         nrowread = np.uint64(nrowread)
         ncolread = np.uint64(ncolread)
         nPatToRead = [ncolread, nrowread]
 
         patterns = np.zeros([int(ncolread*nrowread),self.patternH,self.patternW],dtype=typeout)
-        xyloc = np.zeros([int(ncolread*nrowread),2],dtype=np.float32)
 
         for i in range(nrowread):
-          pstart = int(int(int(rowstart+i)*self.nCols)+colstart)
-          ptemp, xyloctemp = self.read_data(convertToFloat=convertToFloat,patStartCount = [pstart,ncolread],returnArrayOnly=True)
+          pstart = int(((rowstart+i)*self.nCols)+colstart)
+          ptemp = self.read_data(convertToFloat=convertToFloat,patStartCount = [pstart,ncolread],returnArrayOnly=True)
 
           patterns[int(i*ncolread):int((i+1)*ncolread), :, :] = ptemp
-          xyloc[int(i*ncolread):int((i+1)*ncolread), :] = xyloctemp
 
     if returnArrayOnly == True:
-      return patterns, xyloc
+      return patterns
     else:  # package this up in an EBSDPatterns Object
       patsout = EBSDPatterns()
       patsout.vendor = self.vendor
       patsout.file = Path(self.filepath).expanduser()
       patsout.filetype = self.filetype
       patsout.patternW = self.patternW
       patsout.patternH = self.patternH
-      patsout.nFileCols = np.uint64(self.nCols)
-      patsout.nFileRows = np.uint64(self.nRows)
+      patsout.nFileCols = self.nCols
+      patsout.nFileRows = self.nRows
       patsout.nPatterns = np.array(nPatToRead)
-      patsout.hexflag = self.hexflag
+      patsout.hexFlag = self.hexFlag
       patsout.xStep = self.xStep
       patsout.yStep = self.yStep
       patsout.patStart = np.array(patStart)
       patsout.patterns = patterns
-      patsout.xyLocations = xyloc
       return patsout # note this function uses multiple return statements
 
-  def pat_reader(self, patStart=0, nPatToRead=1):
-    '''Depending on the file type, it will return a numpy array of patterns, and the positions of the patterns
-    in the scan.'''
+  def pat_reader(self, patStart, nPatToRead):
+    '''Depending on the file type, it will return a numpy array of patterns.'''
     pass
 
   def write_header(self):
     pass
 
   def write_data(self, newpatterns=None, patStartCount = [0,-1], writeHead=False,
                  flt2int='clip', scalevalue = 0.98, maxScale = None):
@@ -342,49 +323,49 @@
       max = maxScale
 
     pStartEnd = np.asarray(patStartCount)
     # npats == number of patterns in the newpatterns
     # self.nPatterns == number of patterns in the file
     # nPats to write == number of patterns to write out
     if pStartEnd.ndim == 1:  # write a continuous set of patterns.
-      patStart = int(patStartCount[0])
-      nPatToWrite = int(patStartCount[-1])
+      patStart = patStartCount[0]
+      nPatToWrite = patStartCount[-1]
       if nPatToWrite == -1:
         nPatToWrite = npats
       if nPatToWrite == 0:
         nPatToWrite = 1
       if (patStart + nPatToWrite) > self.nPatterns:
         nPatToWrite = self.nPatterns - patStart
 
       typewrite = self.filedatatype
       pat2write = pat_flt2int(pats,typeout=typewrite,method=flt2int,scalevalue=scalevalue,maxScale=None)
       self.pat_writer(pat2write,patStart,nPatToWrite, typewrite)
 
     elif pStartEnd.ndim == 2: # write a slab of patterns.
-        colstart = int(pStartEnd[0,0])
-        ncolwrite = int(pStartEnd[1,0])
-        rowstart = int(pStartEnd[0,1])
-        nrowwrite = int(pStartEnd[1,1])
+        colstart = pStartEnd[0,0]
+        ncolwrite = pStartEnd[1,0]
+        rowstart = pStartEnd[0,1]
+        nrowwrite = pStartEnd[1,1]
 
         patStart = [colstart, rowstart]
         if ncolwrite < 0:
-          ncolwrite = int(self.nCols - colstart)
+          ncolwrite = self.nCols - colstart
         if nrowwrite < 0:
-          nrowwrite = int(self.nRows - rowstart)
+          nrowwrite = self.nRows - rowstart
 
         if (colstart+ncolwrite) > self.nCols:
-          ncolwrite = int(self.nCols - colstart)
+          ncolwrite = self.nCols - colstart
 
         if (rowstart+nrowwrite) > self.nRows:
-          nrowwrite = int(self.nRows - rowstart)
+          nrowwrite = self.nRows - rowstart
 
 
         for i in range(nrowwrite):
-          pstart = int(int(int(rowstart+i)*self.nCols)+colstart)
-          self.write_data(newpatterns = pats[int(i*ncolwrite):int((i+1)*ncolwrite), :, :], patStartCount=[pstart,ncolwrite],writeHead=False,
+          pstart = ((rowstart+i)*self.nCols)+colstart
+          self.write_data(newpatterns = pats[i*ncolwrite:(i+1)*ncolwrite, :, :], patStartCount=[pstart,ncolwrite],writeHead=False,
                           flt2int=flt2int,scalevalue=0.98, maxScale = max)
   def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite):
     pass
 
 
   def copy_file(self, newpath, **kwargs):
     src = Path(self.filepath).expanduser().resolve()
@@ -395,31 +376,31 @@
       dst = Path(str(src.expanduser().resolve())+'.copy')
     shutil.copyfile(src,dst)
 
   def copy_obj(self):
     return copy.deepcopy(self)
 
   def set_scan_rc(self, rc=(0,0)): # helper function for pattern files that don't record the scan rows and columns
-    self.nCols = np.uint64(rc[1])
-    self.nRows = np.uint64(rc[0])
-    self.nPatterns = np.uint64(self.nCols * self.nRows)
+    self.nCols = rc[1]
+    self.nRows = rc[0]
+    self.nPatterns = self.nCols * self.nRows
 
 
 class UPFile(EBSDPatternFile):
 
   def __init__(self, path=None):
     EBSDPatternFile.__init__(self, path)
     self.filetype = 'UP'
     self.vendor = 'EDAX'
     self.filedatatype = None
     #UP only attributes
     #self.bitdepth = None
     self.filePos = None  # file location in bytes where pattern data starts
     self.extraPatterns = 0
-    self.hexflag = 0
+    self.hexFlag = 0
 
 
   def read_header(self,path=None,bitdepth=None):  # readInterval=[0, -1], arrayOnly=False,
     if path is not None:
       self.filepath = path
 
     extension = str.lower(Path(self.filepath).suffix)
@@ -450,45 +431,35 @@
 
     self.version = np.fromfile(f, dtype=np.uint32, count=1)[0]
     if self.version == 1:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
-      self.nPatterns = int((Path(self.filepath).expanduser().stat().st_size - 16) /
+      self.nPatterns = np.int((Path(self.filepath).expanduser().stat().st_size - 16) /
                               (self.patternW * self.patternH * (self.filedatatype(0).nbytes)))
-      if self.xStep is None:
-        self.xStep = 0.0
-      if self.yStep is None:
-        self.yStep = 0.0
-      if self.nCols is None:
-        self.nCols = np.uint64(1)
-      if self.nCols == 0:
-        self.nCols = np.uint64(1)
-      if self.nRows is None:
-        self.nRows = np.uint64(np.floor(self.nPatterns/self.nCols))
 
     elif self.version >= 3:
       dat = np.fromfile(f, dtype=np.uint32, count=3)
       self.patternW = dat[0]
       self.patternH = dat[1]
       self.filePos = dat[2]
       self.extraPatterns = np.fromfile(f, dtype=np.uint8, count=1)[0]
       dat = np.fromfile(f, dtype=np.uint32, count=2)
-      self.nCols = np.uint64(dat[0])
-      self.nRows = np.uint64(dat[1])
-      self.nPatterns = int(self.nCols.astype(np.uint64) * self.nRows.astype(np.uint64))
-      self.hexflag = np.fromfile(f, dtype=np.uint8, count=1)[0]
+      self.nCols = dat[0]
+      self.nRows = dat[1]
+      self.nPatterns = np.int(self.nCols.astype(np.uint64) * self.nRows.astype(np.uint64))
+      self.hexFlag = np.fromfile(f, dtype=np.uint8, count=1)[0]
       dat = np.fromfile(f, dtype=np.float64, count=2)
       self.xStep = dat[0]
       self.yStep = dat[1]
     f.close()
     return 0 #note this function uses multiple returns
 
-  def pat_reader(self, patStart=0, nPatToRead=1):
+  def pat_reader(self, patStart, nPatToRead):
     try:
       f = open(Path(self.filepath).expanduser(),'rb')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
     f.seek(self.filePos)
@@ -496,23 +467,15 @@
     typeread = self.filedatatype
     typebyte = self.filedatatype(0).nbytes
 
     f.seek(int(nPerPat * patStart * typebyte),1)
     readpats = np.fromfile(f,dtype=typeread,count=int(nPatToRead * nPerPat))
     readpats = readpats.reshape(nPatToRead,self.patternH,self.patternW)
     f.close()
-    yx = np.unravel_index(np.arange(int(patStart), int(patStart+nPatToRead), dtype = np.uint64),
-                          (int(self.nRows), int(self.nCols)))
-
-    xyloc = np.array([yx[1],yx[0]]).T.copy().astype(np.float32)
-    xyloc[:,0] -= self.nCols * 0.5
-    xyloc[:, 1] -= self.nRows * 0.5
-    xyloc[:,0] *= self.xStep
-    xyloc[:,1] *= self.yStep
-    return readpats, xyloc
+    return readpats
 
 
   def write_header(self, writeBlank=False, bitdepth=None):
 
     filepath = self.filepath
     extension = str.lower(Path(filepath).suffix)
     try:
@@ -541,35 +504,28 @@
       else:
         f = open(Path(filepath).expanduser(),'w+b')
         f.seek(0)
     except:
       print("File Not Found:", str(Path(filepath)))
       return -1
 
-    if self.version is None:
-      self.version = 3
-
     np.asarray(self.version, dtype=np.uint32).tofile(f)
     if self.version == 1:
-      if self.filePos is None:
-        self.filePos = 16
       np.asarray(self.patternW,dtype=np.uint32).tofile(f)
       np.asarray(self.patternH,dtype=np.uint32).tofile(f)
       np.asarray(self.filePos,dtype=np.uint32).tofile(f)
 
     elif self.version >= 3:
-      if self.filePos is None:
-        self.filePos = 42
       np.asarray(self.patternW,dtype=np.uint32).tofile(f)
       np.asarray(self.patternH,dtype=np.uint32).tofile(f)
       np.asarray(self.filePos,dtype=np.uint32).tofile(f)
       np.asarray(self.extraPatterns,dtype=np.uint8).tofile(f)
       np.asarray(self.nCols,dtype=np.uint32).tofile(f)
       np.asarray(self.nRows,dtype=np.uint32).tofile(f)
-      np.asarray(self.hexflag,dtype=np.uint8).tofile(f)
+      np.asarray(self.hexFlag,dtype=np.uint8).tofile(f)
       np.asarray(self.xStep,dtype=np.float64).tofile(f)
       np.asarray(self.yStep,dtype=np.float64).tofile(f)
 
     if writeBlank == True:
       typewrite = self.filedatatype
       # if self.bitdepth == 8:
       #   type = np.uint8
@@ -581,44 +537,40 @@
         for i in range(self.nCols):
           blank.tofile(f)
     f.close()
 
 
   def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite):
     try:
-      with open(Path(self.filepath).expanduser(),'br+') as f:
-        #print(patStart)
-        f.seek(0,0)
-        nPerPat = int(self.patternW * self.patternH)
-        nPerPatByte = int(nPerPat * typewrite(0).nbytes)
-        f.seek(int(nPerPatByte * (patStart) + self.filePos), 0)
-        pat2write[0:nPatToWrite, :, :].tofile(f)
-        #print(patStart)
-    except Exception as e:
-      print(e)
-      print(str(Path(self.filepath)))
+      f = open(Path(self.filepath).expanduser(),'br+')
+      f.seek(0,0)
+    except:
+      print("File Not Found:",str(Path(self.filepath)))
       return -1
 
-
-
+    nPerPat = self.patternW * self.patternH
+    nPerPatByte = nPerPat * typewrite(0).nbytes
+    f.seek(int(nPerPatByte * (patStart) + self.filePos),0)
+    pat2write[0:nPatToWrite,:,:].tofile(f)
+    f.close()
 
 
 
   def file_from_pattern_obj(self, patternobj, filepath=None, bitdepth = None):
     if self.version is None:
       self.version = 3
     if self.xStep is None:
       self.xStep = 1.0
     if self.yStep is None:
       self.yStep = 1.0
 
 
     self.filePos = 42  # file location in bytes where pattern data starts
     self.extraPatterns = 0
-    self.hexflag = 0
+    self.hexFlag = 0
 
     if isinstance(patternobj, EBSDPatterns):
       shp = (patternobj.nPatterns.prod(),patternobj.patternH,patternobj.patternW)
       mx = patternobj.patterns.max()
     elif isinstance(patternobj, np.ndarray):
       shp = patternobj.shape
       mx = patternobj.max()
@@ -626,427 +578,22 @@
       if ndim == 2: #
         shp = (1,shp[0], shp[1])
       elif ndim == 3:
         shp = shp
     self.patternH = shp[1]
     self.patternW = shp[2]
 
-    self.nCols = np.uint64(shp[0])
-    self.nRows = np.uint64(1)
-    self.nPatterns = np.uint64(shp[0])
+    self.nCols = shp[0]
+    self.nRows = 1
+    self.nPatterns = shp[0]
 
     if bitdepth is None: #make a guess
       self.bitdepth = 16
       if mx <= 256:
         self.bitdepth = 8
-  def copy_file(self, newpath, **kwargs):
-    src = Path(self.filepath).expanduser().resolve()
-    if newpath is not None:
-      path = np.atleast_1d(newpath)
-      dst = Path(path[0]).expanduser().resolve()
-    else:
-      dst = Path(str(src.expanduser().resolve())+'.copy')
-    try:
-      if 'empty_data' in kwargs:
-        if kwargs['empty_data'] == True:
-          with open(src, 'rb') as srcf:
-            head = srcf.read(self.filePos)
-            size = srcf.seek(0, 2)
-            #print('checkpoint' ,size)
-          with open(dst, 'wb') as dstf:
-            head = dstf.write(head)
-            #print('write head')
-            dstf.seek(size-1,0)
-            #print('seek done')
-            dstf.write(b"\0")
-          return
-    except:
-      pass
-    shutil.copyfile(src,dst)
-
-class EBSPFile(EBSDPatternFile):
-  """
-    Notes
-    -----
-    Information about the .ebsp file format was generously provided by
-    Oxford Instruments.
-    """
-  def __init__(self, path=None):
-    EBSDPatternFile.__init__(self, path)
-    self.filetype = 'EBSP'
-    self.vendor = 'OXFORD'
-    self.filedatatype = None
-    # EBSP only attributes
-    # self.bitdepth = None
-    self.filePos = None  # file location in bytes where each pattern data starts
-    self.hasxypos = False
-
-  def read_header(self, path=None, bitdepth=None):  # readInterval=[0, -1], arrayOnly=False,
-    if path is not None:
-      self.filepath = path
-
-    try:
-      f = open(Path(self.filepath).expanduser(), 'rb')
-    except:
-      print("File Not Found:", str(Path(self.filepath)))
-      return -1
-
-    f.seek(0)
-    version = np.fromfile(f, dtype=np.int64, count=1)
-    version = int(-1*version)
-    if version <= 0:
-      self.version = 0
-    else:
-      self.version = version
-
-    per_pat_header = 4
-    if self.version >= 5:
-      per_pat_header = 6
-
-    if self.version >= 1:
-      memoffset = 8
-      if self.version >= 4:
-        self.mysterybyte = np.fromfile(f, dtype=np.uint8, count=1)
-        memoffset = 9
-      #loc0 = int(np.fromfile(f, dtype=np.uint64, count=1))
-      #currentloc = f.tell()
-      #loc1 = loc0
-      #npat = 0
-
-      #while loc1 != currentloc:
-      #  loc11 = int(np.fromfile(f, dtype=np.uint64, count = 1))
-      #  loc1 = min([loc1, loc11])
-      #  currentloc = f.tell()
-
-      # do the same as above, but in memory ... so much faster
-      loc0 = 0
-      counter = 0
-      while loc0 == 0: # check for non-stored points.
-        loc0 = int(np.fromfile(f, dtype=np.uint64, count=1))
-        counter += 1
-      f.seek(-8*counter, 1) # move back 8 bytes (or however far we needed to move into the file to find a legitamte offset.
-
-      loc02N = np.fromfile(f, dtype=np.uint64, count=int((loc0)/8+0.001))
-
-
-      if self.version <=4:
-        loc1 = int((loc0-memoffset)/8+0.001)
-
-        counter = 0
-        while loc1 != counter:
-          if loc02N[counter] != 0:  # a non-stored pattern? Crazy.
-            loc_i = int((loc02N[counter]-memoffset)/8)
-            loc1 = min([loc1, loc_i])
-          counter += 1
-
-
-        self.nPatterns = int((counter))
-      elif self.version == 5:
-        f.seek(loc02N[0], 0)
-        patdata = np.fromfile(f, dtype=np.uint32, count=per_pat_header)
-        if patdata[0] == 1:
-          print("Sorry, compressed EBSP files are not supported")
-          return None
-        patternW = int(patdata[-2])
-        patternH = int(patdata[-3])
-        magic_indx = patternH + (patternW << 32)
-        wh = np.nonzero(loc02N == magic_indx)
-        self.nPatterns = wh[0].min()
-
-
-
-      if self.version == 0:
-        f.seek(0)
-      if self.version >=1.0:
-        f.seek(8)
-      if self.version >= 4:
-        f.seek(1,1)
-
-
-
-      self.filePos = np.fromfile(f, dtype=np.uint64, count=self.nPatterns)
-
-      # going to assume that all patterns are the same as the first pattern the file.
-      f.seek(self.filePos[0])
-      #patdata = np.fromfile(f, dtype=np.uint32, count=4)
-      #patdata0 = np.fromfile(f, dtype=np.uint8, count=1)
-
-      #patdata = np.fromfile(f, dtype=np.uint32, count=4)
-
-      patdata = np.fromfile(f, dtype=np.uint32, count=per_pat_header)
-
-      if patdata[0] == 1:
-        print("Sorry, compressed EBSP files are not supported")
-        return None
-
-      #print(loc0, patdata)
-      #f.seek(self.filePos[2])
-      #print(np.fromfile(f, dtype=np.uint32, count=4))
-      #print(np.fromfile(f, dtype=np.uint32, count=8))
-      #print(np.fromfile(f, dtype=np.uint32, count=1))
-
-      self.patternW = np.uint32(patdata[-2])
-      self.patternH = np.uint32(patdata[-3])
-      nbytespat = patdata[-1]
-
-
-      #if self.version == 1:
-      bitdepth = nbytespat / (self.patternW * self.patternH) * 8
-      #elif self.version >= 2:
-      #bitdepth = nbytespat
-
-      if bitdepth == 8:
-        self.filedatatype = np.uint8
-      if bitdepth == 16:
-        self.filedatatype = np.uint16
-      if bitdepth == 32:
-        self.filedatatype = np.uint32
-
-
-      #self.nPatterns = int(
-      #                (Path(self.filepath).expanduser().stat().st_size - int(8)) /
-      #                        (24 + 18 +
-      #                         int(self.patternW) * int(self.patternH) * int(self.filedatatype(0).nbytes)))
-
-      #print(self.nPatterns)
-
-
-
-      xall = np.zeros(self.nPatterns, dtype=np.float64)
-      yall = np.zeros(self.nPatterns, dtype=np.float64)
-      self.hasxypos = False
-      if self.version != 0:
-        if self.version ==1:
-          footoffset = 0
-          self.hasxypos = True
-        else:
-          loc0 = np.min(self.filePos[self.filePos > 0])
-          f.seek(int(loc0 + 4*per_pat_header + nbytespat))
-          havepos = np.fromfile(f, dtype=np.uint8, count=1)
-          if havepos > 0:
-            footoffset = 1
-            self.hasxypos = True
-
-      if self.hasxypos == False:
-        self.xStep = 1.0
-        self.yStep = 1.0
-        self.nCols = 1
-        self.nRows = self.nPatterns
-      else:
-        for i in range(self.nPatterns):
-          if self.filePos[i] > 0:
-            f.seek(int(self.filePos[i] + 4*per_pat_header + nbytespat + footoffset))
-
-            x1 = np.fromfile(f, dtype=np.float64, count=1)
-            #print(x1, i)
-            xall[i] = x1
-            f.seek(footoffset, 1)
-            yall[i] = np.fromfile(f, dtype=np.float64, count=1)
-
-
-        self.xStep = xall[1] - xall[0]
-        if self.xStep > 1e-6:
-          ncol = (xall.max() - xall.min()) / self.xStep
-          ncol = np.round(ncol+1)
-        else:
-          ncol = 1
-
-        self.nCols = np.uint64(ncol)
-
-
-        self.yStep = yall[0] - yall[self.nCols]
-
-        if self.yStep > 1e-6:
-          nrow = (yall.max() - yall.min()) / self.yStep
-          nrow = np.round(nrow+1)
-          self.nRows = int(nrow)
-        else:
-          self.nRows = int(self.nPatterns/self.nCols+0.001)
-
-      if self.xStep is None:
-        self.xStep = 1.0
-      if self.yStep is None:
-        self.yStep = 1.0
-      if self.nCols is None:
-        self.nCols = np.uint64(1)
-      if self.nCols == 0:
-        self.nCols = np.uint64(1)
-      if self.nRows is None:
-        self.nRows = np.uint64(np.floor(self.nPatterns / self.nCols))
-    f.close()
-
-    return 0  # note this function uses multiple returns
-
-  def pat_reader(self, patStart=0, nPatToRead=1):
-    try:
-      f = open(Path(self.filepath).expanduser(), 'rb')
-    except:
-      print("File Not Found:", str(Path(self.filepath)))
-      return -1
-
-    readpats = np.zeros((nPatToRead, self.patternH * self.patternW), dtype=self.filedatatype)
-    xyloc = np.zeros((nPatToRead, 2), dtype=np.float64)
-    # f.seek(self.filePos)
-    nPerPat = self.patternW * self.patternH
-    typeread = self.filedatatype
-    typebyte = self.filedatatype(0).nbytes
-
-    readxypos = self.hasxypos
-    if self.version == 1:
-      xyoffset = 0
-    else:
-      xyoffset = 1
-
-    per_pat_head = 16
-    if self.version >= 5:
-      per_pat_head = 24
-
-    for i in range(int(patStart), int(patStart + nPatToRead)):
-      ii = int(i - patStart)
-      if self.filePos[i] > 0:
-        f.seek(int(self.filePos[i] + per_pat_head))
-        readpats[ii, :] = np.fromfile(f, dtype=typeread, count=int(nPerPat))
-        if readxypos == True:
-          f.seek(xyoffset, 1)
-          xyloc[ii, 0] = np.fromfile(f, dtype=np.float64, count=1)
-          f.seek(xyoffset, 1)
-          xyloc[ii, 1] = np.fromfile(f, dtype=np.float64, count=1)
-
-    readpats = readpats.reshape(nPatToRead, self.patternH, self.patternW)
-    f.close()
-
-    # yx = np.unravel_index(np.arange(int(patStart), int(patStart+nPatToRead), dtype = np.uint64),
-    #                       (int(self.nRows), int(self.nCols)))
-
-    # xyloc = np.array([yx[1],yx[0]]).T.copy().astype(np.float32)
-    # xyloc[:,0] -= self.nCols * 0.5
-    # xyloc[:, 1] -= self.nRows * 0.5
-    # xyloc[:,0] *= self.xStep
-    # xyloc[:,1] *= self.yStep
-    return readpats, xyloc
-
-  def write_header(self, writeBlank=False, bitdepth=8):
-
-    filepath = self.filepath
-    extension = str.lower(Path(filepath).suffix)
-    try:
-      if (bitdepth is None) and (self.filedatatype is None):
-        raise ValueError('Error: extension not recognized, set "bitdepth" parameter')
-      elif (bitdepth == 8):
-        self.filedatatype = np.uint8
-      elif (bitdepth == 16):
-        self.filedatatype = np.uint16
-    except ValueError as exp:
-      print(exp)
-      return -1
-
-    try:
-      if os.path.isfile(Path(self.filepath).expanduser()):
-        f = open(Path(filepath).expanduser(), 'r+b')
-        f.seek(0)
-      else:
-        f = open(Path(filepath).expanduser(), 'w+b')
-        f.seek(0)
-    except:
-      print("File Not Found:", str(Path(filepath)))
-      return -1
-
-    if self.version is None:
-      self.version = 2
-
-    if self.version > 0:
-      version = np.uint64(-self.version)
-      np.asarray(version, dtype=np.uint64).tofile(f)
-
-    if self.version >= 0:
-      if self.filePos is None:
-        file_head_length = 0
-        pat_footer_length = 0
-        if self.version >= 1:
-          file_head_length = 8
-          pat_footer_length = 16
-        if self.version >= 2:
-          if self.hasxypos == True:
-            pat_footer_length = 18
-          else:
-            pat_footer_length = 1
-
-        if self.version >= 4:
-          file_head_length = 9
-
-        self.filePos = np.arange(
-          self.nPatterns, dtype=np.uint64)*(16+pat_footer_length+self.patternH*self.patternW*self.filedatatype(0).nbytes)\
-                       +file_head_length+8*self.nPatterns
-
-      if self.version >= 4:
-        np.uint8(0).tofile(f)
-
-      np.asarray(self.filePos, dtype=np.uint64).tofile(f)
-
-    if writeBlank == True:
-      typewrite = self.filedatatype
-      # if self.bitdepth == 8:
-      #   type = np.uint8
-      # if self.bitdepth == 16:
-      #   type = np.uint16
-
-      blank = np.zeros((self.patternH, self.patternW), dtype=typewrite)
-      pathead = np.array([0, self.patternH, self.patternW,
-                          self.patternH * self.patternW * self.filedatatype(0).nbytes], dtype=np.uint32)
-
-      for j in range(self.nRows):
-        for i in range(self.nCols):
-          pathead.tofile(f)
-          blank.tofile(f)
-          if (self.version > 0) and self.hasxypos:
-            if self.version >= 2:
-              np.uint8(1).tofile(f)
-            np.float64(i * self.xStep - 0.5*(self.nCols*self.xStep)).tofile(f)
-            if self.version >= 2:
-              np.uint8(1).tofile(f)
-            np.float64(j * self.yStep - 0.5*(self.nRows*self.yStep)).tofile(f)
-          else: # no xy_pos info
-            if self.version >= 2:
-              np.uint8(0).tofile(f)
-    f.close()
-
-  def pat_writer(self, pat2write, patStart, nPatToWrite, typewrite=None):
-    try:
-      f = open(Path(self.filepath).expanduser(), 'br+')
-      f.seek(0, 0)
-    except:
-      print("File Not Found:", str(Path(self.filepath)))
-      return -1
-
-    nPerPat = self.patternW * self.patternH
-    nPerPatByte = nPerPat * typewrite(0).nbytes
-    pathead = np.array([0, int(self.patternH), int(self.patternW),
-                        int(self.patternH * self.patternW * self.filedatatype(0).nbytes)], dtype=np.uint32)
-
-    write_xypos = self.hasxypos
-
-    for i in range(int(patStart), int(patStart + nPatToWrite)):
-      if int(self.filePos[i]) > 0:
-        f.seek(int(self.filePos[i]), 0)
-        ii = int(i - patStart)
-        pathead.tofile(f)
-        pat2write[ii, :, :].tofile(f)
-        if write_xypos:
-          if self.version >= 2:
-            np.uint8(1).tofile(f)
-          yx = np.array(np.unravel_index(i, (self.nRows, self.nCols))).astype(np.float64)
-          yx[1] -= float(self.nCols * 0.5)
-          yx[1] *= self.xStep
-          yx[0] -= float(self.nRows * 0.5)
-          yx[0] *= self.yStep
-          np.float64(yx[1]).tofile(f)
-          if self.version >= 2:
-            np.uint8(1).tofile(f)
-          np.float64(yx[0]).tofile(f)
-    f.close()
 
 
 class HDF5PatFile(EBSDPatternFile):
   def __init__(self, path=None):
     filepath = None
     hdf5path = None
     self.patternh5id = 'Pattern'  # the name used for the pattern dataset array in the h5 file.
@@ -1096,49 +643,41 @@
         if 'EBSD' in f[grpset]:
           if 'Data' in f[grpset + '/EBSD/']:
             if self.patternh5id in f[grpset + '/EBSD/Data']:
               if (grpset  not in self.h5datagroups):
                 self.h5datagroups.append(grpset)
       else:
         self.h5othergrps.append(grpset)
-    f.close()
+
     if len(self.h5datagroups) < 1:
       print("No viable EBSD patterns found:",str(Path(self.filepath)))
       return -2
     else:
       if verbose > 0:
         print(self.h5datagroups)
     return len(self.h5datagroups)
 
 
 
-  def pat_reader(self,patStart=0,nPatToRead=1):
+  def pat_reader(self,patStart,nPatToRead):
     '''This is a basic function that will read a chunk of patterns from the HDF5 file.
     Mainly this is intended to be called by the parent class function read_data.
     It assumes that patterns are laid out in a HDF5 dataset as an array
     of N patterns x pattern height x pattern width.  '''
     try:
       f = h5py.File(Path(self.filepath).expanduser(),'r')
     except:
       print("File Not Found:",str(Path(self.filepath)))
       return -1
 
     patterndset = f[self.h5patdatpth]
     readpats = np.array(patterndset[int(patStart):int(patStart+nPatToRead), :, :])
     readpats = readpats.reshape(nPatToRead,self.patternH,self.patternW)
     f.close()
-    yx = np.unravel_index(np.arange(patStart, patStart + nPatToRead), (self.nRows, self.nCols))
-
-    xyloc = np.array([yx[1], yx[0]]).T.copy().astype(np.float32)
-    xyloc[:, 0] -= self.nCols * 0.5
-    xyloc[:, 1] -= self.nRows * 0.5
-    xyloc[:, 0] *= self.xStep
-    xyloc[:, 1] *= self.yStep
-
-    return readpats, xyloc
+    return readpats
 
   def copy_file(self, newpath, **kwargs):
     # oh - this is a mess!
     pathtemp = np.atleast_1d(newpath)
     fpath = Path(pathtemp[0]).expanduser().resolve()
     #print(pathtemp)
     hdf5path = None
@@ -1218,24 +757,14 @@
     if self.h5patdatpth is not None:
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
-      if self.xStep is None:
-        self.xStep = 0.0
-      if self.yStep is None:
-        self.yStep = 0.0
-      if self.nCols is None:
-        self.nCols = np.uint64(1)
-      if self.nCols == 0:
-        self.nCols = np.uint64(1)
-      if self.nRows is None:
-        self.nRows = np.uint64(np.floor(self.nPatterns/self.nCols))
 
 class EDAXOH5(HDF5PatFile):
   def __init__(self, path=None):
     HDF5PatFile.__init__(self, path)
     self.vendor = 'EDAX'
     #EDAXOH5 only attributes
     self.filedatatype = None # np.uint8
@@ -1275,17 +804,17 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.uint32(headerpath['nColumns'][()][0])
-      self.nRows = np.uint32(headerpath['nRows'][()][0])
-      self.hexflag = np.uint32(headerpath['Grid Type'][()][0] == 'HexGrid')
+      self.nCols = np.int32(headerpath['nColumns'][()][0])
+      self.nRows = np.int32(headerpath['nRows'][()][0])
+      self.hexFlag = np.int32(headerpath['Grid Type'][()][0] == 'HexGrid')
 
       self.xStep = np.float32(headerpath['Step X'][()][0])
       self.yStep = np.float32(headerpath['Step Y'][()][0])
 
     return 0 #note this function uses multiple returns
 
 class KIKUCHIPYH5(HDF5PatFile):
@@ -1330,17 +859,17 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.uint32(headerpath['n_columns'][()][0])
-      self.nRows = np.uint32(headerpath['n_rows'][()][0])
-      self.hexflag = np.uint32(headerpath['grid_type'][()][0] == 'hexagonal')
+      self.nCols = np.int32(headerpath['n_columns'][()][0])
+      self.nRows = np.int32(headerpath['n_rows'][()][0])
+      self.hexFlag = np.int32(headerpath['grid_type'][()][0] == 'hexagonal')
 
       self.xStep = np.float32(headerpath['step_x'][()][0])
       self.yStep = np.float32(headerpath['step_y'][()][0])
 
     return 0 #note this function uses multiple returns
 
 
@@ -1385,118 +914,15 @@
       dset = f[self.h5patdatpth]
       shp = np.array(dset.shape)
       self.patternW = shp[-1]
       self.patternH = shp[-2]
       self.nPatterns = shp[-3]
       self.filedatatype = dset.dtype.type
       headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.uint32(headerpath['NCOLS'][()][0])
-      self.nRows = np.uint32(headerpath['NROWS'][()][0])
-      #self.hexflag = np.int32(f[headerpath+'Grid Type'][()][0] == 'HexGrid')
+      self.nCols = np.int32(headerpath['NCOLS'][()][0])
+      self.nRows = np.int32(headerpath['NROWS'][()][0])
+      #self.hexFlag = np.int32(f[headerpath+'Grid Type'][()][0] == 'HexGrid')
 
       self.xStep = np.float32(headerpath['XSTEP'][()][0])
       self.yStep = np.float32(headerpath['YSTEP'][()][0])
 
     return 0 #note this function uses multiple returns
-
-class OXFORDOINA(HDF5PatFile):
-  def __init__(self, path=None):
-    HDF5PatFile.__init__(self, path)
-    self.vendor = 'OXFORD'
-    #OXFORDOINA only attributes
-    self.filedatatype = None # np.uint8
-    self.patternh5id = 'Processed Patterns' # Could also be 'Raw Patterns'
-
-    if self.filepath is not None:
-      self.get_data_paths()
-
-  def set_data_path(self, datapath=None, pathindex=0): #overloaded from parent - will default to first group.
-    if datapath is not None:
-      self.h5patdatpth = datapath
-    else:
-      if len(self.h5datagroups) > 0:
-        #self.activegroupid = pathindex
-        self.h5patdatpth = self.h5datagroups[pathindex] + '/EBSD/Data/' + self.patternh5id
-  def get_data_paths(self, verbose=0, getraw = False):
-    '''Based on the OINA spec this will search for viable Pattern Datasets '''
-    try:
-      f = h5py.File(self.filepath,'r')
-    except:
-      print("File Not Found:",str(Path(self.filepath)))
-      return -1
-    self.h5datagroups = []
-    self.h5othergrps = []
-    if getraw is True:
-      self.patternh5id = 'Raw Patterns'
-    groupsets = list(f.keys())
-    for grpset in groupsets:
-      if isinstance(f[grpset],h5py.Group):
-        if 'EBSD' in f[grpset]:
-          if 'Data' in f[grpset + '/EBSD/']:
-            if self.patternh5id in f[grpset + '/EBSD/Data']:
-              if (grpset  not in self.h5datagroups):
-                self.h5datagroups.append(grpset)
-      else:
-        self.h5othergrps.append(grpset)
-    f.close()
-
-    if (len(self.h5datagroups) < 1) and (getraw is False):
-      self.get_data_paths(self, verbose=False, getraw=True)
-
-    if len(self.h5datagroups) < 1:
-      print("No viable EBSD patterns found:",str(Path(self.filepath)))
-      return -2
-    else:
-      if verbose > 0:
-        print(self.h5datagroups)
-    return len(self.h5datagroups)
-  def read_header(self, path=None):
-    
-    if path is not None:
-      self.filepath = path
-
-    try:
-      f = h5py.File(Path(self.filepath).expanduser(),'r')
-    except:
-      print("File Not Found:",str(Path(self.filepath)))
-      return -1
-
-    self.version = str(f['Format Version'][()][0])
-
-    if self.version >= '5.0':
-      ngrp = self.get_data_paths()
-      if ngrp <= 0:
-        f.close()
-        return -2 # no data groups with patterns found.
-      if self.h5patdatpth is None: # default to the first datagroup
-        self.set_data_path(pathindex=0)
-
-      dset = f[self.h5patdatpth]
-      shp = np.array(dset.shape)
-      self.patternW = shp[-1]
-      self.patternH = shp[-2]
-      self.nPatterns = shp[-3]
-      self.filedatatype = dset.dtype.type
-      headerpath = (f[self.h5patdatpth].parent.parent)["Header"]
-      self.nCols = np.uint32(headerpath['X Cells'][()][0])
-      self.nRows = np.uint32(headerpath['Y Cells'][()][0])
-      #self.hexflag = np.int32(headerpath['Grid Type'][()][0] == 'HexGrid')
-
-      self.xStep = np.float32(headerpath['X Step'][()][0])
-      self.yStep = np.float32(headerpath['Y Step'][()][0])
-
-    return 0 #note this function uses multiple returns
-
-  def pat_reader(self, patStart=0, nPatToRead=1):
-
-    patterns, xyloc = HDF5PatFile.pat_reader(self, patStart, nPatToRead)
-    try:
-      f = h5py.File(Path(self.filepath).expanduser(),'r')
-      xloc = (f[self.h5patdatpth].parent)["Beam Position X"]
-      xyloc[:,0] = np.array(xloc[int(patStart):int(patStart + nPatToRead)]).astype(np.float32)
-      yloc = (f[self.h5patdatpth].parent)["Beam Position Y"]
-      xyloc[:, 1] = np.array(yloc[int(patStart):int(patStart + nPatToRead)]).astype(np.float32)
-      f.close()
-    except:
-      print("File Not Found:",str(Path(self.filepath)))
-
-    return patterns, xyloc
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/nlpar.py` & `pyebsdindex-0.2.dev0/pyebsdindex/nlpar.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 # This software can be redistributed and/or modified freely provided that any derivative
 # works bear some notice that they are derived from it, and any modified versions bear
 # some notice that they have been modified.
 #
 # Author: David Rowenhorst;
 # The US Naval Research Laboratory Date: 21 Aug 2020
 
-# For more info see
-# Patrick T. Brewick, Stuart I. Wright, David J. Rowenhorst. Ultramicroscopy, 200:50–61, May 2019.
-
 """Non-local pattern averaging and re-indexing (NLPAR)."""
 
 from pathlib import Path
 from timeit import default_timer as timer
 
 import numba
 import numpy as np
@@ -73,31 +70,22 @@
     hdf5path = None
     if pathtemp.size > 1:
       hdf5path = pathtemp[1]
     if fpath is not None:
       self.filepath = Path(fpath)
       self.hdfdatapath = hdf5path
 
-  def setoutfile(self, patternfile, filepath=None):
-    """Set the output file.
 
-    Parameters
-    ----------
-    patternfile
-      Input pattern file object from ebsd_pattern.
-    filepath
-      String.
-
-    Notes
-    -----
-    In the future I want to be able to specify the HDF5 data path to
-    store the output data, but that is proving to be a bit of a mess.
-    For now, a copy of the original HDF5 is made, and the NLPAR patterns
-    will be overwritten on top of the originals.
-    """
+
+
+  def setoutfile(self,patternfile, filepath=None):
+    '''patternfile is an input pattern file object from ebsd_pattern.  Filepath is a string.
+    In the future I want to be able to specify the HDF5 data path to store the output data, but that
+    is proving to be a bit of a mess.  For now, a copy of the original HDF5 is made, and the NLPAR patterns will be
+    overwritten on top of the originals. '''
     self.filepathout = None
     self.hdfdatapathout = None
     pathtemp = np.atleast_1d(filepath)
     fpath = pathtemp[0]
     hdf5path = None
     #if pathtemp.size > 1:
     #  hdf5path = pathtemp[1]
@@ -109,85 +97,69 @@
         pathok = self.filepathout.exists()
         if pathok:
           pathok = not self.filepathout.samefile(patternfile.filepath)
           if not pathok:
             raise ValueError('Error: File input and output are exactly the same.')
             return
 
-        patternfile.copy_file([self.filepathout,self.hdfdatapathout], empty_data=True)
+        patternfile.copy_file([self.filepathout,self.hdfdatapathout] )
         return  # fpath and (maybe) hdf5 path were set manually.
       else: # this is a hdf5 file
         if self.hdfdatapathout is None:
-          patternfile.copy_file(self.filepathout, empty_data=True)
+          patternfile.copy_file(self.filepathout)
           self.hdfdatapathout = patternfile.h5patdatpth
           return
         else:
-          patternfile.copy_file([self.filepathout, self.hdfdatapathout], empty_data=True)
+          patternfile.copy_file([self.filepathout, self.hdfdatapathout])
           return
 
     if patternfile is not None: # the user has set no path.
       hdf5path = None
-      
-      if patternfile.filetype in ['UP', 'EBSP']:
+      if patternfile.filetype == 'UP':
         p = Path(patternfile.filepath)
         appnd = "_NLPAR_l{:1.2f}".format(self.lam) + "sr{:d}".format(self.searchradius)
         newfilepath = str(p.parent / Path(p.stem + appnd + p.suffix))
-        patternfile.copy_file(newfilepath,empty_data=True)
+        patternfile.copy_file(newfilepath)
 
       if patternfile.filetype == 'HDF5':
         hdf5path_tmp = str(patternfile.h5patdatpth).split('/')
         if hdf5path_tmp[0] == '':
           hdf5path_org =  hdf5path_tmp[1]
         else:
           hdf5path_org = hdf5path_tmp[0]
         p = Path(patternfile.filepath)
         appnd = "_NLPAR_l{:1.2f}".format(self.lam) + "sr{:d}".format(self.searchradius)
         hdf5path = hdf5path_org+appnd
         newfilepath = str(p.parent / Path(p.stem + appnd + p.suffix))
         #patternfile.copy_file([newfilepath, hdf5path_org], newh5path=hdf5path)
-        patternfile.copy_file([newfilepath], empty_data=True)
+        patternfile.copy_file([newfilepath])
         hdf5path = patternfile.h5patdatpth
 
       self.filepathout = newfilepath
       self.hdfdatapathout = hdf5path
       return
 
   def getinfileobj(self):
     if self.filepath is not None:
       fID = ebsd_pattern.get_pattern_file_obj([self.filepath, self.hdfdatapath])
-      if (fID.nRows is not None):
-        if (self.nrows is None):
-          self.nrows = fID.nRows
-        else:
-          fID.nRows = self.nrows
-
-      if (fID.nCols is not None):
-        if (self.ncols is None):
-          self.ncols = fID.nCols
-        else:
-          fID.nCols = self.ncols
-
+      if fID.nRows is not None:
+        self.nrows = fID.nRows
+      else:
+        fID.nRows = self.nrows
+      if fID.nCols is not None:
+        self.ncols = fID.nCols
+      else:
+        fID.nCols = self.ncols
       return fID
-
     else:
       return None
 
   def getoutfileobj(self):
     if self.filepathout is not None:
-      fID = ebsd_pattern.get_pattern_file_obj([self.filepathout, self.hdfdatapathout])
-      if self.nrows is not None:
-        fID.nRows = self.nrows
-      else:
-        self.nrows = fID.nRows
-
-      if self.ncols is not None:
-        fID.nCols = self.ncols
-      else:
-        self.ncols = fID.nCols
-      return fID
+      return ebsd_pattern.get_pattern_file_obj([self.filepathout, self.hdfdatapathout])
     else:
       return None
 
   def opt_lambda(self,chunksize=0,saturation_protect=True,automask=True, backsub = False,
                  target_weights=[0.5, 0.34, 0.25], dthresh=0.0, autoupdate=True):
 
     target_weights = np.asarray(target_weights)
@@ -242,22 +214,21 @@
 
     sigma = np.zeros((nrows,ncols),dtype=np.float32)+1e24
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
 
 
     dthresh = np.float32(dthresh)
     lamopt_values = []
-    
     for j in range(0,nrows,chunksize):
       print('Block',j)
       #rowstartread = np.int64(max(0,j - nn))
       rowstartread = np.int64(j)
       rowend = min(j + chunksize + nn,nrows)
       rowcountread = np.int64(rowend - rowstartread)
-      data, xyloc = patternfile.read_data(patStartCount=[[0,rowstartread],[ncols,rowcountread]],
+      data = patternfile.read_data(patStartCount=[[0,rowstartread],[ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shp = data.shape
 
       if backsub is True:
         data = self.backsub(data)
         #back = np.mean(data, axis=0)
@@ -373,23 +344,18 @@
 
     nthreadpos = numba.get_num_threads()
     #numba.set_num_threads(36)
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
     print(lam, sr, dthresh)
 
     for j in range(0,nrows,chunksize):
-      print('Row start', j)
-
       rowstartread = np.int64(max(0, j-sr))
       rowend = min(j + chunksize+sr,nrows)
-
-      if (rowend - rowstartread) < (2*sr+1):
-        rowstartread = np.int64(max(0, rowend - (2*sr+1)))
       rowcountread = np.int64(rowend-rowstartread)
-      data, xyloc = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
+      data = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shpdata = data.shape
 
       if backsub is True:
         data = self.backsub(data)
 
@@ -401,38 +367,36 @@
         sigchunk, tmp = self.sigma_numba(data,1,rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
         del tmp
         tmp = (sigma[rowstartread:rowend,:] < sigchunk).choose(sigchunk,sigma[rowstartread:rowend,:])
         sigma[rowstartread:rowend,:] = tmp
       else:
         sigchunk = sigma[rowstartread:rowend,:]
 
-      #dataout = data
-
+      print('Block', j)
       dataout = self.nlpar_nb(data,lam, sr, dthresh, sigchunk,
                               rowcountread,ncols,indices,saturation_protect)
 
       dataout = dataout.reshape(rowcountread, ncols, phw)
       dataout = dataout[j-rowstartread:, :, : ]
       shpout = dataout.shape
       dataout = dataout.reshape(shpout[0]*shpout[1], pheight, pwidth)
       if rescale == True:
         for i in range(dataout.shape[0]):
           temp = dataout[i,:,:]
           temp -= temp.min()
-          temp *= np.float32(mxval)/temp.max()
+          temp *= float(mxval)/temp.max()
           dataout[i,:,:] = temp
 
       patternfileout.write_data(newpatterns=dataout,patStartCount = [[0,j], [ncols, shpout[0]]],
                                      flt2int='clip',scalevalue=1.0 )
       #self.patternfileout.write_data(newpatterns=dataout,patStartCount=[j*ncols,shpout[0]*shpout[1]],
       #                               flt2int='clip',scalevalue=1.0 )
       #return dataout
       #sigma[j:j+rowstartcount[1],:] += \
       #  sigchunk[rowstartcount[0]:rowstartcount[0]+rowstartcount[1],:]
-
     numba.set_num_threads(nthreadpos)
 
 
   def calcsigma(self,chunksize=0,nn=1,saturation_protect=True,automask=True):
 
     patternfile = self.getinfileobj()
 
@@ -459,35 +423,33 @@
       self.mask = np.ones((pheight,pwidth), dytype=np.uint8)
 
     indices = np.asarray( (self.mask.flatten().nonzero())[0], np.uint64)
 
     sigma = np.zeros((nrows, ncols), dtype=np.float32)
     #d_nn = np.zeros((nrows, ncols, int((2*nn+1)**2)), dtype=np.float32)
     colstartcount = np.asarray([0,ncols],dtype=np.int64)
-
+    dave = 0.0
     for j in range(0,nrows,chunksize):
       rowstartread = np.int64(max(0, j-nn))
       rowend = min(j + chunksize+nn,nrows)
-      if (rowend - rowstartread) < (3):
-        rowstartread = np.int64(max(0, rowend - (3)))
       rowcountread = np.int64(rowend-rowstartread)
-      data, xyloc = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
+      data = patternfile.read_data(patStartCount = [[0,rowstartread], [ncols,rowcountread]],
                                         convertToFloat=True,returnArrayOnly=True)
 
       shp = data.shape
       data = data.reshape(data.shape[0], phw)
 
       #data = None
       if rowend == nrows:
         rowstartcount = np.asarray([j-rowstartread,rowcountread - (j-rowstartread) ], dtype=np.int64)
       else:
         rowstartcount = np.asarray([j-rowstartread,chunksize ], dtype=np.int64)
-
+      dtic = timer()
       sigchunk, temp = self.sigma_numba(data,nn, rowcountread,ncols,rowstartcount,colstartcount,indices,saturation_protect)
-
+      dave += (timer() - dtic)
       sigma[j:j+rowstartcount[1],:] += \
         sigchunk[rowstartcount[0]:rowstartcount[0]+rowstartcount[1],:]
 
     return sigma
 
   def backsub(self, data):
     # This function will fit a 2D gaussian on top of a plane to the averaged set of patterns (data) that is provided.
@@ -591,41 +553,39 @@
         count = 0
         for j_nn in range(nn_r_start,nn_r_end ):
           for i_nn in range(nn_c_start,nn_c_end):
             dij[j,i,count,0] = np.uint64(j_nn)
             dij[j,i,count,1] = np.uint64(i_nn) # want to save this for labmda optimization
             indx_nn = i_nn+ncols*j_nn
             d2 = np.float32(0.0)
-            n2 = np.float32(1.0e-12)
+            n2 = np.float32(0.0)
             nout[j,i,count] = n0 # want to save this for labmda optimization
             if not((i == i_nn) and (j == j_nn)):
               for q in range(shpind[0]):
                 d0 = data[indx_0, indices[q]]
                 d1 = data[indx_nn, indices[q]]
                 if (d1 < mxval) and (d0 < mxval):
                   n2 += 1.0
                   d2 += (d0 - d1)**2
               nout[j,i,count] = n2
-
+              s0 = d2 / np.float32(n2 * 2.0)
               if d2 >= 1.e-3: #sometimes EDAX collects the same pattern twice
-                s0 = d2 / np.float32(n2 * 2.0)
                 if s0 < mind:
                   mind = s0
             dout[j,i,count] = d2 # want to save this for labmda optimization
 
             count += 1
 
         sigma[j,i] = np.sqrt(mind)
-        #if sigma[j,i] > 1e12:
-        #  print(sigma[j,i], dout[j,i,:], nout[i,j,:])
     return sigma,( dout, nout, dij)
 
   @staticmethod
-  @numba.jit(nopython=True,cache=True,fastmath=False,parallel=True)
+  @numba.jit(nopython=True,cache=True,fastmath=True,parallel=True)
   def nlpar_nb(data,lam, sr, dthresh, sigma, nrows,ncols,indices,saturation_protect=True):
+
     def getpairid(idx0, idx1):
       idx0_t = int(idx0)
       idx1_t = int(idx1)
       if idx0 < idx1:
         pairid = idx0_t + (idx1_t << 32)
       else:
         pairid = idx1_t + (idx0_t << 32)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/opencl/band_detect_cl.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/band_detect_cl.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,28 +87,28 @@
       lmaxtime = 0.0
       blabeltime = 0.0
 
       for chnk in chunk_start_end:
         tic1 = timer()
         nPatsChunk = chnk[1] - chnk[0]
         #rdnNorm, clparams, rdnNorm_gpu = self.calc_rdn(patterns[chnk[0]:chnk[1],:,:], clparams, use_gpu=self.CLOps[0])
-        rdnNorm, clparams = self.radon_fasterCL(patterns[chnk[0]:chnk[1],:,:], padding=self.padding,
+        rdnNorm, clparams = self.radon_fasterCL(patterns[chnk[0]:chnk[1],:,:], self.padding,
                                                                        fixArtifacts=False, background=self.backgroundsub,
                                                                        returnBuff=True, clparams=clparams)
 
         #if (self.EDAXIQ == True): # I think EDAX actually uses the convolved radon for IQ
           #nTp = self.nTheta + 2 * self.padding[1]
           #nRp = self.nRho + 2 * self.padding[0]
           #nImCL = int(rdnNorm_gpu.size/(nTp*nRp*4))
           #rdnNorm_nocov = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
           #cl.enqueue_copy(clparams.queue,rdnNorm_nocov,rdnNorm,is_blocking=True)
 
         rdntime += timer() - tic1
         tic1 = timer()
-        rdnConv, clparams = self.rdn_convCL2(rdnNorm, clparams=clparams, returnBuff=True, separableKernel=True)
+        rdnConv, clparams = self.rdn_convCL2(rdnNorm, clparams=clparams, returnBuff=True)
         rdnNorm.release()
         convtime += timer()-tic1
         tic1 = timer()
         lMaxRdn, clparams =  self.rdn_local_maxCL(rdnConv, clparams=clparams, returnBuff=True)
         lmaxtime +=  timer()-tic1
         tic1 = timer()
 
@@ -131,31 +131,31 @@
           nRp = self.nRho + 2 * self.padding[0]
           nImCL = int(rdnConv.size / (nTp * nRp * 4))
           rdnConvarray = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
           cl.enqueue_copy(clparams.queue,rdnConvarray,rdnConv,is_blocking=True)
           rdnConvarray = rdnConvarray[:,:,0:chnk[1]-chnk[0] ]
 
         rdnConv.release()
-        rdnConv = None
         blabeltime += timer() - tic1
 
       tottime = timer() - tic0
       # going to manually clear the clparams queue -- this should clear the memory of the queue off the GPU
 
       #if clparams is not None:
-      #  clparams.queue.finish()
-      #  clparams.queue = None
+        #clparams.queue.finish()
+        #clparams.queue = None
 
       if verbose > 0:
         print('Radon Time:',rdntime)
         print('Convolution Time:', convtime)
         print('Peak ID Time:', lmaxtime)
         print('Band Label Time:', blabeltime)
         print('Total Band Find Time:',tottime)
       if verbose > 1:
+        plt.clf()
 
         if len(rdnConvarray.shape) == 3:
           im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1], -1]
         else:
           im2show = rdnConvarray[self.padding[0]:-self.padding[0],self.padding[1]:-self.padding[1]]
 
         rhoMaskTrim = np.int32(im2show.shape[0] * self.rhoMaskFrac)
@@ -163,40 +163,31 @@
         stdv = np.std(im2show[rhoMaskTrim:-rhoMaskTrim, 1:-2])
         im2show -= mean
         im2show /= stdv
         im2show = im2show.clip(-4, None)
         im2show += 6
         im2show[0:rhoMaskTrim,:] = 0
         im2show[-rhoMaskTrim:,:] = 0
-
         im2show = np.fliplr(im2show)
-        fig = plt.figure(figsize=(12, 4))
-        subrdn = fig.add_subplot(121, xlim=(0, 180), ylim=(-self.rhoMax, self.rhoMax))
-        subrdn.imshow(
-            im2show,
-            cmap='gray',
-            extent=[0, 180, -self.rhoMax, self.rhoMax],
-            interpolation='none',
-            zorder=1,
-            aspect='auto'
-        )
+        plt.figure()
+        plt.imshow(im2show, cmap='gray', extent=[0, 180, -self.rhoMax, self.rhoMax],
+                   interpolation='none', zorder=1, aspect='auto')
         width = bandData['width'][-1, :]
         width /= width.min()
-        width *= 2.0
-        xplt = np.squeeze(180.0 - np.interp(bandData['aveloc'][-1,:,1]+0.5, np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
-        yplt = np.squeeze( -1.0 * np.interp(bandData['aveloc'][-1,:,0]-0.5, np.arange(self.radonPlan.nRho), self.radonPlan.rho))
+        width *= 2
+        xplt = np.squeeze(180.0 - np.interp(bandData['aveloc'][-1,:,1], np.arange(self.radonPlan.nTheta), self.radonPlan.theta))
+        yplt = np.squeeze( -1.0 * np.interp(bandData['aveloc'][-1,:,0], np.arange(self.radonPlan.nRho), self.radonPlan.rho))
 
-        subrdn.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
+        plt.scatter(y=yplt, x=xplt, c='r', s=width, zorder=2)
 
         for pt in range(self.nBands):
-          subrdn.annotate(str(pt + 1), np.squeeze([xplt[pt] + 4, yplt[pt]]), color='yellow')
-        #subrdn.xlim(0,180)
-        #subrdn.ylim(-self.rhoMax, self.rhoMax)
-        subpat = fig.add_subplot(122)
-        subpat.imshow(patterns[-1, :, :], cmap='gray')
+          plt.annotate(str(pt + 1),np.squeeze([xplt[pt],yplt[pt]]), color='yellow')
+        plt.xlim(0,180)
+        plt.ylim(-self.rhoMax, self.rhoMax)
+
 
     except Exception as e: # something went wrong - try the CPU
       print(e)
       bandData = band_detect.BandDetect.find_bands(self, patternsIn, verbose=verbose, chunksize=-1, **kwargs)
 
     return bandData
 
@@ -231,15 +222,18 @@
       shapeIm = np.shape(image)
     else:
       nIm = shapeIm[0]
     #  reform = False
 
     clvtypesize = 16 # this is the vector size to be used in the openCL implementation.
     nImCL = np.int32(clvtypesize * (np.int64(np.ceil(nIm/clvtypesize))))
-
+    # there is something very strange that happens if the number of images
+    # is a exact multiple of the max group size (typically 256)
+    mxGroupSz = gpu[gpu_id].get_info(cl.device_info.MAX_WORK_GROUP_SIZE)
+    #nImCL += np.int64(16 * (1 - np.int64(np.mod(nImCL, mxGroupSz ) > 0)))
     image_align = np.ones((shapeIm[1], shapeIm[2], nImCL), dtype = np.float32)
     image_align[:,:,0:nIm] = np.transpose(image, [1,2,0]).copy()
     shpRdn = np.asarray( ((self.nRho+2*padding[0]), (self.nTheta+2*padding[1]), nImCL),dtype=np.uint64)
     radon_gpu = cl.Buffer(ctx,mf.READ_WRITE,size=int((self.nRho+2*padding[0])*(self.nTheta+2*padding[1])*nImCL*4))
     #radon_gpu = cl.Buffer(ctx,mf.READ_WRITE,size=radon.nbytes)
     #radon_gpu = cl.Buffer(ctx,mf.READ_WRITE | mf.COPY_HOST_PTR,hostbuf=radon)
     image_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=image_align)
@@ -257,23 +251,23 @@
 
     if background is not None:
       back_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=background.astype(np.float32))
       prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
       imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
       cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
 
-    cl.enqueue_fill_buffer(queue, radon_gpu, np.float32(-1.0), 0, radon_gpu.size)
+
     prg.radonSum(queue,(nImChunk,rdnstep),None,rdnIndx_gpu,image_gpu,radon_gpu,
                   imstep, indxstep,
                  shpRdn[0], shpRdn[1],
                  padRho, padTheta, np.uint64(self.nTheta))
 
 
     if (fixArtifacts == True):
-       prg.radonFixArt(queue,(nImChunk,shpRdn[0]),None,radon_gpu,
+       prg.radonFixArt(queue,(nImChunk,self.nRho),None,radon_gpu,
                        shpRdn[0],shpRdn[1],padTheta)
 
 
 
 
     if returnBuff == False:
       radon = np.zeros([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1],nImCL],dtype=np.float32)
@@ -355,21 +349,21 @@
     nImChunk = np.uint64(nImCL / clvtypesize)
     resultConv = np.full(shp,0.0,dtype=np.float32)
 
     rdnConv_gpu = cl.Buffer(ctx,mf.WRITE_ONLY ,size=resultConv.nbytes)
     # pad out the radon buffers
     prg.radonPadTheta(queue,(shp[2],shp[0],1),None,rdn_gpu,
                     np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[1]))
-    prg.radonPadRho2(queue,(shp[2],shp[1],1),None,rdn_gpu,
-                      np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[0]+1))
+    prg.radonPadRho(queue,(shp[2],shp[1],1),None,rdn_gpu,
+                      np.uint64(shp[0]),np.uint64(shp[1]),np.uint64(self.padding[0]))
     kern_gpu = None
     if separableKernel == False:
       # for now I will assume that the kernel(s) can fit in local memory on the GPU
       # also going to assume that there is only one kernel -- this will be something to fix at some point.
-      k0 = np.array(self.kernel[0,:,:], dtype=np.float32)
+      k0 = self.kernel[0,:,:]
       kshp = np.asarray(k0.shape, dtype=np.int32)
       pad = kshp/2
       kern_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                         rdn_gpu, kern_gpu,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[2]),
                         np.int32(kshp[1]), np.int32(kshp[0]), np.int32(pad[1]), np.int32(pad[0]), rdnConv_gpu)
 
@@ -377,29 +371,29 @@
 
       #tic = timer()
     else: # convolution is separable
       tempConvbuff = cl.Buffer(ctx,mf.HOST_NO_ACCESS,size=(shp[0]*shp[1]*shp[2]*4))
 
       kshp = np.asarray(self.kernel[0,:,:].shape,dtype=np.int32)
       pad = kshp
-      k0x = np.require(self.kernel[0, np.int64(kshp[0] / 2), :], requirements=['C', 'A', 'W', 'O'], dtype=np.float32)
+      k0x = np.require(self.kernel[0, np.int64(kshp[0] / 2), :], requirements=['C', 'A', 'W', 'O'])
       k0x *= 1.0 / k0x.sum()
       k0x = (k0x[...,:]).reshape(1,kshp[1])
 
 
 
       kshp = np.asarray(k0x.shape,dtype=np.int32)
 
       kern_gpu_x = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0x)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                           rdn_gpu,kern_gpu_x,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[2]),
                           np.int32(kshp[1]),np.int32(kshp[0]),np.int32(pad[1]),np.int32(pad[0]),tempConvbuff)
 
       kshp = np.asarray(self.kernel[0,:,:].shape,dtype=np.int32)
-      k0y = np.require(self.kernel[0, :, np.int32(kshp[1] / 2)], requirements=['C', 'A', 'W', 'O'], dtype=np.float32)
+      k0y = np.require(self.kernel[0, :, np.int32(kshp[1] / 2)], requirements=['C', 'A', 'W', 'O'])
       k0y *= 1.0 / k0y.sum()
       k0y = (k0y[...,:]).reshape(kshp[0],1)
       kshp = np.asarray(k0y.shape,dtype=np.int32)
 
       kern_gpu_y = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=k0y)
       prg.convolution3d2d(queue,(np.int32((shp[1]-2*pad[1])),np.int32((shp[0]-2*pad[0])), nImChunk),None,
                           tempConvbuff,kern_gpu_y,np.int32(shp[1]),np.int32(shp[0]),np.int32(shp[0]),
@@ -487,15 +481,15 @@
         radon = radonIn
       shp = radon.shape
       nIm = shp[2]
       nImCL = np.int32(clvtypesize * (np.int64(np.ceil(nIm / clvtypesize))))
       # there is something very strange that happens if the number of images
       # is a exact multiple of the max group size (typically 256)
       mxGroupSz = gpu[gpu_id].get_info(cl.device_info.MAX_WORK_GROUP_SIZE)
-      nImCL += np.int64(16 * (1 - np.int(np.mod(nImCL,mxGroupSz) > 0)))
+      nImCL += np.int(16 * (1 - np.int(np.mod(nImCL,mxGroupSz) > 0)))
       radonCL = np.zeros((nRp,nTp,nImCL),dtype=np.float32)
       radonCL[:,:,0:shp[2]] = radon
       rdn_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=radonCL)
       shp = (nRp,nTp,nImCL)
 
     nImChunk = np.uint64(nImCL / clvtypesize)
     #out = np.zeros((shp), dtype = np.int32)
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/opencl/clkernels.cl` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/clkernels.cl`

 * *Files 2% similar despite different names*

```diff
@@ -39,37 +39,14 @@
     imVal =  im1[indx+i];
     imVal -= b1;   
     im1[indx+i] = imVal;
   }
   
 }
 
-//Do a background division on the pattern
-__kernel void backDiv( __global float16 *im1, __global const float *back,
-                        const unsigned long int nImChunk)
-  {
-  const unsigned long int xy = get_global_id(0);
-  //const unsigned long int szim = get_global_size(0);
-  unsigned long i;
-  float16 imVal;
-
-  float b1 = back[xy];
-  if (b1 < 1.0){
-    b1 = 1.0;
-  }
-  
-  const unsigned long indx = nImChunk * xy;
-  for(i = 0; i< nImChunk; ++i){
-    imVal =  im1[indx+i];
-    imVal /= b1;   
-    im1[indx+i] = imVal;
-  }
-  
-}
-
 
 __kernel void radonSum(
       __global const unsigned long int *rdnIndx, __global const float16 *images, __global float16 *radon,
       const unsigned long int imstep, const unsigned long int indxstep,
       const unsigned int long nRhoP, const unsigned long int nThetaP,
       const unsigned long int rhoPad, const unsigned long int thetaPad,const unsigned long int nTheta )
     {
@@ -93,37 +70,33 @@
         sum += images[idx*nImChunk + gid_im];
         count += 1.0;
       }
     }
 
 
     const unsigned long int rndIndx = (theta+thetaPad + (rho+rhoPad)*nThetaP)*nImChunk + gid_im;
-    if (count > 1.0e-6){
-      radon[rndIndx] = sum/count;}
-    else{
-      radon[rndIndx] = -1.0;
-    }
-    
+    radon[rndIndx] = sum/count;
+    //radon[rndIndx] = gid_im;
     }
 
-__kernel void radonFixArt(
+  __kernel void radonFixArt(
       __global float16 *radon,
       const unsigned long int nRho, const unsigned long int nTheta,
       const unsigned long int thetaPad)
   {
     const unsigned long int gid_im = get_global_id(0);
     const unsigned long int nImChunk = get_global_size(0);
     const unsigned long int rho = get_global_id(1);
     const unsigned long int rhoIndx = nTheta * rho;
     //rndIndx = nTheta * nRho * gid_im + (nTheta * rho);
-    
+
+    //radon[gid_rdn+thetaPad] = radon[gid_rdn+thetaPad+1];
     radon[(thetaPad + rhoIndx)*nImChunk + gid_im] = radon[(thetaPad + 1 + rhoIndx)*nImChunk + gid_im];
-   
+    //radon[gid_rdn+nTheta-1-thetaPad] = radon[gid_rdn+nTheta-2-thetaPad];
     radon[(nTheta-1-thetaPad + rhoIndx)*nImChunk + gid_im] = radon[(+nTheta-2-thetaPad + rhoIndx)*nImChunk + gid_im];
-    //}
   }
 
 // Padding of the radon Theta -- 0 and 180* are symmetric with a vertical flip.
 __kernel void radonPadTheta(
       __global float *radon,
       const unsigned long int nRho, const unsigned long int nTheta,
       const unsigned long int thetaPad)
@@ -166,52 +139,14 @@
         gid_rdn2 = ((nTheta* (nRho-1-rhoPad+i)) + gid_theta)*nImChunk + gid_im;
         radon[gid_rdn1] = rd1p;
         radon[gid_rdn2] = rd2p;
     }
 
   }
 
-// Padding of the radon Rho -- copy the previous line to the next row ...
-  __kernel void radonPadRho2(
-      __global float *radon,
-      const unsigned long int nRho, const unsigned long int nTheta,
-      const unsigned long int rhoPad)
-  {
-    const unsigned long int gid_im = get_global_id(0);
-    const unsigned long int nImChunk = get_global_size(0);
-    const unsigned long int gid_theta = get_global_id(1);
-    unsigned long int i, gid_rdn1, gid_rdn2;
-    //indxim = nTheta * nRho * gid_im;
-    //rd1p =  radon[indxim + (nTheta * rhoPad) + gid_theta] ;
-    //rd2p =  radon[ indxim + (nTheta * (nRho -1 - rhoPad)) + gid_theta] ;
-    float rd1p =  radon[((nTheta * rhoPad) + gid_theta)*nImChunk + gid_im] ;
-    float rd2p =  radon[((nTheta * (nRho -1 - rhoPad)) + gid_theta)*nImChunk+gid_im];
-
-    for (i = 0; i <= rhoPad; ++i){
-
-        //gid_rdn1 = indxim + (nTheta*i) + gid_theta;
-        //gid_rdn2 = indxim + (nTheta* (nRho-1-rhoPad+i)) + gid_theta;
-        
-        gid_rdn1 = ((nTheta*i) + gid_theta)*nImChunk + gid_im;
-        gid_rdn2 = ((nTheta* (nRho-1-rhoPad+i)) + gid_theta)*nImChunk + gid_im;
-        
-        if (radon[gid_rdn1] < 0){
-          radon[gid_rdn1] = rd1p;
-        }
-        if (radon[gid_rdn2] < 0){
-          radon[gid_rdn2] = rd2p;
-        }
-        rd1p =  radon[gid_rdn1] ;
-        rd2p =  radon[gid_rdn2] ;
-
-    }
-
-  }
-
-
 // Convolution of a stack of images by a 2D kernel
 // At somepoint we might want to consider the ability to chain together convolutions -- keeping the max at each pixel...
 __kernel void convolution3d2d( __global const float16 *in, __constant float *kern, const int imszx, const int imszy, const int imszz, 
   const int kszx, const int kszy, const int padx, const int pady, __global float16 *out)
 {
   // IDs of work-item represent x and y coordinates in image
   const long x = get_global_id(0) + padx;
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/opencl/openclparam.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/openclparam.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,17 +39,16 @@
     self.ngpu = 0
     self.gpu_id = gpu_id
     self.ctx = None
     self.prg = None
     self.queue = None
     self.memflags = cl.mem_flags
 
-
     try:
-      self.get_gpu()
+      self.get_context()
 
     except Exception as e:
       if hasattr(e,'message'):
         print(e.message)
       else:
         print(e)
 
@@ -61,28 +60,30 @@
       self.get_platform()
 
     self.gpu = self.platform.get_devices(device_type=cl.device_type.GPU)
     self.ngpu = len(self.gpu)
     if len(self.gpu)-1 < self.gpu_id:
       self.gpu_id = len(self.gpu)-1
 
-  def get_context(self, gpu_id=None):
+  def get_context(self):
     if self.gpu is None:
       self.get_gpu()
 
+    self.ctx = cl.Context(devices = self.gpu)
+    kernel_location = path.dirname(__file__)
+    self.prg = cl.Program(self.ctx,open(path.join(kernel_location,'clkernels.cl')).read()).build()
+
+  def get_queue(self, gpu_id=None, random_gpu=False):
+
+    if self.ctx is None:
+      self.get_context()
+
     if gpu_id is None:
       gpu_id = self.gpu_id
 
+    if random_gpu == True:
+      gpu_id = np.random.randint(len(self.gpu))
     gpuindx = min(len(self.gpu)-1, gpu_id)
     self.gpu_id = gpuindx
-    self.ctx = cl.Context(devices = [self.gpu[self.gpu_id]])
-
-    kernel_location = path.dirname(__file__)
-    self.prg = cl.Program(self.ctx,open(path.join(kernel_location,'clkernels.cl')).read()).build()
-    #print('ctx', self.gpu_id)
-  def get_queue(self, gpu_id=None):
-    if self.ctx is None:
-      self.get_context(gpu_id=None)
-
-    self.queue = cl.CommandQueue(self.ctx)
+    self.queue = cl.CommandQueue(self.ctx, device=self.gpu[gpuindx])
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/opencl/radon_fast_cl.py` & `pyebsdindex-0.2.dev0/pyebsdindex/opencl/radon_fast_cl.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,15 @@
     if clparams is None:
       self.clparams = openclparam.OpenClParam()
       self.clparams.get_queue()
     else:
       self.clparams = clparams
 
 
-  def radon_fasterCL(self,image,padding = np.array([0,0]), fixArtifacts = False,
-                     background = None, background_method = 'SUBTRACT',
-                     returnBuff = True, clparams=None ):
+  def radon_fasterCL(self,image,padding = np.array([0,0]), fixArtifacts = False, background = None, returnBuff = True, clparams=None ):
 
     tic = timer()
     # make sure we have an OpenCL environment
     if clparams is not None:
       if clparams.queue is None:
         clparams.get_queue()
       gpu = clparams.gpu
@@ -106,30 +104,27 @@
     padTheta = np.uint64(padding[1])
     tic = timer()
 
     nImChunk = np.uint64(nImCL/clvtypesize)
 
     if background is not None:
       back_gpu = cl.Buffer(ctx,mf.READ_ONLY | mf.COPY_HOST_PTR,hostbuf=background.astype(np.float32))
-      if str.upper(background_method) == 'DIVIDE':
-        prg.backDiv(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
-      else:
-        prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
-        #imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
-        #cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
+      prg.backSub(queue,(imstep, 1, 1),None,image_gpu,back_gpu,nImChunk)
+      imBack = np.zeros((shapeIm[1], shapeIm[2], nImCL),dtype=np.float32)
+      cl.enqueue_copy(queue,imBack,image_gpu,is_blocking=True)
+
 
-    cl.enqueue_fill_buffer(queue, radon_gpu, np.float32(0.0), 0, radon_gpu.size)
     prg.radonSum(queue,(nImChunk,rdnstep),None,rdnIndx_gpu,image_gpu,radon_gpu,
                   imstep, indxstep,
                  shpRdn[0], shpRdn[1],
                  padRho, padTheta, np.uint64(self.nTheta))
 
 
     if (fixArtifacts == True):
-       prg.radonFixArt(queue,(nImChunk,shpRdn[0]),None,radon_gpu,
+       prg.radonFixArt(queue,(nImChunk,self.nRho),None,radon_gpu,
                        shpRdn[0],shpRdn[1],padTheta)
 
 
 
 
     if returnBuff == False:
       radon = np.zeros([self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1],nImCL],dtype=np.float32)
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/pairlib.py` & `pyebsdindex-0.2.dev0/pyebsdindex/pairlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     #libANG, libID = self.sortlib_id(libANG,libID,findDups = True)
     #print(libANG)
     #print(libANG.shape)
     angTable = self.calc_pole_dot(sympolesComplete,sympolesComplete)
     angTable = np.arccos(angTable)*RADEG
     famindx0 = ((np.concatenate( ([0],np.cumsum(nFamComplete)) ))[0:-1]).astype(dtype=np.int)
     cartPoles = self.xstalplane2cart(sympolesComplete)
-    cartPoles /= np.linalg.norm(cartPoles, axis = 1).reshape(int(cartPoles.size/3),1)
+    cartPoles /= np.linalg.norm(cartPoles, axis = 1).reshape(np.int(cartPoles.size/3),1)
     self.completelib = {
                    'poles' : sympolesComplete,
                    'polesCart': cartPoles,
                    'angTable' : angTable,
                    'nFamily'  : nFamComplete,
                    'famIndex' : famindx0
                   }
@@ -208,16 +208,16 @@
       testSum = np.sum( (test < -0.99999).astype(np.int32)*np.arange(nf).reshape(1,nf), axis = 1)
       whpos = np.nonzero( np.logical_or(testSum < np.arange(nf), (testSum == 0)))[0]
       polesout = polesout[whpos, :]
     return polesout
 
   def calc_pole_dot(self,poles1,poles2,rMetricTensor = np.identity(3)):
 
-    p1 = poles1.reshape(int(poles1.size // 3), 3)
-    p2 = poles2.reshape(int(poles2.size // 3), 3)
+    p1 = poles1.reshape(np.int(poles1.size / 3), 3)
+    p2 = poles2.reshape(np.int(poles2.size / 3), 3)
 
     n1 = p1.shape[0]
     n2 = p2.shape[0]
 
     t1 = p1.dot(rMetricTensor)
     t2 = rMetricTensor.dot(p2.T)
     dot = t1.dot(p2.T)
@@ -239,15 +239,15 @@
     LUTA = np.array([[0,1,2],[0,2,1],[1,0,2],[1,2,0],[2,0,1],[2,1,0]])
     LUTB = np.array([[0,1,2],[1,0,2],[0,2,1],[2,0,1],[1,2,0],[2,1,0]])
 
     LUT = np.zeros((3,3,3,3), dtype=np.int64)
     for i in range(6):
       LUT[:, LUTA[i,0], LUTA[i,1], LUTA[i,2]] = LUTB[i,:]
 
-    ntrips = int(libANG.size // 3)
+    ntrips = np.int(libANG.size / 3)
     for i in range(ntrips):
       temp = np.squeeze(libANG[i,:])
       srt = np.argsort(temp)
       libANG[i,:] = temp[srt]
       srt2 = LUT[:,srt[0], srt[1], srt[2]]
       temp2 = libID[i,:]
       temp2 = temp2[srt2]
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/radon_fast.py` & `pyebsdindex-0.2.dev0/pyebsdindex/radon_fast.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,36 +106,32 @@
         #else:
           #indx_x = np.ceil(a[i] * n + b1).astype(np.int64)
         indx_x = np.round(a[i] * n + b1).astype(np.int64)
         indx_x = np.where(indx_x < 0, outofbounds, indx_x)
         indx_x = np.where(indx_x >= self.imDim[1], outofbounds, indx_x)
         indx1D = np.clip(indx_x+self.imDim[1]*n, 0, outofbounds)
         self.indexPlan[:, i, 0:self.imDim[0]] = indx1D
-    self.indexPlan.sort(axis = -1)
+      self.indexPlan.sort(axis = -1)
 
 
-  def radon_fast(self, imageIn, padding = np.array([0,0]), fixArtifacts = False,
-                 background = None, background_method = 'SUBTRACT'):
+  def radon_fast(self, imageIn, padding = np.array([0,0]), fixArtifacts = False, background = None):
     tic = timer()
     shapeIm = np.shape(imageIn)
     if imageIn.ndim == 2:
       nIm = 1
       image = imageIn[np.newaxis, : ,:]
       reform = True
     else:
       nIm = shapeIm[0]
       reform = False
 
     if background is None:
       image = imageIn.reshape(-1)
     else:
-      if str.upper(background_method) == 'DIVIDE':
-        image = imageIn / background
-      else:
-        image = imageIn - background
+      image = imageIn - background
       image = image.reshape(-1)
 
     nPx = shapeIm[-1]*shapeIm[-2]
     im = np.zeros(nPx+1, dtype=np.float32)
     #radon = np.zeros([nIm, self.nRho, self.nTheta], dtype=np.float32)
     radon = np.zeros([nIm,self.nRho + 2 * padding[0],self.nTheta + 2 * padding[1]],dtype=np.float32)
     shpRdn = radon.shape
@@ -226,14 +222,18 @@
     if PC is None:
       PC = np.array([0.471659,0.675044,0.630139])
     ven = str.upper(vendor)
 
     nPats = bandData.shape[0]
     nBands = bandData.shape[1]
 
+    # This translation from the Radon to theta and rho assumes that the first pixel read
+    # in off the detector is in the bottom left corner. -- No longer the assumption --- see below.
+    # theta = self.radonPlan.theta[np.array(bandData['aveloc'][:,:,1], dtype=np.int)]/RADEG
+    # rho = self.radonPlan.rho[np.array(bandData['aveloc'][:, :, 0], dtype=np.int)]
 
     # This translation from the Radon to theta and rho assumes that the first pixel read
     # in off the detector is in the top left corner.
 
     #theta = np.pi - self.radonPlan.theta[np.array(bandData['aveloc'][:,:,1],dtype=np.int64)] / RADEG
     #rho = -1.0 * self.radonPlan.rho[np.array(bandData['aveloc'][:,:,0],dtype=np.int64)]
 
@@ -264,17 +264,15 @@
           pctemp = np.tile(pctemp[0,:], nPats).reshape(nPats,4)
       t = pctemp[:,0:3]
       t[:,2] /= pctemp[:,3] # normalize by pixel size
 
 
 
     dimf = np.array(self.imDim, dtype=np.float32)
-    if ven in ['EDAX']:
-      t *= np.array([dimf[1], dimf[0], -np.min(dimf[0:2])])
-    if ven in ['OXFORD']:
+    if ven in ['EDAX', 'OXFORD']:
       t *= np.array([dimf[1], dimf[1], -dimf[1]])
     if ven == 'EMSOFT':
       t[:, 0] *= -1.0
       t += np.array([dimf[1] / 2.0, dimf[0] / 2.0, 0.0])
       t[:, 2] *= -1.0
     if ven in ['KIKUCHIPY', 'BRUKER']:
       t *=  np.array([dimf[1], dimf[0], -dimf[0]])
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/rotations.py` & `pyebsdindex-0.2.dev0/pyebsdindex/rotations.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/rotlib.py` & `pyebsdindex-0.2.dev0/pyebsdindex/rotlib.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/conftest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/numbatest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/numbatest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/raytest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/raytest.py`

 * *Files identical despite different names*

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/rotlibunittest.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/rotlibunittest.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 pi = np.pi
 RADDEG = 180.0/pi
 # I had some issues with the periodic boundaries in cubochoric/homochoric/quaternion spaces, so I am using
 # quaternion misorientation to evaluate the error.
 
 def testrotlib(float32=False, return_quat=False, seed = 1, n = 1000000):
-  n = int(n)
+  n = np.int(n)
   np.random.seed(seed)
   qu = (np.random.random((n,4))*2.0-1)
   if float32 is True:
     qu = qu.astype(np.float32)
   qu = quatnorm(qu)
   qu[0, :] = np.array([1.0, 0.0, 0.0, 0.0])
   qu[1, :] = np.array([0.0,0.0,0.0,-1.0])
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/test_ebsd_index.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_ebsd_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,18 +40,18 @@
         indexer = EBSDIndexer()
         assert indexer.phaselist == ["FCC"]
         assert indexer.sampleTilt == 70
         assert indexer.camElev == 5.3
         assert indexer.vendor == "EDAX"
 
     def test_index_pats(self, pattern_al_sim_20kv):
-        """Test Radon indexing and setting/passing projection center
+        """Test Hough indexing and setting/passing projection center
         values.
         """
-        pc = (0.4, 0.72, 0.6)
+        pc = (0.4, 0.6, 0.5)
 
         # Set PC upon initialization of indexer
         indexer = EBSDIndexer(PC=pc, patDim=pattern_al_sim_20kv.shape)
         data = indexer.index_pats(pattern_al_sim_20kv)[0]
         assert np.allclose(data[0]["quat"], data[1]["quat"])
 
         # Pass PC upon indexing
@@ -63,19 +63,18 @@
 
         # Expected rotation
         euler = np.rad2deg(qu2eu(data[0]["quat"]))
         assert np.isclose(euler, self._possible_euler, atol=2).any()
 
     @pytest.mark.skipif(not _ray_installed, reason="ray is not installed")
     def test_index_pats_multi(self, pattern_al_sim_20kv):
-        """Test Radon indexing parallelized with ray."""
+        """Test Hough indexing parallelized with ray."""
         from pyebsdindex.ebsd_index import index_pats_distributed
 
         patterns = np.repeat(pattern_al_sim_20kv[None, ...], 4, axis=0)
-        indexer = EBSDIndexer(PC=(0.4, 0.72, 0.6), patDim=patterns.shape[1:])
-        data = index_pats_distributed(patsin=patterns, ebsd_indexer_obj=indexer)[0]
+        indexer = EBSDIndexer(PC=(0.4, 0.6, 0.5), patDim=patterns.shape[1:])
+        data = index_pats_distributed(patterns, ebsd_indexer_obj=indexer)
 
         # Expected rotation
         euler = np.rad2deg(qu2eu(data[0]["quat"]))
-
         assert np.isclose(euler[0], self._possible_euler, atol=2).any()
         assert np.allclose(euler[0], euler[1:])
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/test_package.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     with pytest.raises(ImportError):
         from pyebsdindex.opencl.band_detect_cl import BandDetect
 
 
 @pytest.mark.skipif(not _ray_installed, reason="ray is not installed")
 def test_available_functionality_with_ray():
     from pyebsdindex.ebsd_index import index_pats_distributed
-    #from pyebsdindex.ebsd_index import IndexerRay
+    from pyebsdindex.ebsd_index import IndexerRay
 
-    #assert callable(index_pats_distributed)
-    #_ = IndexerRay.remote()
+    assert callable(index_pats_distributed)
+    _ = IndexerRay.remote()
 
 
 @pytest.mark.skipif(_ray_installed, reason="ray is installed")
 def test_unavailable_functionality_without_ray():
     with pytest.raises(ImportError):
         from pyebsdindex.ebsd_index import index_pats_distributed
-    #with pytest.raises(ImportError):
-    #    from pyebsdindex.ebsd_index import IndexerRay
+    with pytest.raises(ImportError):
+        from pyebsdindex.ebsd_index import IndexerRay
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex/tests/test_pcopt.py` & `pyebsdindex-0.2.dev0/pyebsdindex/tests/test_pcopt.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 import numpy as np
 
 from pyebsdindex import ebsd_index, pcopt
 
 
 class TestPCOptimization:
     def test_pc_optimize(self, pattern_al_sim_20kv):
-        pc0 = (0.4, 0.72, 0.6)
+        pc0 = (0.4, 0.6, 0.5)
         indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
 
     def test_pc_optimize_pso(self, pattern_al_sim_20kv):
-        pc0 = (0.4, 0.72, 0.6)
+        pc0 = (0.4, 0.6, 0.5)
         indexer = ebsd_index.EBSDIndexer(patDim=pattern_al_sim_20kv.shape)
         new_pc = pcopt.optimize_pso(pattern_al_sim_20kv, indexer, PC0=pc0)
         assert np.allclose(new_pc, pc0, atol=0.05)
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex.egg-info/PKG-INFO` & `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pyebsdindex
-Version: 0.2.0
+Version: 0.2.dev0
 Summary: Python based tool for Hough/Radon based EBSD indexing
 Home-page: https://pyebsdindex.readthedocs.io
 Download-URL: https://pypi.python.org/pypi/pyebsdindex
 Author: ['Dave Rowenhorst', 'Håkon Wiik Ånes']
 Maintainer: Dave Rowenhorst
 Maintainer-email: 
 License: Custom
 Project-URL: Bug Tracker, https://github.com/USNavalResearchLaboratory/PyEBSDIndex/issues
 Project-URL: Documentation, https://pyebsdindex.readthedocs.io
 Project-URL: Source Code, https://github.com/USNavalResearchLaboratory/PyEBSDIndex
-Keywords: EBSD,electron backscatter diffraction,HI,Radon indexing,NLPAR
+Keywords: EBSD,electron backscatter diffraction,HI,Hough indexing,NLPAR
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -33,15 +32,15 @@
 Provides-Extra: parallel
 Provides-Extra: dev
 Provides-Extra: all
 License-File: License
 
 # PyEBSDIndex
 
-Python based tool for Radon based EBSD orientation indexing.
+Python based tool for Hough/Radon based EBSD orientation indexing.
 
 [![Build status](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml/badge.svg)](https://github.com/USNavalResearchLaboratory/PyEBSDIndex/actions/workflows/build.yml)
 [![Documentation status](https://readthedocs.org/projects/pyebsdindex/badge/?version=latest)](https://pyebsdindex.readthedocs.io/en/latest/)
 [![PyPI version](https://img.shields.io/pypi/v/pyebsdindex.svg)](https://pypi.python.org/pypi/pyebsdindex)
 
 The pattern processing is based on a GPU pipeline, and is based on the work of S. I.
 Wright and B. L. Adams. Metallurgical Transactions A-Physical Metallurgy and Materials
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex.egg-info/SOURCES.txt` & `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 .readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 IPFCubic.pdf
 IPFCubic.png
-IPFHex.pdf
-IPFHex.png
 License
 MANIFEST.in
 README.md
 RELEASE.rst
 setup.cfg
 setup.py
 doc/Makefile
@@ -39,22 +37,22 @@
 pyebsdindex/band_detect.py
 pyebsdindex/band_vote.py
 pyebsdindex/crystal_sym.py
 pyebsdindex/crystallometry.py
 pyebsdindex/ebsd_index.py
 pyebsdindex/ebsd_pattern.py
 pyebsdindex/ebsdfile.py
-pyebsdindex/misorientation.py
 pyebsdindex/nlpar.py
 pyebsdindex/pairlib.py
 pyebsdindex/pcopt.py
 pyebsdindex/radon_fast.py
 pyebsdindex/rotations.py
 pyebsdindex/rotlib.py
-pyebsdindex/tripletvote.py
+pyebsdindex/spherical_radon_fast.py
+pyebsdindex/tripletlib.py
 pyebsdindex.egg-info/PKG-INFO
 pyebsdindex.egg-info/SOURCES.txt
 pyebsdindex.egg-info/dependency_links.txt
 pyebsdindex.egg-info/requires.txt
 pyebsdindex.egg-info/top_level.txt
 pyebsdindex.egg-info/zip-safe
 pyebsdindex/EBSDImage/IPFcolor.py
@@ -68,10 +66,9 @@
 pyebsdindex/tests/conftest.py
 pyebsdindex/tests/numbatest.py
 pyebsdindex/tests/raytest.py
 pyebsdindex/tests/rotlibunittest.py
 pyebsdindex/tests/test_ebsd_index.py
 pyebsdindex/tests/test_package.py
 pyebsdindex/tests/test_pcopt.py
-pyebsdindex/tests/test_tripletvote.py
 pyebsdindex/tests/data/al_sim_20kv/al_sim_20kv.png
 pyebsdindex/tests/data/al_sim_20kv/generate_al_sim_20kv.py
```

### Comparing `pyebsdindex-0.2.0/pyebsdindex.egg-info/requires.txt` & `pyebsdindex-0.2.dev0/pyebsdindex.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 h5py
 matplotlib
 numpy
 numba
+pyswarms
 scipy
 
 [all]
 pyopencl
 ray[default]>=1.13
-pydantic<2
 nbsphinx>=0.7
 numpydoc
 pydata-sphinx-theme
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]
 sphinx-copybutton>=0.2.5
 sphinx-design
@@ -30,15 +30,14 @@
 sphinx-design
 sphinx-gallery
 coverage>=5.0
 pytest>=5.4
 pytest-cov>=2.8.1
 pyopencl
 ray[default]>=1.13
-pydantic<2
 
 [doc]
 nbsphinx>=0.7
 numpydoc
 pydata-sphinx-theme
 sphinx>=3.0.2
 sphinx-codeautolink[ipython]
@@ -47,13 +46,12 @@
 sphinx-gallery
 
 [gpu]
 pyopencl
 
 [parallel]
 ray[default]>=1.13
-pydantic<2
 
 [tests]
 coverage>=5.0
 pytest>=5.4
 pytest-cov>=2.8.1
```

### Comparing `pyebsdindex-0.2.0/setup.py` & `pyebsdindex-0.2.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,21 @@
         "sphinx-copybutton              >= 0.2.5",
         "sphinx-design",
         "sphinx-gallery",
     ],
     "tests": [
         "coverage                       >= 5.0",
         "pytest                         >= 5.4",
-        "pytest-cov                     >= 2.8.1",
+        "pytest-cov                     >= 2.8.1"
     ],
     "gpu": [
         "pyopencl",
     ],
     "parallel": [
         "ray[default]                   >= 1.13",
-        "pydantic                       < 2",
     ]
 }
 # Create a development installation "dev" including "doc" and "tests"
 # projects
 extra_feature_requirements["dev"] = list(
     chain(*list(extra_feature_requirements.values()))
 )
@@ -57,28 +56,27 @@
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: Other/Proprietary License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     keywords=[
         "EBSD",
         "electron backscatter diffraction",
         "HI",
-        "Radon indexing",
+        "Hough indexing",
         "NLPAR",
     ],
     zip_safe=True,
     # Contact
     author=__credits__,
     download_url="https://pypi.python.org/pypi/pyebsdindex",
     maintainer=__author__,
@@ -92,14 +90,15 @@
     # Dependencies
     extras_require=extra_feature_requirements,
     install_requires=[
         "h5py",
         "matplotlib",
         "numpy",
         "numba",
+        "pyswarms",
         "scipy",
     ],
     # Files to include when distributing package (see also MANIFEST.in)
     packages=find_packages(),
     package_dir={"pyebsdindex": "pyebsdindex"},
     include_package_data=True,
 )
```

