# Comparing `tmp/bw_graph_tools-0.2.3.tar.gz` & `tmp/bw_graph_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.2.3.tar", last modified: Mon May 22 20:03:36 2023, max compression
+gzip compressed data, was "bw_graph_tools-0.2.5.tar", last modified: Tue Aug  8 09:18:30 2023, max compression
```

## Comparing `bw_graph_tools-0.2.3.tar` & `bw_graph_tools-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.177734 bw_graph_tools-0.2.3/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-22 20:03:36.177821 bw_graph_tools-0.2.3/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     2290 2023-05-07 12:27:17.000000 bw_graph_tools-0.2.3/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.175410 bw_graph_tools-0.2.3/bw_graph_tools/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-05-22 19:57:10.000000 bw_graph_tools-0.2.3/bw_graph_tools/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      652 2023-05-07 12:32:09.000000 bw_graph_tools-0.2.3/bw_graph_tools/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      123 2023-05-07 12:43:29.000000 bw_graph_tools-0.2.3/bw_graph_tools/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    25891 2023-05-07 12:32:18.000000 bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2074 2023-05-07 12:32:31.000000 bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     8742 2023-05-07 11:32:56.000000 bw_graph_tools-0.2.3/bw_graph_tools/matrix_tools.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1265 2023-05-08 06:15:47.000000 bw_graph_tools-0.2.3/bw_graph_tools/testing.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.2.3/bw_graph_tools/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.176319 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      928 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      183 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-05-22 20:03:36.000000 bw_graph_tools-0.2.3/bw_graph_tools.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.173592 bw_graph_tools-0.2.3/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.2.3/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.3/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-05-22 20:03:36.178212 bw_graph_tools-0.2.3/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.177499 bw_graph_tools-0.2.3/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5819 2023-05-07 12:32:46.000000 bw_graph_tools-0.2.3/tests/test_first_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.2.3/tests/test_get_path_from_matrix.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     1176 2023-05-07 12:33:16.000000 bw_graph_tools-0.2.3/tests/test_matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-05-07 12:33:27.000000 bw_graph_tools-0.2.3/tests/test_second_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-05-07 12:33:33.000000 bw_graph_tools-0.2.3/tests/test_third_heuristic.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-22 20:03:36.175151 bw_graph_tools-0.2.3/tests/traversal/
--rw-r--r--   0 chrismutel   (501) staff       (20)     5256 2023-05-22 19:43:23.000000 bw_graph_tools-0.2.3/tests/traversal/test_marc_vd_meide.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7103 2023-05-08 06:12:24.000000 bw_graph_tools-0.2.3/tests/traversal/test_negative_production.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7095 2023-05-08 06:12:07.000000 bw_graph_tools-0.2.3/tests/traversal/test_nonunitary_production_with_recursion.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4550 2023-05-08 06:11:53.000000 bw_graph_tools-0.2.3/tests/traversal/test_only_one_layer.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7254 2023-05-08 06:11:38.000000 bw_graph_tools-0.2.3/tests/traversal/test_separate_production.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.559263 bw_graph_tools-0.2.5/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.5/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.5/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4460 2023-08-08 09:18:30.559321 bw_graph_tools-0.2.5/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3493 2023-06-08 20:05:32.000000 bw_graph_tools-0.2.5/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.557064 bw_graph_tools-0.2.5/bw_graph_tools/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-08 09:16:27.000000 bw_graph_tools-0.2.5/bw_graph_tools/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      652 2023-05-07 12:32:09.000000 bw_graph_tools-0.2.5/bw_graph_tools/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      123 2023-06-05 09:23:35.000000 bw_graph_tools-0.2.5/bw_graph_tools/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    25895 2023-08-08 09:16:27.000000 bw_graph_tools-0.2.5/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2074 2023-05-07 12:32:31.000000 bw_graph_tools-0.2.5/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8742 2023-05-07 11:32:56.000000 bw_graph_tools-0.2.5/bw_graph_tools/matrix_tools.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1265 2023-05-08 06:15:47.000000 bw_graph_tools-0.2.5/bw_graph_tools/testing.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.2.5/bw_graph_tools/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.557908 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4460 2023-08-08 09:18:30.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      928 2023-08-08 09:18:30.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-08 09:18:30.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      197 2023-08-08 09:18:30.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-08-08 09:18:30.000000 bw_graph_tools-0.2.5/bw_graph_tools.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.555613 bw_graph_tools-0.2.5/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.2.5/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.5/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1726 2023-08-08 09:18:30.559713 bw_graph_tools-0.2.5/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.559026 bw_graph_tools-0.2.5/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5819 2023-05-07 12:32:46.000000 bw_graph_tools-0.2.5/tests/test_first_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.2.5/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1176 2023-05-07 12:33:16.000000 bw_graph_tools-0.2.5/tests/test_matrix_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-05-07 12:33:27.000000 bw_graph_tools-0.2.5/tests/test_second_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-05-07 12:33:33.000000 bw_graph_tools-0.2.5/tests/test_third_heuristic.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-08 09:18:30.556817 bw_graph_tools-0.2.5/tests/traversal/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5256 2023-05-22 19:43:23.000000 bw_graph_tools-0.2.5/tests/traversal/test_marc_vd_meide.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7103 2023-05-08 06:12:24.000000 bw_graph_tools-0.2.5/tests/traversal/test_negative_production.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7095 2023-05-08 06:12:07.000000 bw_graph_tools-0.2.5/tests/traversal/test_nonunitary_production_with_recursion.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4550 2023-05-08 06:11:53.000000 bw_graph_tools-0.2.5/tests/traversal/test_only_one_layer.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7254 2023-05-08 06:11:38.000000 bw_graph_tools-0.2.5/tests/traversal/test_separate_production.py
```

### Comparing `bw_graph_tools-0.2.3/LICENSE` & `bw_graph_tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/PKG-INFO` & `bw_graph_tools-0.2.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: bw_graph_tools
-Version: 0.2.3
-Summary: Graph traversal class and utilities
-Home-page: https://github.com/brightway-lca/bw_graph_tools
-Author: Chris Mutel
-Author-email: <cmutel@gmail.com>
-Maintainer: Chris Mutel
-Maintainer-email: <cmutel@gmail.com>
-License: BSD-3-Clause
-Project-URL: source, https://github.com/brightway-lca/bw_graph_tools
-Project-URL: homepage, https://github.com/brightway-lca/bw_graph_tools
-Project-URL: tracker, https://github.com/brightway-lca/bw_graph_tools/issues
-Keywords: "brightway","development"
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: testing
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # bw_graph_tools
 
 [![PyPI](https://img.shields.io/pypi/v/bw_graph_tools.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw_graph_tools.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw_graph_tools)][pypi status]
 [![License](https://img.shields.io/pypi/l/bw_graph_tools)][license]
 
@@ -52,14 +25,30 @@
 
 ```console
 $ pip install bw_graph_tools
 ```
 
 Packages are also on conda at the [channel cmutel](https://anaconda.org/cmutel/bw_graph_tools).
 
+## Usage
+
+`bw_graph_tools` has three main components: A graph traversal class `NewNodeEachVisitGraphTraversal`; a function to guess production exchanges using only `bw_processing` datapackages `guess_production_exchanges`; and a function to find the path from node `A` to node `B` with the largest amount of the reference product of `A`, `get_path_from_matrix` and it's sister `path_as_brightway_objects`.
+
+### `NewNodeEachVisitGraphTraversal`
+
+Normally we construct matrices and solve the resulting set of linear equations to get a life cycle inventory or impact assessment result. The matrix approach is elegant, in that it simultaneously solves all equations and handles cycles in the graph, and much faster than graph traversal. However, in some cases we want to actually traverse the supply chain graph and calculate the individual impact of visiting nodes at that point in the graph. Graph traversal's use cases include:
+
+* Distinguishing between different paths to the same object
+
+* Convolving temporal distributions
+
+If we add temporal information using `bw_temporalis`, then the same node can occur at different times depending on how the temporal dynamics its preceding path. For example:
+
+
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools/__init__.py` & `bw_graph_tools-0.2.5/bw_graph_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.2.5/bw_graph_tools/graph_traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,25 +453,25 @@
         biosphere_cutoff_score: float,
         cutoff_score: float,
     ) -> None:
         for product_index, product_amount in zip(product_indices, product_amounts):
             producer_index = production_exchange_mapping[product_index]
 
             if producer_index in static_activity_indices:
-                return
+                continue
 
             supply = caching_solver(product_index, product_amount)
             cumulative_score = float((characterized_biosphere * supply).sum())
             reference_product_net_production_amount = matrix[
                 product_index, producer_index
             ]
             scale = product_amount / reference_product_net_production_amount
 
             if abs(cumulative_score) < cutoff_score:
-                return
+                continue
 
             producing_node = Node(
                 unique_id=next(calculation_count),
                 activity_datapackage_id=lca.dicts.activity.reversed[producer_index],
                 activity_index=producer_index,
                 reference_product_datapackage_id=lca.dicts.product.reversed[
                     product_index
```

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.2.5/bw_graph_tools/graph_traversal_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools/matrix_tools.py` & `bw_graph_tools-0.2.5/bw_graph_tools/matrix_tools.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools/testing.py` & `bw_graph_tools-0.2.5/bw_graph_tools/testing.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/bw_graph_tools.egg-info/SOURCES.txt` & `bw_graph_tools-0.2.5/bw_graph_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/docs/conf.py` & `bw_graph_tools-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/setup.cfg` & `bw_graph_tools-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 python_requires = >=3.8
 install_requires = 
 	bw2calc >=2.0.dev13
 	matrix_utils
 	numpy
 	scikit-network ==0.30.0
 	scipy
+	bw_processing
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `bw_graph_tools-0.2.3/tests/test_first_heuristic.py` & `bw_graph_tools-0.2.5/tests/test_first_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.2.5/tests/test_get_path_from_matrix.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/test_matrix_utils.py` & `bw_graph_tools-0.2.5/tests/test_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/test_second_heuristic.py` & `bw_graph_tools-0.2.5/tests/test_second_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/test_third_heuristic.py` & `bw_graph_tools-0.2.5/tests/test_third_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/traversal/test_marc_vd_meide.py` & `bw_graph_tools-0.2.5/tests/traversal/test_marc_vd_meide.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/traversal/test_negative_production.py` & `bw_graph_tools-0.2.5/tests/traversal/test_negative_production.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/traversal/test_nonunitary_production_with_recursion.py` & `bw_graph_tools-0.2.5/tests/traversal/test_nonunitary_production_with_recursion.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/traversal/test_only_one_layer.py` & `bw_graph_tools-0.2.5/tests/traversal/test_only_one_layer.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.2.3/tests/traversal/test_separate_production.py` & `bw_graph_tools-0.2.5/tests/traversal/test_separate_production.py`

 * *Files identical despite different names*

