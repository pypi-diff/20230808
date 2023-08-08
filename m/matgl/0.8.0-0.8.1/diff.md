# Comparing `tmp/matgl-0.8.0.tar.gz` & `tmp/matgl-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.8.0.tar", last modified: Mon Jul 31 15:11:49 2023, max compression
+gzip compressed data, was "matgl-0.8.1.tar", last modified: Tue Aug  8 01:47:35 2023, max compression
```

## Comparing `matgl-0.8.0.tar` & `matgl-0.8.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-31 15:08:34.000000 matgl-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-31 15:11:49.167516 matgl-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-31 15:08:34.000000 matgl-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.143516 matgl-0.8.0/matgl/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/apps/pes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl/data/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/data/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.151516 matgl-0.8.0/matgl/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16099 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.151516 matgl-0.8.0/matgl/graph/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12742 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/graph/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.159516 matgl-0.8.0/matgl/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_bond.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.163516 matgl-0.8.0/matgl/models/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_m3gnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/models/_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/matgl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)   131200 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/sb_roots.npy
--rw-r--r--   0 runner    (1001) docker     (123)    13697 2023-07-31 15:08:34.000000 matgl-0.8.0/matgl/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.147516 matgl-0.8.0/matgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13724 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 15:11:49.000000 matgl-0.8.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-31 15:08:34.000000 matgl-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:11:49.167516 matgl-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-31 15:08:34.000000 matgl-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:11:49.167516 matgl-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 15:08:34.000000 matgl-0.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 15:08:34.000000 matgl-0.8.0/tests/test_integration.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:35.005746 matgl-0.8.1/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.8.1/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    13908 2023-08-08 01:47:35.005559 matgl-0.8.1/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)    12739 2023-08-08 01:07:48.000000 matgl-0.8.1/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.996695 matgl-0.8.1/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.997974 matgl-0.8.1/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4220 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6277 2023-08-07 19:48:01.000000 matgl-0.8.1/matgl/cli.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1996 2023-07-28 14:26:46.000000 matgl-0.8.1/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.998431 matgl-0.8.1/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2542 2023-06-23 19:04:34.000000 matgl-0.8.1/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.999082 matgl-0.8.1/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16251 2023-08-01 16:55:16.000000 matgl-0.8.1/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4569 2023-07-27 14:35:43.000000 matgl-0.8.1/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.999915 matgl-0.8.1/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5495 2023-08-07 13:11:13.000000 matgl-0.8.1/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2113 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12742 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:35.002122 matgl-0.8.1/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      716 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2037 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3139 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12728 2023-07-13 17:50:13.000000 matgl-0.8.1/matgl/layers/_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2231 2023-06-23 19:04:34.000000 matgl-0.8.1/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6036 2023-08-07 14:16:02.000000 matgl-0.8.1/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3578 2023-06-23 19:04:34.000000 matgl-0.8.1/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16645 2023-08-01 18:00:48.000000 matgl-0.8.1/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3892 2023-07-29 15:14:27.000000 matgl-0.8.1/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4022 2023-08-07 20:19:37.000000 matgl-0.8.1/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:35.002981 matgl-0.8.1/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12494 2023-08-07 17:53:06.000000 matgl-0.8.1/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9147 2023-08-07 17:50:57.000000 matgl-0.8.1/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2255 2023-06-22 13:23:58.000000 matgl-0.8.1/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:35.004514 matgl-0.8.1/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1372 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10614 2023-08-07 21:30:43.000000 matgl-0.8.1/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7121 2023-07-28 14:26:46.000000 matgl-0.8.1/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-06-21 14:46:11.000000 matgl-0.8.1/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    13697 2023-07-10 14:51:23.000000 matgl-0.8.1/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:34.997609 matgl-0.8.1/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    13908 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1068 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       39 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/entry_points.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-08-08 01:47:34.000000 matgl-0.8.1/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2897 2023-08-07 19:46:19.000000 matgl-0.8.1/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-08-08 01:47:35.005795 matgl-0.8.1/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1958 2023-08-07 13:11:13.000000 matgl-0.8.1/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-08-08 01:47:35.005138 matgl-0.8.1/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)     1008 2023-08-07 17:00:26.000000 matgl-0.8.1/tests/test_cli.py
+-rw-r--r--   0 shyue      (501) staff       (20)      194 2023-06-15 14:49:26.000000 matgl-0.8.1/tests/test_config.py
+-rw-r--r--   0 shyue      (501) staff       (20)      656 2023-08-06 15:48:51.000000 matgl-0.8.1/tests/test_integration.py
```

### Comparing `matgl-0.8.0/LICENSE` & `matgl-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/PKG-INFO` & `matgl-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.8.0
+Version: 0.8.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -20,17 +20,17 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml/badge.svg)](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
-[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
+[![codecov](https://codecov.io/gh/materialsvirtuallab/matgl/branch/main/graph/badge.svg?token=3V3O79GODQ)](https://codecov.io/gh/materialsvirtuallab/matgl)
 
 # Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 ## Official Documentation [:books:]
 
 <https://matgl.ai>
 
@@ -175,14 +175,16 @@
 [jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
 - [API docs][apidocs] for all classes and methods.
 - [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
+- AdvancedSoft has implemented a [LAMMPS interface](https://github.com/advancesoftcorp/lammps/tree/based-on-lammps_2Jun2022/src/ML-M3GNET)
+  to both the TF and MatGL version of M3Gnet.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
```

### Comparing `matgl-0.8.0/README.md` & `matgl-0.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml/badge.svg)](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
-[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
+[![codecov](https://codecov.io/gh/materialsvirtuallab/matgl/branch/main/graph/badge.svg?token=3V3O79GODQ)](https://codecov.io/gh/materialsvirtuallab/matgl)
 
 # Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 ## Official Documentation [:books:]
 
 <https://matgl.ai>
 
@@ -151,14 +151,16 @@
 [jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
 - [API docs][apidocs] for all classes and methods.
 - [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
+- AdvancedSoft has implemented a [LAMMPS interface](https://github.com/advancesoftcorp/lammps/tree/based-on-lammps_2Jun2022/src/ML-M3GNET)
+  to both the TF and MatGL version of M3Gnet.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
```

### Comparing `matgl-0.8.0/matgl/apps/pes.py` & `matgl-0.8.1/matgl/apps/pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/cli.py` & `matgl-0.8.1/matgl/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Command line interface for matgl."""
 from __future__ import annotations
 
 import argparse
 import logging
 import os
-import sys
 import warnings
 
+import numpy as np
+import torch
 from pymatgen.core.structure import Structure
 from pymatgen.ext.matproj import MPRester
 
 import matgl
 from matgl.ext.ase import Relaxer
 
 warnings.simplefilter("ignore")
@@ -28,48 +29,67 @@
         structure = Structure.from_file(fn)
 
         if args.verbose:
             logging.basicConfig(level=logging.INFO)
 
         logger.info(f"Initial structure\n{structure}")
         logger.info("Loading model...")
-        pot = matgl.load_model("M3GNet-MP-2021.2.8-PES")
+        pot = matgl.load_model(args.model)
         logger.info("Relaxing...")
         relaxer = Relaxer(potential=pot)
         relax_results = relaxer.relax(structure, fmax=0.01)
         final_structure = relax_results["final_structure"]
 
         if args.suffix:
             basename, ext = os.path.splitext(fn)
             outfn = f"{basename}{args.suffix}{ext}"
             final_structure.to(filename=outfn)
             print(f"Structure written to {outfn}!")
         elif args.outfile is not None:
             final_structure.to(filename=args.outfile)
             print(f"Structure written to {args.outfile}!")
         else:
-            print("Final structure")
-            print(final_structure)
+            print("Lattice parameters")
+            old_lattice = structure.lattice
+            new_lattice = final_structure.lattice
+            for param in ("a", "b", "c", "alpha", "beta", "gamma"):
+                print(f"{param}: {getattr(old_lattice, param):.3f} -> {getattr(new_lattice, param):.3f}")
+            print("Sites (Fractional coordinates)")
+
+            def fmt_fcoords(fc):
+                return np.array2string(fc, formatter={"float_kind": lambda x: "%.5f" % x})
+
+            for old_site, new_site in zip(structure, final_structure):
+                print(f"{old_site.species}: {fmt_fcoords(old_site.frac_coords)} -> {fmt_fcoords(new_site.frac_coords)}")
 
     return 0
 
 
 def predict_structure(args):
     """
     Use MatGL models to perform predictions on structures.
 
     Args:
         args: Args from CLI.
     """
     model = matgl.load_model(args.model)
     if args.infile:
-        for f in args.infile:
-            structure = Structure.from_file(f)
-            val = model.predict_structure(structure)
-            print(f"{args.model} prediction for {f}: {val}.")
+        if args.model == "MEGNet-MP-2019.4.1-BandGap-mfi":
+            state_dict = ["PBE", "GLLB-SC", "HSE", "SCAN"]
+            for count, f in enumerate(args.infile):
+                s = args.state_attr[count]  # Get the corresponding state attribute
+                structure = Structure.from_file(f)
+                val = model.predict_structure(structure, torch.tensor(int(s)))
+                print(f"{args.model} prediction for {f} with {state_dict[int(s)]} bandgap: {val} eV.")
+
+        else:
+            for f in args.infile:
+                structure = Structure.from_file(f)
+                val = model.predict_structure(structure)
+                print(f"{args.model} prediction for {f}: {val} eV/atom.")
     if args.mpids:
         mpr = MPRester()
         for mid in args.mpids:
             structure = mpr.get_structure_by_material_id(mid)
             val = model.predict_structure(structure)
             print(f"{args.model} prediction for {mid} ({structure.composition.reduced_formula}): {val}.")
 
@@ -103,14 +123,23 @@
         dest="infile",
         nargs="+",
         required=True,
         help="Input files containing structure. Any format supported by pymatgen's Structure.from_file method.",
     )
 
     p_relax.add_argument(
+        "-m",
+        "--model",
+        dest="model",
+        choices=[m for m in matgl.get_available_pretrained_models() if m.endswith("PES")],
+        default="M3GNet-MP-2021.2.8-DIRECT-PES",
+        help="Model to use.",
+    )
+
+    p_relax.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         default=False,
         action="store_true",
         help="Verbose output.",
     )
@@ -148,14 +177,22 @@
         "--infile",
         dest="infile",
         nargs="+",
         help="Input files containing structure. Any format supported by pymatgen's Structure.from_file method.",
     )
 
     p_predict.add_argument(
+        "-s",
+        "--state",
+        dest="state_attr",
+        nargs="+",
+        help="state attributes containing label. This should be an integer.",
+    )
+
+    p_predict.add_argument(
         "-m",
         "--model",
         dest="model",
         choices=matgl.get_available_pretrained_models(),
         required=True,
         help="Model to use",
     )
@@ -172,12 +209,8 @@
         help="Skip confirmation.",
     )
 
     p_clear.set_defaults(func=clear_cache)
 
     args = parser.parse_args()
 
-    try:
-        return args.func(args)
-    except AttributeError:
-        parser.print_help()
-        sys.exit(-1)
+    return args.func(args)
```

### Comparing `matgl-0.8.0/matgl/config.py` & `matgl-0.8.1/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/data/transformer.py` & `matgl-0.8.1/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/ext/ase.py` & `matgl-0.8.1/matgl/ext/ase.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import collections
 import contextlib
 import io
 import pickle
 import sys
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal
 
 import numpy as np
 import pandas as pd
 import torch
 from ase import Atoms, units
 from ase.calculators.calculator import Calculator, all_changes
 from ase.constraints import ExpCellFilter
@@ -325,15 +325,15 @@
     """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
         state_attr: torch.Tensor | None = None,
-        ensemble: str = "nvt",
+        ensemble: Literal["nvt", "npt", "npt_berendsen"] = "nvt",
         temperature: int = 300,
         timestep: float = 1.0,
         pressure: float = 1.01325 * units.bar,
         taut: float | None = None,
         taup: float | None = None,
         compressibility_au: float | None = None,
         trajectory: str | Trajectory | None = None,
@@ -448,11 +448,13 @@
 
     def set_atoms(self, atoms: Atoms):
         """Set new atoms to run MD.
 
         Args:
             atoms (Atoms): new atoms for running MD.
         """
+        if isinstance(atoms, (Structure, Molecule)):
+            atoms = AseAtomsAdaptor().get_atoms(atoms)
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
```

### Comparing `matgl-0.8.0/matgl/ext/pymatgen.py` & `matgl-0.8.1/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/graph/compute.py` & `matgl-0.8.1/matgl/graph/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,15 @@
 
     Returns:
     cos_theta: torch.Tensor
     phi: torch.Tensor
     triple_bond_lengths (torch.tensor):
     """
     angles = compute_theta(edges, cosine=True)
-    angles.update(
-        {
-            "phi": torch.zeros_like(angles["cos_theta"]),
-        }
-    )
+    angles["phi"] = torch.zeros_like(angles["cos_theta"])
     return angles
 
 
 def compute_theta(edges: dgl.udf.EdgeBatch, cosine: bool = False) -> dict[str, torch.Tensor]:
     """User defined dgl function to calculate bond angles from edges in a graph.
 
     Args:
```

### Comparing `matgl-0.8.0/matgl/graph/converters.py` & `matgl-0.8.1/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/graph/data.py` & `matgl-0.8.1/matgl/graph/data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/__init__.py` & `matgl-0.8.1/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_activations.py` & `matgl-0.8.1/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_atom_ref.py` & `matgl-0.8.1/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_basis.py` & `matgl-0.8.1/matgl/layers/_basis.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_bond.py` & `matgl-0.8.1/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_core.py` & `matgl-0.8.1/matgl/layers/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     @property
     def last_linear(self) -> Linear | None:
         """:return: The last linear layer."""
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
                 return layer
-        return None
+        raise RuntimeError
 
     @property
     def depth(self) -> int:
         """Returns depth of MLP."""
         return self._depth
 
     @property
```

### Comparing `matgl-0.8.0/matgl/layers/_embedding.py` & `matgl-0.8.1/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_graph_convolution.py` & `matgl-0.8.1/matgl/layers/_graph_convolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,10 +451,11 @@
         :return: A tuple of updated features
         """
         edge_feat, node_feat, state_feat = self.conv(graph, edge_feat, node_feat, state_feat)
 
         if self.dropout:
             edge_feat = self.dropout(edge_feat)  # pylint: disable=E1102
             node_feat = self.dropout(node_feat)  # pylint: disable=E1102
-            state_feat = self.dropout(state_feat)  # pylint: disable=E1102
+            if state_feat is not None:
+                state_feat = self.dropout(state_feat)  # pylint: disable=E1102
 
         return edge_feat, node_feat, state_feat
```

### Comparing `matgl-0.8.0/matgl/layers/_readout.py` & `matgl-0.8.1/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/layers/_three_body.py` & `matgl-0.8.1/matgl/layers/_three_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             three_cutoff: cutoff radius
             node_feat: node features
             edge_feat: edge features.
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
-        atoms = torch.squeeze(atoms[end_atom_index])
+        atoms = torch.squeeze(atoms[end_atom_index.long()])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)  # type: ignore
         weights = torch.reshape(three_cutoff[torch.stack(list(line_graph.edges()), dim=1)], (-1, 2))  # type: ignore
         weights = torch.prod(weights, axis=-1)  # type: ignore
         basis = basis * weights[:, None]
         new_bonds = scatter_sum(
             basis.to(torch.float32),
```

### Comparing `matgl-0.8.0/matgl/models/_m3gnet.py` & `matgl-0.8.1/matgl/models/_m3gnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         elif activation_type == "sigmoid":
             activation = nn.Sigmoid()  # type: ignore
         elif activation_type == "softplus2":
             activation = SoftPlus2()  # type: ignore
         elif activation_type == "softexp":
             activation = SoftExponential()  # type: ignore
         else:
-            raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
+            raise ValueError("Invalid activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
         if element_types is None:
             self.element_types = DEFAULT_ELEMENT_TYPES
         else:
             self.element_types = element_types  # type: ignore
 
         self.bond_expansion = BondExpansion(max_l, max_n, cutoff, rbf_type=rbf_type, smooth=use_smooth)
@@ -201,15 +201,15 @@
             dims_final_layer = [readout_feats, units, units, ntargets]
             self.final_layer = MLP(dims_final_layer, activation, activate_last=False)
             if task_type == "classification":
                 self.sigmoid = nn.Sigmoid()
 
         else:
             if task_type == "classification":
-                raise ValueError("Classification task cannot be extensive")
+                raise ValueError("Classification task cannot be extensive.")
             self.final_layer = WeightedReadOut(
                 in_feats=dim_node_embedding, dims=[units, units], num_targets=ntargets  # type: ignore
             )
 
         self.max_n = max_n
         self.max_l = max_l
         self.n_blocks = nblocks
```

### Comparing `matgl-0.8.0/matgl/models/_megnet.py` & `matgl-0.8.1/matgl/models/_megnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         elif activation_type == "tanh":
             activation = nn.Tanh()
         elif activation_type == "softplus2":
             activation = SoftPlus2()
         elif activation_type == "softexp":
             activation = SoftExponential()
         else:
-            raise Exception("Undefined activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
+            raise ValueError("Invalid activation type, please try using swish, sigmoid, tanh, softplus2, softexp")
 
         self.embedding = EmbeddingBlock(
             degree_rbf=dim_edge_embedding,
             dim_node_embedding=dim_node_embedding,
             ntypes_node=len(self.element_types),
             ntypes_state=ntypes_state,
             include_state=include_state,
```

### Comparing `matgl-0.8.0/matgl/models/_wrappers.py` & `matgl-0.8.1/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/utils/cutoff.py` & `matgl-0.8.1/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/utils/io.py` & `matgl-0.8.1/matgl/utils/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,19 +107,17 @@
         fpaths = path if isinstance(path, dict) else _get_file_paths(Path(path), **kwargs)
 
         with open(fpaths["model.json"]) as f:
             model_data = json.load(f)
 
         _check_ver(cls, model_data)
 
-        if not torch.cuda.is_available():
-            state = torch.load(fpaths["state.pt"], map_location=torch.device("cpu"))
-        else:
-            state = torch.load(fpaths["state.pt"])
-        d = torch.load(fpaths["model.pt"])
+        map_location = torch.device("cpu") if not torch.cuda.is_available() else None
+        state = torch.load(fpaths["state.pt"], map_location=map_location)
+        d = torch.load(fpaths["model.pt"], map_location=map_location)
 
         # Deserialize any args that are IOMixIn subclasses.
         for k, v in d.items():
             if isinstance(v, dict) and "@class" in v and "@module" in v:
                 modname = v["@module"]
                 classname = v["@class"]
                 mod = __import__(modname, globals(), locals(), [classname], 0)
@@ -145,27 +143,30 @@
             force_download: To speed up access, a model with the same name in the cache location will be used if
             present. If you want to force a re-download, set this to True.
         """
         self.uri = uri
         toks = uri.split("/")
         self.model_name = toks[-2]
         self.fname = toks[-1]
-        cache_location = Path(cache_location)
-        os.makedirs(cache_location / self.model_name, exist_ok=True)
-        self.local_path = cache_location / self.model_name / self.fname
+        self.cache_location = Path(cache_location)
+        self.local_path = self.cache_location / self.model_name / self.fname
         if (not self.local_path.exists()) or force_download:
             logger.info("Downloading from remote location...")
             self._download()
         else:
             logger.info(f"Using cached local file at {self.local_path}...")
 
     def _download(self):
-        r = requests.get(self.uri, allow_redirects=True)
-        with open(self.local_path, "wb") as f:
-            f.write(r.content)
+        r = requests.get(self.uri)
+        if r.status_code == 200:
+            os.makedirs(self.cache_location / self.model_name, exist_ok=True)
+            with open(self.local_path, "wb") as f:
+                f.write(r.content)
+        else:
+            raise requests.RequestException(f"Bad uri: {self.uri}")
 
     def __enter__(self):
         """Support with context.
 
         Returns:
             Stream on local path.
         """
@@ -206,15 +207,15 @@
             classname = d["@class"]
 
             mod = __import__(modname, globals(), locals(), [classname], 0)
             cls_ = getattr(mod, classname)
             return cls_.load(fpaths, **kwargs)
     except BaseException:
         raise ValueError(
-            "Bad serialized model detected. It is possible that you have an older model cached. Please "
+            "Bad serialized model or bad model name. It is possible that you have an older model cached. Please "
             'clear your cache by running `python -c "import matgl; matgl.clear_cache()"`'
         ) from None
 
 
 def _get_file_paths(path: Path, **kwargs):
     """Search path for files.
 
@@ -234,19 +235,16 @@
     fnames = ("model.pt", "state.pt", "model.json")
 
     if all((path / fn).exists() for fn in fnames):
         return {fn: path / fn for fn in fnames}
 
     try:
         return {fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames}
-    except BaseException:
-        raise ValueError(
-            f"No valid model found in {path} or among pre-trained_models at "
-            f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
-        ) from None
+    except requests.RequestException:
+        raise ValueError(f"No valid model found in pre-trained_models at {PRETRAINED_MODELS_BASE_URL}.") from None
 
 
 def _check_ver(cls_, d: dict):
     """Check version of cls_ in current matgl against those noted in a model.json dict.
 
     Args:
         cls_: Class object.
```

### Comparing `matgl-0.8.0/matgl/utils/maths.py` & `matgl-0.8.1/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/utils/sb_roots.npy` & `matgl-0.8.1/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl/utils/training.py` & `matgl-0.8.1/matgl/utils/training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.8.0/matgl.egg-info/PKG-INFO` & `matgl-0.8.1/matgl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.8.0
+Version: 0.8.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -20,17 +20,17 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
-[![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
+[![Testing](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml/badge.svg)](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
-[![Coverage Status](https://coveralls.io/repos/github/materialsvirtuallab/matgl/badge.svg?branch=main)](https://coveralls.io/github/materialsvirtuallab/matgl?branch=main)
+[![codecov](https://codecov.io/gh/materialsvirtuallab/matgl/branch/main/graph/badge.svg?token=3V3O79GODQ)](https://codecov.io/gh/materialsvirtuallab/matgl)
 
 # Materials Graph Library <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
 
 ## Official Documentation [:books:]
 
 <https://matgl.ai>
 
@@ -175,14 +175,16 @@
 [jupyternb], which can be directly run on [Google Colab].
 
 ## Resources
 
 - [API docs][apidocs] for all classes and methods.
 - [Developer Guide](developer.md) outlines the key design elements of `matgl`, especially for developers wishing to
   train and contribute matgl models.
+- AdvancedSoft has implemented a [LAMMPS interface](https://github.com/advancesoftcorp/lammps/tree/based-on-lammps_2Jun2022/src/ML-M3GNET)
+  to both the TF and MatGL version of M3Gnet.
 
 ## References
 
 A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
 information. If you are using any of the pretrained models, please cite the relevant works below:
 
 > **MEGNet**
```

### Comparing `matgl-0.8.0/matgl.egg-info/SOURCES.txt` & `matgl-0.8.1/matgl.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,9 +38,10 @@
 matgl/models/_wrappers.py
 matgl/utils/__init__.py
 matgl/utils/cutoff.py
 matgl/utils/io.py
 matgl/utils/maths.py
 matgl/utils/sb_roots.npy
 matgl/utils/training.py
+tests/test_cli.py
 tests/test_config.py
 tests/test_integration.py
```

### Comparing `matgl-0.8.0/pyproject.toml` & `matgl-0.8.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -109,9 +109,13 @@
   "if 0:",
   "if __name__ == .__main__.:",
   "if self.debug:",
   "if settings.DEBUG",
   "pragma: no cover",
   "raise AssertionError",
   "raise NotImplementedError",
-  "input"
+  "input",
+  "if TYPE_CHECKING:",
+  "except PackageNotFoundError:",
+  "raise RuntimeError",
+  "logging.basicConfig"
 ]
```

### Comparing `matgl-0.8.0/setup.py` & `matgl-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.8.0",
+    version="0.8.1",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

