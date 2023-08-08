# Comparing `tmp/symfem-2023.4.1.tar.gz` & `tmp/symfem-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symfem-2023.4.1.tar", last modified: Wed Apr 26 17:07:49 2023, max compression
+gzip compressed data, was "symfem-2023.8.0.tar", last modified: Tue Aug  8 12:03:56 2023, max compression
```

## Comparing `symfem-2023.4.1.tar` & `symfem-2023.8.0.tar`

### file list

```diff
@@ -1,103 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.263639 symfem-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 17:07:26.000000 symfem-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-26 17:07:49.263639 symfem-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-26 17:07:49.000000 symfem-2023.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 17:07:49.267639 symfem-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-26 17:07:26.000000 symfem-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.243639 symfem-2023.4.1/symfem/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.259639 symfem-2023.4.1/symfem/elements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/_guzman_neilan_tetrahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/_guzman_neilan_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/abf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/argyris.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/aw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bddm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bernardi_raugel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/conforming_crouzeix_raviart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/crouzeix_raviart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/direct_serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/dpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/dual.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/enriched_galerkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/fortin_soulie.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/guzman_neilan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hermite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hhj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/huang_zhang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/kmv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/morley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/morley_wang_xu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/mtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/nedelec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/nedelec_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/p1_iso_p2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rannacher_turek.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/regge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rhct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/tnt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/trimmed_serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/vector_enriched_galerkin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/wu_xu.py
--rw-r--r--   0 runner    (1001) docker     (123)    38368 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/finite_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    57827 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/functionals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55195 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/piecewise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33258 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    42389 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/polynomials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)    77252 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/references.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.243639 symfem-2023.4.1/symfem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.263639 symfem-2023.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_against_basix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_against_computed_by_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_arnold_winther.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_dof_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_guzman_neilan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_nedelec.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_p1_iso_p2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_polynomials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_references.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_stiffness_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_tensor_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.753827 symfem-2023.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-08 12:03:51.000000 symfem-2023.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-08-08 12:03:56.753827 symfem-2023.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-08 12:03:56.000000 symfem-2023.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-08 12:03:56.753827 symfem-2023.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-08 12:03:51.000000 symfem-2023.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.733826 symfem-2023.8.0/symfem/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.745827 symfem-2023.8.0/symfem/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/_guzman_neilan_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/_guzman_neilan_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/abf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/alfeld_sorokina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/argyris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/aw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bernardi_raugel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/bubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/conforming_crouzeix_raviart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/crouzeix_raviart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/direct_serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/dpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/enriched_galerkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/fortin_soulie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/guzman_neilan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/hermite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/hhj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/huang_zhang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/kmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/lagrange_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/lagrange_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/morley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/morley_wang_xu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/mtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/nedelec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/nedelec_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/p1_iso_p2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/p1_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/rannacher_turek.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/regge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/rhct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/tnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/trimmed_serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/vector_enriched_galerkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/elements/wu_xu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40213 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58419 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/functionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55564 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/piecewise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33258 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.745827 symfem-2023.8.0/symfem/polynomials/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/polynomials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/polynomials/dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/polynomials/legendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/polynomials/lobatto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/polynomials/polysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78431 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 12:03:51.000000 symfem-2023.8.0/symfem/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.737827 symfem-2023.8.0/symfem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-08-08 12:03:56.000000 symfem-2023.8.0/symfem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-08 12:03:56.000000 symfem-2023.8.0/symfem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:03:56.000000 symfem-2023.8.0/symfem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 12:03:56.000000 symfem-2023.8.0/symfem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-08 12:03:56.000000 symfem-2023.8.0/symfem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:03:56.753827 symfem-2023.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_against_basix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_against_computed_by_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_alfeld_sorokina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_arnold_winther.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_bell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_dof_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_guzman_neilan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_lagrange_polynomial_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_nedelec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_p1_iso_p2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_stiffness_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/test_tensor_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-08-08 12:03:51.000000 symfem-2023.8.0/test/utils.py
```

### Comparing `symfem-2023.4.1/LICENSE` & `symfem-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/PKG-INFO` & `symfem-2023.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symfem
-Version: 2023.4.1
+Version: 2023.8.0
 Summary: a symbolic finite element definition library
 Home-page: https://github.com/mscroggs/symfem
 Author: Matthew Scroggs
 Author-email: symfem@mscroggs.co.uk
 Maintainer-email: symfem@mscroggs.co.uk
 License: MIT
 Description-Content-Type: text/markdown
@@ -160,25 +160,27 @@
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
 - enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
+- P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
 
 ## Triangle
 The reference triangle has vertices (0, 0), (1, 0), and (0, 1). Its sub-entities are numbered as follows.
 
 ![The numbering of a reference triangle](https://raw.githubusercontent.com/mscroggs/symfem/main/img/triangle_numbering.png)
 
 ### List of supported elements
+- Alfeld-Sorokina (alternative names: AS)
 - Argyris
 - Arnold-Winther (alternative names: AW, conforming Arnold-Winther)
 - Bell
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
@@ -199,14 +201,15 @@
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley
 - Morley-Wang-Xu (alternative names: MWX)
 - Nedelec (alternative names: Nedelec1, N1curl)
 - Nedelec2 (alternative names: N2curl)
 - nonconforming Arnold-Winther (alternative names: nonconforming AW)
+- P1 macro
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Raviart-Thomas (alternative names: RT, N1div)
 - reduced Hsieh-Clough-Tocher (alternative names: rHCT)
 - Regge
 - symmetric matrix Lagrange
 - Taylor (alternative names: discontinuous Taylor)
 - transition
```

### Comparing `symfem-2023.4.1/README.md` & `symfem-2023.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,25 +144,27 @@
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
 - enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
+- P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
 
 ## Triangle
 The reference triangle has vertices (0, 0), (1, 0), and (0, 1). Its sub-entities are numbered as follows.
 
 ![The numbering of a reference triangle](https://raw.githubusercontent.com/mscroggs/symfem/main/img/triangle_numbering.png)
 
 ### List of supported elements
+- Alfeld-Sorokina (alternative names: AS)
 - Argyris
 - Arnold-Winther (alternative names: AW, conforming Arnold-Winther)
 - Bell
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
@@ -183,14 +185,15 @@
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley
 - Morley-Wang-Xu (alternative names: MWX)
 - Nedelec (alternative names: Nedelec1, N1curl)
 - Nedelec2 (alternative names: N2curl)
 - nonconforming Arnold-Winther (alternative names: nonconforming AW)
+- P1 macro
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Raviart-Thomas (alternative names: RT, N1div)
 - reduced Hsieh-Clough-Tocher (alternative names: rHCT)
 - Regge
 - symmetric matrix Lagrange
 - Taylor (alternative names: discontinuous Taylor)
 - transition
```

### Comparing `symfem-2023.4.1/setup.py` & `symfem-2023.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 if __name__ == "__main__":
     setuptools.setup(
         name="symfem",
         description="a symbolic finite element definition library",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        version="2023.4.1",
+        version="2023.8.0",
         author="Matthew Scroggs",
         license="MIT",
         author_email="symfem@mscroggs.co.uk",
         maintainer_email="symfem@mscroggs.co.uk",
         url="https://github.com/mscroggs/symfem",
-        packages=["symfem", "symfem.elements"],
+        packages=["symfem", "symfem.elements", "symfem.polynomials"],
         package_data={"symfem": ["py.typed"]},
         include_package_data=True,
         data_files=data_files,
-        install_requires=["sympy>=1.10"],
+        install_requires=["sympy>=1.10", "appdirs"],
         extras_require={
             "style": ["flake8", "pydocstyle", "mypy", "isort"],
             "docs": ["sphinx", "sphinx-autoapi"],
             "optional": ["CairoSVG>=2.6.0"],
             "test": ["pytest", "symfem[optional]", "numpy"],
         }
     )
```

### Comparing `symfem-2023.4.1/symfem/basis_functions.py` & `symfem-2023.8.0/symfem/basis_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -346,14 +346,19 @@
         """Return a version the function with floats as coefficients.
 
         Returns:
             The function with floats as coefficients
         """
         return self.get_function().with_floats()
 
+    def __iter__(self) -> typing.Iterator[AnyFunction]:
+        """Iterate through components of vector function."""
+        f = self.get_function()
+        return f.__iter__()
+
 
 class SubbedBasisFunction(BasisFunction):
     """A basis function following a substitution."""
 
     def __init__(
         self, f: BasisFunction, vars: AxisVariables, values: ValuesToSubstitute
     ):
@@ -394,8 +399,8 @@
 
         Args:
             reference: The domain to plot the function on
             img: The image to plot the values on
             value_scale: The factor to scale values by
             n: The number of plotting points
         """
-        self.f.plot_values(reference, img, value_scale, n)
+        self.get_function().plot_values(reference, img, value_scale, n)
```

### Comparing `symfem-2023.4.1/symfem/create.py` & `symfem-2023.8.0/symfem/create.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,16 @@
         n_tri = int(cell_type.split("(")[1].split(")")[0])
         return _references.DualPolygon(n_tri, *args)
     else:
         raise ValueError(f"Unknown cell type: {cell_type}")
 
 
 def create_element(
-    cell_type: str, element_type: str, order: int, **kwargs: _typing.Any
+    cell_type: str, element_type: str, order: int,
+    vertices: _typing.Optional[_SetOfPointsInput] = None, **kwargs: _typing.Any
 ) -> _FiniteElement:
     """Make a finite element.
 
     Args:
         cell_type: The reference cell type.
                    Supported values: point, interval, triangle, quadrilateral, tetrahedron,
                    hexahedron, prism, pyramid, dual polygon(number_of_triangles)
@@ -164,18 +165,25 @@
                       TNTdiv, tiniest tensor Hdiv,
                       Arnold-Boffi-Falk, ABF,
                       Arbogast-Correa, AC, AC full, Arbogast-Correa full,
                       Rannacher-Turek,
                       P1-iso-P2, P2-iso-P1, iso-P2 P1,
                       Huang-Zhang, HZ,
                       enriched Galerkin, EG,
-                      enriched vector Galerkin, locking-free enriched Galerkin, LFEG
+                      enriched vector Galerkin, locking-free enriched Galerkin, LFEG,
+                      P1 macro,
+                      Alfeld-Sorokina, AS
         order: The order of the element.
+        vertices: The vertices of the reference.
     """
-    reference = create_reference(cell_type)
+    reference = create_reference(cell_type, vertices=vertices)
+
+    if reference.tdim != reference.gdim:
+        raise ValueError("Cannot create element on cell with different "
+                         "topological and geometric dimensions.")
 
     if element_type in _elementmap:
         if reference.name not in _elementmap[element_type]:
             raise ValueError(f"{element_type} element cannot be created on a {reference.name}.")
         element_class = _elementmap[element_type][reference.name]
         if not _order_is_allowed(element_class, reference.name, order):
             raise ValueError(f"Order {order} {element_type} element cannot be created.")
```

### Comparing `symfem-2023.4.1/symfem/elements/_guzman_neilan_tetrahedron.py` & `symfem-2023.8.0/symfem/elements/_guzman_neilan_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/symfem/elements/_guzman_neilan_triangle.py` & `symfem-2023.8.0/symfem/elements/_guzman_neilan_triangle.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/symfem/elements/abf.py` & `symfem-2023.8.0/symfem/elements/abf.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralMoment, IntegralOfDivergenceAgainst, ListOfFunctionals,
                            NormalIntegralMoment)
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import Lagrange
 from .q import Nedelec
 
 
 class ArnoldBoffiFalk(CiarletElement):
     """An Arnold-Boffi-Falk element."""
@@ -25,14 +25,17 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         assert reference.name == "quadrilateral"
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += [
             (x[0] ** i * x[1] ** j, 0)
             for i in range(order + 3) for j in range(order + 1)]
         poly += [(0, x[0] ** i * x[1] ** j)
                  for i in range(order + 1) for j in range(order + 3)]
 
@@ -40,18 +43,18 @@
             reference,
             edges=(NormalIntegralMoment, Lagrange, order, {"variant": variant}),
             faces=(IntegralMoment, Nedelec, order, {"variant": variant})
         )
 
         for i in range(order + 1):
             dofs.append(IntegralOfDivergenceAgainst(
-                reference, reference, x[0] ** (order + 1) * x[1] ** i,
+                reference, x[0] ** (order + 1) * x[1] ** i,
                 entity=(2, 0), mapping="contravariant"))
             dofs.append(IntegralOfDivergenceAgainst(
-                reference, reference, x[0] ** i * x[1] ** (order + 1),
+                reference, x[0] ** i * x[1] ** (order + 1),
                 entity=(2, 0), mapping="contravariant"))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
@@ -61,7 +64,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Arnold-Boffi-Falk", "ABF"]
     references = ["quadrilateral"]
     min_order = 0
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/ac.py` & `symfem-2023.8.0/symfem/elements/ac.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralAgainst, ListOfFunctionals, NormalIntegralMoment
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import Hdiv_serendipity, polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .dpc import DPC
 
 
 class AC(CiarletElement):
     """Arbogast-Correa Hdiv finite element."""
 
@@ -23,14 +23,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
         if order == 0:
             poly += [(x[0], 0), (0, x[1])]
         else:
             poly += Hdiv_serendipity(reference.tdim, reference.tdim, order)
             poly += [(x[0] ** (i + 1) * x[1] ** (order - i), x[0] ** i * x[1] ** (1 + order - i))
@@ -41,24 +44,24 @@
             facets=(NormalIntegralMoment, DPC, order, {"variant": variant}),
         )
 
         for i in range(order + 1):
             for j in range(order + 1 - i):
                 if i + j > 0:
                     f = (i * x[0] ** (i - 1) * x[1] ** j, j * x[0] ** i * x[1] ** (j - 1))
-                    dofs.append(IntegralAgainst(reference, reference, f, entity=(2, 0),
+                    dofs.append(IntegralAgainst(reference, f, entity=(2, 0),
                                                 mapping="contravariant"))
 
         for i in range(1, order - 1):
             for j in range(1, order - i):
                 f = (
                     x[0] ** i * (1 - x[0]) * x[1] ** (j - 1) * (j * (1 - x[1]) - x[1]),
                     -x[0] ** (i - 1) * (i * (1 - x[0]) - x[0]) * x[1] ** j * (1 - x[1])
                 )
-                dofs.append(IntegralAgainst(reference, reference, f, entity=(2, 0),
+                dofs.append(IntegralAgainst(reference, f, entity=(2, 0),
                                             mapping="contravariant"))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
@@ -68,7 +71,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Arbogast-Correa", "AC", "AC full", "Arbogast-Correa full"]
     references = ["quadrilateral"]
     min_order = 0
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/argyris.py` & `symfem-2023.8.0/symfem/elements/argyris.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,32 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import (ListOfFunctionals, PointComponentSecondDerivativeEvaluation,
                            PointDirectionalDerivativeEvaluation, PointEvaluation,
                            PointNormalDerivativeEvaluation)
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class Argyris(CiarletElement):
     """Argyris finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         assert order == 5
         assert reference.name == "triangle"
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         dofs: ListOfFunctionals = []
         for v_n, vs in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, vs, entity=(0, v_n)))
             for i in range(reference.tdim):
                 direction = tuple(1 if i == j else 0 for j in range(reference.tdim))
                 dofs.append(PointDirectionalDerivativeEvaluation(
                     reference, vs, direction, entity=(0, v_n)))
@@ -49,7 +52,8 @@
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Argyris"]
     references = ["triangle"]
     min_order = 5
     max_order = 5
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/aw.py` & `symfem-2023.8.0/symfem/elements/aw.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import typing
 
 import sympy
 
 from ..finite_element import CiarletElement
 from ..functionals import (InnerProductIntegralMoment, IntegralMoment, ListOfFunctionals,
-                           PointInnerProduct, VecIntegralMoment)
+                           PointInnerProduct)
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_vector
 from ..references import Reference
 from ..symbols import x
 from .lagrange import Lagrange
 
 
@@ -54,36 +54,37 @@
         for e_n in range(reference.sub_entity_count(1)):
             sub_ref = reference.sub_entity(1, e_n)
             sub_e = Lagrange(sub_ref.default_reference(), order - 2, variant)
             for dof_n, dof in enumerate(sub_e.dofs):
                 p = sub_e.get_basis_function(dof_n).get_function()
                 for component in [sub_ref.normal(), sub_ref.tangent()]:
                     InnerProductIntegralMoment(
-                        reference, sub_ref, p, component, sub_ref.normal(), dof,
+                        reference, p, component, sub_ref.normal(), dof,
                         entity=(1, e_n), mapping="double_contravariant")
                     dofs.append(
                         InnerProductIntegralMoment(
-                            reference, sub_ref, p, component, sub_ref.normal(), dof,
+                            reference, p, component, sub_ref.normal(), dof,
                             entity=(1, e_n), mapping="double_contravariant"))
         sub_e = Lagrange(reference, order - 3, variant)
         for dof_n, dof in enumerate(sub_e.dofs):
             p = sub_e.get_basis_function(dof_n).get_function()
             for component22 in [((1, 0), (0, 0)), ((0, 1), (0, 0)), ((0, 0), (0, 1))]:
-                dofs.append(VecIntegralMoment(
-                    reference, reference, p, component22, dof, entity=(2, 0)))
+                dofs.append(IntegralMoment(
+                    reference, tuple(tuple(p * j for j in i) for i in component22),
+                    dof, entity=(2, 0)))
 
         if order >= 4:
             sub_e = Lagrange(reference, order - 4, variant)
             for p, dof in zip(sub_e.get_basis_functions(), sub_e.dofs):
                 if sympy.Poly(p.as_sympy(), x[:2]).degree() != order - 4:
                     continue
                 f = p * x[0] ** 2 * x[1] ** 2 * (1 - x[0] - x[1]) ** 2
                 J = tuple(tuple(f.diff(x[i]).diff(x[j]) for j in range(2))
                           for i in range(2))
-                dofs.append(IntegralMoment(reference, reference, J, dof, entity=(2, 0)))
+                dofs.append(IntegralMoment(reference, J, dof, entity=(2, 0)))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim ** 2,
                          (reference.tdim, reference.tdim))
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
@@ -92,14 +93,15 @@
         """
         return {"variant": self.variant}
 
     names = ["Arnold-Winther", "AW", "conforming Arnold-Winther"]
     references = ["triangle"]
     min_order = 3
     continuity = "integral inner H(div)"
+    last_updated = "2023.05"
 
 
 class NonConformingArnoldWinther(CiarletElement):
     """A nonconforming Arnold-Winther element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -130,22 +132,23 @@
             sub_ref = reference.sub_entity(1, e_n)
             sub_e = Lagrange(sub_ref.default_reference(), 1, variant)
             for dof_n, dof in enumerate(sub_e.dofs):
                 p = sub_e.get_basis_function(dof_n).get_function()
                 for component in [sub_ref.normal(), sub_ref.tangent()]:
                     dofs.append(
                         InnerProductIntegralMoment(
-                            reference, sub_ref, p, component, sub_ref.normal(), dof,
+                            reference, p, component, sub_ref.normal(), dof,
                             entity=(1, e_n), mapping="double_contravariant"))
         sub_e = Lagrange(reference, 0, variant)
         for dof_n, dof in enumerate(sub_e.dofs):
             p = sub_e.get_basis_function(dof_n).get_function()
             for component22 in [((1, 0), (0, 0)), ((0, 1), (0, 0)), ((0, 0), (0, 1))]:
-                dofs.append(VecIntegralMoment(
-                    reference, reference, p, component22, dof, entity=(2, 0)))
+                dofs.append(IntegralMoment(
+                    reference, tuple(tuple(p * j for j in i) for i in component22),
+                    dof, entity=(2, 0)))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim ** 2,
                          (reference.tdim, reference.tdim))
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
@@ -155,7 +158,8 @@
         return {"variant": self.variant}
 
     names = ["nonconforming Arnold-Winther", "nonconforming AW"]
     references = ["triangle"]
     min_order = 2
     max_order = 2
     continuity = "integral inner H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/bddm.py` & `symfem-2023.8.0/symfem/elements/bddm.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralMoment, ListOfFunctionals, NormalIntegralMoment
 from ..functions import FunctionInput, VectorFunction
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .dpc import DPC, VectorDPC
 
 
 def bddf_polyset(reference: Reference, order: int) -> typing.List[FunctionInput]:
     """Create the polynomial basis for a BDDF element.
 
     Args:
         reference: The reference cell
         order: The polynomial order
 
     Returns:
         The polynomial basis
     """
-    dim = reference.tdim
     assert reference.name == "hexahedron"
+
+    dim = reference.tdim
     pset: typing.List[FunctionInput] = []
     pset += polynomial_set_vector(dim, dim, order)
     pset.append(VectorFunction((0, 0, x[0] ** (order + 1) * x[1])).curl())
     pset.append(VectorFunction((0, x[0] * x[2] ** (order + 1), 0)).curl())
     pset.append(VectorFunction((x[1] ** (order + 1) * x[2], 0, 0)).curl())
     for i in range(1, order + 1):
         pset.append(VectorFunction((0, 0, x[0] * x[1] ** (i + 1) * x[2] ** (order - i))).curl())
@@ -48,14 +49,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly = bddf_polyset(reference, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             facets=(NormalIntegralMoment, DPC, order, {"variant": variant}),
             cells=(IntegralMoment, VectorDPC, order - 2, {"variant": variant})
         )
