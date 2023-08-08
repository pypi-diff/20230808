# Comparing `tmp/cblearn-0.1.0.tar.gz` & `tmp/cblearn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cblearn-0.1.0.tar", last modified: Wed Mar 22 13:44:29 2023, max compression
+gzip compressed data, was "cblearn-0.1.1.tar", last modified: Tue Aug  8 20:52:58 2023, max compression
```

## Comparing `cblearn-0.1.0.tar` & `cblearn-0.1.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.090994 cblearn-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-22 13:44:13.000000 cblearn-0.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-22 13:44:13.000000 cblearn-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-22 13:44:13.000000 cblearn-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-22 13:44:13.000000 cblearn-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-03-22 13:44:29.090994 cblearn-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-03-22 13:44:13.000000 cblearn-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.090994 cblearn-0.1.0/cblearn/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-22 13:44:29.090994 cblearn-0.1.0/cblearn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.070994 cblearn-0.1.0/cblearn/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/cluster/_comparison_hc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.070994 cblearn-0.1.0/cblearn/cluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/cluster/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/cluster/tests/test_comparison_hc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.074994 cblearn-0.1.0/cblearn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_car_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_food_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_imagenet_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_material_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_musician_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_nature_vogue_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_similarity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_things_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_triplet_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_triplet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/_triplet_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.074994 cblearn-0.1.0/cblearn/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/data/musician_names.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.078994 cblearn-0.1.0/cblearn/datasets/descr/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/car_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/food_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/imagenet_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/material_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/musician_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/nature_vogue_similarity.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/similarity_matrix.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/descr/things_similarity.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.078994 cblearn-0.1.0/cblearn/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/tests/test_food_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/tests/test_musician_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/datasets/tests/test_triplet_indices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.078994 cblearn-0.1.0/cblearn/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_ckl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_forte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_gnmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_mlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_oenn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_soe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/_torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.082994 cblearn-0.1.0/cblearn/embedding/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/wrapper/_mlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/wrapper/_r_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/embedding/wrapper/_soe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.082994 cblearn-0.1.0/cblearn/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/_triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.082994 cblearn-0.1.0/cblearn/metrics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/tests/test_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/metrics/tests/test_triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.082994 cblearn-0.1.0/cblearn/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/preprocessing/_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/preprocessing/_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.082994 cblearn-0.1.0/cblearn/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/preprocessing/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/cblearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/_data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/_validate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/_validate_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/cblearn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/tests/test_validate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-22 13:44:13.000000 cblearn-0.1.0/cblearn/utils/tests/test_validate_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.070994 cblearn-0.1.0/cblearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-03-22 13:44:29.000000 cblearn-0.1.0/cblearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-03-22 13:44:29.000000 cblearn-0.1.0/cblearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:44:29.000000 cblearn-0.1.0/cblearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:44:28.000000 cblearn-0.1.0/cblearn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-22 13:44:29.000000 cblearn-0.1.0/cblearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 13:44:29.000000 cblearn-0.1.0/cblearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/docs/contributor_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/contributor_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/docs/references/
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/references/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.086994 cblearn-0.1.0/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-22 13:44:13.000000 cblearn-0.1.0/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:44:29.090994 cblearn-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-22 13:44:13.000000 cblearn-0.1.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-22 13:44:13.000000 cblearn-0.1.0/examples/ordinal_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-03-22 13:44:13.000000 cblearn-0.1.0/examples/plot_psychophysical_scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-22 13:44:13.000000 cblearn-0.1.0/examples/small_embedding_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-22 13:44:13.000000 cblearn-0.1.0/examples/triplet_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-22 13:44:13.000000 cblearn-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-22 13:44:29.090994 cblearn-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-22 13:44:13.000000 cblearn-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-22 13:44:13.000000 cblearn-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.816126 cblearn-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 20:52:47.000000 cblearn-0.1.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-08 20:52:47.000000 cblearn-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 20:52:47.000000 cblearn-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 20:52:47.000000 cblearn-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-08-08 20:52:58.816126 cblearn-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-08-08 20:52:47.000000 cblearn-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.816126 cblearn-0.1.1/cblearn/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 20:52:58.816126 cblearn-0.1.1/cblearn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.804127 cblearn-0.1.1/cblearn/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9509 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/cluster/_comparison_hc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.804127 cblearn-0.1.1/cblearn/cluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/cluster/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/cluster/tests/test_comparison_hc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.808127 cblearn-0.1.1/cblearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_car_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_food_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_imagenet_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_material_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_musician_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_nature_vogue_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_similarity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_things_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_triplet_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_triplet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/_triplet_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.808127 cblearn-0.1.1/cblearn/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/data/musician_names.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.808127 cblearn-0.1.1/cblearn/datasets/descr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/car_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/food_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/imagenet_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/material_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/musician_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/nature_vogue_similarity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/similarity_matrix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/descr/things_similarity.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.808127 cblearn-0.1.1/cblearn/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/tests/test_food_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/tests/test_musician_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/datasets/tests/test_triplet_indices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.808127 cblearn-0.1.1/cblearn/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_ckl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_forte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_gnmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_mlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_oenn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_soe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/embedding/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/wrapper/_mlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/wrapper/_r_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/embedding/wrapper/_soe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/_triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/tests/test_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/metrics/tests/test_triplets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/preprocessing/_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/preprocessing/_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/preprocessing/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/_data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/_validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/_validate_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/cblearn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/tests/test_validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-08 20:52:47.000000 cblearn-0.1.1/cblearn/utils/tests/test_validate_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.804127 cblearn-0.1.1/cblearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 20:52:58.000000 cblearn-0.1.1/cblearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/docs/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.812126 cblearn-0.1.1/docs/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/references/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.816126 cblearn-0.1.1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-08 20:52:47.000000 cblearn-0.1.1/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:52:58.816126 cblearn-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 20:52:47.000000 cblearn-0.1.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-08-08 20:52:47.000000 cblearn-0.1.1/examples/ordinal_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-08-08 20:52:47.000000 cblearn-0.1.1/examples/plot_psychophysical_scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-08 20:52:47.000000 cblearn-0.1.1/examples/small_embedding_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-08 20:52:47.000000 cblearn-0.1.1/examples/triplet_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-08 20:52:47.000000 cblearn-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-08 20:52:58.816126 cblearn-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-08 20:52:47.000000 cblearn-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-08-08 20:52:47.000000 cblearn-0.1.1/versioneer.py
```

### Comparing `cblearn-0.1.0/LICENSE` & `cblearn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/PKG-INFO` & `cblearn-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblearn
-Version: 0.1.0
+Version: 0.1.1
 Summary: Comparison-based Machine Learning in Python.
 Home-page: https://github.com/dekuenstle/cblearn
 Author: David-Elias Künstle
 Author-email: david-elias.kuenstle@uni-tuebingen.de
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
@@ -27,31 +27,27 @@
 Provides-Extra: octave_wrapper
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # cblearn
 ## Comparison-based Machine Learning in Python