@@ -72,7 +76,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Brezzi-Douglas-Duran-Fortin", "BDDF"]
     references = ["hexahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/bdfm.py` & `symfem-2023.8.0/symfem/elements/bdfm.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralMoment, ListOfFunctionals, NormalIntegralMoment
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .dpc import DPC, VectorDPC
 from .lagrange import Lagrange, VectorLagrange
 
 
 def bdfm_polyset(reference: Reference, order: int) -> typing.List[FunctionInput]:
     """Create the polynomial basis for a BDFM element.
@@ -61,14 +61,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly = bdfm_polyset(reference, order)
 
         dofs: ListOfFunctionals = []
         if reference.name in ["triangle", "tetrahedron"]:
             dofs = make_integral_moment_dofs(
                 reference,
                 facets=(NormalIntegralMoment, Lagrange, order - 1, {"variant": variant}),
@@ -92,7 +95,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Brezzi-Douglas-Fortin-Marini", "BDFM"]
     references = ["triangle", "quadrilateral", "hexahedron", "tetrahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/bdm.py` & `symfem-2023.8.0/symfem/elements/bdm.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralMoment, ListOfFunctionals, NormalIntegralMoment
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from .lagrange import Lagrange
 from .nedelec import NedelecFirstKind
 
 
 class BDM(CiarletElement):
     """Brezzi-Douglas-Marini Hdiv finite element."""
 
@@ -23,14 +23,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             facets=(NormalIntegralMoment, Lagrange, order, {"variant": variant}),
             cells=(IntegralMoment, NedelecFirstKind, order - 1, {"variant": variant}),
@@ -47,7 +50,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Brezzi-Douglas-Marini", "BDM", "N2div"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/bell.py` & `symfem-2023.8.0/symfem/elements/bell.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 This element's definition is given in https://doi.org/10.1002/nme.1620010108 (Bell, 1969)
 """
 
 import typing
 
 from ..finite_element import CiarletElement
-from ..functionals import (DerivativePointEvaluation, ListOfFunctionals,
-                           NormalDerivativeIntegralMoment, PointEvaluation)
+from ..functionals import DerivativePointEvaluation, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_1d
 from ..references import Reference
-from .lagrange import Lagrange
+from ..symbols import x
 
 
 class Bell(CiarletElement):
     """Bell finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -32,22 +30,21 @@
         for v_n, v in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             dofs.append(DerivativePointEvaluation(reference, v, (1, 0), entity=(0, v_n)))
             dofs.append(DerivativePointEvaluation(reference, v, (0, 1), entity=(0, v_n)))
             dofs.append(DerivativePointEvaluation(reference, v, (2, 0), entity=(0, v_n)))
             dofs.append(DerivativePointEvaluation(reference, v, (1, 1), entity=(0, v_n)))
             dofs.append(DerivativePointEvaluation(reference, v, (0, 2), entity=(0, v_n)))
-        dofs += make_integral_moment_dofs(
-            reference,
-            edges=(NormalDerivativeIntegralMoment, Lagrange, 0, {"variant": variant}),
-        )
         self.variant = variant
 
         poly: typing.List[FunctionInput] = []
-        poly += polynomial_set_1d(reference.tdim, order)
+        poly += polynomial_set_1d(reference.tdim, 4)
+        poly.append(x[0]**5 - x[1]**5)
+        poly.append(x[0]**3*x[1]**2 - x[0]**2*x[1]**3)
+        poly.append(5*x[0]**2*x[1]**3 - x[0]**5)
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
         Returns:
@@ -56,7 +53,8 @@
         return {"variant": self.variant}
 
     names = ["Bell"]
     references = ["triangle"]
     min_order = 5
     max_order = 5
     continuity = "C1"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/bernardi_raugel.py` & `symfem-2023.8.0/symfem/elements/bernardi_raugel.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import (DivergenceIntegralMoment, DotPointEvaluation, ListOfFunctionals,
                            NormalIntegralMoment)
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import Lagrange
 
 
 class BernardiRaugel(CiarletElement):
     """Bernardi-Raugel Hdiv finite element."""
 
@@ -26,14 +26,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
 
         p = Lagrange(reference, 1, variant="equispaced")
 
         for i in range(reference.sub_entity_count(reference.tdim - 1)):
             sub_e = reference.sub_entity(reference.tdim - 1, i)
@@ -82,18 +85,19 @@
                     dofs.append(DotPointEvaluation(
                         reference, midpoint, normal, entity=(2, f_n), mapping="contravariant"))
 
             p = Lagrange(reference, 0, variant="equispaced")
 
             for i in range(3):
                 dofs.append(DivergenceIntegralMoment(
-                    reference, reference, x[i], p.dofs[0], entity=(3, 0),
+                    reference, x[i], p.dofs[0], entity=(3, 0),
                     mapping="contravariant"
                 ))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
 
     names = ["Bernardi-Raugel"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     max_order = {"triangle": 1, "tetrahedron": 2}
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/bernstein.py` & `symfem-2023.8.0/symfem/elements/bernstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,7 +218,8 @@
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Bernstein", "Bernstein-Bezier"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/bfs.py` & `symfem-2023.8.0/symfem/elements/bfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,10 @@
         poly += quolynomial_set_1d(reference.tdim, order)
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Bogner-Fox-Schmit", "BFS"]
     references = ["quadrilateral"]
     min_order = 3
     max_order = 3
-    continuity = "C1"
+    continuity = "C0"
+    # continuity = "C1"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/bubble.py` & `symfem-2023.8.0/symfem/elements/bubble.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
 from ..functionals import DotPointEvaluation, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..polynomials import polynomial_set_1d, quolynomial_set_1d
 from ..references import Reference
 from .lagrange import Lagrange
 
 
 class Bubble(CiarletElement):
     """Bubble finite element."""
 
@@ -25,43 +24,42 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         from .. import create_element
-        p1 = create_element(reference.name, "Lagrange", 1)
+
+        p1 = create_element(reference.name, "Lagrange", 1, vertices=reference.vertices)
         bubble = 1
         for f in p1.get_basis_functions():
             bubble *= f
 
-        poly: typing.List[FunctionInput] = []
-
-        # TODO: variants
-        if reference.name == "interval":
-            poly += [bubble * p for p in polynomial_set_1d(reference.tdim, order - 2)]
+        if reference.name in ["interval", "quadrilateral", "hexahedron"]:
+            o = order - 2
         elif reference.name == "triangle":
-            poly += [bubble * p for p in polynomial_set_1d(reference.tdim, order - 3)]
+            o = order - 3
         elif reference.name == "tetrahedron":
-            poly += [bubble * p for p in polynomial_set_1d(reference.tdim, order - 4)]
-        elif reference.name == "quadrilateral":
-            poly += [bubble * p for p in quolynomial_set_1d(reference.tdim, order - 2)]
-        elif reference.name == "hexahedron":
-            poly += [bubble * p for p in quolynomial_set_1d(reference.tdim, order - 2)]
+            o = order - 4
         else:
             raise ValueError(f"Unsupported reference: {reference.name}")
 
+        pn = create_element(reference.name, "Lagrange", o, vertices=reference.vertices,
+                            variant=variant)
+
+        poly = [bubble * p for p in pn.get_basis_functions()]
+
         dofs: ListOfFunctionals = []
         if reference.name in ["interval", "triangle", "tetrahedron"]:
             def func(i): return sum(i)
         else:
             def func(i): return max(i)
         for i in product(range(1, order), repeat=reference.tdim):
             if func(i) < order:
-                point = tuple(sympy.Rational(j, order) for j in i)
+                point = reference.get_point(tuple(sympy.Rational(j, order) for j in i))
                 dofs.append(PointEvaluation(reference, point, entity=(reference.tdim, 0)))
 
         self.variant = variant
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, 1
         )
@@ -75,14 +73,15 @@
         return {"variant": self.variant}
 
     names = ["bubble"]
     references = ["interval", "triangle", "tetrahedron", "quadrilateral", "hexahedron"]
     min_order = {"interval": 2, "triangle": 3, "tetrahedron": 4,
                  "quadrilateral": 2, "hexahedron": 2}
     continuity = "C0"
+    last_updated = "2023.06.1"
 
 
 class BubbleEnrichedLagrange(CiarletElement):
     """Bubble enriched Lagrange element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -115,14 +114,15 @@
         """
         return {"variant": self.variant}
 
     names = ["bubble enriched Lagrange"]
     references = ["triangle"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.06"
 
 
 class BubbleEnrichedVectorLagrange(CiarletElement):
     """Bubble enriched Lagrange element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -157,7 +157,8 @@
         """
         return {"variant": self.variant}
 
     names = ["bubble enriched vector Lagrange"]
     references = ["triangle"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/conforming_crouzeix_raviart.py` & `symfem-2023.8.0/symfem/elements/conforming_crouzeix_raviart.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 import sympy
 
 from ..finite_element import CiarletElement
 from ..functionals import ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 
 
 class ConformingCrouzeixRaviart(CiarletElement):
     """Conforming Crouzeix-Raviart finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         if reference.vertices != reference.reference_vertices:
-            raise NotImplementedError()
+            raise NonDefaultReferenceError()
         assert reference.name == "triangle"
 
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
 
         poly += [
             x[0] ** i * x[1] ** (order - i) * (x[0] + x[1])
@@ -57,7 +57,8 @@
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["conforming Crouzeix-Raviart", "conforming CR"]
     references = ["triangle"]
     min_order = 1
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/crouzeix_raviart.py` & `symfem-2023.8.0/symfem/elements/crouzeix_raviart.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,7 +73,8 @@
         return {"variant": self.variant}
 
     names = ["Crouzeix-Raviart", "CR", "Crouzeix-Falk", "CF"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     max_order = {"tetrahedron": 1}
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/direct_serendipity.py` & `symfem-2023.8.0/symfem/elements/direct_serendipity.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,7 +76,8 @@
         super().__init__(reference, order, basis_functions, basis_entities,
                          reference.tdim, 1)
 
     names = ["direct serendipity"]
     references = ["quadrilateral"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/dpc.py` & `symfem-2023.8.0/symfem/elements/dpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,48 +2,58 @@
 
 import typing
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
-from ..functionals import DotPointEvaluation, ListOfFunctionals, PointEvaluation
+from ..functionals import DotPointEvaluation, IntegralAgainst, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d, polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from .lagrange import Lagrange
 
 
 class DPC(CiarletElement):
     """A dPc element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        dofs: ListOfFunctionals = []
         if reference.name == "interval":
-            points = [d.dof_point() for d in Lagrange(reference, order, variant).dofs]
-        elif order == 0:
-            points = [tuple(sympy.Rational(1, 2) for _ in range(reference.tdim))]
+            for d in Lagrange(reference, order, variant).dofs:
+                if isinstance(d, PointEvaluation):
+                    dofs.append(PointEvaluation(reference, d.point, entity=(reference.tdim, 0)))
+                elif isinstance(d, IntegralAgainst):
+                    dofs.append(IntegralAgainst(
+                        reference, d.f * reference.jacobian(), entity=(reference.tdim, 0)))
         else:
-            points = [
-                tuple(sympy.Rational(j, order) for j in i[::-1])
-                for i in product(range(order + 1), repeat=reference.tdim)
-                if sum(i) <= order
-            ]
+            if order == 0:
+                points = [reference.get_point(tuple(
+                    sympy.Rational(1, 2) for _ in range(reference.tdim)))]
+            else:
+                points = [
+                    reference.get_point(tuple(sympy.Rational(j, order) for j in i[::-1]))
+                    for i in product(range(order + 1), repeat=reference.tdim)
+                    if sum(i) <= order
+                ]
 
-        dofs: ListOfFunctionals = [
-            PointEvaluation(reference, d, entity=(reference.tdim, 0)) for d in points]
+            dofs = [
+                PointEvaluation(reference, d, entity=(reference.tdim, 0)) for d in points]
 
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
+        poly = reference.map_polyset_from_default(poly)
+
         super().__init__(
             reference, order, poly, dofs, reference.tdim, 1
         )
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
@@ -53,27 +63,31 @@
         """
         return {"variant": self.variant}
 
     names = ["dPc"]
     references = ["interval", "quadrilateral", "hexahedron"]
     min_order = 0
     continuity = "L2"
+    last_updated = "2023.07.1"
 
 
 class VectorDPC(CiarletElement):
     """Vector dPc finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         scalar_space = DPC(reference, order, variant)
         dofs: ListOfFunctionals = []
         if reference.tdim == 1:
             directions: typing.List[typing.Tuple[int, ...]] = [(1, )]
         else:
             directions = [
                 tuple(1 if i == j else 0 for j in range(reference.tdim))
@@ -97,7 +111,8 @@
         """
         return {"variant": self.variant}
 
     names = ["vector dPc"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 0
     continuity = "L2"
+    last_updated = "2023.07"
```

### Comparing `symfem-2023.4.1/symfem/elements/dual.py` & `symfem-2023.8.0/symfem/elements/dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sympy
 
 from ..finite_element import FiniteElement
 from ..functions import AnyFunction, FunctionInput, VectorFunction
 from ..geometry import PointType, SetOfPoints, SetOfPointsInput
 from ..piecewise_functions import PiecewiseFunction
-from ..references import DualPolygon
+from ..references import DualPolygon, NonDefaultReferenceError
 
 
 class DualCiarletElement(FiniteElement):
     """Abstract barycentric finite element."""
 
     def __init__(
         self, dual_coefficients: typing.List[typing.List[typing.List[
@@ -37,14 +37,17 @@
             order: The polynomia order of the fine space
             dof_entities: The cell entity that each basis function is associated with
             domain_dim: the topological dimension of the domain
             range_dim: the dimension of the range
             range_shape: the shape of the range
             dof_directions: The direction that each basis function is associated with
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         self.dual_coefficients = dual_coefficients
         self.fine_space = fine_space
         super().__init__(reference, order, len(dual_coefficients), domain_dim, range_dim,
                          range_shape=range_shape)
         self._basis_functions: typing.Union[typing.List[AnyFunction], None] = None
         self._dof_entities = dof_entities
         self._dof_directions = dof_directions
@@ -233,14 +236,15 @@
         )
 
     names = ["dual polynomial", "dual P", "dual"]
     references = ["dual polygon"]
     min_order = 0
     max_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
 
 
 class BuffaChristiansen(DualCiarletElement):
     """Buffa-Christiansen barycentric dual finite element."""
 
     def __init__(self, reference: DualPolygon, order: int):
         """Create the element.
@@ -276,14 +280,15 @@
             dof_directions=tuple(dof_directions))
 
     names = ["Buffa-Christiansen", "BC"]
     references = ["dual polygon"]
     min_order = 1
     max_order = 1
     continuity = "H(div)"
+    last_updated = "2023.05"
 
 
 class RotatedBuffaChristiansen(DualCiarletElement):
     """RotatedBuffa-Christiansen barycentric dual finite element."""
 
     def __init__(self, reference: DualPolygon, order: int):
         """Create the element.
@@ -319,7 +324,8 @@
             reference.tdim, 2, dof_directions=tuple(dof_directions))
 
     names = ["rotated Buffa-Christiansen", "RBC"]
     references = ["dual polygon"]
     min_order = 1
     max_order = 1
     continuity = "H(div)"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/enriched_galerkin.py` & `symfem-2023.8.0/symfem/elements/enriched_galerkin.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,7 +25,8 @@
         else:
             super().__init__([Lagrange(reference, order), Lagrange(reference, 0)])
 
     names = ["enriched Galerkin", "EG"]
     references = ["interval", "triangle", "quadrilateral", "tetrahedron", "hexahedron"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/fortin_soulie.py` & `symfem-2023.8.0/symfem/elements/fortin_soulie.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 
 import sympy
 
 from ..finite_element import CiarletElement
 from ..functionals import ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class FortinSoulie(CiarletElement):
     """Fortin-Soulie finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         assert reference.name == "triangle"
-
         assert order == 2
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
 
         third = sympy.Rational(1, 3)
         two_thirds = sympy.Rational(2, 3)
         dofs: ListOfFunctionals = [
             PointEvaluation(reference, (two_thirds, third), entity=(1, 0)),
             PointEvaluation(reference, (third, two_thirds), entity=(1, 0)),
             PointEvaluation(reference, (0, third), entity=(1, 1)),
@@ -45,7 +46,8 @@
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Fortin-Soulie", "FS"]
     references = ["triangle"]
     min_order = 2
     max_order = 2
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/guzman_neilan.py` & `symfem-2023.8.0/symfem/elements/guzman_neilan.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,32 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import DotPointEvaluation, ListOfFunctionals, NormalIntegralMoment
 from ..functions import FunctionInput, VectorFunction
 from ..geometry import SetOfPoints, SetOfPointsInput
 from ..moments import make_integral_moment_dofs
 from ..piecewise_functions import PiecewiseFunction
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from .bernardi_raugel import BernardiRaugel
 from .lagrange import Lagrange, VectorLagrange
 
 
 class GuzmanNeilan(CiarletElement):
     """Guzman-Neilan Hdiv finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         if reference.name == "triangle":
             poly = self._make_polyset_triangle(reference, order)
         else:
             poly = self._make_polyset_tetrahedron(reference, order)
 
         dofs: ListOfFunctionals = []
 
@@ -173,14 +176,15 @@
         return basis
 
     names = ["Guzman-Neilan"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     max_order = {"triangle": 1, "tetrahedron": 2}
     continuity = "H(div)"
+    last_updated = "2023.06"
 
 
 def make_piecewise_lagrange(
     sub_cells: typing.List[SetOfPoints], cell_name, order: int, zero_on_boundary: bool = False,
     zero_at_centre: bool = False
 ) -> typing.List[PiecewiseFunction]:
     """Make the basis functions of a piecewise Lagrange space.
```

### Comparing `symfem-2023.4.1/symfem/elements/hermite.py` & `symfem-2023.8.0/symfem/elements/hermite.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Hermite"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 3
     max_order = 3
-    continuity = "C1"
+    continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/hhj.py` & `symfem-2023.8.0/symfem/elements/hhj.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralMoment, ListOfFunctionals, NormalInnerProductIntegralMoment
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from .lagrange import Lagrange, SymmetricMatrixLagrange
 
 
 class HellanHerrmannJohnson(CiarletElement):
     """A Hellan-Herrmann-Johnson element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
@@ -23,15 +23,15 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         if reference.vertices != reference.reference_vertices:
-            raise NotImplementedError()
+            raise NonDefaultReferenceError()
         assert reference.name == "triangle"
 
         poly: typing.List[FunctionInput] = []
         poly += [((p[0], p[1]), (p[1], p[2]))
                  for p in polynomial_set_vector(reference.tdim, 3, order)]
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
@@ -55,7 +55,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Hellan-Herrmann-Johnson", "HHJ"]
     references = ["triangle"]
     min_order = 0
     continuity = "inner H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/huang_zhang.py` & `symfem-2023.8.0/symfem/elements/huang_zhang.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralAgainst, ListOfFunctionals, NormalIntegralMoment,
                            TangentIntegralMoment)
 from ..functions import FunctionInput, VectorFunction
 from ..moments import make_integral_moment_dofs
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import Lagrange
 
 
 class HuangZhang(CiarletElement):
     """Huang-Zhang finite element."""
 
@@ -24,14 +24,17 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         assert reference.name == "quadrilateral"
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         self.variant = variant
 
         dofs: ListOfFunctionals = []
         poly: typing.List[FunctionInput] = []
         poly += [
             VectorFunction([x[0] ** i * x[1] ** j, 0])
             for i in range(order + 1)
@@ -53,17 +56,17 @@
             facets=(TangentIntegralMoment, Lagrange, order - 2,
                     {"variant": variant}),
         )
 
         for i in range(order - 1):
             for j in range(order - 2):
                 dofs.append(IntegralAgainst(
-                    reference, reference, (x[0] ** i * x[1] ** j, 0), (2, 0)))
+                    reference, (x[0] ** i * x[1] ** j, 0), (2, 0)))
                 dofs.append(IntegralAgainst(
-                    reference, reference, (0, x[0] ** j * x[1] ** i), (2, 0)))
+                    reference, (0, x[0] ** j * x[1] ** i), (2, 0)))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
         Returns:
@@ -71,7 +74,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Huang-Zhang", "HZ"]
     references = ["quadrilateral"]
     min_order = 2
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/kmv.py` & `symfem-2023.8.0/symfem/elements/kmv.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sympy
 
 from ..finite_element import CiarletElement
 from ..functionals import ListOfFunctionals, WeightedPointEvaluation
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 
 
 def kmv_tri_polyset(m: int, mf: int) -> typing.List[FunctionInput]:
     """Create the polynomial set for a KMV space on a triangle.
 
     Args:
@@ -71,14 +71,17 @@
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         dofs: ListOfFunctionals = []
         if reference.name == "triangle":
             if order == 1:
                 for v_n, v in enumerate(reference.vertices):
                     dofs.append(WeightedPointEvaluation(
                         reference, v, sympy.Rational(1, 6), entity=(0, v_n)))
                 poly = kmv_tri_polyset(1, 1)
@@ -164,7 +167,8 @@
             reference, order, poly, dofs, reference.tdim, 1
         )
 
     names = ["Kong-Mulder-Veldhuizen", "KMV"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/lagrange.py` & `symfem-2023.8.0/symfem/elements/lagrange.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 import typing
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
-from ..functionals import DotPointEvaluation, ListOfFunctionals, PointEvaluation
+from ..functionals import DotPointEvaluation, IntegralAgainst, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..polynomials import polynomial_set_1d, polynomial_set_vector
+from ..polynomials import (lobatto_dual_basis, orthonormal_basis, polynomial_set_1d,
+                           polynomial_set_vector)
 from ..quadrature import get_quadrature
 from ..references import Reference
 
 
 class Lagrange(CiarletElement):
     """Lagrange finite element."""
 
@@ -21,36 +22,50 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         dofs: ListOfFunctionals = []
-        if order == 0:
-            dofs = [
+        if variant == "legendre":
+            basis = orthonormal_basis(reference.name, order, 0)[0]
+            for f in basis:
+                dofs.append(IntegralAgainst(reference, f, (reference.tdim, 0)))
+        elif order == 0:
+            dofs.append(
                 PointEvaluation(
-                    reference, tuple(
+                    reference, reference.get_point(tuple(
                         sympy.Rational(1, reference.tdim + 1)
                         for i in range(reference.tdim)
-                    ),
+                    )),
                     entity=(reference.tdim, 0)
                 )
-            ]
+            )
+        elif variant == "lobatto":
+            for v_n, v in enumerate(reference.vertices):
+                dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
+            for edim in range(1, 4):
+                for e_n in range(reference.sub_entity_count(edim)):
+                    entity = reference.sub_entity(edim, e_n)
+                    basis = lobatto_dual_basis(entity.name, order, False)
+                    for f in basis:
+                        dofs.append(IntegralAgainst(reference, f, (edim, e_n)))
         else:
             points, _ = get_quadrature(variant, order + 1)
 
-            for v_n, v in enumerate(reference.reference_vertices):
+            for v_n, v in enumerate(reference.vertices):
                 dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             for edim in range(1, 4):
                 for e_n in range(reference.sub_entity_count(edim)):
                     entity = reference.sub_entity(edim, e_n)
                     for i in product(range(1, order), repeat=edim):
                         if sum(i) < order:
                             point = entity.get_point([sympy.Rational(j, order) for j in i[::-1]])
-                            dofs.append(PointEvaluation(reference, point, entity=(edim, e_n)))
+                            dofs.append(PointEvaluation(reference, point,
+                                                        entity=(edim, e_n)))
 
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
@@ -61,14 +76,15 @@
         """
         return {"variant": self.variant}
 
     names = ["Lagrange", "P"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.07"
 
 
 class VectorLagrange(CiarletElement):
     """Vector Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -79,27 +95,37 @@
             variant: The variant of the element
         """
         scalar_space = Lagrange(reference, order, variant)
         dofs: ListOfFunctionals = []
         poly: typing.List[FunctionInput] = []
         if reference.tdim == 1:
             for p in scalar_space.dofs:
-                dofs.append(PointEvaluation(reference, p.dof_point(), entity=p.entity))
+                if isinstance(p, PointEvaluation):
+                    dofs.append(PointEvaluation(reference, p.dof_point(), entity=p.entity))
+                elif isinstance(p, IntegralAgainst):
+                    dofs.append(IntegralAgainst(
+                        reference, p.f * reference.jacobian(), entity=p.entity))
 
             poly += polynomial_set_1d(reference.tdim, order)
         else:
             directions = [
                 tuple(1 if i == j else 0 for j in range(reference.tdim))
                 for i in range(reference.tdim)
             ]
             for p in scalar_space.dofs:
                 for d in directions:
-                    dofs.append(DotPointEvaluation(reference, p.dof_point(), d, entity=p.entity))
+                    if isinstance(p, PointEvaluation):
+                        dofs.append(DotPointEvaluation(
+                            reference, p.dof_point(), d, entity=p.entity))
+                    elif isinstance(p, IntegralAgainst):
+                        dofs.append(IntegralAgainst(
+                            reference, tuple(p.f * i for i in d), entity=p.entity))
 
             poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
+
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
         Returns:
@@ -107,14 +133,15 @@
         """
         return {"variant": self.variant}
 
     names = ["vector Lagrange", "vP"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.07.1"
 
 
 class MatrixLagrange(CiarletElement):
     """Matrix Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -152,14 +179,15 @@
         """
         return {"variant": self.variant}
 
     names = ["matrix Lagrange"]
     references = ["triangle", "tetrahedron"]
     min_order = 0
     continuity = "L2"
+    last_updated = "2023.07"
 
 
 class SymmetricMatrixLagrange(CiarletElement):
     """Symmetric matrix Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -216,7 +244,8 @@
         """
         return {"variant": self.variant}
 
     names = ["symmetric matrix Lagrange"]
     references = ["triangle", "tetrahedron"]
     min_order = 0
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/lagrange_prism.py` & `symfem-2023.8.0/symfem/elements/lagrange_prism.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,43 +2,52 @@
 
 import typing
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
-from ..functionals import DotPointEvaluation, ListOfFunctionals, PointEvaluation
+from ..functionals import DotPointEvaluation, IntegralAgainst, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..polynomials import prism_polynomial_set_1d, prism_polynomial_set_vector
+from ..polynomials import orthonormal_basis, prism_polynomial_set_1d, prism_polynomial_set_vector
 from ..quadrature import get_quadrature
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class Lagrange(CiarletElement):
     """Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         dofs: ListOfFunctionals = []
-        if order == 0:
+        if variant == "legendre":
+            basis = orthonormal_basis(reference.name, order, 0)[0]
+            for f in basis:
+                dofs.append(IntegralAgainst(reference, f, (reference.tdim, 0)))
+        elif order == 0:
             dofs = [
                 PointEvaluation(
                     reference, tuple(
                         sympy.Rational(1, reference.tdim + 1)
                         for i in range(reference.tdim)
                     ),
                     entity=(reference.tdim, 0)
                 )
             ]
+        elif variant == "lobatto":
+            raise NotImplementedError()
         else:
             points, _ = get_quadrature(variant, order + 1)
 
             # Vertices
             for v_n, v in enumerate(reference.vertices):
                 dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             # Edges
@@ -84,14 +93,15 @@
         """
         return {"variant": self.variant}
 
     names = ["Lagrange", "P"]
     references = ["prism"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.07"
 
 
 class VectorLagrange(CiarletElement):
     """Vector Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -131,7 +141,8 @@
         """
         return {"variant": self.variant}
 
     names: typing.List[str] = []
     references = ["prism"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/lagrange_pyramid.py` & `symfem-2023.8.0/symfem/elements/lagrange_pyramid.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,52 @@
 
 import typing
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
-from ..functionals import ListOfFunctionals, PointEvaluation
+from ..functionals import IntegralAgainst, ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..polynomials import pyramid_polynomial_set_1d
+from ..polynomials import orthonormal_basis, pyramid_polynomial_set_1d
 from ..quadrature import get_quadrature
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class Lagrange(CiarletElement):
     """Lagrange finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         dofs: ListOfFunctionals = []
-        if order == 0:
+        if variant == "legendre":
+            basis = orthonormal_basis(reference.name, order, 0)[0]
+            for f in basis:
+                dofs.append(IntegralAgainst(reference, f, (reference.tdim, 0)))
+        elif order == 0:
             dofs = [
                 PointEvaluation(
                     reference, tuple(
                         sympy.Rational(1, reference.tdim + 1)
                         for i in range(reference.tdim)
                     ),
                     entity=(reference.tdim, 0)
                 )
             ]
+        elif variant == "lobatto":
+            raise NotImplementedError()
         else:
             points, _ = get_quadrature(variant, order + 1)
 
             # Vertices
             for v_n, v in enumerate(reference.vertices):
                 dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             # Edges
@@ -90,7 +99,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Lagrange", "P"]
     references = ["pyramid"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.07"
```

### Comparing `symfem-2023.4.1/symfem/elements/morley.py` & `symfem-2023.8.0/symfem/elements/morley.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import ListOfFunctionals, PointEvaluation, PointNormalDerivativeEvaluation
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class Morley(CiarletElement):
     """Morley finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         if reference.vertices != reference.reference_vertices:
-            raise NotImplementedError()
+            raise NonDefaultReferenceError()
         assert order == 2
         assert reference.name == "triangle"
         dofs: ListOfFunctionals = []
         for v_n, vs in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, vs, entity=(0, v_n)))
         for e_n in range(reference.sub_entity_count(1)):
             sub_ref = reference.sub_entity(1, e_n)
@@ -42,7 +42,8 @@
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Morley"]
     references = ["triangle"]
     min_order = 2
     max_order = 2
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/morley_wang_xu.py` & `symfem-2023.8.0/symfem/elements/morley_wang_xu.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,58 +7,61 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralAgainst, IntegralOfDirectionalMultiderivative, ListOfFunctionals,
                            PointEvaluation)
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class MorleyWangXu(CiarletElement):
     """Morley-Wang-Xu finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         assert order <= reference.tdim
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
 
         dofs: ListOfFunctionals = []
 
         if order == 1:
             if reference.tdim == 1:
                 for v_n, v in enumerate(reference.vertices):
                     dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             else:
                 dim = reference.tdim - 1
                 for facet_n in range(reference.sub_entity_count(dim)):
                     facet = reference.sub_entity(dim, facet_n)
-                    dofs.append(IntegralAgainst(reference, facet, 1 / facet.jacobian(),
+                    dofs.append(IntegralAgainst(reference, 1 / facet.jacobian(),
                                                 entity=(dim, facet_n)))
         elif order == 2:
             if reference.tdim == 2:
                 for v_n, v in enumerate(reference.vertices):
                     dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             else:
                 dim = reference.tdim - 2
                 for ridge_n in range(reference.sub_entity_count(dim)):
                     ridge = reference.sub_entity(dim, ridge_n)
-                    dofs.append(IntegralAgainst(reference, ridge, 1 / ridge.jacobian(),
+                    dofs.append(IntegralAgainst(reference, 1 / ridge.jacobian(),
                                                 entity=(dim, ridge_n)))
             dim = reference.tdim - 1
             for facet_n in range(reference.sub_entity_count(dim)):
                 facet = reference.sub_entity(dim, facet_n)
                 dofs.append(IntegralOfDirectionalMultiderivative(
-                    reference, facet, (facet.normal(), ), (1, ), (dim, facet_n),
+                    reference, (facet.normal(), ), (1, ), (dim, facet_n),
                     scale=1 / facet.jacobian()))
         else:
             assert order == reference.tdim == 3
             for v_n, v in enumerate(reference.vertices):
                 dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             for e_n, vs in enumerate(reference.sub_entities(1)):
                 subentity = reference.sub_entity(1, e_n)
@@ -66,23 +69,25 @@
                 normals = []
                 for f_n, f_vs in enumerate(reference.sub_entities(2)):
                     if vs[0] in f_vs and vs[1] in f_vs:
                         face = reference.sub_entity(2, f_n)
                         normals.append(face.normal())
                 for orders in [(1, 0), (0, 1)]:
                     dofs.append(IntegralOfDirectionalMultiderivative(
-                        reference, subentity, tuple(normals), orders, (1, e_n),
+                        reference, tuple(normals), orders, (1, e_n),
                         scale=1 / volume))
             for f_n, vs in enumerate(reference.sub_entities(2)):
                 subentity = reference.sub_entity(2, f_n)
                 volume = subentity.jacobian()
                 dofs.append(IntegralOfDirectionalMultiderivative(
-                    reference, subentity, (subentity.normal(), ), (2, ), (2, f_n),
+                    reference, (subentity.normal(), ), (2, ), (2, f_n),
                     scale=1 / volume))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Morley-Wang-Xu", "MWX"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 1
     max_order = {"interval": 1, "triangle": 2, "tetrahedron": 3}
-    continuity = "C{order}"
+    # continuity = "C{order}"
+    continuity = "C0"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/mtw.py` & `symfem-2023.8.0/symfem/elements/mtw.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralMoment, ListOfFunctionals, NormalIntegralMoment,
                            TangentIntegralMoment)
 from ..functions import FunctionInput, VectorFunction
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import Lagrange
 from .nedelec import NedelecFirstKind
 
 
 class MardalTaiWinther(CiarletElement):
     """Mardal-Tai-Winther Hdiv finite element."""
@@ -27,14 +27,16 @@
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         assert order == 3
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference, facets=(NormalIntegralMoment, Lagrange, 1,
                                "contravariant", {"variant": variant}))
 
         poly: typing.List[FunctionInput] = []
         if reference.name == "triangle":
@@ -77,7 +79,8 @@
         return {"variant": self.variant}
 
     names = ["Mardal-Tai-Winther", "MTW"]
     references = ["triangle", "tetrahedron"]
     min_order = 3
     max_order = 3
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/nedelec.py` & `symfem-2023.8.0/symfem/elements/nedelec.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         """
         return {"variant": self.variant}
 
     names = ["Nedelec", "Nedelec1", "N1curl"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.06"
 
 
 class NedelecSecondKind(CiarletElement):
     """Nedelec second kind Hcurl finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
@@ -89,7 +90,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Nedelec2", "N2curl"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/nedelec_prism.py` & `symfem-2023.8.0/symfem/elements/nedelec_prism.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import IntegralAgainst, IntegralMoment, ListOfFunctionals, TangentIntegralMoment
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import Hcurl_polynomials, polynomial_set_1d, polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import Lagrange, VectorLagrange
 from .q import RaviartThomas as QRT
 
 
 class Nedelec(CiarletElement):
     """Nedelec Hcurl finite element."""
@@ -22,14 +22,17 @@
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         from .. import create_reference
 
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += [
             (i[0] * j, i[1] * j, 0)
             for i in polynomial_set_vector(2, 2, order - 1) + Hcurl_polynomials(2, 2, order)
             for j in polynomial_set_1d(1, order, x[2:])]
         poly += [(0, 0, i * j)
                  for i in polynomial_set_1d(2, order, x[:2])
@@ -57,15 +60,15 @@
             # TODO: correct these for order > 2
             for i in range(space1.space_dim):
                 for j in range(space2.space_dim):
                     f = (space2.get_basis_function(j) * space1.get_basis_function(i)[0],
                          space2.get_basis_function(j) * space1.get_basis_function(i)[1],
                          0)
                     dofs.append(IntegralAgainst(
-                        reference, reference, f, entity=(3, 0), mapping="covariant"))
+                        reference, f, entity=(3, 0), mapping="covariant"))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim)
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
@@ -75,7 +78,8 @@
         return {"variant": self.variant}
 
     names = ["Nedelec", "Ncurl"]
     references = ["prism"]
     min_order = 1
     max_order = 2
     continuity = "H(curl)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/q.py` & `symfem-2023.8.0/symfem/elements/q.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,40 +2,56 @@
 
 import typing
 from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement, FiniteElement
-from ..functionals import (DotPointEvaluation, IntegralMoment, ListOfFunctionals,
+from ..functionals import (DotPointEvaluation, IntegralAgainst, IntegralMoment, ListOfFunctionals,
                            NormalIntegralMoment, PointEvaluation, TangentIntegralMoment)
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
-from ..polynomials import (Hcurl_quolynomials, Hdiv_quolynomials, quolynomial_set_1d,
-                           quolynomial_set_vector)
+from ..polynomials import (Hcurl_quolynomials, Hdiv_quolynomials, lobatto_dual_basis,
+                           orthonormal_basis, quolynomial_set_1d, quolynomial_set_vector)
 from ..quadrature import get_quadrature
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 
 
 class Q(CiarletElement):
     """A Q element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         dofs: ListOfFunctionals = []
-        if order == 0:
+        if variant == "legendre":
+            basis = orthonormal_basis(reference.name, order, 0)[0]
+            for f in basis:
+                dofs.append(IntegralAgainst(reference, f, (reference.tdim, 0)))
+        elif order == 0:
             dofs = [PointEvaluation(
-                reference, tuple(sympy.Rational(1, 2) for i in range(reference.tdim)),
+                reference,
+                reference.get_point(tuple(sympy.Rational(1, 2) for i in range(reference.tdim))),
                 entity=(reference.tdim, 0))]
+        elif variant == "lobatto":
+            if reference != reference.default_reference():
+                raise NonDefaultReferenceError()
+            for v_n, v in enumerate(reference.vertices):
+                dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
+            for edim in range(1, 4):
+                for e_n in range(reference.sub_entity_count(edim)):
+                    entity = reference.sub_entity(edim, e_n)
+                    basis = lobatto_dual_basis(entity.name, order, False)
+                    for f in basis:
+                        dofs.append(IntegralAgainst(reference, f, (edim, e_n)))
         else:
             points, _ = get_quadrature(variant, order + 1)
 
             for v_n, v in enumerate(reference.vertices):
                 dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             for edim in range(1, 4):
                 for e_n in range(reference.sub_entity_count(edim)):
@@ -46,26 +62,29 @@
                                 reference, tuple(o + sum(a[j] * points[b]
                                                          for a, b in zip(entity.axes, i[::-1]))
                                                  for j, o in enumerate(entity.origin)),
                                 entity=(edim, e_n)))
 
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_1d(reference.tdim, order)
+        poly = reference.map_polyset_from_default(poly)
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
         self.variant = variant
 
     def get_tensor_factorisation(
         self
     ) -> typing.List[typing.Tuple[str, typing.List[FiniteElement], typing.List[int]]]:
         """Get the representation of the element as a tensor product.
 
         Returns:
             The tensor factorisation
         """
+        if self.variant == "lobatto":
+            return super().get_tensor_factorisation()
         from symfem import create_element
         interval_q = create_element("interval", "Lagrange", self.order)
 
         if self.order == 0:
             perm = [0]
         elif self.reference.name == "quadrilateral":
             n = self.order - 1
@@ -104,27 +123,31 @@
         """
         return {"variant": self.variant}
 
     names = ["Q", "Lagrange", "P"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.07.1"
 
 
 class VectorQ(CiarletElement):
     """A vector Q element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         scalar_space = Q(reference, order, variant)
         dofs: ListOfFunctionals = []
         poly: typing.List[FunctionInput] = []
         if reference.tdim == 1:
             for p in scalar_space.dofs:
                 dofs.append(PointEvaluation(reference, p.dof_point(), entity=p.entity))
 
@@ -151,27 +174,31 @@
         """
         return {"variant": self.variant}
 
     names = ["vector Q", "vQ"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 0
     continuity = "C0"
+    last_updated = "2023.06"
 
 
 class Nedelec(CiarletElement):
     """Nedelec Hcurl finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_vector(reference.tdim, reference.tdim, order - 1)
         poly += Hcurl_quolynomials(reference.tdim, reference.tdim, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             edges=(TangentIntegralMoment, Q, order - 1, {"variant": variant}),
@@ -190,27 +217,31 @@
         """
         return {"variant": self.variant}
 
     names = ["NCE", "RTCE", "Qcurl", "Nedelec", "Ncurl"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.06"
 
 
 class RaviartThomas(CiarletElement):
     """Raviart-Thomas Hdiv finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_vector(reference.tdim, reference.tdim, order - 1)
         poly += Hdiv_quolynomials(reference.tdim, reference.tdim, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             facets=(NormalIntegralMoment, Q, order - 1, {"variant": variant}),
@@ -228,7 +259,8 @@
         """
         return {"variant": self.variant}
 
     names = ["NCF", "RTCF", "Qdiv"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/rannacher_turek.py` & `symfem-2023.8.0/symfem/elements/rannacher_turek.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,31 @@
 """
 
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import ListOfFunctionals, PointEvaluation
 from ..functions import FunctionInput
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 
 
 class RannacherTurek(CiarletElement):
     """Rannacher-Turek finite element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         assert order == 1
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
 
         dofs: ListOfFunctionals = []
         for e_n, vs in enumerate(reference.sub_entities(reference.tdim - 1)):
             pt = reference.sub_entity(reference.tdim - 1, e_n).midpoint()
             dofs.append(PointEvaluation(reference, pt, entity=(reference.tdim - 1, e_n)))
 
         poly: typing.List[FunctionInput] = []
@@ -47,7 +49,8 @@
         return {}
 
     names = ["Rannacher-Turek"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     max_order = 1
     continuity = "L2"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/regge.py` & `symfem-2023.8.0/symfem/elements/regge.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             basis = [f.subs(x, t) for f in space.get_basis_functions()]
             for e_n, vs in enumerate(reference.sub_entities(1)):
                 edge_e = reference.sub_entity(1, e_n)
                 tangent = tuple((b - a) / edge_e.jacobian()
                                 for a, b in zip(edge_e.vertices[0], edge_e.vertices[1]))
                 for f, dof in zip(basis, space.dofs):
                     dofs.append(InnerProductIntegralMoment(
-                        reference, edge_e, f, tangent, tangent, dof, entity=(1, e_n),
+                        reference, f, tangent, tangent, dof, entity=(1, e_n),
                         mapping="double_covariant"))
 
             if reference.tdim == 2:
                 if order > 0:
                     dofs += make_integral_moment_dofs(
                         reference,
                         cells=(IntegralMoment, Regge, order - 1, "double_covariant",
@@ -86,15 +86,15 @@
                 if order > 0:
                     rspace = Regge(create_reference("triangle"), order - 1, "integral")
                     basis = [f.subs(x, t) for f in rspace.get_basis_functions()]
                     for f_n, vs in enumerate(reference.sub_entities(2)):
                         face = reference.sub_entity(2, f_n)
                         for f, dof in zip(basis, rspace.dofs):
                             dofs.append(IntegralMoment(
-                                reference, face, f * face.jacobian(), dof,
+                                reference, f * face.jacobian(), dof,
                                 entity=(2, f_n), mapping="double_covariant"))
 
                 if order > 1:
                     dofs += make_integral_moment_dofs(
                         reference,
                         cells=(IntegralMoment, Regge, order - 2, "double_covariant",
                                {"variant": "integral"}),
@@ -115,14 +115,15 @@
         """
         return {"variant": self.variant}
 
     names = ["Regge"]
     references = ["triangle", "tetrahedron"]
     min_order = 0
     continuity = "inner H(curl)"
+    last_updated = "2023.06"
 
 
 class ReggeTP(CiarletElement):
     """A Regge element on a tensor product cell."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "integral"):
         """Create the element.
@@ -173,72 +174,71 @@
             basis = [f.subs(x, t) for f in space.get_basis_functions()]
             for e_n, vs in enumerate(reference.sub_entities(1)):
                 edge = reference.sub_entity(1, e_n)
                 tangent = tuple((b - a) / edge.jacobian()
                                 for a, b in zip(edge.vertices[0], edge.vertices[1]))
                 for f, dof in zip(basis, space.dofs):
                     dofs.append(InnerProductIntegralMoment(
-                        reference, edge, f, tangent, tangent, dof, entity=(1, e_n),
+                        reference, f, tangent, tangent, dof, entity=(1, e_n),
                         mapping="double_covariant"))
 
             # DOFs on faces
             for f_n, vs in enumerate(reference.sub_entities(2)):
-                face = reference.sub_entity(2, f_n)
                 for i in range(order + 1):
                     for j in range(order + 1):
                         dofs.append(IntegralAgainst(
-                            reference, face,
+                            reference,
                             ((0, x[0] ** i * x[1] ** j), (x[0] ** i * x[1] ** j, 0)),
                             entity=(2, f_n), mapping="double_covariant"))
                 for i in range(1, order + 1):
                     for j in range(order + 1):
                         dofs.append(IntegralAgainst(
-                            reference, face, ((x[1] ** i * x[0] ** j * (1 - x[1]), 0), (0, 0)),
+                            reference, ((x[1] ** i * x[0] ** j * (1 - x[1]), 0), (0, 0)),
                             entity=(2, f_n), mapping="double_covariant"))
                         dofs.append(IntegralAgainst(
-                            reference, face, ((0, 0), (0, x[0] ** i * x[1] ** j * (1 - x[0]))),
+                            reference, ((0, 0), (0, x[0] ** i * x[1] ** j * (1 - x[0]))),
                             entity=(2, f_n), mapping="double_covariant"))
 
             if reference.tdim == 3:
                 # DOFs on cell
                 for i in range(1, order + 1):
                     for j in range(order + 1):
                         for k in range(order + 1):
                             f = x[0] ** i * x[1] ** j * x[2] ** k * (1 - x[0])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((0, 0, 0), (0, 0, f), (0, f, 0)),
+                                reference, ((0, 0, 0), (0, 0, f), (0, f, 0)),
                                 entity=(3, 0), mapping="double_covariant"))
                             f = x[1] ** i * x[0] ** j * x[2] ** k * (1 - x[1])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((0, 0, f), (0, 0, 0), (f, 0, 0)),
+                                reference, ((0, 0, f), (0, 0, 0), (f, 0, 0)),
                                 entity=(3, 0), mapping="double_covariant"))
                             f = x[2] ** i * x[0] ** j * x[1] ** k * (1 - x[2])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((0, f, 0), (f, 0, 0), (0, 0, 0)),
+                                reference, ((0, f, 0), (f, 0, 0), (0, 0, 0)),
                                 entity=(3, 0), mapping="double_covariant"))
                 for i in range(order + 1):
                     for j in range(1, order + 1):
                         for k in range(1, order + 1):
                             f = x[0] ** i * x[1] ** j * x[2] ** k * (1 - x[1]) * (1 - x[2])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((f, 0, 0), (0, 0, 0), (0, 0, 0)),
+                                reference, ((f, 0, 0), (0, 0, 0), (0, 0, 0)),
                                 entity=(3, 0), mapping="double_covariant"))
                             f = x[1] ** i * x[0] ** j * x[2] ** k * (1 - x[0]) * (1 - x[2])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((0, 0, 0), (0, f, 0), (0, 0, 0)),
+                                reference, ((0, 0, 0), (0, f, 0), (0, 0, 0)),
                                 entity=(3, 0), mapping="double_covariant"))
                             f = x[2] ** i * x[0] ** j * x[1] ** k * (1 - x[0]) * (1 - x[1])
                             assert isinstance(f, sympy.core.expr.Expr)
                             dofs.append(IntegralAgainst(
-                                reference, reference, ((0, 0, 0), (0, 0, 0), (0, 0, f)),
+                                reference, ((0, 0, 0), (0, 0, 0), (0, 0, f)),
                                 entity=(3, 0), mapping="double_covariant"))
         else:
             raise ValueError(f"Unknown variant: {variant}")
 
         super().__init__(reference, order, poly, dofs, reference.tdim, reference.tdim ** 2,
                          (reference.tdim, reference.tdim))
         self.variant = variant
@@ -251,7 +251,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Regge"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 0
     continuity = "inner H(curl)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/rhct.py` & `symfem-2023.8.0/symfem/elements/transition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,126 @@
-"""Reduced Hsieh-Clough-Tocher elements on simplices.
-
-This element's definition appears in https://doi.org/10.2307/2006147
-(Ciarlet, 1978)
-"""
+"""Transition elements on simplices."""
 
 import typing
+from itertools import product
 
 import sympy
 
 from ..finite_element import CiarletElement
-from ..functionals import DerivativePointEvaluation, ListOfFunctionals, PointEvaluation
-from ..functions import FunctionInput
-from ..piecewise_functions import PiecewiseFunction
+from ..functionals import ListOfFunctionals, PointEvaluation
+from ..functions import FunctionInput, ScalarFunction
+from ..polynomials import polynomial_set_1d
+from ..quadrature import get_quadrature
 from ..references import Reference
 from ..symbols import x
+from .lagrange import Lagrange
 
 
-class P1Hermite(CiarletElement):
-    """P1Hermite finite element."""
+class Transition(CiarletElement):
+    """Transition finite element."""
 
-    def __init__(self, reference: Reference, order: int, poly: typing.List[FunctionInput]):
+    def __init__(self, reference: Reference, order: int,
+                 edge_orders: typing.Optional[typing.List[int]] = None,
+                 face_orders: typing.Optional[typing.List[int]] = None,
+                 variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
-            poly: The polynomial basis
+            edge_orders: the polynomial order for each edge
+            face_orders: the polynomial order for each face
+            variant: The variant of the element
         """
-        assert order == 3
+        if reference.name == "triangle":
+            assert face_orders is None
+            assert edge_orders is not None
+            assert len(edge_orders) == 3
+        elif reference.name == "tetrahedron":
+            assert face_orders is not None
+            assert edge_orders is not None
+            assert len(face_orders) == 4
+            assert len(edge_orders) == 6
+        bubble_space = Lagrange(reference.default_reference(), 1)
+
         dofs: ListOfFunctionals = []
-        for v_n, vs in enumerate(reference.vertices):
-            dofs.append(PointEvaluation(reference, vs, entity=(0, v_n)))
-            dofs.append(DerivativePointEvaluation(reference, vs, (1, 0), entity=(0, v_n)))
-            dofs.append(DerivativePointEvaluation(reference, vs, (0, 1), entity=(0, v_n)))
+        for v_n, v in enumerate(reference.vertices):
+            dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
+
+        poly: typing.List[FunctionInput] = []
+        poly += polynomial_set_1d(reference.tdim, 1)
+
+        for edim in range(1, 4):
+            for e_n in range(reference.sub_entity_count(edim)):
+                entity = reference.sub_entity(edim, e_n)
+                ref_entity = reference.default_reference().sub_entity(edim, e_n)
+                if edim == reference.tdim:
+                    entity_order = order
+                elif edim == 1:
+                    assert edge_orders is not None
+                    entity_order = edge_orders[e_n]
+                elif edim == 2:
+                    assert face_orders is not None
+                    entity_order = face_orders[e_n]
+                else:
+                    raise RuntimeError("Could not find order for this entity.")
+
+                # DOFs
+                points, _ = get_quadrature(variant, entity_order + 1)
+                for ii in product(range(1, entity_order), repeat=edim):
+                    if sum(ii) < entity_order:
+                        pt = entity.get_point([points[j] for j in ii])
+                        dofs.append(PointEvaluation(reference, pt, entity=(edim, e_n)))
+
+                # Basis
+                if entity_order > edim:
+                    if edim == reference.tdim:
+                        bubble = sympy.Integer(1)
+                        for f in bubble_space.get_basis_functions():
+                            bubble *= f
+                    elif edim == reference.tdim - 1:
+                        bubble = sympy.Integer(1)
+                        for i, f in enumerate(bubble_space.get_basis_functions()):
+                            if i != e_n:
+                                bubble *= f
+                    else:
+                        assert edim == 1 and reference.tdim == 3
+                        bubble = sympy.Integer(1)
+                        for i, f in enumerate(bubble_space.get_basis_functions()):
+                            if i in reference.edges[e_n]:
+                                bubble *= f
+                    space = Lagrange(entity.default_reference(), entity_order - edim - 1,
+                                     variant=variant)
+                    variables = []
+                    origin = ref_entity.vertices[0]
+                    used = []
+                    for p in ref_entity.vertices[1:]:
+                        i = 0
+                        while p[i] == origin[i] or origin[i] == 1 or i in used:
+                            i += 1
+                        used.append(i)
+                        variables.append(origin[i] + (p[i] - origin[i]) * x[i])
+                    for f in space.get_basis_functions():
+                        assert isinstance(f, ScalarFunction)
+                        poly.append(f.subs(x, variables) * bubble)
+
+        poly = reference.map_polyset_from_default(poly)
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
+        self.variant = variant
+        self.face_orders = face_orders
+        self.edge_orders = edge_orders
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
         """Return the kwargs used to create this element.
 
         Returns:
             Keyword argument dictionary
         """
-        return {"poly": self._basis}
+        return {"variant": self.variant, "face_orders": self.face_orders,
+                "edge_orders": self.edge_orders}
 
-    names: typing.List[str] = []
-    references = ["triangle"]
-    min_order = 3
-    max_order = 3
+    names = ["transition"]
+    references = ["triangle", "tetrahedron"]
+    min_order = 1
     continuity = "C0"
-
-
-class ReducedHsiehCloughTocher(CiarletElement):
-    """Reduced Hsieh-Clough-Tocher finite element."""
-
-    def __init__(self, reference: Reference, order: int):
-        """Create the element.
-
-        Args:
-            reference: The reference element
-            order: The polynomial order
-        """
-        from symfem import create_reference
-        assert order == 3
-        assert reference.name == "triangle"
-        dofs: ListOfFunctionals = []
-        for v_n, vs in enumerate(reference.vertices):
-            dofs.append(PointEvaluation(reference, vs, entity=(0, v_n)))
-            dofs.append(DerivativePointEvaluation(reference, vs, (1, 0), entity=(0, v_n)))
-            dofs.append(DerivativePointEvaluation(reference, vs, (0, 1), entity=(0, v_n)))
-
-        mid = tuple(sympy.Rational(sum(i), len(i)) for i in zip(*reference.vertices))
-
-        subs = [
-            (reference.vertices[0], reference.vertices[1], mid),
-            (reference.vertices[1], reference.vertices[2], mid),
-            (reference.vertices[2], reference.vertices[0], mid)]
-
-        refs = [create_reference("triangle", vs) for vs in subs]
-
-        polys: typing.List[typing.List[FunctionInput]] = [[], [], []]
-        for i in range(order + 1):
-            for j in range(order + 1 - i):
-                if i != 2 or j != 1:
-                    polys[0].append(x[0] ** i * x[1] ** j)
-        polys[1] += [1, x[0], x[0] ** 2, x[1], x[0] * x[1], x[1] ** 2,
-                     x[0] * x[1] ** 2 - x[0] ** 2 * x[1],
-                     x[0] ** 3 - x[1] ** 3, x[0] ** 3 + 3 * x[0] * x[1] ** 2]
-        for i in range(order + 1):
-            for j in range(order + 1 - i):
-                if i != 1 or j != 2:
-                    polys[2].append(x[0] ** i * x[1] ** j)
-
-        bases = []
-        for r, p in zip(refs, polys):
-            bf = []
-            for f in P1Hermite(r, 3, p).get_basis_functions():
-                bf.append(f)
-            bases.append(bf)
-
-        piece_list: typing.List[typing.Tuple[FunctionInput, ...]] = []
-        piece_list.append((bases[0][0], 0, bases[2][3]))
-        piece_list.append((bases[0][1], 0, bases[2][4]))
-        piece_list.append((bases[0][2], 0, bases[2][5]))
-        piece_list.append((bases[0][3], bases[1][0], 0))
-        piece_list.append((bases[0][4], bases[1][1], 0))
-        piece_list.append((bases[0][5], bases[1][2], 0))
-        # TODO: are these right to remove??
-        # piece_list.append((bases[0][6], bases[1][6], bases[2][6]))
-        # piece_list.append((bases[0][7], bases[1][7], bases[2][7]))
-        # piece_list.append((bases[0][8], bases[1][8], bases[2][8]))
-        piece_list.append((0, bases[1][3], bases[2][0]))
-        piece_list.append((0, bases[1][4], bases[2][1]))
-        piece_list.append((0, bases[1][5], bases[2][2]))
-
-        poly: typing.List[FunctionInput] = []
-        poly += [
-            PiecewiseFunction({i: j for i, j in zip(subs, p)}, 2)
-            for p in piece_list
-        ]
-
-        super().__init__(
-            reference, order, poly, dofs, reference.tdim, 1
-        )
-
-    names = ["reduced Hsieh-Clough-Tocher", "rHCT"]
-    references = ["triangle"]
-    min_order = 3
-    max_order = 3
-    continuity = "C1"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/rt.py` & `symfem-2023.8.0/symfem/elements/rt.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,7 +49,8 @@
         """
         return {"variant": self.variant}
 
     names = ["Raviart-Thomas", "RT", "N1div"]
     references = ["triangle", "tetrahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/serendipity.py` & `symfem-2023.8.0/symfem/elements/serendipity.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralMoment, ListOfFunctionals, NormalIntegralMoment, PointEvaluation,
                            TangentIntegralMoment)
 from ..functions import FunctionInput
 from ..moments import make_integral_moment_dofs
 from ..polynomials import (Hcurl_serendipity, Hdiv_serendipity, polynomial_set_1d,
                            polynomial_set_vector, serendipity_set_1d)
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from .dpc import DPC, VectorDPC
 
 
 class Serendipity(CiarletElement):
     """A serendipity element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
@@ -27,14 +27,15 @@
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
         poly += serendipity_set_1d(reference.tdim, order)
+        poly = reference.map_polyset_from_default(poly)
 
         dofs: ListOfFunctionals = []
         for v_n, p in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, p, entity=(0, v_n)))
         dofs += make_integral_moment_dofs(
             reference,
             edges=(IntegralMoment, DPC, order - 2, {"variant": variant}),
@@ -53,27 +54,31 @@
         """
         return {"variant": self.variant}
 
     names = ["serendipity", "S"]
     references = ["interval", "quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.06"
 
 
 class SerendipityCurl(CiarletElement):
     """A serendipity Hcurl element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
         poly += Hcurl_serendipity(reference.tdim, reference.tdim, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             edges=(TangentIntegralMoment, DPC, order, {"variant": variant}),
@@ -94,27 +99,31 @@
         """
         return {"variant": self.variant}
 
     names = ["serendipity Hcurl", "Scurl", "BDMCE", "AAE"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.07"
 
 
 class SerendipityDiv(CiarletElement):
     """A serendipity Hdiv element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order)
         poly += Hdiv_serendipity(reference.tdim, reference.tdim, order)
 
         dofs: ListOfFunctionals = make_integral_moment_dofs(
             reference,
             facets=(NormalIntegralMoment, DPC, order, {"variant": variant}),
@@ -133,7 +142,8 @@
         """
         return {"variant": self.variant}
 
     names = ["serendipity Hdiv", "Sdiv", "BDMCF", "AAF"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.07"
```

### Comparing `symfem-2023.4.1/symfem/elements/taylor.py` & `symfem-2023.8.0/symfem/elements/taylor.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Taylor", "discontinuous Taylor"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = 0
     continuity = "L2"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/tnt.py` & `symfem-2023.8.0/symfem/elements/tnt.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import (DerivativeIntegralMoment, IntegralAgainst, ListOfFunctionals,
                            NormalIntegralMoment, PointEvaluation, TangentIntegralMoment)
 from ..functions import FunctionInput, ScalarFunction, VectorFunction
 from ..moments import make_integral_moment_dofs
 from ..polynomials import orthogonal_basis, quolynomial_set_1d, quolynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import t, x
 from .q import Q
 
 
 def p(k: int, v: sympy.core.symbol.Symbol) -> ScalarFunction:
     """Return the kth Legendre polynomial.
 
@@ -58,14 +58,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_1d(reference.tdim, order)
         if reference.tdim == 2:
             for i in range(2):
                 variables = [x[j] for j in range(2) if j != i]
                 for f in [1 - variables[0], variables[0]]:
                     poly.append(f * b(order + 1, x[i]))
@@ -80,36 +83,34 @@
         dofs: ListOfFunctionals = []
         for i, v in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, v, entity=(0, i)))
 
         for i in range(1, order + 1):
             f = i * t[0] ** (i - 1)
             for edge_n in range(reference.sub_entity_count(1)):
-                edge = reference.sub_entity(1, edge_n)
                 dofs.append(IntegralAgainst(
-                    reference, edge, f, entity=(1, edge_n), mapping="identity"))
+                    reference, f, entity=(1, edge_n), mapping="identity"))
 
         for i in range(1, order):
             for j in range(1, order):
                 f = t[0] ** i * (t[0] - 1) * t[1] ** j * (t[1] - 1)
                 delta_f = (f.diff(t[0]).diff(t[0]) + f.diff(t[1]).diff(t[1])).expand()
                 for face_n in range(reference.sub_entity_count(2)):
-                    face = reference.sub_entity(2, face_n)
                     dofs.append(IntegralAgainst(
-                        reference, face, delta_f, entity=(2, face_n), mapping="identity"))
+                        reference, delta_f, entity=(2, face_n), mapping="identity"))
 
         if reference.tdim == 3:
             dummy_dof = PointEvaluation(reference, reference.midpoint(), (3, 0))
             for ii in product(range(1, order), repeat=3):
                 f = sympy.Integer(1)
                 for j, k in zip(ii, x):
                     f *= k ** j * (k - 1)
                 grad_f = tuple(sympy.S(j).expand() for j in ScalarFunction(f).grad(3))
                 dofs.append(DerivativeIntegralMoment(
-                    reference, reference, 1, grad_f, dummy_dof, entity=(3, 0), mapping="identity"))
+                    reference, 1, grad_f, dummy_dof, entity=(3, 0), mapping="identity"))
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, 1
         )
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
@@ -120,27 +121,31 @@
         """
         return {"variant": self.variant}
 
     names = ["tiniest tensor", "TNT"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.06"
 
 
 class TNTcurl(CiarletElement):
     """TiNiest Tensor Hcurl finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_vector(reference.tdim, reference.tdim, order)
         if reference.tdim == 2:
             for ii in product([0, 1], repeat=2):
                 if sum(ii) != 0:
                     poly.append(tuple(sympy.S(j).expand() for j in [
                         p(order, ii[0] * x[0]) * b(order + 1, ii[1] * x[1]),
@@ -181,52 +186,51 @@
             for j in range(2, order + 1):
                 face_moments.append(VectorFunction((
                     t[1] ** (j - 1) * (1 - t[1]) * t[0] ** (i - 2) * (i * t[0] - i + 1),
                     -t[0] ** (i - 1) * (1 - t[0]) * t[1] ** (j - 2) * (j - 1 - j * t[1]))))
         if reference.tdim == 2:
             for f in face_moments:
                 dofs.append(IntegralAgainst(
-                    reference, reference, f, entity=(2, 0), mapping="contravariant"))
+                    reference, f, entity=(2, 0), mapping="contravariant"))
         elif reference.tdim == 3:
             for face_n in range(6):
-                face = reference.sub_entity(2, face_n)
                 for f in face_moments:
                     dofs.append(IntegralAgainst(
-                        reference, face, f, entity=(2, face_n), mapping="contravariant"))
+                        reference, f, entity=(2, face_n), mapping="contravariant"))
 
         # Interior Moments
         if reference.tdim == 3:
             for i in range(1, order):
                 for j in range(1, order):
                     for k in range(order + 1):
                         f = (x[0] ** k * x[1] ** i * (1 - x[1]) * x[2] ** j * (1 - x[2]), 0, 0)
                         dofs.append(IntegralAgainst(
-                            reference, reference, VectorFunction(f).curl().curl(), entity=(3, 0),
+                            reference, VectorFunction(f).curl().curl(), entity=(3, 0),
                             mapping="covariant"))
 
                         f = (0, x[1] ** k * x[0] ** i * (1 - x[0]) * x[2] ** j * (1 - x[2]), 0)
                         dofs.append(IntegralAgainst(
-                            reference, reference, VectorFunction(f).curl().curl(), entity=(3, 0),
+                            reference, VectorFunction(f).curl().curl(), entity=(3, 0),
                             mapping="covariant"))
 
                         if k in [0, 2]:
                             f = (0, 0,  x[2] ** k * x[0] ** i * (1 - x[0]) * x[1] ** j * (1 - x[1]))
                             dofs.append(IntegralAgainst(
-                                reference, reference, VectorFunction(f).curl().curl(),
+                                reference, VectorFunction(f).curl().curl(),
                                 entity=(3, 0), mapping="covariant"))
 
             for i in range(2, order + 1):
                 for j in range(2, order + 1):
                     for k in range(2, order + 1):
                         f = x[0] ** (i - 1) * x[0] ** i
                         f *= x[1] ** (j - 1) * x[1] ** j
                         f *= x[2] ** (k - 1) * x[2] ** k
                         grad_f = ScalarFunction(f).grad(3)
                         dofs.append(IntegralAgainst(
-                            reference, reference, grad_f, entity=(3, 0), mapping="contravariant"))
+                            reference, grad_f, entity=(3, 0), mapping="contravariant"))
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, reference.tdim
         )
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
@@ -237,27 +241,31 @@
         """
         return {"variant": self.variant}
 
     names = ["tiniest tensor Hcurl", "TNTcurl"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.06"
 
 
 class TNTdiv(CiarletElement):
     """TiNiest Tensor Hdiv finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += quolynomial_set_vector(reference.tdim, reference.tdim, order)
         if reference.tdim == 2:
             for ii in product([0, 1], repeat=2):
                 if sum(ii) != 0:
                     poly.append(tuple(sympy.S(j).expand() for j in [
                         b(order + 1, ii[0] * x[0]) * p(order, ii[1] * x[1]),
@@ -285,57 +293,57 @@
             if sum(ii) > 0:
                 if reference.tdim == 2:
                     f = x[0] ** ii[0] * x[1] ** ii[1]
                 else:
                     f = x[0] ** ii[0] * x[1] ** ii[1] * x[2] ** ii[2]
                 grad_f = ScalarFunction(f).grad(reference.tdim)
                 dofs.append(IntegralAgainst(
-                    reference, reference, grad_f, entity=(reference.tdim, 0), mapping="covariant"))
+                    reference, grad_f, entity=(reference.tdim, 0), mapping="covariant"))
 
         if reference.tdim == 2:
             for i in range(2, order + 1):
                 for j in range(2, order + 1):
                     f = (x[0] ** (i - 1) * (1 - x[0]) * x[1] ** (j - 2) * (j - 1 - j * x[1]),
                          x[1] ** (j - 1) * (1 - x[1]) * x[0] ** (i - 2) * (i * x[0] - i + 1))
                     dofs.append(IntegralAgainst(
-                        reference, reference, f, entity=(reference.tdim, 0), mapping="covariant"))
+                        reference, f, entity=(reference.tdim, 0), mapping="covariant"))
         if reference.tdim == 3:
             for i in range(2, order + 1):
                 for j in range(2, order + 1):
                     for k in range(order + 1):
                         f = (
                             x[2] ** k * x[0] ** (i - 1) * (1 - x[0]) * x[2] ** (j - 2) * (
                                 j - 1 - j * x[1]),
                             x[2] ** k * x[1] ** (j - 1) * (1 - x[1]) * x[0] ** (i - 2) * (
                                 i * x[0] - i + 1),
                             0
                         )
                         dofs.append(IntegralAgainst(
-                            reference, reference, f, entity=(reference.tdim, 0),
+                            reference, f, entity=(reference.tdim, 0),
                             mapping="covariant"))
                         f = (
                             x[1] ** k * x[0] ** (i - 1) * (1 - x[0]) * x[2] ** (j - 2) * (
                                 j - 1 - j * x[2]),
                             0,
                             x[1] ** k * x[2] ** (j - 1) * (1 - x[2]) * x[0] ** (i - 2) * (
                                 i * x[0] - i + 1)
                         )
                         dofs.append(IntegralAgainst(
-                            reference, reference, f, entity=(reference.tdim, 0),
+                            reference, f, entity=(reference.tdim, 0),
                             mapping="covariant"))
                         if k in [0, 2]:
                             f = (
                                 0,
                                 x[0] ** k * x[1] ** (i - 1) * (1 - x[1]) * x[2] ** (j - 2) * (
                                     j - 1 - j * x[2]),
                                 x[0] ** k * x[2] ** (j - 1) * (1 - x[2]) * x[1] ** (i - 2) * (
                                     i * x[1] - i + 1)
                             )
                             dofs.append(IntegralAgainst(
-                                reference, reference, f, entity=(reference.tdim, 0),
+                                reference, f, entity=(reference.tdim, 0),
                                 mapping="covariant"))
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, reference.tdim
         )
         self.variant = variant
 
@@ -347,7 +355,8 @@
         """
         return {"variant": self.variant}
 
     names = ["tiniest tensor Hdiv", "TNTdiv"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/trimmed_serendipity.py` & `symfem-2023.8.0/symfem/elements/trimmed_serendipity.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from ..finite_element import CiarletElement
 from ..functionals import (IntegralAgainst, IntegralMoment, ListOfFunctionals, NormalIntegralMoment,
                            TangentIntegralMoment)
 from ..functions import FunctionInput, ScalarFunction, VectorFunction
 from ..moments import make_integral_moment_dofs
 from ..polynomials import polynomial_set_vector
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import t, x
 from .dpc import DPC, VectorDPC
 
 
 class TrimmedSerendipityHcurl(CiarletElement):
     """Trimmed serendipity Hcurl finite element."""
 
@@ -25,14 +25,17 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order - 1)
         if reference.tdim == 2:
             poly += [
                 (x[0] ** j * x[1] ** (order - j), -x[0] ** (j + 1) * x[1] ** (order - 1 - j))
                 for j in range(order)]
             if order == 1:
@@ -80,20 +83,19 @@
             faces=(IntegralMoment, VectorDPC, order - 3, "contravariant",
                    {"variant": variant}),
             volumes=(IntegralMoment, VectorDPC, order - 5, "contravariant",
                      {"variant": variant}),
         )
         if order >= 2:
             for f_n in range(reference.sub_entity_count(2)):
-                face = reference.sub_entity(2, f_n)
                 for i in range(order):
                     f = ScalarFunction(x[0] ** (order - 1 - i) * x[1] ** i).grad(2)
                     f2 = VectorFunction((f[1], -f[0])).subs(x, tuple(t))
                     dofs.append(IntegralAgainst(
-                        reference, face, f2, entity=(2, f_n), mapping="contravariant"))
+                        reference, f2, entity=(2, f_n), mapping="contravariant"))
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, reference.tdim
         )
         self.variant = variant
 
     def init_kwargs(self) -> typing.Dict[str, typing.Any]:
@@ -104,27 +106,31 @@
         """
         return {"variant": self.variant}
 
     names = ["trimmed serendipity Hcurl", "TScurl"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(curl)"
+    last_updated = "2023.06"
 
 
 class TrimmedSerendipityHdiv(CiarletElement):
     """Trimmed serendipity Hdiv finite element."""
 
     def __init__(self, reference: Reference, order: int, variant: str = "equispaced"):
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
             variant: The variant of the element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_vector(reference.tdim, reference.tdim, order - 1)
         if reference.tdim == 2:
             poly += [
                 (x[0] ** (j + 1) * x[1] ** (order - 1 - j), x[0] ** j * x[1] ** (order - j))
                 for j in range(order)]
             if order == 1:
@@ -161,15 +167,15 @@
                 fs = [ScalarFunction(x[0] ** (order - 1 - i) * x[1] ** i).grad(2)
                       for i in range(order)]
             else:
                 fs = [ScalarFunction(x[0] ** (order - 1 - i - j) * x[1] ** i * x[2] ** j).grad(3)
                       for i in range(order) for j in range(order - i)]
             for f in fs:
                 f2 = f.subs(x, tuple(t))
-                dofs.append(IntegralAgainst(reference, reference, f2, entity=(reference.tdim, 0),
+                dofs.append(IntegralAgainst(reference, f2, entity=(reference.tdim, 0),
                                             mapping="covariant"))
 
         super().__init__(
             reference, order, poly, dofs, reference.tdim, reference.tdim
         )
         self.variant = variant
 
@@ -181,7 +187,8 @@
         """
         return {"variant": self.variant}
 
     names = ["trimmed serendipity Hdiv", "TSdiv"]
     references = ["quadrilateral", "hexahedron"]
     min_order = 1
     continuity = "H(div)"
+    last_updated = "2023.06"
```

### Comparing `symfem-2023.4.1/symfem/elements/vector_enriched_galerkin.py` & `symfem-2023.8.0/symfem/elements/vector_enriched_galerkin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,42 +5,45 @@
 """
 
 import typing
 
 from ..finite_element import CiarletElement, EnrichedElement
 from ..functionals import BaseFunctional, IntegralAgainst
 from ..functions import FunctionInput, VectorFunction
-from ..references import Reference
+from ..references import NonDefaultReferenceError, Reference
 from ..symbols import x
 from .lagrange import VectorLagrange
 from .q import VectorQ
 
 
 class Enrichment(CiarletElement):
     """An LF enriched Galerkin element."""
 
     def __init__(self, reference: Reference):
         """Create the element.
 
         Args:
             reference: The reference element
         """
+        if reference.vertices != reference.reference_vertices:
+            raise NonDefaultReferenceError()
         f = VectorFunction(tuple(x[i] - j for i, j in enumerate(reference.midpoint())))
         poly: typing.List[FunctionInput] = [f]
         size = f.dot(f).integral(reference, x)
         dofs: typing.List[BaseFunctional] = [IntegralAgainst(
-            reference, reference, tuple(i / size for i in f), (reference.tdim, 0), "contravariant")]
+            reference, tuple(i / size for i in f), (reference.tdim, 0), "contravariant")]
 
         super().__init__(reference, 1, poly, dofs, reference.tdim, reference.tdim)
 
-    names = []
+    names: typing.List[str] = []
     references = ["triangle", "quadrilateral", "tetrahedron", "hexahedron"]
     min_order = 1
     max_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
 
 
 class VectorEnrichedGalerkin(EnrichedElement):
     """An LF enriched Galerkin element."""
 
     def __init__(self, reference: Reference, order: int):
         """Create the element.
@@ -54,7 +57,8 @@
         else:
             super().__init__([VectorLagrange(reference, order), Enrichment(reference)])
 
     names = ["enriched vector Galerkin", "locking-free enriched Galerkin", "LFEG"]
     references = ["triangle", "quadrilateral", "tetrahedron", "hexahedron"]
     min_order = 1
     continuity = "C0"
+    last_updated = "2023.05"
```

### Comparing `symfem-2023.4.1/symfem/elements/wu_xu.py` & `symfem-2023.8.0/symfem/elements/wu_xu.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import typing
 
 from ..finite_element import CiarletElement
 from ..functionals import (DerivativePointEvaluation, IntegralOfDirectionalMultiderivative,
                            ListOfFunctionals, PointEvaluation)
 from ..functions import FunctionInput
 from ..polynomials import polynomial_set_1d
-from ..references import Reference
-from ..symbols import x
+from ..references import NonDefaultReferenceError, Reference
 
 
 def derivatives(dim: int, order: int) -> typing.List[typing.Tuple[int, ...]]:
     """Return all the orders of a multidimensional derivative.
 
     Args:
         dim: The topological dimension
@@ -41,23 +40,27 @@
         """Create the element.
 
         Args:
             reference: The reference element
             order: The polynomial order
         """
         assert order == reference.tdim + 1
+        if reference.name == "tetrahedron" and reference != reference.default_reference():
+            raise NonDefaultReferenceError()
+
         poly: typing.List[FunctionInput] = []
         poly += polynomial_set_1d(reference.tdim, order)
 
+        invmap = reference.get_inverse_map_to_self()
         if reference.name == "interval":
-            bubble = x[0] * (1 - x[0])
+            bubble = invmap[0] * (1 - invmap[0])
         elif reference.name == "triangle":
-            bubble = x[0] * x[1] * (1 - x[0] - x[1])
+            bubble = invmap[0] * invmap[1] * (1 - invmap[0] - invmap[1])
         elif reference.name == "tetrahedron":
-            bubble = x[0] * x[1] * x[2] * (1 - x[0] - x[1] - x[2])
+            bubble = invmap[0] * invmap[1] * invmap[2] * (1 - invmap[0] - invmap[1] - invmap[2])
 
         poly += [bubble * i for i in polynomial_set_1d(reference.tdim, 1)[1:]]
 
         dofs: ListOfFunctionals = []
         for v_n, v in enumerate(reference.vertices):
             dofs.append(PointEvaluation(reference, v, entity=(0, v_n)))
             for i in range(reference.tdim):
@@ -77,17 +80,19 @@
                         if vs[0] in f_vs and vs[1] in f_vs:
                             face = reference.sub_entity(2, f_n)
                             normals.append(face.normal())
                 else:
                     raise NotImplementedError
                 for orders in derivatives(len(normals), len(normals)):
                     dofs.append(IntegralOfDirectionalMultiderivative(
-                        reference, subentity, tuple(normals), orders, (dim, e_n),
+                        reference, tuple(normals), orders, (dim, e_n),
                         scale=1 / volume))
 
         super().__init__(reference, order, poly, dofs, reference.tdim, 1)
 
     names = ["Wu-Xu"]
     references = ["interval", "triangle", "tetrahedron"]
     min_order = {"interval": 2, "triangle": 3, "tetrahedron": 4}
     max_order = {"interval": 2, "triangle": 3, "tetrahedron": 4}
-    continuity = "C{order}"
+    continuity = "C0"
+    # continuity = "C{order}"
+    last_updated = "2023.06.1"
```

### Comparing `symfem-2023.4.1/symfem/finite_element.py` & `symfem-2023.8.0/symfem/finite_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 import typing
 from abc import ABC, abstractmethod
 from itertools import product
 
 import sympy
 
 from .basis_functions import BasisFunction
+from .caching import load_cached_matrix, save_cached_matrix
 from .functionals import ListOfFunctionals
 from .functions import (AnyFunction, FunctionInput, ScalarFunction, VectorFunction,
                         parse_function_input)
 from .geometry import PointType, SetOfPointsInput, parse_set_of_points_input
+from .mappings import MappingNotImplemented
 from .piecewise_functions import PiecewiseFunction
 from .plotting import Picture, colors
-from .references import Reference
+from .references import NonDefaultReferenceError, Reference
 from .symbols import x
 from .utils import allequal
+from .version import version
 
 TabulatedBasis = typing.Union[
     typing.List[typing.Union[sympy.core.expr.Expr, int]],
     typing.List[typing.Tuple[typing.Union[sympy.core.expr.Expr, int], ...]],
     typing.List[typing.Tuple[typing.Tuple[typing.Union[sympy.core.expr.Expr, int], ...], ...]],
     typing.List[sympy.matrices.dense.MutableDenseMatrix],
 ]
@@ -284,15 +287,15 @@
         Returns:
             The polynomial basis
         """
         pass
 
     def test(self):
         """Run tests for this element."""
-        if self.order <= 4:
+        if self.order <= self._max_continuity_test_order:
             self.test_continuity()
 
     def test_continuity(self):
         """Test that this element has the correct continuity."""
         continuity = self.continuity
         if "{order}" in continuity:
             continuity = continuity.replace("{order}", f"{self.order}")
@@ -335,50 +338,60 @@
             return
 
         for dim, entities in entity_pairs:
             for fi, gi in zip(*[self.entity_dofs(dim, i) for i in entities]):
                 basis = self.get_basis_functions()
                 try:
                     basis2 = self.map_to_cell(vertices)
-                except NotImplementedError:
+                except (MappingNotImplemented, NonDefaultReferenceError):
                     return "Mapping not implemented for this element."
 
                 f = basis[fi]
                 g = basis2[gi]
 
                 def get_piece(f, point):
                     if isinstance(f, PiecewiseFunction):
                         return f.get_piece(point)
                     if isinstance(f, list):
                         return [get_piece(g, point) for g in f]
                     if isinstance(f, tuple):
                         return tuple(get_piece(g, point) for g in f)
                     return f
 
-                if self.reference.tdim == 2:
+                if self.reference.tdim == 1:
+                    f = get_piece(f, (0, ))
+                    g = get_piece(g, (0, ))
+                elif self.reference.tdim == 2:
                     f = get_piece(f, (0, sympy.Rational(1, 2)))
                     g = get_piece(g, (0, sympy.Rational(1, 2)))
                 elif self.reference.tdim == 3:
                     f = get_piece(f, (0, sympy.Rational(1, 3), sympy.Rational(1, 3)))
                     g = get_piece(g, (0, sympy.Rational(1, 3), sympy.Rational(1, 3)))
 
-                f = f.subs(x[0], 0)
-                g = g.subs(x[0], 0)
-
                 if continuity[0] == "C":
                     order = int(continuity[1:])
                     deriv_f = [f]
                     deriv_g = [g]
                     f = [f]
                     g = [g]
                     for _ in range(order):
                         deriv_f = [d.diff(i) for d in deriv_f for i in x[:self.reference.tdim]]
                         f += deriv_f
                         deriv_g = [d.diff(i) for d in deriv_g for i in x[:self.reference.tdim]]
                         g += deriv_g
+
+                    f = [i.subs(x[0], 0) for i in f]
+                    g = [i.subs(x[0], 0) for i in g]
+                else:
+                    f = f.subs(x[0], 0)
+                    g = g.subs(x[0], 0)
+
+                if continuity[0] == "C":
+                    pass
+
                 elif continuity == "H(div)":
                     f = f[0]
                     g = g[0]
                 elif continuity == "inner H(div)":
                     f = f[0, 0]
                     g = g[0, 0]
                 elif continuity == "H(curl)":
@@ -438,25 +451,36 @@
                     basis[p] = ScalarFunction(1)
                     for i in k:
                         basis[p] *= i
             else:
                 raise ValueError(f"Unknown tensor product type: {t_type}")
         return [basis[i] for i in range(len(basis))]
 
+    def init_kwargs(self) -> typing.Dict[str, typing.Any]:
+        """Return the keyword arguments used to create this element.
+
+        Returns:
+            Keyword arguments dictionary
+        """
+        return {}
+
     @property
     def name(self) -> str:
         """Get the name of the element.
 
         Returns:
             The name of the element's family
         """
         return self.names[0]
 
     names: typing.List[str] = []
     references: typing.List[str] = []
+    last_updated = version
+    cache = True
+    _max_continuity_test_order = 4
 
 
 class CiarletElement(FiniteElement):
     """Finite element defined using the Ciarlet definition."""
 
     def __init__(
         self, reference: Reference, order: int, basis: typing.List[FunctionInput],
@@ -522,36 +546,42 @@
         """Get the symbolic polynomial basis for the element.
 
         Returns:
             The polynomial basis
         """
         return self._basis
 
-    def get_dual_matrix(self) -> sympy.matrices.dense.MutableDenseMatrix:
+    def get_dual_matrix(
+        self, inverse=False, caching=True
+    ) -> sympy.matrices.dense.MutableDenseMatrix:
         """Get the dual matrix.
 
-        Returns:
-            The dual matrix
-        """
-        mat = []
-        for b in self.get_polynomial_basis():
-            row = []
-            for d in self.dofs:
-                entry = d.eval_symbolic(b).as_sympy()
-                row.append(entry)
-            mat.append(row)
-        return sympy.Matrix(mat)
-
-    def init_kwargs(self) -> typing.Dict[str, typing.Any]:
-        """Return the keyword arguments used to create this element.
+        Args:
+            inverse: Should the dual matrix be inverted?
+            caching: Should the result be cached
 
         Returns:
-            Keyword arguments dictionary
+            The dual matrix
         """
-        return {}
+        if caching and self.cache:
+            cid = (f"{self.__class__.__name__} {self.order} {self.reference.vertices} "
+                   f"{self.init_kwargs()} {self.last_updated}")
+            matrix_type = "dualinv" if inverse else "dual"
+            mat = load_cached_matrix(matrix_type, cid, (len(self.dofs), len(self.dofs)))
+            if mat is None:
+                mat = self.get_dual_matrix(inverse, caching=False)
+                save_cached_matrix(matrix_type, cid, mat)
+            return mat
+        else:
+            mat = sympy.Matrix([[d.eval_symbolic(b).as_sympy() for d in self.dofs]
+                                for b in self.get_polynomial_basis()])
+            if inverse:
+                return mat.inv("LU")
+            else:
+                return mat
 
     def get_basis_functions(
         self, use_tensor_factorisation: bool = False
     ) -> typing.List[AnyFunction]:
         """Get the basis functions of the element.
 
         Args:
@@ -560,17 +590,15 @@
         Returns:
             The basis functions
         """
         if self._basis_functions is None:
             if use_tensor_factorisation:
                 self._basis_functions = self._get_basis_functions_tensor()
             else:
-                m = self.get_dual_matrix()
-                assert isinstance(m, sympy.Matrix)
-                minv = m.inv("LU")
+                minv = self.get_dual_matrix(inverse=True)
 
                 sfs: typing.List[AnyFunction] = []
                 pb = self.get_polynomial_basis()
                 for i, dof in enumerate(self.dofs):
                     sf = ScalarFunction(minv[i, 0]) * pb[0]
                     for c, d in zip(minv.row(i)[1:], pb[1:]):
                         sf += ScalarFunction(c) * d
@@ -633,39 +661,44 @@
         if basis is None:
             basis = self.get_basis_functions()
         if forward_map is None:
             forward_map = self.reference.get_map_to(vertices)
         if inverse_map is None:
             inverse_map = self.reference.get_inverse_map_to(vertices)
 
-        functions: typing.List[AnyFunction] = [ScalarFunction(0) for f in basis]
-        for dim in range(self.reference.tdim + 1):
-            for e in range(self.reference.sub_entity_count(dim)):
-                entity_dofs = self.entity_dofs(dim, e)
-                dofs_by_type: typing.Dict[
-                    typing.Tuple[typing.Type, typing.Union[str, None]], typing.List[int]
-                ] = {}
-                for d in entity_dofs:
-                    dof = self.dofs[d]
-                    t = (type(dof), dof.mapping)
-                    if t not in dofs_by_type:
-                        dofs_by_type[t] = []
-                    dofs_by_type[t].append(d)
-                for ds in dofs_by_type.values():
-                    mapped_dofs = self.dofs[ds[0]].perform_mapping(
-                        [basis[d] for d in ds],
-                        forward_map, inverse_map, self.reference.tdim)
-                    for d_n, mdof in zip(ds, mapped_dofs):
-                        functions[d_n] = mdof
-
-        for fun in functions:
-            if isinstance(fun, PiecewiseFunction):
-                fun.map_pieces(forward_map)
-
-        return functions
+        try:
+            functions: typing.List[AnyFunction] = [ScalarFunction(0) for f in basis]
+            for dim in range(self.reference.tdim + 1):
+                for e in range(self.reference.sub_entity_count(dim)):
+                    entity_dofs = self.entity_dofs(dim, e)
+                    dofs_by_type: typing.Dict[
+                        typing.Tuple[typing.Type, typing.Union[str, None]], typing.List[int]
+                    ] = {}
+                    for d in entity_dofs:
+                        dof = self.dofs[d]
+                        t = (type(dof), dof.mapping)
+                        if t not in dofs_by_type:
+                            dofs_by_type[t] = []
+                        dofs_by_type[t].append(d)
+                    for ds in dofs_by_type.values():
+                        mapped_dofs = self.dofs[ds[0]].perform_mapping(
+                            [basis[d] for d in ds],
+                            forward_map, inverse_map, self.reference.tdim)
+                        for d_n, mdof in zip(ds, mapped_dofs):
+                            functions[d_n] = mdof
+
+            for fun in functions:
+                if isinstance(fun, PiecewiseFunction):
+                    fun.map_pieces(forward_map)
+
+            return functions
+        except MappingNotImplemented:
+            element = self.__class__(
+                self.reference.__class__(vertices=vertices), self.order, **self.init_kwargs())
+            return element.get_basis_functions()
 
     def test(self):
         """Run tests for this element."""
         super().test()
         self.test_functional_entities()
         self.test_functionals()
         self.test_dof_points()
@@ -833,15 +866,20 @@
             basis: The basis functions
             forward_map: The map from the reference to the cell
             inverse_map: The map to the reference from the cell
 
         Returns:
             The basis functions mapped to the cell
         """
-        raise NotImplementedError()
+        raise MappingNotImplemented()
+        # TODO: make this work
+        # vertices = parse_set_of_points_input(vertices_in)
+        # e = self.__class__(self.reference.__class__(vertices=vertices), self.order,
+        #                   **self.init_kwargs())
+        # return e.get_basis_functions()
 
     def get_polynomial_basis(self) -> typing.List[AnyFunction]:
         """Get the symbolic polynomial basis for the element.
 
         Returns:
             The polynomial basis
         """
```

### Comparing `symfem-2023.4.1/symfem/functionals.py` & `symfem-2023.8.0/symfem/functionals.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 import sympy
 
 from . import mappings
 from .functions import (AnyFunction, FunctionInput, ScalarFunction, VectorFunction,
                         parse_function_input)
 from .geometry import PointType, SetOfPoints
-from .references import Interval, Reference
+from .piecewise_functions import PiecewiseFunction
+from .references import Interval, NonDefaultReferenceError, Reference
 from .symbols import t, x
 
 ScalarValueOrFloat = typing.Union[sympy.core.expr.Expr, float]
 
 
 def _to_tex(f: FunctionInput, tfrac: bool = False) -> str:
     r"""Convert an expresson to TeX.
@@ -36,20 +37,22 @@
 def _nth(n: int) -> str:
     """Add th, st or nd to a number.
 
     Args:
         n: The number
 
     Returns:
-        The string (n)th, (n)st or (n)nd
+        The string (n)th, (n)st, (n)rd or (n)nd
     """
     if n % 10 == 1 and n != 11:
         return f"{n}st"
     if n % 10 == 2 and n != 12:
         return f"{n}nd"
+    if n % 10 == 3 and n != 12:
+        return f"{n}rd"
     return f"{n}th"
 
 
 class BaseFunctional(ABC):
     """A functional."""
 
     def __init__(self, reference: Reference, entity: typing.Tuple[int, int],
@@ -393,30 +396,15 @@
             map: Map from the reference cell to a physical cell
             inverse_map: Map to the reference cell from a physical cell
             tdim: The topological dimension of the cell
 
         Returns:
             Mapped functions
         """
-        if self.mapping is not None:
-            return super().perform_mapping(fs, map, inverse_map, tdim)
-        out = []
-        J = sympy.Matrix([[map[i].diff(x[j]) for j in range(tdim)] for i in range(tdim)])
-        for dofs in zip(*[fs[i::tdim] for i in range(tdim)]):
-            for i in range(tdim):
-                f = ScalarFunction(0)
-                for a, b in zip(dofs, J.row(i)):
-                    f += a * b
-                out.append(f)
-
-        out2: typing.List[AnyFunction] = []
-        for b in out:
-            item = b.subs(x, inverse_map)
-            out2.append(item)
-        return out2
+        raise mappings.MappingNotImplemented()
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
@@ -777,58 +765,136 @@
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
         desc = "\\boldsymbol{v}\\mapsto"
         desc += "\\boldsymbol{v}(" + ",".join([_to_tex(i, True) for i in self.dof_point()]) + ")"
-        if isinstance(self.vector, (tuple, list)):
+        if self.vector.is_vector:
             desc += "\\cdot\\left(\\begin{array}{c}"
+            assert hasattr(self.vector, "__iter__")
             desc += "\\\\".join([_to_tex(i) for i in self.vector])
             desc += "\\end{array}\\right)"
         elif self.vector != 1:
             desc += f"\\cdot{_to_tex(self.vector)}"
         return desc, []
 
     name = "Dot point evaluation"
 
 
+class PointDivergenceEvaluation(BaseFunctional):
+    """A point evaluation of the divergence."""
+
+    def __init__(self, reference: Reference, point_in: FunctionInput,
+                 entity: typing.Tuple[int, int], mapping: typing.Union[str, None] = "identity"):
+        """Create the functional.
+
+        Args:
+            reference: The reference cell
+            point_in: The points
+            entity: The entity the functional is associated with
+            mapping: The type of mappping from the reference cell to a physical cell
+        """
+        super().__init__(reference, entity, mapping)
+        self.point = parse_function_input(point_in)
+        assert self.point.is_vector
+
+    def _eval_symbolic(self, function: AnyFunction) -> AnyFunction:
+        """Apply to the functional to a function.
+
+        Args:
+            function: The function
+
+        Returns:
+            The value of the functional for the function
+        """
+        out = ScalarFunction(0)
+        if isinstance(function, PiecewiseFunction):
+            pt = self.point.as_sympy()
+            assert isinstance(pt, tuple)
+            function = function.get_piece(pt)
+        assert isinstance(function, VectorFunction)
+        for f, i in zip(function, x):
+            out += f.diff(i)
+        return out.subs(x, self.point)
+
+    def dof_point(self) -> PointType:
+        """Get the location of the DOF in the cell.
+
+        Returns:
+            The point
+        """
+        pt = self.point.as_sympy()
+        assert isinstance(pt, tuple)
+        return pt
+
+    def dof_direction(self) -> typing.Union[PointType, None]:
+        """Get the direction of the DOF.
+
+        Returns:
+            The direction
+        """
+        return None
+
+    def adjusted_dof_point(self) -> PointType:
+        """Get the adjusted position of the DOF in the cell for plotting.
+
+        Returns:
+            The point
+        """
+        return self.dof_point()
+
+    def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
+        """Get a representation of the functional as TeX, and list of terms involved.
+
+        Returns:
+            Representation of the functional as TeX, and list of terms involved
+        """
+        desc = "\\boldsymbol{v}\\mapsto"
+        desc += "\\nablaa\\cdot\\boldsymbol{v}"
+        desc += "(" + ",".join([_to_tex(i, True) for i in self.dof_point()]) + ")"
+        return desc, []
+
+    name = "Point evaluation of divergence"
+
+
 class IntegralAgainst(BaseFunctional):
     """An integral against a function."""
 
     f: AnyFunction
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  entity: typing.Tuple[int, int], mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         super().__init__(reference, entity, mapping)
-        self.integral_domain = integral_domain
+        self.integral_domain = reference.sub_entity(*entity)
 
-        f = parse_function_input(f_in)
+        f = parse_function_input(f_in) / reference.jacobian()
         f = f.subs(x, t)
 
         if f.is_vector:
             assert len(f) == self.integral_domain.tdim
             self.f = mappings.contravariant(
-                f, integral_domain.get_map_to_self(), integral_domain.get_inverse_map_to_self(),
-                integral_domain.tdim)
+                f, self.integral_domain.get_map_to_self(),
+                self.integral_domain.get_inverse_map_to_self(),
+                self.integral_domain.tdim)
         elif f.is_matrix:
             assert f.shape[0] == self.integral_domain.tdim
             assert f.shape[1] == self.integral_domain.tdim
             self.f = mappings.double_contravariant(
-                f, integral_domain.get_map_to_self(), integral_domain.get_inverse_map_to_self(),
-                integral_domain.tdim)
+                f, self.integral_domain.get_map_to_self(),
+                self.integral_domain.get_inverse_map_to_self(),
+                self.integral_domain.tdim)
         else:
             self.f = f
 
     def dof_point(self) -> PointType:
         """Get the location of the DOF in the cell.
 
         Returns:
@@ -868,15 +934,15 @@
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
         entity = self.entity_tex()
         entity_def = self.entity_definition()
-        if isinstance(self.f, tuple):
+        if self.f.is_vector:
             desc = "\\mathbf{v}\\mapsto"
             desc += f"\\displaystyle\\int_{{{entity}}}"
             desc += _to_tex(self.f, True) + "\\cdot"
             desc += "\\mathbf{v}"
         else:
             desc = "\\mathbf{v}\\mapsto"
             desc += f"\\displaystyle\\int_{{{entity}}}"
@@ -887,27 +953,26 @@
 
     name = "Integral against"
 
 
 class IntegralOfDivergenceAgainst(BaseFunctional):
     """An integral of the divergence against a function."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  entity: typing.Tuple[int, int], mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         super().__init__(reference, entity, mapping)