-:warning: **cblearn** is **work in progress**. The API can change and bugs appear. Please help us by posting an [issue]( https://github.com/dekuenstle/cblearn/issues/new) :construction:
-
 [![PyPI version](https://img.shields.io/pypi/v/cblearn.svg)](https://pypi.python.org/pypi/cblearn)
 [![Documentation](https://readthedocs.org/projects/cblearn/badge/?version=latest)](https://cblearn.readthedocs.io/en/latest/?badge=latest)
-[![Unit tests](https://github.com/dekuenstle/cblearn/workflows/Python%20package/badge.svg)](https://github.com/dekuenstle/cblearn/actions)
-[![Test Coverage](https://codecov.io/gh/dekuenstle/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/dekuenstle/cblearn)
+[![Test status](https://github.com/cblearn/cblearn/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/cblearn/cblearn/actions/workflows/test.yml)
+[![Test Coverage](https://codecov.io/gh/cblearn/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/cblearn/cblearn)
 
 Comparison-based Learning algorithms are the Machine Learning algorithms to use when training data contains similarity comparisons ("A and B are more similar than C and D") instead of data points. 
 
-**:eyes: VSS 2022: Please find an example of psychophysical scaling with triplets and ordinal embedding [here](https://cblearn.readthedocs.io/en/latest/generated_examples/plot_psychophysical_scales.html) :eyes:**
-
 Triplet comparisons from human observers help model the perceived similarity of objects.
 These human triplets are collected in studies, asking questions like 
 "Which of the following bands is most similar to Queen?" or 
-"Which colour appears most similar to the reference?".
+"Which color appears most similar to the reference?".
 
-This library provides an easy to use interface to comparison-based learning algorithms.
+This library provides an easy-to-use interface for comparison-based learning algorithms.
 It plays hand-in-hand with scikit-learn:
 
 ```python
 from sklearn.datasets import load_iris
 from sklearn.model_selection import cross_val_score
 
 from cblearn.datasets import make_random_triplets
@@ -116,29 +112,35 @@
 We are happy about your bug reports, questions or suggestions as Github Issues and code or documentation contributions as Github Pull Requests. 
 Please see our [Contributor Guide](https://cblearn.readthedocs.io/en/latest/contributor_guide/index.html). 
 
 ## Authors and Acknowledgement
 *cblearn* was initiated by current and former members of the [Theory of Machine Learning group](http://www.tml.cs.uni-tuebingen.de/index.php) of Prof. Dr. Ulrike von Luxburg at the University of Tübingen.
 The leading developer is [David-Elias Künstle](http://www.tml.cs.uni-tuebingen.de/team/kuenstle/index.php).
 
-We would like to thank all the contributors here on Github.
+We want to thank all the contributors here on GitHub.
 This work has been supported by the Machine Learning Cluster of Excellence, funded by EXC number 2064/1 – Project number 390727645. The authors would like to thank the International Max Planck Research School for Intelligent Systems (IMPRS-IS) for supporting David-Elias Künstle. 
 
 ## License
 
-This library is free to use under the [MIT License](https://github.com/dekuenstle/cblearn/blob/master/LICENSE) conditions.
-Please reference this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used. 
+This library is free under the [MIT License](https://github.com/cblearn/cblearn/blob/master/LICENSE) conditions.
+Please cite this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used. 
 
 # Changelog
 
+## 0.1.1
+
+- Minor fixes in the documentation.
+- Adapt loading of food and imagenet dataset to solve problems caused by changes in externally hosted files
+  
 ## 0.1.0
 
 - Support python 3.9 and 3.10.
 - Introduce semantic versioning
 - Publish to PyPI
+
 MIT License
 
 Copyright (c) 2020-2021 The cblearn developers.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `cblearn-0.1.0/README.md` & `cblearn-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # cblearn
 ## Comparison-based Machine Learning in Python
-:warning: **cblearn** is **work in progress**. The API can change and bugs appear. Please help us by posting an [issue]( https://github.com/dekuenstle/cblearn/issues/new) :construction:
-
 [![PyPI version](https://img.shields.io/pypi/v/cblearn.svg)](https://pypi.python.org/pypi/cblearn)
 [![Documentation](https://readthedocs.org/projects/cblearn/badge/?version=latest)](https://cblearn.readthedocs.io/en/latest/?badge=latest)
-[![Unit tests](https://github.com/dekuenstle/cblearn/workflows/Python%20package/badge.svg)](https://github.com/dekuenstle/cblearn/actions)
-[![Test Coverage](https://codecov.io/gh/dekuenstle/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/dekuenstle/cblearn)
+[![Test status](https://github.com/cblearn/cblearn/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/cblearn/cblearn/actions/workflows/test.yml)
+[![Test Coverage](https://codecov.io/gh/cblearn/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/cblearn/cblearn)
 
 Comparison-based Learning algorithms are the Machine Learning algorithms to use when training data contains similarity comparisons ("A and B are more similar than C and D") instead of data points. 
 
-**:eyes: VSS 2022: Please find an example of psychophysical scaling with triplets and ordinal embedding [here](https://cblearn.readthedocs.io/en/latest/generated_examples/plot_psychophysical_scales.html) :eyes:**
-
 Triplet comparisons from human observers help model the perceived similarity of objects.
 These human triplets are collected in studies, asking questions like 
 "Which of the following bands is most similar to Queen?" or 
-"Which colour appears most similar to the reference?".
+"Which color appears most similar to the reference?".
 
-This library provides an easy to use interface to comparison-based learning algorithms.
+This library provides an easy-to-use interface for comparison-based learning algorithms.
 It plays hand-in-hand with scikit-learn:
 
 ```python
 from sklearn.datasets import load_iris
 from sklearn.model_selection import cross_val_score
 
 from cblearn.datasets import make_random_triplets
@@ -85,14 +81,14 @@
 We are happy about your bug reports, questions or suggestions as Github Issues and code or documentation contributions as Github Pull Requests. 
 Please see our [Contributor Guide](https://cblearn.readthedocs.io/en/latest/contributor_guide/index.html). 
 
 ## Authors and Acknowledgement
 *cblearn* was initiated by current and former members of the [Theory of Machine Learning group](http://www.tml.cs.uni-tuebingen.de/index.php) of Prof. Dr. Ulrike von Luxburg at the University of Tübingen.
 The leading developer is [David-Elias Künstle](http://www.tml.cs.uni-tuebingen.de/team/kuenstle/index.php).
 
-We would like to thank all the contributors here on Github.
+We want to thank all the contributors here on GitHub.
 This work has been supported by the Machine Learning Cluster of Excellence, funded by EXC number 2064/1 – Project number 390727645. The authors would like to thank the International Max Planck Research School for Intelligent Systems (IMPRS-IS) for supporting David-Elias Künstle. 
 
 ## License
 
-This library is free to use under the [MIT License](https://github.com/dekuenstle/cblearn/blob/master/LICENSE) conditions.
-Please reference this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used. 
+This library is free under the [MIT License](https://github.com/cblearn/cblearn/blob/master/LICENSE) conditions.
+Please cite this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used.
```

### Comparing `cblearn-0.1.0/cblearn/cluster/_comparison_hc.py` & `cblearn-0.1.1/cblearn/cluster/_comparison_hc.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/cluster/tests/test_comparison_hc.py` & `cblearn-0.1.1/cblearn/cluster/tests/test_comparison_hc.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/__init__.py` & `cblearn-0.1.1/cblearn/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_car_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_car_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_food_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_food_similarity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 import logging
 import joblib
 import os
 from typing import Optional, Union
 import zipfile
+import ssl
 
 import numpy as np
 from sklearn.datasets import _base
 from sklearn.utils import check_random_state, Bunch
 
 
 ARCHIVE = _base.RemoteFileMetadata(
@@ -19,14 +20,18 @@
 
 
 def fetch_food_similarity(data_home: Optional[os.PathLike] = None, download_if_missing: bool = True,
                           shuffle: bool = True, random_state: Optional[np.random.RandomState] = None,
                           return_triplets: bool = False) -> Union[Bunch, np.ndarray]:
     """ Load the Food-100 food similarity dataset (triplets).
 
+    .. warning::
+        This function downloads the file without verifying the ssl signature to circumvent an outdated certificate of the dataset hosts.
+        However, after downloading the function verifies the file checksum before loading the file to minimize the risk of man-in-the-middle attacks.
+    
     ===================   =====================
     Triplets                             190376
     Objects                                 100
     Dimensionality                      unknown
     ===================   =====================
 
     See :ref:`food_similarity_dataset` for a detailed description.
@@ -68,15 +73,21 @@
     filepath = Path(_base._pkl_filepath(data_home, 'food_similarity.pkz'))
     if not filepath.exists():
         if not download_if_missing:
             raise IOError("Data not found and `download_if_missing` is False")
 
         logger.info('Downloading food similarity from {} to {}'.format(ARCHIVE.url, data_home))
 
-        archive_path = _base._fetch_remote(ARCHIVE, dirname=data_home)
+        try:
+            ssl_default = ssl._create_default_https_context
+            ssl._create_default_https_context = ssl._create_unverified_context
+            archive_path = _base._fetch_remote(ARCHIVE, dirname=data_home)
+        finally:
+            ssl._create_default_https_context = ssl_default
+            
         with zipfile.ZipFile(archive_path) as zf:
             with zf.open('food100-dataset/all-triplets.csv', 'r') as f:
                 triplets = np.loadtxt(f, dtype=str, delimiter=';')
 
             image_names = np.asarray([name[len('food100-dataset/'):] for name in zf.namelist()
                                       if name.startswith('food100-dataset/images/')
                                       and name.endswith('.jpg')])
```

### Comparing `cblearn-0.1.0/cblearn/datasets/_imagenet_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_imagenet_similarity.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,21 +108,21 @@
         archive_path = (ARCHIVE.filename if data_home is None
                         else join(data_home, ARCHIVE.filename))
         urlretrieve(ARCHIVE.url, archive_path)
 
         with zipfile.ZipFile(archive_path) as zf:
             import h5py
 
-            with zf.open('val/data/psiz0.4.1/obs-118.hdf5', 'r') as f:
+            with zf.open('data/deprecated/psiz0.4.1/obs-118.hdf5', 'r') as f:
                 data_v1 = {k: np.asarray(v[()]) for k, v in h5py.File(f, mode='r').items()}
 
-            with zf.open('val/data/psiz0.4.1/obs-195.hdf5', 'r') as f:
+            with zf.open('data/deprecated/psiz0.4.1/obs-195.hdf5', 'r') as f:
                 data_v2 = {k: np.asarray(v[()]) for k, v in h5py.File(f, mode='r').items()}
 
-            with zf.open('val/data/psiz0.4.1/catalog.hdf5', 'r') as f:
+            with zf.open('data/deprecated/psiz0.4.1/catalog.hdf5', 'r') as f:
                 catalog = {k: np.asarray(v[()]) for k, v in h5py.File(f, mode='r').items()}
 
         joblib.dump((data_v1, data_v2, catalog), filepath, compress=6)
         os.remove(archive_path)
     else:
         (data_v1, data_v2, catalog) = joblib.load(filepath)
```

### Comparing `cblearn-0.1.0/cblearn/datasets/_material_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_material_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_musician_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_musician_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_nature_vogue_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_nature_vogue_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_similarity_matrix.py` & `cblearn-0.1.1/cblearn/datasets/_similarity_matrix.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_things_similarity.py` & `cblearn-0.1.1/cblearn/datasets/_things_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_triplet_indices.py` & `cblearn-0.1.1/cblearn/datasets/_triplet_indices.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_triplet_response.py` & `cblearn-0.1.1/cblearn/datasets/_triplet_response.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/_triplet_simulation.py` & `cblearn-0.1.1/cblearn/datasets/_triplet_simulation.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/data/musician_names.txt` & `cblearn-0.1.1/cblearn/datasets/data/musician_names.txt`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/car_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/car_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/food_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/food_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/imagenet_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/imagenet_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/material_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/material_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/musician_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/musician_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/nature_vogue_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/nature_vogue_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/similarity_matrix.rst` & `cblearn-0.1.1/cblearn/datasets/descr/similarity_matrix.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/descr/things_similarity.rst` & `cblearn-0.1.1/cblearn/datasets/descr/things_similarity.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/tests/test_food_similarity.py` & `cblearn-0.1.1/cblearn/datasets/tests/test_food_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/tests/test_musician_similarity.py` & `cblearn-0.1.1/cblearn/datasets/tests/test_musician_similarity.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/datasets/tests/test_triplet_indices.py` & `cblearn-0.1.1/cblearn/datasets/tests/test_triplet_indices.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_base.py` & `cblearn-0.1.1/cblearn/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_ckl.py` & `cblearn-0.1.1/cblearn/embedding/_ckl.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_forte.py` & `cblearn-0.1.1/cblearn/embedding/_forte.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_gnmds.py` & `cblearn-0.1.1/cblearn/embedding/_gnmds.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_mlds.py` & `cblearn-0.1.1/cblearn/embedding/_mlds.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_oenn.py` & `cblearn-0.1.1/cblearn/embedding/_oenn.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_soe.py` & `cblearn-0.1.1/cblearn/embedding/_soe.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_ste.py` & `cblearn-0.1.1/cblearn/embedding/_ste.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/_torch_utils.py` & `cblearn-0.1.1/cblearn/embedding/_torch_utils.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/wrapper/_mlds.py` & `cblearn-0.1.1/cblearn/embedding/wrapper/_mlds.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/wrapper/_r_base.py` & `cblearn-0.1.1/cblearn/embedding/wrapper/_r_base.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/embedding/wrapper/_soe.py` & `cblearn-0.1.1/cblearn/embedding/wrapper/_soe.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/metrics/_procrustes.py` & `cblearn-0.1.1/cblearn/metrics/_procrustes.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/metrics/_triplets.py` & `cblearn-0.1.1/cblearn/metrics/_triplets.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/metrics/tests/test_procrustes.py` & `cblearn-0.1.1/cblearn/metrics/tests/test_procrustes.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/metrics/tests/test_triplets.py` & `cblearn-0.1.1/cblearn/metrics/tests/test_triplets.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/preprocessing/_label.py` & `cblearn-0.1.1/cblearn/preprocessing/_label.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/preprocessing/_query.py` & `cblearn-0.1.1/cblearn/preprocessing/_query.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/preprocessing/tests/test_query.py` & `cblearn-0.1.1/cblearn/preprocessing/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/utils/_data_format.py` & `cblearn-0.1.1/cblearn/utils/_data_format.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/utils/_validate_data.py` & `cblearn-0.1.1/cblearn/utils/_validate_data.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/utils/_validate_size.py` & `cblearn-0.1.1/cblearn/utils/_validate_size.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn/utils/tests/test_validate_data.py` & `cblearn-0.1.1/cblearn/utils/tests/test_validate_data.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/cblearn.egg-info/PKG-INFO` & `cblearn-0.1.1/cblearn.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cblearn
-Version: 0.1.0
+Version: 0.1.1
 Summary: Comparison-based Machine Learning in Python.
 Home-page: https://github.com/dekuenstle/cblearn
 Author: David-Elias Künstle
 Author-email: david-elias.kuenstle@uni-tuebingen.de
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
@@ -27,31 +27,27 @@
 Provides-Extra: octave_wrapper
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 # cblearn
 ## Comparison-based Machine Learning in Python
-:warning: **cblearn** is **work in progress**. The API can change and bugs appear. Please help us by posting an [issue]( https://github.com/dekuenstle/cblearn/issues/new) :construction:
-
 [![PyPI version](https://img.shields.io/pypi/v/cblearn.svg)](https://pypi.python.org/pypi/cblearn)
 [![Documentation](https://readthedocs.org/projects/cblearn/badge/?version=latest)](https://cblearn.readthedocs.io/en/latest/?badge=latest)
-[![Unit tests](https://github.com/dekuenstle/cblearn/workflows/Python%20package/badge.svg)](https://github.com/dekuenstle/cblearn/actions)
-[![Test Coverage](https://codecov.io/gh/dekuenstle/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/dekuenstle/cblearn)
+[![Test status](https://github.com/cblearn/cblearn/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/cblearn/cblearn/actions/workflows/test.yml)
+[![Test Coverage](https://codecov.io/gh/cblearn/cblearn/branch/master/graph/badge.svg?token=P9JRT6OK6O)](https://codecov.io/gh/cblearn/cblearn)
 
 Comparison-based Learning algorithms are the Machine Learning algorithms to use when training data contains similarity comparisons ("A and B are more similar than C and D") instead of data points. 
 
-**:eyes: VSS 2022: Please find an example of psychophysical scaling with triplets and ordinal embedding [here](https://cblearn.readthedocs.io/en/latest/generated_examples/plot_psychophysical_scales.html) :eyes:**
-
 Triplet comparisons from human observers help model the perceived similarity of objects.
 These human triplets are collected in studies, asking questions like 
 "Which of the following bands is most similar to Queen?" or 
-"Which colour appears most similar to the reference?".
+"Which color appears most similar to the reference?".
 
-This library provides an easy to use interface to comparison-based learning algorithms.
+This library provides an easy-to-use interface for comparison-based learning algorithms.
 It plays hand-in-hand with scikit-learn:
 
 ```python
 from sklearn.datasets import load_iris
 from sklearn.model_selection import cross_val_score
 
 from cblearn.datasets import make_random_triplets
@@ -116,29 +112,35 @@
 We are happy about your bug reports, questions or suggestions as Github Issues and code or documentation contributions as Github Pull Requests. 
 Please see our [Contributor Guide](https://cblearn.readthedocs.io/en/latest/contributor_guide/index.html). 
 
 ## Authors and Acknowledgement
 *cblearn* was initiated by current and former members of the [Theory of Machine Learning group](http://www.tml.cs.uni-tuebingen.de/index.php) of Prof. Dr. Ulrike von Luxburg at the University of Tübingen.
 The leading developer is [David-Elias Künstle](http://www.tml.cs.uni-tuebingen.de/team/kuenstle/index.php).
 
-We would like to thank all the contributors here on Github.
+We want to thank all the contributors here on GitHub.
 This work has been supported by the Machine Learning Cluster of Excellence, funded by EXC number 2064/1 – Project number 390727645. The authors would like to thank the International Max Planck Research School for Intelligent Systems (IMPRS-IS) for supporting David-Elias Künstle. 
 
 ## License
 
-This library is free to use under the [MIT License](https://github.com/dekuenstle/cblearn/blob/master/LICENSE) conditions.
-Please reference this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used. 
+This library is free under the [MIT License](https://github.com/cblearn/cblearn/blob/master/LICENSE) conditions.
+Please cite this library appropriately if it contributes to your scientific publication. We would also appreciate a short email (optionally) to see how our library is being used. 
 
 # Changelog
 
+## 0.1.1
+
+- Minor fixes in the documentation.
+- Adapt loading of food and imagenet dataset to solve problems caused by changes in externally hosted files
+  
 ## 0.1.0
 
 - Support python 3.9 and 3.10.
 - Introduce semantic versioning
 - Publish to PyPI
+
 MIT License
 
 Copyright (c) 2020-2021 The cblearn developers.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `cblearn-0.1.0/cblearn.egg-info/SOURCES.txt` & `cblearn-0.1.1/cblearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/docs/Makefile` & `cblearn-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/docs/conf.py` & `cblearn-0.1.1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'cblearn'
-author = 'David-Elias Künstle, Leena Suresh, Siyavash Haghiri, Michael Perrot, Debarghya Ghoshdastidari, Ulrike von Luxburg'
-copyright = f'2021, {author}'
+author = 'David-Elias Künstle & Ulrike von Luxburg'
+copyright = f'2023, {author}'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
@@ -67,17 +67,15 @@
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
-rst_prolog = """.. attention::
-    cblearn is work in progress. The API is still changing and a errors are known. Please help us by posting an issue on Github.
-"""
+rst_prolog = """"""
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
```

### Comparing `cblearn-0.1.0/docs/contributor_guide/index.rst` & `cblearn-0.1.1/docs/contributor_guide/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,51 +9,51 @@
 .. _Github issues: https://github.com/dekuenstle/cblearn/issues
 
 
 ---------------
 Getting Started
 ---------------
 
-We assume, you downloaded and installed cblearn as described in :ref:`developer_install`.
+We assume you downloaded and installed ``cblearn`` as described in :ref:`developer_install`.
 
 The project directory contains the code directory ``cblearn/`` and the documentation ``docs/``.
-In addition, there are readme, license, and a multiple configuration files as well as an examples folder.
+In addition, the folder contains a readme, license, multiple configuration files, and an examples folder.
 
 -------------
 Changing Code
 -------------
 
 The Python code is structured in :ref:`modules`. Each module contains
-a `tests` folder with unit-tests.
+a `tests` folder with unit tests.
 There should be such a test for every method and function.
-Use ``pytest --cov`` to run these tests and to measure the coverage, no tests should fail.
+Use ``pytest --cov`` to run these tests and to measure the coverage; no tests should fail.
 The coverage indicates the tested fraction of code and should be close to *100%*.
 You can exclude some of the more time expensive tests by ``pytest -m "not (sklearn or download)``.
 
 All Python code follows the `PEP8 Style Guide`_. The style
 of all code can be checked, running ``flake8 .`` and should print no warnings.
 
-Every class, method, and function should also have a docstring, describing the functionality and parameters.
+Every class, method, and function should have a docstring describing the functionality and parameters.
 Please follow the `Google Docstring Style`_.
 The docstring will be added to the :ref:`api_ref` by adding the function name in ``docs/references/index.rst``.
 Check the syntax of the docstring by running ``make html`` in the ``docs/`` folder.
 
-Types should not be added to the docstring, but in the code as `type hints`_.
+Types should not be added to the docstring but in the code as `type hints`_.
 Typechecks can be performed using ``mypy cblearn``.
 
 .. _PEP8 Style Guide: https://www.python.org/dev/peps/pep-0008/
 .. _Google Docstring Style: https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html
 .. _type hints: https://docs.python.org/3/library/typing.html
 
 ----------------------
 Changing Documentation
 ----------------------
 
 The documentation is contained in the `docs/` folder.
-It can be build by running ``make html``.
+It can be built by running ``make html``.
 Open ``docs/_build/html/index.html`` in a browser to view the local build of the documentation.
 
 The documentation is structured in multiple folders and written as `reStructuredText`_.
 
 .. _reStructuredText: https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html
 
 -----------------------------------
@@ -61,42 +61,42 @@
 -----------------------------------
 
 Instead of running the different tests above independently, it is also possible
 to run the whole testing workflow, which is used on Github, locally.
 
 Install nektos' `act`_ and then run `act -P ubuntu-latest=nektos/act-environments-ubuntu:18.04-full`
 
-`act` is using docker images with preinstalled software to provide almost the same test environment as Github.
-If it is not yet so, you have to `install docker`_ and, optionally, make it accessible for nonroot user.
+`act` uses docker images with preinstalled software to provide almost the same test environment as Github.
+If it is not yet so, you have to `install docker`_ and, optionally, make it accessible for non-root users.
 
 .. note::
     The docker image requires about 18 GB disk space. The first start of act might take some time,
     because it downloads about 12 GB of image files.
 
 .. _act: https://github.com/nektos/act
 .. _`install docker`: https://docs-stage.docker.com/engine/install/
 .. _`accessible for nonroot user`: https://docs.docker.com/engine/install/linux-postinstall/
 
 ------------------
 Publish Changes
 ------------------
 
-Most contributions will change files either in the code or in the documentation directory, as described in the
+Most contributions will change files in the code or the documentation directory, as described in the
 sections below. Commit your changes to a separate *git* branch (do **not** commit to ``master``).
-After you finished changing push this branch to Github and open a pull request to the ``master`` branch there.
+After changing, push this branch to Github and open a pull request to the ``master`` branch there.
 Once the request is opened, automated tests are run.
 If these tests indicate a problem, you can fix this problem on your branch and push again.
-Once the automated tests are successful, maintainers of cblearn will review the changes and provide feedback.
-Usually after some iterations, your changes will be merged to the ``master`` branch.
+Once the automated tests are successful, maintainers of ``cblearn`` will review the changes and provide feedback.
+Usually, after some iterations, your changes will be merged into the ``main`` branch.
 
 .. Note:
 
     If you state a pull request, your changes will be published under `this open source license`_.
 
 .. _this open source license: https://github.com/dekuenstle/cblearn/blob/master/LICENSE
 
 
 Versions should be semantic and follow PIP440_: The version indicates ``major.minor.fix``;
 breaking changes are just allowed with major version steps. 
-A new version is indicated with a Github release tag, which trigger continuous deployment to PyPI via Github Actions.
+A Github release tag indicates a new version, which triggers a continuous deployment to PyPI via Github Actions.
 
 .. _PIP440: https://peps.python.org/pep-0440/
```

### Comparing `cblearn-0.1.0/docs/index.rst` & `cblearn-0.1.1/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,14 @@
    sphinx-quickstart on Thu Sep 24 11:10:46 2020.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to cblearn's documentation!
 ===================================
 
-.. warning::
-    cblearn is work in progress. The API can change and bugs appear. Please help us by posting an issue on Github.
-
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    install
    user_guide/index
    generated_examples/index.rst
```

### Comparing `cblearn-0.1.0/docs/install.rst` & `cblearn-0.1.1/docs/install.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ============
 Installation
 ============
 
-cblearn requires Python 3.8 or newer.
+``cblearn`` requires Python 3.9 or newer.
 We recommend using Anaconda_ to install Python and
 dependencies in separated environments.
-We support Linux (tested on Ubuntu 20.4), Windows and Mac OS.
+We mainly test on Linux (tested on Ubuntu 20.4), but Windows and Mac OS should also work.
 Examples in this installation guide Linux shell commands.
 
 .. _Anaconda: https://docs.anaconda.com/anaconda/install/
 
 ```
-conda create -n cblearn python==3.8
+conda create -n cblearn python==3.9
 conda activate cblearn
 ```
 
 -----------------
 User Installation
 -----------------
 
-cblearn and its dependencies can be installed using `pip`:
+``cblearn`` and its dependencies can be installed using `pip`:
 
 .. code-block:: bash
 
     $ pip install cblearn
 
 
 .. _extras_install:
@@ -32,16 +32,16 @@
 ===================
 
 The installation routine above installs a minimal set of required packages, sufficient
 for most uses.
 However, some features require more packages that can be installed by adding 
 an `option` to the install command..
 
-For example, to use estimators on GPU, based on pytorch, and estimators
-wrapping paper author's original implementation in R-lang:
+For example, to use estimators on GPU, based on ``pytorch``, and estimators
+wrapping paper author's original implementation in ``R``-lang:
 
 .. code-block:: bash
 
     $ pip install git+https://github.com/dekuenstle/cblearn.git#egg=cblearn[torch,wrapper]
 
 ======= =============================================================
 Extras  Description
@@ -58,14 +58,14 @@
 ------------------------
 Contributor Installation
 ------------------------
 
 If you want to make changes to the code or documentation, you should
 first download the repository and install the project in developer mode with
 developer dependencies.
-This way, changes in the code are directly considered without the need of re-installation.
+This way, changes in the code are directly considered without the need for re-installation.
 
 .. code-block:: bash
 
     $ git clone git@github.com/dekuenstle/cblearn.git
     $ cd cblearn
     $ pip install -e.[tests,docs]
```

### Comparing `cblearn-0.1.0/docs/make.bat` & `cblearn-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/docs/references/index.rst` & `cblearn-0.1.1/docs/references/index.rst`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/docs/user_guide/index.rst` & `cblearn-0.1.1/docs/user_guide/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 ==========
 User Guide
 ==========
 
 Most Machine Learning algorithms use numerical training data (features) for inference,
 either representing points in a Euclidean space, similarities, or distances.
 The are settings, e.g. in human studies, when metric points are not available but only ordinal comparisons.
-Comparison-based Learning are Machine Learning algorithms, applicable in this setting.
+Comparison-based learning algorithms are the machine learning algorithms applicable in this setting.
 
 -------------------
 Triplet comparisons
 -------------------
 
 Triplet comparisons are the most common form of ordinal comparisons. For the triplet of objects :math:`(i, j, k)`
-one can ask "Is the object i more similar to the object j or to the object k?".
+one can ask, "Is the object i more similar to the object j or k?".
 For the unknown points :math:`(x_i, x_j, x_k)` and the distance metric :math:`\delta`, the question corresponds to the following
 inequality:
 
 .. math::
 
     \delta(x_i, x_j) \le \delta(x_i, x_k).
 
-This library supports two representation formats of triplets, in an array or in an sparse matrix.
+This library supports two representation formats of triplets in an array or a sparse matrix form.
+The array form uses 2d ``numpy`` arrays representing a triplet per row and columns for ``i,j,k``. 
+Alternatively to the ordering, an additional response array containing 1 or -1 can specify if  ``(i,j,k)`` is correct or wrong.
+The sparse matrix is an alternative representation, where triplets are naturally specified as the matrix indices, containing entries 1 or -1.
 
 
 -------------------------
 Dataset loading utilities
 -------------------------
 
 .. include:: ../../cblearn/datasets/descr/musician_similarity.rst
```

### Comparing `cblearn-0.1.0/examples/ordinal_embedding.py` & `cblearn-0.1.1/examples/ordinal_embedding.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/examples/plot_psychophysical_scales.py` & `cblearn-0.1.1/examples/plot_psychophysical_scales.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/examples/small_embedding_benchmark.py` & `cblearn-0.1.1/examples/small_embedding_benchmark.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/examples/triplet_formats.py` & `cblearn-0.1.1/examples/triplet_formats.py`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/setup.cfg` & `cblearn-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cblearn-0.1.0/versioneer.py` & `cblearn-0.1.1/versioneer.py`

 * *Files identical despite different names*