-        self.integral_domain = integral_domain
+        self.integral_domain = reference.sub_entity(*entity)
 
         f = parse_function_input(f_in)
         self.f = f.subs(x, t)
 
     def dof_point(self) -> PointType:
         """Get the location of the DOF in the cell.
 
@@ -961,30 +1026,30 @@
 
     name = "Integral of divergence against"
 
 
 class IntegralOfDirectionalMultiderivative(BaseFunctional):
     """An integral of a directional derivative of a scalar function."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, directions: SetOfPoints,
+    def __init__(self, reference: Reference, directions: SetOfPoints,
                  orders: typing.Tuple[int, ...], entity: typing.Tuple[int, int], scale: int = 1,
                  mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
             integral_domain: The domain of the integral
             directions: The diections of the derivatives
             orders: The orders of the derivatives
             entity: The entity the functional is associated with
             scale: The scale factor
             mapping: The type of mappping from the reference cell to a physical cell
         """
         super().__init__(reference, entity, mapping)
-        self.integral_domain = integral_domain
+        self.integral_domain = reference.sub_entity(*entity)
         self.directions = directions
         self.orders = orders
         self.scale = scale
 
     def dof_point(self) -> PointType:
         """Get the location of the DOF in the cell.
 
@@ -1022,17 +1087,15 @@
             map: Map from the reference cell to a physical cell
             inverse_map: Map to the reference cell from a physical cell
             tdim: The topological dimension of the cell
 
         Returns:
             Mapped functions
         """
-        if sum(self.orders) > 0:
-            raise NotImplementedError("Mapping high order derivatives not implemented")
-        return super().perform_mapping(fs, map, inverse_map, tdim)
+        raise mappings.MappingNotImplemented()
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
@@ -1060,47 +1123,59 @@
 
 
 class IntegralMoment(BaseFunctional):
     """An integral moment."""
 
     f: AnyFunction
 
-    def __init__(self, reference: Reference, integral_domain: Reference,
-                 f_in: FunctionInput, dof: BaseFunctional,
-                 entity: typing.Tuple[int, int], mapping: typing.Union[str, None] = "identity"):
+    def __init__(self, reference: Reference,
+                 f_in: FunctionInput, dof: BaseFunctional, entity: typing.Tuple[int, int],
+                 mapping: typing.Union[str, None] = "identity", map_function: bool = True):
         """Create the functional.
 
         Args:
             reference: The reference cell
             integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
+            map_function: Should the function be mapped?
         """
         super().__init__(reference, entity, mapping)
-        self.integral_domain = integral_domain
+        self.integral_domain = reference.sub_entity(*entity)
         self.dof = dof
 
+        id_def = reference.default_reference().sub_entity(*entity)
+
         f = parse_function_input(f_in)
-        f = f.subs(x, t)
+        self.f = f.subs(x, t)
 
-        if f.is_vector:
-            assert len(f) == self.integral_domain.tdim
-            self.f = mappings.contravariant(
-                f, integral_domain.get_map_to_self(), integral_domain.get_inverse_map_to_self(),
-                integral_domain.tdim)
-        elif f.is_matrix:
-            assert f.shape[0] == self.integral_domain.tdim
-            assert f.shape[1] == self.integral_domain.tdim
-            self.f = mappings.double_contravariant(
-                f, integral_domain.get_map_to_self(), integral_domain.get_inverse_map_to_self(),
-                integral_domain.tdim)
-        else:
-            self.f = f
+        # Map from reference entity to entity
+        if id_def.default_reference() != id_def:
+            if self.f.is_vector and len(self.f) != reference.gdim:
+                self.f = mappings.contravariant(
+                    self.f, id_def.get_map_to_self(),
+                    id_def.get_inverse_map_to_self(), id_def.tdim)
+            elif self.f.is_matrix:
+                assert self.f.shape[0] == id_def.tdim
+                assert self.f.shape[1] == id_def.tdim
+                self.f = mappings.double_contravariant(
+                    self.f, id_def.get_map_to_self(),
+                    id_def.get_inverse_map_to_self(), id_def.tdim)
+
+        # Map from default reference to reference
+        if map_function and reference != reference.default_reference():
+            if mapping is None or not hasattr(mappings, f"{mapping}_inverse_transpose"):
+                raise NonDefaultReferenceError()
+            mf = getattr(mappings, f"{mapping}_inverse_transpose")
+            self.f = mf(self.f, reference.get_map_to_self(),
+                        reference.get_inverse_map_to_self(),
+                        reference.tdim, substitute=False)
+            self.f *= id_def.volume() / self.integral_domain.volume()
 
     def _eval_symbolic(self, function: AnyFunction) -> AnyFunction:
         """Apply to the functional to a function.
 
         Args:
             function: The function
 
@@ -1143,14 +1218,18 @@
         """Get the direction of the DOF.
 
         Returns:
             The direction
         """
         p = self.dof.dof_direction()
         if p is None:
+            if self.f.is_vector:
+                p = (self.f.subs(t, self.dof_point())).as_sympy()
+                assert isinstance(p, tuple)
+                return p
             return None
         vp = VectorFunction(p)
         out = []
         for i in range(self.integral_domain.gdim):
             entry = vp.dot(VectorFunction([a[i] for a in self.integral_domain.axes])).as_sympy()
             assert isinstance(entry, sympy.core.expr.Expr)
             out.append(entry)
@@ -1160,20 +1239,21 @@
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
         entity = self.entity_tex()
         entity_def = self.entity_definition()
-        if isinstance(self.f, tuple):
+        if self.f.is_vector:
             if len(self.f) in [self.reference.tdim, self.integral_domain.tdim]:
                 desc = "\\boldsymbol{v}\\mapsto"
                 desc += f"\\displaystyle\\int_{{{entity}}}"
                 desc += "\\boldsymbol{v}\\cdot"
                 desc += "\\left(\\begin{array}{c}"
+                assert hasattr(self.f, "__iter__")
                 desc += "\\\\".join([_to_tex(i) for i in self.f])
                 desc += "\\end{array}\\right)"
             else:
                 if len(self.f) == self.integral_domain.tdim ** 2:
                     size = self.integral_domain.tdim
                 elif len(self.f) == self.reference.tdim ** 2:
                     size = self.reference.tdim
@@ -1194,94 +1274,31 @@
                 desc += "(" + _to_tex(self.f) + ")"
             desc += "v"
         return desc, [entity_def]
 
     name = "Integral moment"
 
 
-class VecIntegralMoment(IntegralMoment):
-    """An integral moment applied to a component of a vector."""
-
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
-                 dot_with_in: FunctionInput, dof: BaseFunctional, entity: typing.Tuple[int, int],
-                 mapping: typing.Union[str, None] = "identity"):
-        """Create the functional.
-
-        Args:
-            reference: The reference cell
-            integral_domain: The domain of the integral
-            f_in: The function to multiply with
-            dot_with_in: The vector to take the dot product with
-            dof: The DOF in a moment space that the function is associated with
-            entity: The entity the functional is associated with
-            mapping: The type of mappping from the reference cell to a physical cell
-        """
-        f = parse_function_input(f_in)
-        super().__init__(reference, integral_domain, f, dof, entity=entity, mapping=mapping)
-        self.dot_with = parse_function_input(dot_with_in)
-
-    def dot(self, function: AnyFunction) -> ScalarFunction:
-        """Dot a function with the moment function.
-
-        Args:
-            function: The function
-
-        Returns:
-            The product of the function and the moment function
-        """
-        return function.dot(self.dot_with) * self.f
-
-    def dof_direction(self) -> typing.Union[PointType, None]:
-        """Get the direction of the DOF.
-
-        Returns:
-            The direction
-        """
-        dw = self.dot_with.as_sympy()
-        if isinstance(dw, tuple):
-            return dw
-        return None
-
-    def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
-        """Get a representation of the functional as TeX, and list of terms involved.
-
-        Returns:
-            Representation of the functional as TeX, and list of terms involved
-        """
-        entity = self.entity_tex()
-        entity_def = self.entity_definition()
-        desc = "\\boldsymbol{v}\\mapsto"
-        desc += f"\\displaystyle\\int_{{{entity}}}"
-        if self.f != 1:
-            desc += "(" + _to_tex(self.f, True) + ")"
-        desc += "\\boldsymbol{v}\\cdot"
-        desc += _to_tex(self.dot_with)
-        return desc, [entity_def]
-
-    name = "Vector integral moment"
-
-
 class DerivativeIntegralMoment(IntegralMoment):
     """An integral moment of the derivative of a scalar function."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f: FunctionInput,
+    def __init__(self, reference: Reference, f: FunctionInput,
                  dot_with_in: FunctionInput, dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f: The function to multiply with
             dot_with_in: The vector to take the dot product with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
-        super().__init__(reference, integral_domain, f, dof, entity=entity, mapping=mapping)
+        super().__init__(reference, f, dof, entity=entity, mapping=mapping)
         self.dot_with = parse_function_input(dot_with_in)
 
     def dot(self, function: AnyFunction) -> ScalarFunction:
         """Dot a function with the moment function.
 
         Args:
             function: The function
@@ -1322,30 +1339,29 @@
 
     name = "Derivative integral moment"
 
 
 class DivergenceIntegralMoment(IntegralMoment):
     """An integral moment of the divergence of a vector function."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         f = parse_function_input(f_in)
         assert f.is_scalar
-        super().__init__(reference, integral_domain, f, dof, entity=entity, mapping=mapping)
+        super().__init__(reference, f, dof, entity=entity, mapping=mapping)
 
     def _eval_symbolic(self, function: AnyFunction) -> AnyFunction:
         """Apply to the functional to a function.
 
         Args:
             function: The function
 
@@ -1374,121 +1390,139 @@
             desc += "(" + _to_tex(self.f, True) + ")"
         desc += "\\nabla\\cdot\\boldsymbol{v}"
         return desc, [entity_def]
 
     name = "Integral moment of divergence"
 
 
-class TangentIntegralMoment(VecIntegralMoment):
+class TangentIntegralMoment(IntegralMoment):
     """An integral moment in the tangential direction."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "covariant"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
-        f = parse_function_input(f_in)
-        assert f.is_scalar
-        super().__init__(reference, integral_domain, f, integral_domain.tangent(), dof,
-                         entity=entity, mapping=mapping)
+        self._scalar_f = parse_function_input(f_in).subs(x, t)
+        integral_domain = reference.sub_entity(*entity)
+        assert self._scalar_f.is_scalar
+        super().__init__(
+            reference, tuple(self._scalar_f * i for i in integral_domain.tangent()), dof,
+            entity=entity, mapping=mapping, map_function=False)
+
+    def dof_direction(self) -> typing.Union[PointType, None]:
+        """Get the direction of the DOF.
+
+        Returns:
+            The direction
+        """
+        return self.integral_domain.tangent()
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
         entity = self.entity_tex()
         entity_n = self.entity_number()
         entity_def = self.entity_definition()
         desc = "\\boldsymbol{v}\\mapsto"
         desc += f"\\displaystyle\\int_{{{entity}}}"
         desc += "\\boldsymbol{v}\\cdot"
         if self.f != 1:
-            desc += "(" + _to_tex(self.f) + ")"
+            desc += "(" + _to_tex(self._scalar_f) + ")"
         desc += "\\hat{\\boldsymbol{t}}" + f"_{{{entity_n}}}"
         return desc, [
             entity_def,
             f"\\(\\hat{{\\boldsymbol{{t}}}}_{{{entity_n}}}\\) is the tangent to edge {entity_n}"
         ]
 
     name = "Tangential integral moment"
 
 
-class NormalIntegralMoment(VecIntegralMoment):
+class NormalIntegralMoment(IntegralMoment):
     """An integral moment in the normal direction."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "contravariant"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
-        f = parse_function_input(f_in)
-        assert f.is_scalar
-        super().__init__(reference, integral_domain, f, integral_domain.normal(), dof,
-                         entity=entity, mapping=mapping)
+        self._scalar_f = parse_function_input(f_in).subs(x, t)
+        assert self._scalar_f.is_scalar
+        integral_domain = reference.sub_entity(*entity)
+        super().__init__(
+            reference, tuple(self._scalar_f * i for i in integral_domain.normal()), dof,
+            entity=entity, mapping=mapping, map_function=False)
+
+    def dof_direction(self) -> typing.Union[PointType, None]:
+        """Get the direction of the DOF.
+
+        Returns:
+            The direction
+        """
+        return self.integral_domain.normal()
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
         """
         entity = self.entity_tex()
         entity_n = self.entity_number()
         entity_def = self.entity_definition()
         desc = "\\boldsymbol{v}\\mapsto"
         desc += f"\\displaystyle\\int_{{{entity}}}"
         desc += "\\boldsymbol{v}\\cdot"
         if self.f != 1:
-            desc += "(" + _to_tex(self.f, True) + ")"
+            desc += "(" + _to_tex(self._scalar_f, True) + ")"
         desc += "\\hat{\\boldsymbol{n}}" + f"_{{{entity_n}}}"
         return desc, [
             entity_def,
             f"\\(\\hat{{\\boldsymbol{{n}}}}_{{{entity_n}}}\\) is the normal to facet {entity_n}"
         ]
 
     name = "Normal integral moment"
 
 
 class NormalDerivativeIntegralMoment(DerivativeIntegralMoment):
     """An integral moment in the normal direction."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         f = parse_function_input(f_in)
         assert f.is_scalar
-        super().__init__(reference, integral_domain, f, integral_domain.normal(), dof,
+        integral_domain = reference.sub_entity(*entity)
+        super().__init__(reference, f, integral_domain.normal(), dof,
                          entity=entity, mapping=mapping)
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
@@ -1509,38 +1543,37 @@
 
     name = "Normal derivative integral moment"
 
 
 class InnerProductIntegralMoment(IntegralMoment):
     """An integral moment of the inner product with a vector."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  inner_with_left_in: FunctionInput, inner_with_right_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "identity"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             inner_with_left_in: The vector to multiply on the left
             inner_with_right_in: The vector to multiply on the right
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         f = parse_function_input(f_in)
         inner_with_left = parse_function_input(inner_with_left_in)
         inner_with_right = parse_function_input(inner_with_right_in)
         assert f.is_scalar
         assert inner_with_left.is_vector
         assert inner_with_right.is_vector
 
-        super().__init__(reference, integral_domain, f, dof, entity=entity, mapping=mapping)
+        super().__init__(reference, f, dof, entity=entity, mapping=mapping)
         self.inner_with_left = inner_with_left
         self.inner_with_right = inner_with_right
 
     def dot(self, function: AnyFunction) -> ScalarFunction:
         """Take the inner product of a function with the moment direction.
 
         Args:
@@ -1584,30 +1617,30 @@
 
     name = "Inner product integral moment"
 
 
 class NormalInnerProductIntegralMoment(InnerProductIntegralMoment):
     """An integral moment of the inner product with the normal direction."""
 
-    def __init__(self, reference: Reference, integral_domain: Reference, f_in: FunctionInput,
+    def __init__(self, reference: Reference, f_in: FunctionInput,
                  dof: BaseFunctional, entity: typing.Tuple[int, int],
                  mapping: typing.Union[str, None] = "double_contravariant"):
         """Create the functional.
 
         Args:
             reference: The reference cell
-            integral_domain: The domain of the integral
             f_in: The function to multiply with
             dof: The DOF in a moment space that the function is associated with
             entity: The entity the functional is associated with
             mapping: The type of mappping from the reference cell to a physical cell
         """
         f = parse_function_input(f_in)
         assert f.is_scalar
-        super().__init__(reference, integral_domain, f, integral_domain.normal(),
+        integral_domain = reference.sub_entity(*entity)
+        super().__init__(reference, f, integral_domain.normal(),
                          integral_domain.normal(), dof, entity=entity, mapping=mapping)
 
     def get_tex(self) -> typing.Tuple[str, typing.List[str]]:
         """Get a representation of the functional as TeX, and list of terms involved.
 
         Returns:
             Representation of the functional as TeX, and list of terms involved
```

### Comparing `symfem-2023.4.1/symfem/functions.py` & `symfem-2023.8.0/symfem/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 
 import sympy
 
+import symfem.references
+
 from .geometry import PointType
-from .references import Reference
 from .symbols import AxisVariables, AxisVariablesNotSingle, t, x
 
 SingleSympyFormat = typing.Union[
     sympy.core.expr.Expr,
     typing.Tuple[sympy.core.expr.Expr, ...],
     sympy.matrices.dense.MutableDenseMatrix
 ]
@@ -311,15 +312,15 @@
         Returns:
             The norm
         """
         pass
 
     @abstractmethod
     def integral(
-        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        self, domain: symfem.references.Reference, vars: AxisVariablesNotSingle = x,
         dummy_vars: AxisVariablesNotSingle = t
     ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
@@ -335,14 +336,18 @@
         """Return a version the function with floats as coefficients.
 
         Returns:
             A version the function with floats as coefficients
         """
         pass
 
+    def __iter__(self) -> typing.Iterator[AnyFunction]:
+        """Iterate through components of vector function."""
+        raise TypeError(f"'{self.__class__.__name__}' object is not iterable")
+
     def integrate(self, *limits: typing.Tuple[
         sympy.core.symbol.Symbol,
         typing.Union[int, sympy.core.expr.Expr],
         typing.Union[int, sympy.core.expr.Expr]
     ]):
         """Integrate the function.
 
@@ -376,15 +381,15 @@
 
         Returns:
             The value shape
         """
         raise AttributeError(f"'{self.__class__.__name__}' object has no attribute 'shape'")
 
     def plot(
-        self, reference: Reference, filename: typing.Union[str, typing.List[str]],
+        self, reference: symfem.references.Reference, filename: typing.Union[str, typing.List[str]],
         dof_point: typing.Optional[PointType] = None,
         dof_direction: typing.Optional[PointType] = None,
         dof_entity: typing.Optional[typing.Tuple[int, int]] = None,
         dof_n: typing.Optional[int] = None, value_scale: sympy.core.expr.Expr = sympy.Integer(1),
         plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
     ):
         """Plot the function.
@@ -439,15 +444,15 @@
                 elif dof_point is not None:
                     assert dof_n is not None
                     img.add_dof_marker(dof_point + extra, dof_n, colors.PURPLE, bold=False)
 
         img.save(filename, plot_options=plot_options)
 
     def plot_values(
-        self, reference: Reference, img: typing.Any,
+        self, reference: symfem.references.Reference, img: typing.Any,
         value_scale: sympy.core.expr.Expr = sympy.Integer(1), n: int = 6
     ):
         """Plot the function's values.
 
         Args:
             reference: The reference cell
             img: The image to plot on
@@ -521,15 +526,15 @@
         """
         super().__init__(scalar=True)
         if isinstance(f, int):
             self._f = sympy.Integer(f)
         else:
             self._f = f
         assert isinstance(self._f, sympy.core.expr.Expr)
-        self._plot_beziers: typing.Dict[typing.Tuple[Reference, int], typing.List[
+        self._plot_beziers: typing.Dict[typing.Tuple[symfem.references.Reference, int], typing.List[
             typing.Tuple[PointType, PointType, PointType, PointType]]] = {}
 
     def __add__(self, other: typing.Any) -> ScalarFunction:
         """Add."""
         if isinstance(other, ScalarFunction):
             return ScalarFunction(self._f + other._f)
         if isinstance(other, (int, sympy.core.expr.Expr)):
@@ -759,15 +764,15 @@
 
         Returns:
             The norm
         """
         return ScalarFunction(abs(self._f))
 
     def integral(
-        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        self, domain: symfem.references.Reference, vars: AxisVariablesNotSingle = x,
         dummy_vars: AxisVariablesNotSingle = t
     ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
@@ -805,15 +810,15 @@
 
         Returns:
             The integral
         """
         return ScalarFunction(self._f.integrate(*limits))
 
     def plot_values(
-        self, reference: Reference, img: typing.Any,
+        self, reference: symfem.references.Reference, img: typing.Any,
         value_scale: sympy.core.expr.Expr = sympy.Integer(1), n: int = 6
     ):
         """Plot the function's values.
 
         Args:
             reference: The reference cell
             img: The image to plot on
@@ -892,15 +897,15 @@
                 vec_l.append(i)
             else:
                 vec_l.append(ScalarFunction(i))
         self._vec = tuple(vec_l)
         for i in self._vec:
             assert i.is_scalar
 
-        self._plot_arrows: typing.Dict[typing.Tuple[Reference, int], typing.List[
+        self._plot_arrows: typing.Dict[typing.Tuple[symfem.references.Reference, int], typing.List[
             typing.Tuple[typing.Tuple[sympy.core.expr.Expr, ...], VectorFunction, float]]] = {}
 
     def __len__(self):
         """Get the length of the vector."""
         return len(self._vec)
 
     @property
@@ -1165,15 +1170,15 @@
         """
         a = sympy.Integer(0)
         for i in self._vec:
             a += i._f ** 2
         return ScalarFunction(sympy.sqrt(a))
 
     def integral(
-        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        self, domain: symfem.references.Reference, vars: AxisVariablesNotSingle = x,
         dummy_vars: AxisVariablesNotSingle = t
     ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
@@ -1194,15 +1199,15 @@
         if self.iter_n < len(self._vec):
             self.iter_n += 1
             return self._vec[self.iter_n - 1]
         else:
             raise StopIteration
 
     def plot_values(
-        self, reference: Reference, img: typing.Any,
+        self, reference: symfem.references.Reference, img: typing.Any,
         value_scale: sympy.core.expr.Expr = sympy.Integer(1), n: int = 6
     ):
         """Plot the function's values.
 
         Args:
             reference: The reference cell
             img: The image to plot on
@@ -1597,15 +1602,15 @@
 
         Returns:
             The norm
         """
         raise NotImplementedError()
 
     def integral(
-        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        self, domain: symfem.references.Reference, vars: AxisVariablesNotSingle = x,
         dummy_vars: AxisVariablesNotSingle = t
     ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
```

### Comparing `symfem-2023.4.1/symfem/geometry.py` & `symfem-2023.8.0/symfem/geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,33 @@
     """
     out = sympy.Integer(0)
     for i, j in zip(v, w):
         out += i * j
     return out
 
 
+def point_in_interval(point: PointType, interval: SetOfPoints) -> bool:
+    """Check if a point is inside an interval.
+
+    Args:
+        point: The point
+        interval: The vertices of the interval
+
+    Returns:
+        Is the point inside the interval?
+    """
+    v = _vsub(point, interval[0])[0] / _vsub(interval[1], interval[0])[0]
+
+    if isinstance(v, sympy.Float) and _is_close(v, 0):
+        v = sympy.Integer(0)
+    if isinstance(v, sympy.Float) and _is_close(v, 1):
+        v = sympy.Integer(1)
+    return 0 <= v <= 1
+
+
 def point_in_triangle(point: PointType, triangle: SetOfPoints) -> bool:
     """Check if a point is inside a triangle.
 
     Args:
         point: The point
         traingle: The vertices of the triangle
```

### Comparing `symfem-2023.4.1/symfem/moments.py` & `symfem-2023.8.0/symfem/moments.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,25 +80,27 @@
 
     # DOFs per dimension
     for dim, moment_data in [
         (0, vertices), (1, edges), (2, faces), (3, volumes),
         (reference.tdim - 3, peaks), (reference.tdim - 2, ridges), (reference.tdim - 1, facets),
         (reference.tdim, cells),
     ]:
-        if moment_data is not None:
-            sub_type = reference.sub_entity_types[dim]
-            if sub_type is not None:
-                assert dim > 0
-                for i, vs in enumerate(reference.sub_entities(dim)):
-                    sub_ref = reference.sub_entity(dim, i, True)
-                    IntegralMoment, SubElement, order, mapping, kwargs = _extract_moment_data(
-                        moment_data, sub_ref.name)
-                    if order >= SubElement.min_order:
-                        sub_element = SubElement(sub_ref.default_reference(), order, **kwargs)
-                        for dn, d in enumerate(sub_element.dofs):
-                            f = sub_element.get_basis_function(dn)
-                            kwargs = {}
-                            if mapping is not None:
-                                kwargs["mapping"] = mapping
-                            dofs.append(IntegralMoment(
-                                reference, sub_ref, f, d, (dim, i), **kwargs))
+        if moment_data is None:
+            continue
+        sub_type = reference.sub_entity_types[dim]
+        if sub_type is None:
+            continue
+        assert dim > 0
+        for i, vs in enumerate(reference.sub_entities(dim)):
+            sub_ref = reference.sub_entity(dim, i, False)
+            IntegralMoment, SubElement, order, mapping, kwargs = _extract_moment_data(
+                moment_data, sub_ref.name)
+            m_kwargs = {}
+            if mapping is not None:
+                m_kwargs["mapping"] = mapping
+            if order < SubElement.min_order:
+                continue
+            sub_element = SubElement(sub_ref.default_reference(), order, **kwargs)
+            for dn, d in enumerate(sub_element.dofs):
+                f = sub_element.get_basis_function(dn)
+                dofs.append(IntegralMoment(reference, f, d, (dim, i), **m_kwargs))
     return dofs
```

### Comparing `symfem-2023.4.1/symfem/piecewise_functions.py` & `symfem-2023.8.0/symfem/piecewise_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import typing
 
 import sympy
 
 from .functions import (AnyFunction, FunctionInput, ScalarFunction, SympyFormat, ValuesToSubstitute,
                         VectorFunction, _to_sympy_format, parse_function_input)
 from .geometry import (PointType, SetOfPoints, SetOfPointsInput, parse_set_of_points_input,
-                       point_in_quadrilateral, point_in_tetrahedron, point_in_triangle)
+                       point_in_interval, point_in_quadrilateral, point_in_tetrahedron,
+                       point_in_triangle)
 from .references import Reference
 from .symbols import AxisVariables, AxisVariablesNotSingle, t, x
 
 
 class PiecewiseFunction(AnyFunction):
     """A piecewise function."""
 
@@ -109,14 +110,18 @@
 
         Args:
             point: The point to get the piece at
 
         Returns:
             The piece of the function that is valid at that point
         """
+        if self.tdim == 1:
+            for cell, value in self._pieces.items():
+                if point_in_interval(point[:1], cell):
+                    return value
         if self.tdim == 2:
             for cell, value in self._pieces.items():
                 if len(cell) == 3:
                     if point_in_triangle(point[:2], cell):
                         return value
                 elif len(cell) == 4:
                     if point_in_quadrilateral(point[:2], cell):
```

### Comparing `symfem-2023.4.1/symfem/plotting.py` & `symfem-2023.8.0/symfem/plotting.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/symfem/quadrature.py` & `symfem-2023.8.0/symfem/quadrature.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/symfem/references.py` & `symfem-2023.8.0/symfem/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,34 @@
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 
 import sympy
 
+import symfem.functions
+
 from .geometry import (PointType, PointTypeInput, SetOfPoints, SetOfPointsInput, parse_point_input,
                        parse_set_of_points_input)
 from .symbols import AxisVariablesNotSingle, t, x
 
 LatticeWithLines = typing.Tuple[SetOfPoints, typing.List[typing.Tuple[int, int]]]
 IntLimits = typing.List[typing.Union[
     typing.Tuple[sympy.core.symbol.Symbol, sympy.core.expr.Expr, sympy.core.expr.Expr],
     typing.Tuple[sympy.core.symbol.Symbol, sympy.core.expr.Expr]]]
 
 
+class NonDefaultReferenceError(NotImplementedError):
+    """Exception to be thrown when an element can only be created on the default reference."""
+
+    def __init__(self):
+        """Initialise the exception."""
+        super().__init__("Cannot create this element on a non-default reference")
+
+
 def _which_side(vs: SetOfPoints, p: PointType, q: PointType) -> typing.Optional[int]:
     """Check which side of a line or plane a set of points are.
 
     Args:
         vs: The set of points
         p: A point on the line or plane
         q: Another point on the line (2D) or the normal to the plane (3D)
@@ -144,15 +154,23 @@
     n = _vnorm(v)
     return tuple(i / n for i in v)
 
 
 class Reference(ABC):
     """A reference cell on which a finite element can be defined."""
 
-    def __init__(
+    @abstractmethod
+    def __init__(self, vertices: SetOfPointsInput = ()):
+        """Create a reference.
+
+        Args:
+            vertices: The vertices of the point.
+        """
+
+    def __build__(
         self, tdim: int, name: str, origin: PointTypeInput, axes: SetOfPointsInput,
         reference_vertices: SetOfPointsInput, vertices: SetOfPointsInput,
         edges: typing.Tuple[typing.Tuple[int, int], ...],
         faces: typing.Tuple[typing.Tuple[int, ...], ...],
         volumes: typing.Tuple[typing.Tuple[int, ...], ...],
         sub_entity_types: typing.List[typing.Union[typing.List[str], str, None]],
         simplex: bool = False, tp: bool = False
@@ -194,14 +212,24 @@
         """Get list of vertices in clockwise order.
 
         Returns:
             A list of vertices
         """
         return self.vertices
 
+    def __eq__(self, other: object) -> bool:
+        """Check if two references are equal."""
+        if not isinstance(other, Reference):
+            return False
+        return type(self) is type(other) and self.vertices == other.vertices
+
+    def __hash__(self) -> int:
+        """Check if two references are equal."""
+        return hash((self.reference_vertices, self.vertices))
+
     def intersection(self, other: Reference) -> typing.Optional[Reference]:
         """Get the intersection of two references.
 
         Returns:
             A reference element that is the intersection
         """
         if self.gdim != other.gdim:
@@ -240,40 +268,37 @@
     @abstractmethod
     def default_reference(self) -> Reference:
         """Get the default reference for this cell type.
 
         Returns:
             The default reference
         """
-        pass
 
     @abstractmethod
     def make_lattice(self, n: int) -> SetOfPoints:
         """Make a lattice of points.
 
         Args:
             n: The number of points along each edge
 
         Returns:
             A lattice of points offset from the edge of the cell
         """
-        pass
 
     @abstractmethod
     def make_lattice_with_lines(self, n: int) -> LatticeWithLines:
         """Make a lattice of points, and a list of lines connecting them.
 
         Args:
             n: The number of points along each edge
 
         Returns:
             A lattice of points including the edges of the cell
             Pairs of point numbers that make a mesh of lines across the cell
         """
-        pass
 
     def make_lattice_float(self, n: int) -> SetOfPoints:
         """Make a lattice of points.
 
         Args:
             n: The number of points along each edge
 
@@ -333,39 +358,36 @@
 
         Args:
             vars: The variables to use for each direction
 
         Returns:
             Integration limits that can be passed into sympy.integrate
         """
-        pass
 
     @abstractmethod
     def get_map_to(self, vertices: SetOfPointsInput) -> PointType:
         """Get the map from the reference to a cell.
 
         Args:
             vertices: The vertices of a call
 
         Returns:
             The map
         """
-        pass
 
     @abstractmethod
     def get_inverse_map_to(self, vertices_in: SetOfPointsInput) -> PointType:
         """Get the inverse map from a cell to the reference.
 
         Args:
             vertices_in: The vertices of a cell
 
         Returns:
             The inverse map
         """
-        pass
 
     def get_map_to_self(self) -> PointType:
         """Get the map from the canonical reference to this reference.
 
         Returns:
             The map
         """
@@ -377,15 +399,14 @@
     @abstractmethod
     def _compute_map_to_self(self) -> PointType:
         """Compute the map from the canonical reference to this reference.
 
         Returns:
             The map
         """
-        pass
 
     def get_inverse_map_to_self(self) -> PointType:
         """Get the inverse map from the canonical reference to this reference.
 
         Returns:
             The map
         """
@@ -397,24 +418,22 @@
     @abstractmethod
     def _compute_inverse_map_to_self(self) -> PointType:
         """Compute the inverse map from the canonical reference to this reference.
 
         Returns:
             The map
         """
-        pass
 
     @abstractmethod
     def volume(self) -> sympy.core.expr.Expr:
         """Calculate the volume.
 
         Returns:
             The volume of the cell
         """
-        pass
 
     def midpoint(self) -> PointType:
         """Calculate the midpoint.
 
         Returns:
             The midpoint of the cell
         """
@@ -603,15 +622,25 @@
 
         Args:
             point: The point
 
         Returns:
             Is the point contained in the reference?
         """
-        pass
+
+    def map_polyset_from_default(
+        self, poly: typing.List[symfem.functions.FunctionInput]
+    ) -> typing.List[symfem.functions.FunctionInput]:
+        """Map the polynomials from the default reference element to this reference."""
+        from .functions import parse_function_input
+
+        if self == self.default_reference():
+            return poly
+        invmap = self.get_inverse_map_to_self()
+        return [parse_function_input(p).subs(x, invmap) for p in poly]
 
     def plot_entity_diagrams(
         self, filename: typing.Union[str, typing.List[str]],
         plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
     ):
         """Plot diagrams showing the entity numbering of the reference."""
         from .plotting import Picture, colors
@@ -684,15 +713,15 @@
     def __init__(self, vertices: SetOfPointsInput = ((), )):
         """Create a point.
 
         Args:
             vertices: The vertices of the point.
         """
         assert len(vertices) == 1
-        super().__init__(
+        super().__build__(
             tdim=0,
             name="point",
             origin=vertices[0],
             axes=(),
             reference_vertices=((), ),
             vertices=vertices,
             edges=(),
@@ -811,15 +840,15 @@
     def __init__(self, vertices: SetOfPointsInput = ((0,), (1,))):
         """Create an interval.
 
         Args:
             vertices: The vertices of the interval.
         """
         assert len(vertices) == 2
-        super().__init__(
+        super().__build__(
             tdim=1,
             name="interval",
             origin=vertices[0],
             axes=(_vsub(vertices[1], vertices[0]),),
             reference_vertices=((0,), (1,)),
             vertices=vertices,
             edges=((0, 1),),
@@ -947,15 +976,15 @@
     def __init__(self, vertices: SetOfPointsInput = ((0, 0), (1, 0), (0, 1))):
         """Create a triangle.
 
         Args:
             vertices: The vertices of the triangle.
         """
         assert len(vertices) == 3
-        super().__init__(
+        super().__build__(
             tdim=2,
             name="triangle",
             origin=vertices[0],
             axes=(_vsub(vertices[1], vertices[0]), _vsub(vertices[2], vertices[0])),
             reference_vertices=((0, 0), (1, 0), (0, 1)),
             vertices=vertices,
             edges=((1, 2), (0, 2), (0, 1)),
@@ -1113,31 +1142,29 @@
         if self.vertices == self.reference_vertices:
             return 0 <= point[0] and 0 <= point[1] and sum(point) <= 1
         elif self.gdim == 2:
             po = _vsub(point, self.origin)
             det = self.axes[0][0] * self.axes[1][1] - self.axes[0][1] * self.axes[1][0]
             t0 = (self.axes[1][1] * po[0] - self.axes[1][0] * po[1]) / det
             t1 = (self.axes[0][0] * po[1] - self.axes[0][1] * po[0]) / det
-            print(self.origin, self.axes, point)
-            print(t0, t1)
             return 0 <= t0 and 0 <= t1 and t0 + t1 <= 1
         raise NotImplementedError()
 
 
 class Tetrahedron(Reference):
     """A tetrahedron."""
 
     def __init__(self, vertices: SetOfPointsInput = ((0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1))):
         """Create a tetrahedron.
 
         Args:
             vertices: The vertices of the tetrahedron.
         """
         assert len(vertices) == 4
-        super().__init__(
+        super().__build__(
             tdim=3,
             name="tetrahedron",
             origin=vertices[0],
             axes=(
                 _vsub(vertices[1], vertices[0]),
                 _vsub(vertices[2], vertices[0]),
                 _vsub(vertices[3], vertices[0]),
@@ -1310,15 +1337,15 @@
     def __init__(self, vertices: SetOfPointsInput = ((0, 0), (1, 0), (0, 1), (1, 1))):
         """Create a quadrilateral.
 
         Args:
             vertices: The vertices of the quadrilateral.
         """
         assert len(vertices) == 4
-        super().__init__(
+        super().__build__(
             tdim=2,
             name="quadrilateral",
             origin=vertices[0],
             axes=(_vsub(vertices[1], vertices[0]), _vsub(vertices[2], vertices[0])),
             reference_vertices=((0, 0), (1, 0), (0, 1), (1, 1)),
             vertices=vertices,
             edges=((0, 1), (0, 2), (1, 3), (2, 3)),
@@ -1512,15 +1539,15 @@
     ):
         """Create a hexahedron.
 
         Args:
             vertices: The vertices of the hexahedron.
         """
         assert len(vertices) == 8
-        super().__init__(
+        super().__build__(
             tdim=3,
             name="hexahedron",
             origin=vertices[0],
             axes=(
                 _vsub(vertices[1], vertices[0]),
                 _vsub(vertices[2], vertices[0]),
                 _vsub(vertices[4], vertices[0]),
@@ -1714,15 +1741,15 @@
     ):
         """Create a prism.
 
         Args:
             vertices: The vertices of the prism.
         """
         assert len(vertices) == 6
-        super().__init__(
+        super().__build__(
             tdim=3,
             name="prism",
             origin=vertices[0],
             axes=(
                 _vsub(vertices[1], vertices[0]),
                 _vsub(vertices[2], vertices[0]),
                 _vsub(vertices[3], vertices[0]),
@@ -1916,15 +1943,15 @@
     ):
         """Create a pyramid.
 
         Args:
             vertices: The vertices of the pyramid.
         """
         assert len(vertices) == 5
-        super().__init__(
+        super().__build__(
             tdim=3,
             name="pyramid",
             origin=vertices[0],
             axes=(
                 _vsub(vertices[1], vertices[0]),
                 _vsub(vertices[2], vertices[0]),
                 _vsub(vertices[4], vertices[0]),
@@ -2138,15 +2165,15 @@
         if vertices is None:
             vertices = tuple(reference_vertices)
         else:
             assert len(vertices) == 1 + len(reference_vertices)
             origin = parse_point_input(vertices[0])
             vertices = vertices[1:]
 
-        super().__init__(
+        super().__build__(
             tdim=2,
             name="dual polygon",
             axes=(),
             origin=origin,
             vertices=vertices,
             reference_vertices=tuple(reference_vertices),
             edges=tuple((i, (i + 1) % (2 * number_of_triangles))
```

### Comparing `symfem-2023.4.1/symfem/utils.py` & `symfem-2023.8.0/symfem/utils.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/symfem.egg-info/PKG-INFO` & `symfem-2023.8.0/symfem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symfem
-Version: 2023.4.1
+Version: 2023.8.0
 Summary: a symbolic finite element definition library
 Home-page: https://github.com/mscroggs/symfem
 Author: Matthew Scroggs
 Author-email: symfem@mscroggs.co.uk
 Maintainer-email: symfem@mscroggs.co.uk
 License: MIT
 Description-Content-Type: text/markdown
@@ -160,25 +160,27 @@
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
 - enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
+- P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
 
 ## Triangle
 The reference triangle has vertices (0, 0), (1, 0), and (0, 1). Its sub-entities are numbered as follows.
 
 ![The numbering of a reference triangle](https://raw.githubusercontent.com/mscroggs/symfem/main/img/triangle_numbering.png)
 
 ### List of supported elements
+- Alfeld-Sorokina (alternative names: AS)
 - Argyris
 - Arnold-Winther (alternative names: AW, conforming Arnold-Winther)
 - Bell
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
@@ -199,14 +201,15 @@
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley
 - Morley-Wang-Xu (alternative names: MWX)
 - Nedelec (alternative names: Nedelec1, N1curl)
 - Nedelec2 (alternative names: N2curl)
 - nonconforming Arnold-Winther (alternative names: nonconforming AW)
+- P1 macro
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Raviart-Thomas (alternative names: RT, N1div)
 - reduced Hsieh-Clough-Tocher (alternative names: rHCT)
 - Regge
 - symmetric matrix Lagrange
 - Taylor (alternative names: discontinuous Taylor)
 - transition
```

### Comparing `symfem-2023.4.1/symfem.egg-info/SOURCES.txt` & `symfem-2023.8.0/symfem.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 symfem/__init__.py
 symfem/basis_functions.py
+symfem/caching.py
 symfem/create.py
 symfem/finite_element.py
 symfem/functionals.py
 symfem/functions.py
 symfem/geometry.py
 symfem/mappings.py
 symfem/moments.py
 symfem/piecewise_functions.py
 symfem/plotting.py
-symfem/polynomials.py
 symfem/quadrature.py
 symfem/references.py
 symfem/symbols.py
 symfem/utils.py
 symfem/version.py
 symfem.egg-info/PKG-INFO
 symfem.egg-info/SOURCES.txt
@@ -25,14 +25,15 @@
 symfem.egg-info/requires.txt
 symfem.egg-info/top_level.txt
 symfem/elements/__init__.py
 symfem/elements/_guzman_neilan_tetrahedron.py
 symfem/elements/_guzman_neilan_triangle.py
 symfem/elements/abf.py
 symfem/elements/ac.py
+symfem/elements/alfeld_sorokina.py
 symfem/elements/argyris.py
 symfem/elements/aw.py
 symfem/elements/bddm.py
 symfem/elements/bdfm.py
 symfem/elements/bdm.py
 symfem/elements/bell.py
 symfem/elements/bernardi_raugel.py
@@ -57,38 +58,49 @@
 symfem/elements/lagrange_pyramid.py
 symfem/elements/morley.py
 symfem/elements/morley_wang_xu.py
 symfem/elements/mtw.py
 symfem/elements/nedelec.py
 symfem/elements/nedelec_prism.py
 symfem/elements/p1_iso_p2.py
+symfem/elements/p1_macro.py
 symfem/elements/q.py
 symfem/elements/rannacher_turek.py
 symfem/elements/regge.py
 symfem/elements/rhct.py
 symfem/elements/rt.py
 symfem/elements/serendipity.py
 symfem/elements/taylor.py
 symfem/elements/tnt.py
 symfem/elements/transition.py
 symfem/elements/trimmed_serendipity.py
 symfem/elements/vector_enriched_galerkin.py
 symfem/elements/wu_xu.py
+symfem/polynomials/__init__.py
+symfem/polynomials/dual.py
+symfem/polynomials/legendre.py
+symfem/polynomials/lobatto.py
+symfem/polynomials/polysets.py
 test/__init__.py
 test/conftest.py
 test/test_against_basix.py
 test/test_against_computed_by_hand.py
+test/test_alfeld_sorokina.py
 test/test_arnold_winther.py
+test/test_bell.py
 test/test_bernstein.py
+test/test_caching.py
 test/test_docs.py
 test/test_dof_descriptions.py
 test/test_elements.py
 test/test_functions.py
 test/test_guzman_neilan.py
 test/test_hct.py
+test/test_lagrange_polynomial_variants.py
+test/test_mapping.py
 test/test_nedelec.py
 test/test_p1_iso_p2.py
 test/test_plotting.py
 test/test_polynomials.py
 test/test_quadrature.py
 test/test_references.py
 test/test_reorder.py
```

### Comparing `symfem-2023.4.1/test/conftest.py` & `symfem-2023.8.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_against_basix.py` & `symfem-2023.8.0/test/test_against_basix.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_against_computed_by_hand.py` & `symfem-2023.8.0/test/test_against_computed_by_hand.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_bernstein.py` & `symfem-2023.8.0/test/test_bernstein.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_docs.py` & `symfem-2023.8.0/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_dof_descriptions.py` & `symfem-2023.8.0/test/test_dof_descriptions.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_elements.py` & `symfem-2023.8.0/test/test_elements.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_functions.py` & `symfem-2023.8.0/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_guzman_neilan.py` & `symfem-2023.8.0/test/test_guzman_neilan.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_hct.py` & `symfem-2023.8.0/test/test_hct.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,67 @@
 """Test Hsieh-Clough-Tocher elements."""
 
+import pytest
 import sympy
 
 import symfem
+from symfem.functions import ScalarFunction
 from symfem.symbols import t, x
 from symfem.utils import allequal
 
 half = sympy.Rational(1, 2)
 
 
-def test_hct():
-    e = symfem.create_element("triangle", "HCT", 3)
+@pytest.mark.parametrize("family", ["HCT", "rHCT"])
+def test_c1_continuity(family):
+    e = symfem.create_element("triangle", family, 3)
     for f in e.get_polynomial_basis():
         # edge from (1,0) to (1/3,1/3)
         f1 = f.get_piece((half, 0))
         f2 = f.get_piece((half, half))
+        grad_f1 = f1.grad(2)
+        grad_f2 = f2.grad(2)
         line = ((1 - 2 * t[0], t[0]))
         f1 = f1.subs(x[:2], line)
         f2 = f2.subs(x[:2], line)
+        grad_f1 = grad_f1.subs(x[:2], line)
+        grad_f2 = grad_f2.subs(x[:2], line)
         assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
+        assert allequal(grad_f1, grad_f2)
 
         # edge from (0,1) to (1/3,1/3)
         f1 = f.get_piece((half, half))
         f2 = f.get_piece((0, half))
+        grad_f1 = f1.grad(2)
+        grad_f2 = f2.grad(2)
         line = ((t[0], 1 - 2 * t[0]))
         f1 = f1.subs(x[:2], line)
         f2 = f2.subs(x[:2], line)
+        grad_f1 = grad_f1.subs(x[:2], line)
+        grad_f2 = grad_f2.subs(x[:2], line)
         assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
+        assert allequal(grad_f1, grad_f2)
 
         # edge from (0,0) to (1/3,1/3)
         f1 = f.get_piece((0, half))
         f2 = f.get_piece((half, 0))
+        grad_f1 = f1.grad(2)
+        grad_f2 = f2.grad(2)
         line = ((t[0], t[0]))
         f1 = f1.subs(x[:2], line)
         f2 = f2.subs(x[:2], line)
+        grad_f1 = grad_f1.subs(x[:2], line)
+        grad_f2 = grad_f2.subs(x[:2], line)
         assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
+        assert allequal(grad_f1, grad_f2)
 
 
-def test_rhct():
+def test_rcht_linear_normal_derivatices():
     e = symfem.create_element("triangle", "rHCT", 3)
     for f in e.get_polynomial_basis():
-        # edge from (1,0) to (1/3,1/3)
-        f1 = f.get_piece((half, 0))
-        f2 = f.get_piece((half, half))
-        line = ((1 - 2 * t[0], t[0]))
-        f1 = f1.subs(x[:2], line)
-        f2 = f2.subs(x[:2], line)
-        assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
-
-        # edge from (0,1) to (1/3,1/3)
-        f1 = f.get_piece((half, half))
-        f2 = f.get_piece((0, half))
-        line = ((t[0], 1 - 2 * t[0]))
-        f1 = f1.subs(x[:2], line)
-        f2 = f2.subs(x[:2], line)
-        assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
-
-        # edge from (0,0) to (1/3,1/3)
-        f1 = f.get_piece((0, half))
-        f2 = f.get_piece((half, 0))
-        line = ((t[0], t[0]))
-        f1 = f1.subs(x[:2], line)
-        f2 = f2.subs(x[:2], line)
-        assert allequal(f1, f2)
-        assert allequal(f1.grad(2), f2.grad(2))
-
         # Check that normal derivatives are linear
         f1 = f.get_piece((half, 0)).diff(x[1]).subs(x[1], 0)
         f2 = f.get_piece((half, half))
         f2 = (f2.diff(x[0]) + f2.diff(x[1])).subs(x[1], 1 - x[0])
         f3 = f.get_piece((0, half)).diff(x[0]).subs(x[0], 0)
         assert f1.diff(x[0]).diff(x[0]) == 0
         assert f2.diff(x[0]).diff(x[0]) == 0
@@ -81,17 +69,18 @@
 
 
 def test_rhct_integral():
     element = symfem.create_element("triangle", "rHCT", 3)
     ref = element.reference
     f1 = element.get_basis_function(1).directional_derivative((1, 0))
     f2 = element.get_basis_function(6).directional_derivative((1, 0))
-    integrand = f1 * f2
 
+    integrand = f1 * f2
     third = sympy.Rational(1, 3)
-    expr = (f1*f2).pieces[((0, 1), (0, 0), (third, third))].as_sympy()
-    assert len((f1*f2).pieces) == 3
-    assert (f1*f2).pieces[((0, 0), (1, 0), (third, third))] == 0
-    assert (f1*f2).pieces[((1, 0), (0, 1), (third, third))] == 0
+    integrand.pieces[((0, 0), (1, 0), (third, third))] = ScalarFunction(0)
+    integrand.pieces[((1, 0), (0, 1), (third, third))] = ScalarFunction(0)
+
+    expr = integrand.pieces[((0, 1), (0, 0), (third, third))].as_sympy()
+    assert len(integrand.pieces) == 3
 
     assert sympy.integrate(sympy.integrate(
         expr, (x[1], x[0], 1 - 2 * x[0])), (x[0], 0, third)) == integrand.integral(ref, x)
```

### Comparing `symfem-2023.4.1/test/test_nedelec.py` & `symfem-2023.8.0/test/test_nedelec.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_p1_iso_p2.py` & `symfem-2023.8.0/test/test_p1_iso_p2.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_plotting.py` & `symfem-2023.8.0/test/test_plotting.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_polynomials.py` & `symfem-2023.8.0/test/test_polynomials.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from random import choice
 
 import pytest
 import sympy
 
 from symfem import create_element, create_reference
 from symfem.functions import VectorFunction
-from symfem.polynomials import (Hcurl_polynomials, Hdiv_polynomials, orthogonal_basis,
+from symfem.polynomials import (Hcurl_polynomials, Hdiv_polynomials, l2_dual, orthogonal_basis,
                                 orthonormal_basis)
 from symfem.symbols import t, x
 
 
 @pytest.mark.parametrize("reference", ["triangle", "tetrahedron"])
 @pytest.mark.parametrize("order", range(1, 4))
 def test_Hdiv_space(reference, order):
@@ -132,7 +132,21 @@
     if speed == "fast" and order > 2:
         pytest.skip()
 
     polynomials = orthonormal_basis(reference, order, 0)[0]
     ref = create_reference(reference)
     for p in polynomials:
         assert (p ** 2).integral(ref, x) == 1
+
+
+@pytest.mark.parametrize("reference, order", [
+    (r, o) for r, m in [("interval", 6), ("triangle", 3), ("quadrilateral", 3),
+                        ("tetrahedron", 2), ("hexahedron", 2), ("prism", 2),
+                        ("pyramid", 2)] for o in range(m)])
+def test_dual(reference, order):
+    ref = create_reference(reference)
+    poly = create_element(reference, "P", order).get_polynomial_basis()
+    dual = l2_dual(reference, poly)
+
+    for i, p in enumerate(poly):
+        for j, d in enumerate(dual):
+            assert (p * d).integrate(*ref.integration_limits(x)) == (1 if i == j else 0)
```

### Comparing `symfem-2023.4.1/test/test_quadrature.py` & `symfem-2023.8.0/test/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_references.py` & `symfem-2023.8.0/test/test_references.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_reorder.py` & `symfem-2023.8.0/test/test_reorder.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_stiffness_matrix.py` & `symfem-2023.8.0/test/test_stiffness_matrix.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/test_tensor_product.py` & `symfem-2023.8.0/test/test_tensor_product.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.4.1/test/utils.py` & `symfem-2023.8.0/test/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 import typing
 
 test_elements: typing.Dict[str, typing.Dict[
     str,
     typing.List[typing.Tuple[typing.Dict[str, typing.Any], typing.Iterable]]
 ]] = {
     "interval": {
-        "P": [({"variant": "equispaced"}, range(6)), ({"variant": "lobatto"}, range(4))],
+        "P": [({"variant": "equispaced"}, range(6)), ({"variant": "lobatto"}, range(4)),
+              ({"variant": "legendre"}, range(5))],
         "vP": [({"variant": "equispaced"}, range(6)), ({"variant": "lobatto"}, range(3)),
                ({"variant": "radau"}, range(3)), ({"variant": "legendre"}, range(3))],
         "dPc": [({"variant": "equispaced"}, range(6)), ({"variant": "lobatto"}, range(4))],
         "bubble": [({"variant": "equispaced"}, range(2, 6)),
                    ({"variant": "lobatto"}, range(2, 3))],
         "serendipity": [({"variant": "equispaced"}, range(1, 6)),
                         ({"variant": "lobatto"}, range(1, 3))],
         "Hermite": [({}, [3])],
         "Bernstein": [({}, range(1, 4))],
         "Taylor": [({}, range(0, 5))],
         "Wu-Xu": [({}, [2])],
         "MWX": [({}, [1])],
         "EG": [({}, range(1, 5))],
+        "P1-iso-P2": [({}, [1])],
     },
     "triangle": {
-        "P": [({"variant": "equispaced"}, range(5)), ({"variant": "lobatto"}, range(3))],
-        "vP": [({"variant": "equispaced"}, range(5)), ({"variant": "lobatto"}, range(3))],
-        "matrix Lagrange": [({"variant": "equispaced"}, range(3)),
-                            ({"variant": "lobatto"}, range(3))],
+        "P": [({"variant": "equispaced"}, range(5))],
+        "vP": [({"variant": "equispaced"}, range(5))],
+        "matrix Lagrange": [({"variant": "equispaced"}, range(3))],
         "symmetric matrix Lagrange": [
-            ({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
-        "bubble": [({"variant": "equispaced"}, range(3, 5)), ({"variant": "lobatto"}, range(3, 3))],
-        "bubble enriched Lagrange": [({"variant": "equispaced"}, range(1, 3)),
-                                     ({"variant": "lobatto"}, range(1, 3))],
+            ({"variant": "equispaced"}, range(3))],
+        "bubble": [({"variant": "equispaced"}, range(3, 5))],
+        "bubble enriched Lagrange": [({"variant": "equispaced"}, range(1, 3))],
         "bubble enriched vector Lagrange":
-            [({"variant": "equispaced"}, range(1, 3)), ({"variant": "lobatto"}, range(1, 3))],
+            [({"variant": "equispaced"}, range(1, 3))],
         "CR": [({"variant": "equispaced"}, [1, 3, 5])],
         "conforming CR": [({}, range(1, 6))],
         "HHJ": [({"variant": "equispaced"}, range(3))],
         "Bell": [({"variant": "equispaced"}, [5])],
         "Morley": [({}, [2])],
         "MWX": [({}, [1, 2])],
         "Regge": [({"variant": "point"}, range(4)), ({"variant": "integral"}, range(3))],
@@ -59,28 +59,27 @@
         "Taylor": [({}, range(0, 5))],
         "Bernardi-Raugel": [({}, [1])],
         "Guzman-Neilan": [({}, [1])],
         "Wu-Xu": [({}, [3])],
         "transition": [({"edge_orders": [1, 1, 1], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [2, 2, 1], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [3, 3, 1], "variant": "equispaced"}, range(1, 6)),
-                       ({"edge_orders": [3, 3, 2], "variant": "equispaced"}, range(1, 6)),
-                       ({"edge_orders": [2, 2, 1], "variant": "lobatto"}, range(1, 3))],
+                       ({"edge_orders": [3, 3, 2], "variant": "equispaced"}, range(1, 6))],
         "P1-iso-P2": [({}, [1])],
         "EG": [({}, range(1, 4))],
         "LFEG": [({}, range(1, 4))],
+        "Alfeld-Sorokina": [({}, [2])],
+        "P1 macro": [({}, [1])],
     },
     "tetrahedron": {
-        "P": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
-        "vP": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
-        "matrix Lagrange": [({"variant": "equispaced"}, range(2)),
-                            ({"variant": "lobatto"}, range(3))],
-        "symmetric matrix Lagrange": [({"variant": "equispaced"}, range(2)),
-                                      ({"variant": "lobatto"}, range(3))],
-        "bubble": [({"variant": "equispaced"}, [4]), ({"variant": "lobatto"}, [4])],
+        "P": [({"variant": "equispaced"}, range(3))],
+        "vP": [({"variant": "equispaced"}, range(3))],
+        "matrix Lagrange": [({"variant": "equispaced"}, range(2))],
+        "symmetric matrix Lagrange": [({"variant": "equispaced"}, range(2))],
+        "bubble": [({"variant": "equispaced"}, [4])],
         "CR": [({"variant": "equispaced"}, [1])],
         "Regge": [({"variant": "point"}, range(3)), ({"variant": "integral"}, range(2))],
         "Nedelec1": [({"variant": "equispaced"}, range(1, 3))],
         "Nedelec2": [({"variant": "equispaced"}, range(1, 3))],
         "RT": [({"variant": "equispaced"}, range(1, 3))],
         "BDFM": [({"variant": "equispaced"}, range(1, 3))],
         "MTW": [({"variant": "equispaced"}, [3])],
```

