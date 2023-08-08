# Comparing `tmp/nzpyida-0.9.3.tar.gz` & `tmp/nzpyida-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.9.3.tar", last modified: Fri Jul 21 14:43:24 2023, max compression
+gzip compressed data, was "nzpyida-0.9.4.tar", last modified: Tue Aug  8 11:08:16 2023, max compression
```

## Comparing `nzpyida-0.9.3.tar` & `nzpyida-0.9.4.tar`

### file list

```diff
@@ -1,163 +1,165 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.209856 nzpyida-0.9.3/
--rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.3/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.3/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      221 2023-07-21 14:42:45.000000 nzpyida-0.9.3/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-21 14:43:24.209985 nzpyida-0.9.3/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.3/README.md
--rw-r--r--   0 mpl        (501) staff       (20)        6 2023-07-21 14:42:45.000000 nzpyida-0.9.3/VERSION
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.186019 nzpyida-0.9.3/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.3/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.188608 nzpyida-0.9.3/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    12029 2023-07-21 10:38:04.000000 nzpyida-0.9.3/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2500 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geo_frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3560 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geo_series.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3638 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4059 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-21 10:38:04.000000 nzpyida-0.9.3/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.3/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23915 2023-07-21 14:42:45.000000 nzpyida-0.9.3/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.3/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.191058 nzpyida-0.9.3/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)     1016 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.193287 nzpyida-0.9.3/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.194949 nzpyida-0.9.3/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.195141 nzpyida-0.9.3/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.195853 nzpyida-0.9.3/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.3/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.3/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.196346 nzpyida-0.9.3/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9129 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    33218 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.198935 nzpyida-0.9.3/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13090 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    29037 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)    11574 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     8585 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10059 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     9562 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/glm.py
--rw-r--r--   0 mpl        (501) staff       (20)    10976 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9665 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5637 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6069 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6285 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5767 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8390 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     8909 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)    12793 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.201843 nzpyida-0.9.3/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     3588 2023-07-06 15:07:05.000000 nzpyida-0.9.3/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3621 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     6796 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_bayesian_networks.py
--rw-r--r--   0 mpl        (501) staff       (20)     2435 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2086 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_cross_validation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2835 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2683 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     4054 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_glm.py
--rw-r--r--   0 mpl        (501) staff       (20)     2303 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2747 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2542 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3503 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2771 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     3067 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2494 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    22367 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-07-20 08:34:06.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_timeseries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2457 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.202305 nzpyida-0.9.3/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10647 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)    11017 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5942 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93635 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.204038 nzpyida-0.9.3/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.3/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90409 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)    37116 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/geo_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)    66784 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/geo_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18287 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.205429 nzpyida-0.9.3/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-07-14 08:41:35.000000 nzpyida-0.9.3/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.3/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.3/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.209682 nzpyida-0.9.3/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13644 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8685 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6758 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9694 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-07-19 07:48:15.000000 nzpyida-0.9.3/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15148 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)     9173 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/test_geo_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     8966 2023-07-21 14:42:45.000000 nzpyida-0.9.3/nzpyida/tests/test_geo_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.3/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11210 2023-07-21 10:38:04.000000 nzpyida-0.9.3/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-07-21 14:43:24.191914 nzpyida-0.9.3/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4930 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-07-21 14:43:24.000000 nzpyida-0.9.3/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      213 2023-07-21 14:43:24.210278 nzpyida-0.9.3/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     3300 2023-07-21 10:38:04.000000 nzpyida-0.9.3/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.656499 nzpyida-0.9.4/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.9.4/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.9.4/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      221 2023-07-21 14:42:45.000000 nzpyida-0.9.4/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-08-08 11:08:16.656588 nzpyida-0.9.4/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3748 2023-05-25 14:48:09.000000 nzpyida-0.9.4/README.md
+-rw-r--r--   0 mpl        (501) staff       (20)        6 2023-08-07 14:42:40.000000 nzpyida-0.9.4/VERSION
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.630773 nzpyida-0.9.4/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.9.4/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.634745 nzpyida-0.9.4/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    12029 2023-07-21 10:38:04.000000 nzpyida-0.9.4/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6663 2023-08-07 10:16:14.000000 nzpyida-0.9.4/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2500 2023-07-21 14:42:45.000000 nzpyida-0.9.4/docs/source/geo_frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3560 2023-07-21 14:42:45.000000 nzpyida-0.9.4/docs/source/geo_series.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3638 2023-07-21 14:42:45.000000 nzpyida-0.9.4/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4059 2023-07-21 14:42:45.000000 nzpyida-0.9.4/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1557 2023-07-21 10:38:04.000000 nzpyida-0.9.4/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2834 2023-06-20 14:25:25.000000 nzpyida-0.9.4/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23915 2023-07-21 14:42:45.000000 nzpyida-0.9.4/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.9.4/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.637489 nzpyida-0.9.4/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)     1008 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.639555 nzpyida-0.9.4/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.640806 nzpyida-0.9.4/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.640999 nzpyida-0.9.4/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.641690 nzpyida-0.9.4/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     2027 2023-06-20 14:25:25.000000 nzpyida-0.9.4/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2320 2023-05-17 10:27:59.000000 nzpyida-0.9.4/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.642220 nzpyida-0.9.4/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9129 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    33218 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.644940 nzpyida-0.9.4/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13090 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)    29037 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11574 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8875 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10059 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9562 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10976 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9665 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5637 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6069 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6902 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5767 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8390 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8909 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12793 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.648401 nzpyida-0.9.4/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     7697 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2501 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3666 2023-07-06 15:02:50.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5410 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_bayesian_networks.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2155 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1826 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_cross_validation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2519 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2433 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3125 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3734 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_glm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2015 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2343 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2169 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3464 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2406 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2994 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2205 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    22395 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2113 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2119 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.648893 nzpyida-0.9.4/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10647 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11017 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5996 2023-08-07 14:42:40.000000 nzpyida-0.9.4/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93635 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.650364 nzpyida-0.9.4/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      877 2023-05-25 14:48:09.000000 nzpyida-0.9.4/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    91025 2023-08-07 10:16:14.000000 nzpyida-0.9.4/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    37116 2023-07-21 14:42:45.000000 nzpyida-0.9.4/nzpyida/geo_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    66784 2023-07-21 14:42:45.000000 nzpyida-0.9.4/nzpyida/geo_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5136 2023-08-07 10:16:14.000000 nzpyida-0.9.4/nzpyida/groupby.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18287 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.651848 nzpyida-0.9.4/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-07-14 08:41:35.000000 nzpyida-0.9.4/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-06-19 09:03:41.000000 nzpyida-0.9.4/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-07-06 15:02:38.000000 nzpyida-0.9.4/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.656276 nzpyida-0.9.4/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13644 2023-07-21 14:42:45.000000 nzpyida-0.9.4/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8685 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6758 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9694 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23494 2023-07-19 07:48:15.000000 nzpyida-0.9.4/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15537 2023-08-07 10:16:14.000000 nzpyida-0.9.4/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9173 2023-07-21 14:42:45.000000 nzpyida-0.9.4/nzpyida/tests/test_geo_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8966 2023-07-21 14:42:45.000000 nzpyida-0.9.4/nzpyida/tests/test_geo_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.9.4/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11210 2023-07-21 10:38:04.000000 nzpyida-0.9.4/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-08-08 11:08:16.638287 nzpyida-0.9.4/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     5489 2023-08-08 11:08:16.000000 nzpyida-0.9.4/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4994 2023-08-08 11:08:16.000000 nzpyida-0.9.4/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-08-08 11:08:16.000000 nzpyida-0.9.4/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-08-08 11:08:16.000000 nzpyida-0.9.4/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-08-08 11:08:16.000000 nzpyida-0.9.4/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      213 2023-08-08 11:08:16.656887 nzpyida-0.9.4/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3300 2023-07-21 10:38:04.000000 nzpyida-0.9.4/setup.py
```

### Comparing `nzpyida-0.9.3/LICENSE.txt` & `nzpyida-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/PKG-INFO` & `nzpyida-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.3
+Version: 0.9.4
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.3/README.md` & `nzpyida-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/.DS_Store` & `nzpyida-0.9.4/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/Makefile` & `nzpyida-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/make.bat` & `nzpyida-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/base.rst` & `nzpyida-0.9.4/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/conf.py` & `nzpyida-0.9.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/frame.rst` & `nzpyida-0.9.4/docs/source/frame.rst`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,25 @@
 -----------
 .. automethod:: IdaDataFrame.pivot_table
 
 sort
 ----
 .. automethod:: IdaDataFrame.sort
 
+groupby
+-------
+.. automethod:: IdaDataFrame.groupby
+
+Obtaing IdaDataFrame with grouped data is possible with aggregate methods of IdaDataFrameGroupBy
+ 
+IdaDataFrameGroupBy
+-------------------
+.. autoclass:: nzpyida.groupby.IdaDataFrameGroupBy
+	:members:
+
 
 Descriptive Statistics
 ======================
 
 describe
 --------
 .. automethod:: IdaDataFrame.describe
```

### Comparing `nzpyida-0.9.3/docs/source/geo_frame.rst` & `nzpyida-0.9.4/docs/source/geo_frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/geo_series.rst` & `nzpyida-0.9.4/docs/source/geo_series.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/geospatial.rst` & `nzpyida-0.9.4/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/ibm.png` & `nzpyida-0.9.4/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/index.rst` & `nzpyida-0.9.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/install.rst` & `nzpyida-0.9.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/kc.ico` & `nzpyida-0.9.4/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/legal.rst` & `nzpyida-0.9.4/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/predictive.rst` & `nzpyida-0.9.4/docs/source/predictive.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/start.rst` & `nzpyida-0.9.4/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/docs/source/utils.rst` & `nzpyida-0.9.4/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/__init__.py` & `nzpyida-0.9.4/nzpyida/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,10 @@
 from .base import IdaDataBase
 from .frame import IdaDataFrame
 from .series import IdaSeries
 from .geo_frame import IdaGeoDataFrame
 from .geo_series import IdaGeoSeries
 
 
-__all__ = ['sampledata', 'tests', 'aggregation', 
-		   'base', 'exceptions', 'filtering', 'frame', 'indexing', 
-		   'internals', 'series', 'sql', 'statistics', 'utils', 'analytics',
-           'geo_frame', 'geo_series']
+__all__ = ['sampledata', 'aggregation', 'base', 'exceptions', 'filtering', 
+           'frame', 'indexing', 'internals', 'series', 'sql', 'statistics', 
+           'utils', 'analytics', 'geo_frame', 'geo_series']
```

### Comparing `nzpyida-0.9.3/nzpyida/ae/__init__.py` & `nzpyida-0.9.4/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/apply.py` & `nzpyida-0.9.4/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.9.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/groupedapply.py` & `nzpyida-0.9.4/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/install.py` & `nzpyida-0.9.4/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/result_builder.py` & `nzpyida-0.9.4/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/shaper.py` & `nzpyida-0.9.4/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/tapply.py` & `nzpyida-0.9.4/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/tapply_class.py` & `nzpyida-0.9.4/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.9.4/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/aggregation.py` & `nzpyida-0.9.4/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/__init__.py` & `nzpyida-0.9.4/nzpyida/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.9.4/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.9.4/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.9.4/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/model_manager.py` & `nzpyida-0.9.4/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/bayesian_networks.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/bayesian_networks.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,33 +194,33 @@
         finally:
             self.idadb.drop_table(out_table)
             if pred_view_needs_delete:
                 self.idadb.drop_view(pred_view)
             if true_view_needs_delete:
                 self.idadb.drop_view(true_view)
     
-    def cross_validation(self, in_df: IdaDataFrame, id_column: str=None, 
-                         target_column: str=None, out_table: str=None, folds: int=10, 
+    def cross_validation(self, in_df: IdaDataFrame, target_column: str,  
+                         id_column: str=None, out_table: str=None, folds: int=10, 
                          rand_seed: float=None) -> Tuple[IdaDataFrame, float]:
         """
         Performs a cross validation on <in_df> data for given model. Numer of batches 
         and size of train/test split isdetermined by parameter <folds>
 
         Parameters
         ----------
         in_df : IdaDataFrame
             the input data frame for scoring
+        
+        target_column : str
+            the input table column representing the class
 
         id_column : str, optional
             the input table column identifying a unique instance id - if skipped, 
             the input data frame indexer must be set and will be used as an instance id
 
-        target_column : str
-            the input table column representing the class
-
         out_table : str, optional
             the output table where the predicted values will be stored
 
         Returns
         -------
         IdaDataFrame
             the data frame with predicted values for all <in_df>
@@ -233,14 +233,22 @@
             'model': self.model_name,
             'intable': in_df,
             'id': q(id_column),
             'target': q(target_column),
             'outtable': out_table,
             'folds': folds,
         }
+
+        if not params.get('id'):
+            if in_df.indexer:
+                params['id'] = q(in_df.indexer)
+            else:
+                raise TypeError('Missing id column - either use id_column attribute or set '
+                    'indexer column in the input data frame')
+
         if isinstance(rand_seed, int):
             params['seed'] = rand_seed
         
         ModelManager(self.idadb).drop_model(self.model_name)
         
         ret_df, ret_acc = call_proc_df_in_out(proc="CROSS_VALIDATION", in_df=in_df, params=params,
                                    out_table=out_table)
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/glm.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/glm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,19 @@
         Returns
         -------
         IdaDataFrame
             the data frame containing row identifiers and predicted target values
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
-
+        
+        if not ModelManager(self.idadb).model_exists(self.model_name):
+                raise KeyError("Model name not found in Model Manager, "
+                            "use 'fit' function to train the model first")
+        
         params['model'] = self.model_name
         return call_proc_df_in_out(proc=self.predict_proc, in_df=in_df, params=params,
             out_table=out_table)[0]
 
     def _score(self, in_df: IdaDataFrame, predict_params:dict, target_column: str) -> float:
         """
         Scores the model. The model must exist.
@@ -129,14 +133,18 @@
         Returns
         -------
         float
             the model score
         """
         if not isinstance(in_df, IdaDataFrame):
             raise TypeError("Argument in_df should be an IdaDataFrame")
+        
+        if not ModelManager(self.idadb).model_exists(self.model_name):
+            raise KeyError("Model name not found in Model Manager, "
+                            "use 'fit' function to train the model first")
 
         if not predict_params.get('id', None):
             if in_df.indexer:
                 predict_params['id'] = q(in_df.indexer)
             else:
                 raise TypeError('Missing id column - either use id_column attribute or set '
                     'indexer column in the input data frame')
@@ -163,18 +171,19 @@
                     else q(self.target_column_in_output),
                 'true_column': q(target_column)
             })
 
             res = self.idadb.ida_query(f'call NZA..{self.score_proc}(\'{params}\')')
             return 1-res[0] if self.score_inv else res[0]
         finally:
-            self.idadb.drop_table(out_table)
-            if pred_view_needs_delete:
+            if self.idadb.exists_table_or_view(out_table):
+                self.idadb.drop_table(out_table)
+            if pred_view_needs_delete and self.idadb.exists_table_or_view(pred_view):
                 self.idadb.drop_view(pred_view)
-            if true_view_needs_delete:
+            if true_view_needs_delete and self.idadb.exists_table_or_view(true_view):
                 self.idadb.drop_view(true_view)
 
     def describe(self) -> str:
         """
         Returns model description.
 
         Returns
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/timeseries.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/timeseries.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.9.4/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_association_rules.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,83 +10,45 @@
 #-----------------------------------------------------------------------------
 
 from nzpyida.analytics.predictive.association_rules import ARule
 from nzpyida.base import IdaDataBase
 from nzpyida.frame import IdaDataFrame
 from nzpyida.analytics.model_manager import ModelManager
 import pytest
-from nzpyida.analytics.tests.conftest import MOD_NAME, TAB_NAME_TRAIN, \
-    TAB_NAME_TEST, OUT_TABLE_PRED
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED
 import pandas as pd
 from random import choice
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
-@pytest.fixture
+@pytest.fixture(scope="module")
 def clean_up(idadb, mm):
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     yield
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
 
-
-
-@pytest.fixture
-def idf_train(idadb: IdaDataBase):
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-    purchases = [[1,2,3,4,5],
-                 [2,4,6,7,10],
-                 [3,5,8,9,10],
-                 [4,6,7,8,10],
-                 [1,2,3,7,10],
-                 [2,3,4,6,9],
-                 [5,6,7,8,10],
-                 [1,3,4,6,9],
-                 [1,2,3,8,9],
-                 [3,5,7,9,10]]
-    df = pd.DataFrame.from_dict({
-        "ID": [ i//5 for i in range(50)],
-        "PRODUCT": [item for sublist in purchases for item in sublist]
-
-    })
-    yield idadb.as_idadataframe(df, TAB_NAME_TRAIN)
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-
-@pytest.fixture
-def idf_test(idadb: IdaDataBase):
-    if idadb.exists_table(TAB_NAME_TEST):
-        idadb.drop_table(TAB_NAME_TEST)
-    df = pd.DataFrame.from_dict({
-        "TID": range(50),
-        "ITEM": [choice(range(10)) for _ in range(50)]
-    })
-    yield idadb.as_idadataframe(df, TAB_NAME_TEST)
-    if idadb.exists_table(TAB_NAME_TEST):
-        idadb.drop_table(TAB_NAME_TEST)
-
-def test_arule(idadb: IdaDataBase, mm: ModelManager, idf_test: IdaDataFrame, 
-               idf_train: IdaDataFrame, clean_up):
+def test_arule(idadb: IdaDataBase, mm: ModelManager, idf_test_purch: IdaDataFrame, 
+               idf_train_purch: IdaDataFrame, clean_up):
     model = ARule(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME) 
 
-    model.fit(idf_train, transaction_id_column='ID', item_column="PRODUCT", 
+    model.fit(idf_train_purch, transaction_id_column='ID', item_column="PRODUCT", 
               support_type='absolute', support=2, confidence=0.4)
     assert mm.model_exists(MOD_NAME) 
 
-    pred_ida = model.predict(idf_test, OUT_TABLE_PRED, max_conviction=1.25, 
+    pred_ida = model.predict(idf_test_purch, OUT_TABLE_PRED, max_conviction=1.25, 
                        max_affinity=0.6, min_lift=1.0, min_leverage=0.03, transaction_id_column='TID', item_column='ITEM')
     assert pred_ida
     assert all(pred_ida.columns == idadb.to_def_case(['GID', 'TID', 'LHS_SID', 'RHS_SID', 'LHS_ITEMS', 'RHS_ITEMS', 'SUPPORT',
        'CONFIDENCE', 'LIFT', 'CONVICTION', 'AFFINITY', 'LEVERAGE']))
     pred = pred_ida.as_dataframe()
     assert all(pred[idadb.to_def_case("SUPPORT")].values >= 0.2)
     assert all(pred[idadb.to_def_case("CONFIDENCE")].values >= 0.4)
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_bayesian_networks.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_bayesian_networks.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.bayesian_networks import TreeBayesNetwork, TreeBayesNetwork1G, \
      TreeBayesNetwork1G2P, TreeBayesNetwork2G, TreeAgumentedNetwork, BinaryTreeBayesNetwork, \
      MultiTreeBayesNetwork
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_train_reg, df_test_reg
+from nzpyida.analytics.tests.conftest import MOD_NAME, MOD_NAME2, OUT_TABLE_PRED,\
+      OUT_TABLE_PRED2
 import pytest
 
-MOD_NAME2 = "TEST_MOD2"
-OUT_TABLE_PRED2 = "OUT_TABLE_PRED2"
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='function')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
@@ -42,127 +40,102 @@
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if mm.model_exists(MOD_NAME2):
         mm.drop_model(MOD_NAME2)
     if idadb.exists_table(OUT_TABLE_PRED2):
         idadb.drop_table(OUT_TABLE_PRED2)
 
-@pytest.fixture(scope='module')
-def idf_train_nom(idadb: IdaDataBase):
-    TAB_NAME_TRAIN_NOM = TAB_NAME_TRAIN + "_NOM"
-    df_train_reg["C"] = ['n', 'p', 'n', 'p', 'n', 'p', 'n', 'p', 'n', 'p']*100
-    yield idadb.as_idadataframe(df_train_reg, tablename=TAB_NAME_TRAIN_NOM, clear_existing=True)
-    if idadb.exists_table(TAB_NAME_TRAIN_NOM):
-        idadb.drop_table(TAB_NAME_TRAIN_NOM)
-
-@pytest.fixture(scope='module')
-def idf_test_nom(idadb: IdaDataBase):
-    TAB_NAME_TEST_NOM = TAB_NAME_TEST + "_NOM"
-    df_test_reg["C"]=['n', 'n', 'p', 'p', 'n']
-    yield idadb.as_idadataframe(df_test_reg, tablename=TAB_NAME_TEST_NOM, clear_existing=True)
-    if idadb.exists_table(TAB_NAME_TEST_NOM):
-        idadb.drop_table(TAB_NAME_TEST_NOM)
-
-@pytest.fixture(scope='module')
-def idf_train(idadb: IdaDataBase):
-    yield idadb.as_idadataframe(df_train_reg, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-
-@pytest.fixture(scope='module')
-def idf_test(idadb: IdaDataBase):
-    yield idadb.as_idadataframe(df_test_reg, tablename=TAB_NAME_TEST, clear_existing=True)
-    if idadb.exists_table(TAB_NAME_TEST):
-        idadb.drop_table(TAB_NAME_TEST)
-
-def test_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame,
-                            idf_test: IdaDataFrame, clear_up):
+def test_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
+                            idf_test_reg, clear_up):
     model = TreeBayesNetwork(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
-    model.fit(idf_train, in_columns=["A", "B"])
+    model.fit(idf_train_reg, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
-    pred  = model.predict(idf_test, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
+    pred  = model.predict(idf_test_reg, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
     # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['B_PRED'].values),  [2, 4, 2223, -999, 11112]))
 
 
-def test_binary_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame ,
-                                   idf_test: IdaDataFrame , clear_up):
+def test_binary_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
+                                   idf_test_reg, clear_up):
     model = BinaryTreeBayesNetwork(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
-    model.fit(idf_train, in_columns=["A", "B"])
+    model.fit(idf_train_reg, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
-    pred  = model.predict(idf_test, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
+    pred  = model.predict(idf_test_reg, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
-    assert any(round(x) == y for x, y in zip(list(pred.head()['B_'+idadb.to_def_case('PRED')].values),  [2, 4, 2223, -999, 11112]))
+    assert any(round(x) == y for x, y in zip(
+        list(pred.head()['B_'+idadb.to_def_case('PRED')].values),  
+        [2, 4, 2223, -999, 11112]))
 
 
-def test_multi_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train_nom: IdaDataFrame ,
-                                   idf_test_nom: IdaDataFrame , clear_up):
+def test_multi_tree_bayes_network(idadb: IdaDataBase, mm: ModelManager, idf_train_nom,
+                                   idf_test_nom, clear_up):
     model = MultiTreeBayesNetwork(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
     model.fit(idf_train_nom, class_column= "C", in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
 
     pred  = model.predict(idf_test_nom, target_column="B", id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == ["ID", "B_" + idadb.to_def_case("PRED")])
-    assert any(round(x) == y for x, y in zip(list(pred.head()['B_' + idadb.to_def_case('PRED')].values),  [2, 4, 2223, -999, 11112]))
+    assert any(round(x) == y for x, y in zip(
+        list(pred.head()['B_' + idadb.to_def_case('PRED')].values),  
+        [2, 4, 2223, -999, 11112]))
 
 
-def test_tree_bayes_network_1g(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame,
+def test_tree_bayes_network_1g(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
                                clear_up):
-    
     model = TreeBayesNetwork1G(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
 
-    outtab = model.grow(idf_train, in_columns=["A", "B"])
+    outtab = model.grow(idf_train_reg, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME)
     assert outtab
     # TODO: check output of an outtab
 
 
-def test_tree_bayes_network_2g(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame,
+def test_tree_bayes_network_2g(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
                                clear_up):
     
     model = TreeBayesNetwork2G(idadb, MOD_NAME2)
     assert model
     assert not mm.model_exists(MOD_NAME2)
 
-    outtab = model.grow(idf_train, in_columns=["A", "B"])
+    outtab = model.grow(idf_train_reg, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME2)
     assert outtab
     # TODO: check output of an outtab
 
-def test_tree_bayes_network_1g2p(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame,
+def test_tree_bayes_network_1g2p(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
                                clear_up):
     
     model = TreeBayesNetwork1G2P(idadb, MOD_NAME2)
     assert model
     assert not mm.model_exists(MOD_NAME2)
 
-    outtab = model.grow(idf_train, in_columns=["A", "B"])
+    outtab = model.grow(idf_train_reg, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME2)
     assert outtab
     # TODO: check output of an outtab
 
 
-def test_tree_agumented_network(idadb: IdaDataBase, mm: ModelManager, idf_train_nom: IdaDataFrame ,
-                                   idf_test_nom: IdaDataFrame , clear_up):
+def test_tree_agumented_network(idadb: IdaDataBase, mm: ModelManager, idf_train_nom,
+                                   idf_test_nom, clear_up):
     model = BinaryTreeBayesNetwork(idadb, MOD_NAME2)
     assert model
     assert not mm.model_exists(MOD_NAME2)
 
     model.fit(idf_train_nom, in_columns=["A", "B"])
     assert mm.model_exists(MOD_NAME2)
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,18 @@
 #-----------------------------------------------------------------------------
 
 from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.bisecting_kmeans import BisectingKMeans
 
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_train_clust, df_test_clust
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CLUST
 import pandas as pd
 import pytest
 
-OUT_TABLE_CLUST = "OUT_TABLE_CLUST"
-
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
@@ -38,29 +35,25 @@
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CLUST):
         idadb.drop_table(OUT_TABLE_CLUST)
 
-def test_bisecting_kmeans(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train_clust, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
-    idf_test = idadb.as_idadataframe(df_test_clust, tablename=TAB_NAME_TEST, clear_existing=True, indexer='ID')
-    assert idf_train
-    assert idf_test
-
+def test_bisecting_kmeans(idadb: IdaDataBase, mm: ModelManager, idf_train_clust,
+                          idf_test_clust, clear_up):
     model = BisectingKMeans(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, distance='manhattan', max_iter=4, min_split=3, max_depth=2,
+    model.fit(idf_train_clust, distance='manhattan', max_iter=4, min_split=3, max_depth=2,
               rand_seed=4321, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, level=5, out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_clust, level=5, out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
     assert all(list(pred.as_dataframe()[idadb.to_def_case('CLUSTER_ID')].values))
 
-    score = model.score(idf_test, target_column="A")
+    score = model.score(idf_test_clust, target_column="A")
 
     assert score
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_cross_validation.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_cross_validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 import pytest
 import numpy as np
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.decision_trees import DecisionTreeClassifier
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test, df_train
-from nzpyida.analytics.tests.conftest import df_train, TAB_NAME_TRAIN, \
-    TAB_NAME_TEST
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 from nzpyida.analytics import AutoDeleteContext
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
@@ -35,20 +32,18 @@
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CM):
         idadb.drop_table(OUT_TABLE_CM)
     
-def test_cross_validation(idadb: IdaDataBase, clear_up):
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True, 
-                                indexer="ID")
+def test_cross_validation(idadb: IdaDataBase, idf_train, clear_up):
 
     model = DecisionTreeClassifier(idadb, MOD_NAME)
     with AutoDeleteContext(idadb):
-        df_cv, acc = model.cross_validation(idf, id_column="ID", target_column="B")
+        df_cv, acc = model.cross_validation(idf_train, id_column="ID", target_column="B")
         assert acc
         assert acc > 0.99
 
         assert df_cv
-        assert len(df_cv) == len(idf)
+        assert len(df_cv) == len(idf_train)
         assert all(df_cv.columns == idadb.to_def_case(["ID", "CLASS", "FOLD"]))
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.decision_trees import DecisionTreeClassifier
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test, df_train
-import pandas as pd
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 import pytest
 
-TAB_NAME_TEST = "TAB_NAME1"
-TAB_NAME_TRAIN = "TAB_NAME2"
-MOD_NAME = "MOD_NAME1"
-
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
@@ -39,37 +32,36 @@
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CM):
         idadb.drop_table(OUT_TABLE_CM)
 
-def test_decision_trees(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    idf_test = idadb.as_idadataframe(df_test, tablename=TAB_NAME_TEST, clear_existing=True)
-    assert idf_train
-    assert idf_test
-
+def test_decision_trees(idadb: IdaDataBase, mm: ModelManager, idf_train,
+                        idf_test, clear_up):
     model = DecisionTreeClassifier(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, id_column="ID", target_column="B", eval_measure='gini', min_improve=0, min_split=200)
+    model.fit(idf_train, id_column="ID", target_column="B", eval_measure='gini', 
+              min_improve=0, min_split=200)
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
-    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) in (['p', 'n', 'n'], ['p', 'p', 'n'])
+    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) in \
+        (['p', 'n', 'n'], ['p', 'p', 'n'])
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
     assert score >= 0.66
 
-    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
+    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', 
+                                      out_matrix_table=OUT_TABLE_CM)
     assert all([cm, acc, wacc])
     assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
     assert len(cm) >= 2
     assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
     assert wacc >= 0.75
     assert acc >= 0.66
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_discretization.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,61 +4,54 @@
 # Copyright (c) 2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
-import pytest
+
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.auto_delete_context import AutoDeleteContext
-from nzpyida.analytics.tests.conftest import df_train, TAB_NAME_TRAIN
 from nzpyida.analytics.transform.discretization import EFDisc, EMDisc, EWDisc
 
 
-
-@pytest.fixture(scope='module')
-def idf(idadb: IdaDataBase):
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')[:10]['A']
-    yield idf
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-
-
-def test_ewdisc(idadb: IdaDataBase, idf):
+def test_ewdisc(idadb: IdaDataBase, idf_train):
+    idf = idf_train[:10]['A']
     with AutoDeleteContext(idadb):
         ewdisc = EWDisc(idadb, bins=5)
         bin_df = ewdisc.fit(idf)
         assert bin_df
         assert len(bin_df) == 4
         assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         ew_df = ewdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
         assert ew_df
         assert len(ew_df) == len(idf)
         assert all(ew_df.columns == ['A', idadb.to_def_case('DISC') + '_A'])
         assert set(ew_df[idadb.to_def_case('DISC') + '_A'].head(10).values) == {'1', '2', '3', '4', '5'}
 
 
-def test_efdisc(idadb: IdaDataBase, idf):
+def test_efdisc(idadb: IdaDataBase, idf_train):
+    idf = idf_train[:10]['A']
     with AutoDeleteContext(idadb):
         efdisc = EFDisc(idadb, bins=2)
         bin_df = efdisc.fit(idf)
         assert bin_df
         assert len(bin_df) == 1
         assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         ef_df = efdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
         assert ef_df
         assert len(ef_df) == len(idf)
         assert all(ef_df.columns == ['A', idadb.to_def_case('DISC') + '_A'])
         assert set(ef_df[idadb.to_def_case('DISC') + '_A'].head(10).values) == {'1', '2'}
 
 
-def test_emdisc(idadb: IdaDataBase, idf):
+def test_emdisc(idadb: IdaDataBase, idf_train):
+    idf = idf_train[:10]['A']
     with AutoDeleteContext(idadb):
         emdisc = EMDisc(idadb, target='A')
         bin_df = emdisc.fit(idf)
         assert bin_df
         assert all(bin_df.columns == idadb.to_def_case(['COLNAME', 'BREAK']))
 
         em_df = emdisc.apply(idf, in_bin_df=bin_df, keep_org_values=True)
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_glm.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_glm.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.glm import BernoulliRegressor, NegativeBinomialRegressor, BinomialRegressor, \
     GaussianRegressor, GammaRegressor, PoissonRegressor, WaldRegressor
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test_reg, df_train_reg
-import pandas as pd
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED
 import pytest
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='function')
@@ -53,28 +50,24 @@
                      "params": {}},
     }
     return models[model_name]
 
 @pytest.mark.parametrize("model_name", ['bernoulli', 'gaussian', 'poisson', 
                                         'binomial', 'negativebinomial', 'wald', 'gamma'
                                         ])
-def test_glm(idadb: IdaDataBase, mm: ModelManager, clear_up, model_name):
-    idf_train = idadb.as_idadataframe(df_train_reg, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    idf_test = idadb.as_idadataframe(df_test_reg, tablename=TAB_NAME_TEST, clear_existing=True)
-    assert idf_train
-    assert idf_test
-    
+def test_glm(idadb: IdaDataBase, mm: ModelManager, clear_up, model_name,
+             idf_train_reg, idf_test_reg):
     model_info = model_family(idadb, model_name)
     
     model = model_info["model"]
     assert model
     assert not mm.model_exists(MOD_NAME)
 
     params = {
-        'in_df': idf_train,
+        'in_df': idf_train_reg,
         'id_column': "ID",
         'target_column': "B",
         'in_columns': None,  
         'intercept': True, 
         'interaction': '', 
         'family_param': -1, 
         'link': 'logit', 
@@ -90,18 +83,18 @@
         'col_properties_table': None
     }
     for k, v in model_info["params"].items():
         params[k] = v
     model.fit(**params)
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_reg, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == ['ID', idadb.to_def_case('PRED')])
     # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['CLASS'].values),  [1, 4, 2223, -999, 11112]))
 
-    score = model.score(idf_test, id_column="ID", target_column="B")
+    score = model.score(idf_test_reg, id_column="ID", target_column="B")
 
     assert score
 
-    mse, mae, rse, rae = model.score_all(idf_test, id_column='ID', target_column='B')
+    mse, mae, rse, rae = model.score_all(idf_test_reg, id_column='ID', target_column='B')
     assert all([mse, mae, rse, rae])
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_kmeans.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,60 +6,54 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.kmeans import KMeans
 
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_train_clust, df_test_clust
-import pandas as pd
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_CLUST, OUT_TABLE_PRED
 import pytest
 
-OUT_TABLE_CLUST = "OUT_TABLE_CLUST"
-
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
-        idadb.drop_table(OUT_TABLE_PRED)
+        idadb.drop_table(OUT_TABLE_PRED) 
     if idadb.exists_table(OUT_TABLE_CLUST):
-        idadb.drop_table(OUT_TABLE_CLUST)
+        idadb.drop_table(OUT_TABLE_CLUST)    
     yield
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
-        idadb.drop_table(OUT_TABLE_PRED)
+        idadb.drop_table(OUT_TABLE_PRED) 
     if idadb.exists_table(OUT_TABLE_CLUST):
-        idadb.drop_table(OUT_TABLE_CLUST)
+        idadb.drop_table(OUT_TABLE_CLUST) 
 
-def test_kmeans(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train_clust, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
-    idf_test = idadb.as_idadataframe(df_test_clust, tablename=TAB_NAME_TEST, clear_existing=True, indexer='ID')
-    assert idf_train
-    assert idf_test
+def test_kmeans(idadb: IdaDataBase, mm: ModelManager, idf_train_clust,
+                idf_test_clust, clear_up):
+    assert idf_train_clust
+    assert idf_test_clust
 
     model = KMeans(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, k=3, out_table=OUT_TABLE_CLUST)
+    model.fit(idf_train_clust, k=3, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_clust, out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
     assert all(list(pred.as_dataframe()[idadb.to_def_case('CLUSTER_ID')].values))
 
-    score = model.score(idf_test, target_column="A")
+    score = model.score(idf_test_clust, target_column="A")
 
     assert score
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
-from nzpyida.analytics.predictive.knn import KNeighborsClassifier
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test, df_train
-import pandas as pd
+from nzpyida.analytics.predictive.naive_bayes import NaiveBayesClassifier
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 import pytest
 
-TAB_NAME_TEST = "TAB_NAME1"
-TAB_NAME_TRAIN = "TAB_NAME2"
-MOD_NAME = "MOD_NAME1"
-
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
@@ -39,37 +32,33 @@
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CM):
         idadb.drop_table(OUT_TABLE_CM)
 
-def test_knn(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    idf_test = idadb.as_idadataframe(df_test, tablename=TAB_NAME_TEST, clear_existing=True)
-    assert idf_train
-    assert idf_test
-
-    model = KNeighborsClassifier(idadb, MOD_NAME)
+def test_naive_bayes(idadb: IdaDataBase, mm: ModelManager, idf_train, idf_test, clear_up):
+    model = NaiveBayesClassifier(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
     model.fit(idf_train, id_column="ID", target_column="B")
     assert mm.model_exists(MOD_NAME)
 
     pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
-    assert list(pred.head()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
+    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
 
     score = model.score(idf_test, id_column="ID", target_column="B")
 
     assert score
     assert 0.67 >= score >= 0.66
 
-    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
+    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', 
+                                      out_matrix_table=OUT_TABLE_CM)
     assert all([cm, acc, wacc])
     assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
     assert len(cm) >= 3
     assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
     assert wacc == 0.75
     assert 0.67 >= acc >= 0.66
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.linear_regression import LinearRegression
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test_reg, df_train_reg
-import pandas as pd
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 import pytest
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
@@ -36,35 +33,28 @@
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CM):
         idadb.drop_table(OUT_TABLE_CM)
 
 @pytest.mark.skip
-def test_linear_regression(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train_reg, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
-    idf_test = idadb.as_idadataframe(df_test_reg, tablename=TAB_NAME_TEST, clear_existing=True, indexer='ID')
-    assert idf_train
-    assert idf_test
-
-    idf_train.indexer = 'ID'
-    idf_test.indexer = 'ID'
-
+def test_linear_regression(idadb: IdaDataBase, mm: ModelManager, 
+                           idf_train_reg, idf_test_reg, clear_up):
     model = LinearRegression(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, id_column="ID", target_column="B")
+    model.fit(idf_train_reg, id_column="ID", target_column="B")
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_reg, out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'B']))
     assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()[idadb.to_def_case('B')].values),  [1, 4, 2223, -999, 11112]))
 
-    score = model.score(idf_test, target_column='B')
+    score = model.score(idf_test_reg, target_column='B')
 
     assert score
     assert score < 0.001
 
-    mse, mae, rse, rae = model.score_all(idf_test, target_column='B')
+    mse, mae, rse, rae = model.score_all(idf_test_reg, target_column='B')
     assert all([mse, mae, rse, rae])
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_model_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 import pytest
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
 from nzpyida.analytics.predictive.decision_trees import DecisionTreeClassifier
-from nzpyida.analytics.tests.conftest import MOD_NAME, TAB_NAME_TRAIN, df_train
+from nzpyida.analytics.tests.conftest import MOD_NAME
 
 import pytest
 
 MOD_NAME_COPY = MOD_NAME+'_COPY'
 PRIVILEGES_OUTPUT1 = "INZAUSER  | TEST_MOD1  |   X X   X"""
 PRIVILEGES_OUTPUT2 = "INZAUSER  | TEST_MOD1  | X X X   X"
 PRIVILEGES_OUTPUT3 = "INZAUSER  | TEST_MOD1  |   X X   X"
@@ -32,55 +31,58 @@
     yield
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if mm.model_exists(MOD_NAME_COPY):
         mm.drop_model(MOD_NAME_COPY)
 
 
-def test_model_manager(idadb, clear_up):
+def test_model_manager(idadb, clear_up, idf_train):
     mm = ModelManager(idadb)
     assert mm
 
     # test listing models
     models_list = mm.list_models()
     assert models_list.exists()
     begin_length = len(mm.list_models()) 
 
     # verify model does not exist
     assert not mm.model_exists(MOD_NAME)
 
     # create model and check if mm.model_exits shows it
-    idf_train = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    DecisionTreeClassifier(idadb, model_name=MOD_NAME).fit(idf_train, id_column='ID', target_column='B')
+    DecisionTreeClassifier(idadb, model_name=MOD_NAME).fit(idf_train, id_column='ID', 
+                                                           target_column='B')
     assert mm.model_exists(MOD_NAME)
 
     # test copy model
     mm.copy_model(name=MOD_NAME, copy_name=MOD_NAME_COPY)
     assert mm.model_exists(MOD_NAME_COPY)
 
     # test listing models 2
     assert len(mm.list_models()) == 2 + begin_length
 
     # test droping model
     mm.drop_model(MOD_NAME)
     assert not mm.model_exists(MOD_NAME)
 
     # test alter model
-    mm.alter_model(MOD_NAME_COPY, name=MOD_NAME, owner="INZAUSER", description="DecTree model",
-                   copyright="Copyright (c) 2023. IBM Corp. All rights reserved.", category="DecTree")
+    mm.alter_model(MOD_NAME_COPY, name=MOD_NAME, owner="INZAUSER", 
+                   description="DecTree model",
+                   copyright="Copyright (c) 2023. IBM Corp. All rights reserved.", 
+                   category="DecTree")
     
     assert mm.model_exists(MOD_NAME)
 
     lm_ida = mm.list_models()
     lm = lm_ida.as_dataframe()
     lm = lm[lm[idadb.to_def_case("MODELNAME")]==idadb.to_def_case(MOD_NAME)]
     assert len(lm) == 1
     assert lm[idadb.to_def_case("OWNER")].iloc[0] == idadb.to_def_case("INZAUSER")
     assert lm[idadb.to_def_case("DESCRIPTION")].iloc[0] == "DecTree model"
-    assert lm[idadb.to_def_case("COPYRIGHT")].iloc[0] == "Copyright (c) 2023. IBM Corp. All rights reserved."
+    assert lm[idadb.to_def_case("COPYRIGHT")].iloc[0] == \
+        "Copyright (c) 2023. IBM Corp. All rights reserved."
     assert lm[idadb.to_def_case("USERCATEGORY")].iloc[0] == "DecTree"
     assert lm[idadb.to_def_case("CREATOR")].iloc[0] == idadb.to_def_case("ADMIN")
     assert lm[idadb.to_def_case("ALGORITHM")].iloc[0] == "Decision Tree"
 
     # test grant privileges
 
     mm.revoke_model(MOD_NAME, ["list", "update"], user=["INZAUSER"])
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
-from nzpyida.analytics.predictive.naive_bayes import NaiveBayesClassifier
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test, df_train
-import pandas as pd
+from nzpyida.analytics.predictive.regression_trees import DecisionTreeRegressor
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 import pytest
 
-TAB_NAME_TEST = "TAB_NAME1"
-TAB_NAME_TRAIN = "TAB_NAME2"
-MOD_NAME = "MOD_NAME1"
-
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
@@ -39,37 +32,27 @@
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
     if idadb.exists_table(OUT_TABLE_CM):
         idadb.drop_table(OUT_TABLE_CM)
 
-def test_naive_bayes(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    idf_test = idadb.as_idadataframe(df_test, tablename=TAB_NAME_TEST, clear_existing=True)
-    assert idf_train
-    assert idf_test
-
-    model = NaiveBayesClassifier(idadb, MOD_NAME)
+def test_regression_trees(idadb: IdaDataBase, mm: ModelManager, idf_train_reg,
+                          idf_test_reg, clear_up):
+    model = DecisionTreeRegressor(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, id_column="ID", target_column="B")
+    model.fit(idf_train_reg, id_column="ID", target_column="B", min_improve=0.001, min_split=200)
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_reg, id_column="ID", out_table=OUT_TABLE_PRED)
     assert pred
     assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
-    assert list(pred.as_dataframe()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
+    # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['CLASS'].values),  [1, 4, 2223, -999, 11112]))
 
-    score = model.score(idf_test, id_column="ID", target_column="B")
+    score = model.score(idf_test_reg, id_column="ID", target_column="B")
 
     assert score
-    assert 0.67 >= score >= 0.66
 
-    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
-    assert all([cm, acc, wacc])
-    assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
-    assert len(cm) >= 3
-    assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
-    assert wacc == 0.75
-    assert 0.67 >= acc >= 0.66
+    mse, mae, rse, rae = model.score_all(idf_test_reg, id_column='ID', target_column='B')
+    assert all([mse, mae, rse, rae])
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_timeseries.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,82 +4,64 @@
 # Copyright (c) 2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
-import pytest
-import numpy as np
-from nzpyida.base import IdaDataBase
-from nzpyida.analytics.auto_delete_context import AutoDeleteContext
-from nzpyida.analytics.tests.conftest import df_train, TAB_NAME_TRAIN, \
-    TAB_NAME_TEST
-from nzpyida.analytics.transform.preparation import std_norm, impute_data, \
-    random_sample, train_test_split
-
-TAB_NAME = "TAB_NAME0"
-
-@pytest.fixture(scope='function')
-def clean_up(idadb: IdaDataBase):
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-    if idadb.exists_table(TAB_NAME_TEST):
-        idadb.drop_table(TAB_NAME_TEST)
-    yield
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-    if idadb.exists_table(TAB_NAME_TEST):
-        idadb.drop_table(TAB_NAME_TEST)
-
-@pytest.fixture(scope='module')
-def idf(idadb: IdaDataBase):
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME, clear_existing=True, indexer='ID')
-    yield idf
-    if idadb.exists_table(TAB_NAME):
-        idadb.drop_table(TAB_NAME)
-
-def test_std_norm(idadb: IdaDataBase, clean_up, idf):
-
-    out_df = std_norm(idf, in_column=['A:S'], by_column=['B'], out_table=TAB_NAME_TEST)
-    assert out_df
-    assert idadb.exists_table_or_view(TAB_NAME_TEST)
-
-    assert all(out_df.columns == ['B', 'ID', 'std_A'])
-
-    assert len(out_df) == len(idf)
 
+from nzpyida.analytics.predictive.timeseries import TimeSeries
+from nzpyida.base import IdaDataBase
+from nzpyida.analytics.model_manager import ModelManager
+import pytest
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED
+import pandas as pd
+from math import sin
 
-def test_random_sample(idadb: IdaDataBase, idf, clean_up):
-    with AutoDeleteContext(idadb):
-        sample_df = random_sample(idf, size=300, by_column=["B"], rand_seed=123)
-        assert sample_df
-
-        assert all(sample_df.columns == [ 'ID', 'A', 'B'])
-
-        assert len(sample_df) == 300
+TAB_NAME = "TEST_TAB_NAME"
 
-        sample_df2 = random_sample(idf, size=300, by_column=["B"], rand_seed=123)
-        sample_df3 = random_sample(idf, size=300, by_column=["B"])
-        assert all((sample_df.head(10) == sample_df2.head(10))['ID'])
-        assert not all((sample_df.head(10) == sample_df3.head(10))['ID'])
+@pytest.fixture(scope='module')
+def mm(idadb: IdaDataBase):
+    return ModelManager(idadb)
 
+@pytest.fixture
+def clean_up(idadb, mm):
+    if mm.model_exists(MOD_NAME):
+        mm.drop_model(MOD_NAME)
+    if idadb.exists_table(OUT_TABLE_PRED):
+        idadb.drop_table(OUT_TABLE_PRED)
+    yield
+    if mm.model_exists(MOD_NAME):
+        mm.drop_model(MOD_NAME)
+    if idadb.exists_table(OUT_TABLE_PRED):
+        idadb.drop_table(OUT_TABLE_PRED)
 
-def test_impute_data(idadb: IdaDataBase, clean_up):
-    df_train['new'] = np.nan
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
 
-    assert idf
-    assert idadb.exists_table_or_view(TAB_NAME_TRAIN)
+@pytest.fixture
+def idf(idadb: IdaDataBase):
+    if idadb.exists_table(TAB_NAME):
+        idadb.drop_table(TAB_NAME)
 
+    time_series = [sin(x)+x for x in range(200)]
+    df = pd.DataFrame.from_dict({
+        "TIME": range(200),
+        "VALUE": time_series
+    })
+    yield idadb.as_idadataframe(df, TAB_NAME)
 
-def test_train_test_split(idadb: IdaDataBase, idf, clean_up):
-    train_df, test_df = train_test_split(idf, TAB_NAME_TRAIN, TAB_NAME_TEST, fraction=0.8,
-                                         id_column="ID")
-    assert test_df
-    assert test_df
-    assert round(len(train_df)/len(idf), 1) == 0.8
-    assert round(len(test_df)/len(idf), 1) == 0.2
+    if idadb.exists_table(TAB_NAME):
+        idadb.drop_table(TAB_NAME)
 
-    train_pdf = train_df['ID'].as_dataframe()
-    assert not any(el in train_pdf.values for el in test_df["ID"].as_dataframe().values)
 
+def test_timeseries(idadb: IdaDataBase, mm: ModelManager, idf, clean_up):
+    model = TimeSeries(idadb, MOD_NAME)
+    assert model
+    assert not mm.model_exists(MOD_NAME) 
+
+    outtab = model.fit_predict(idf, time_column="TIME", target_column="VALUE", 
+                               out_table=OUT_TABLE_PRED, forecast_horizon='399')
+
+    assert mm.model_exists(MOD_NAME) 
+    assert outtab
+    assert len(outtab) == 200
+    assert round(outtab.head(10).iloc[-1]["VALUE"]) == round(sin(210)+210)
+    assert round(outtab.tail().iloc[-1]["VALUE"]) == round(sin(399)+399)
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,60 +6,52 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.frame import IdaDataFrame
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.model_manager import ModelManager
-from nzpyida.analytics.predictive.regression_trees import DecisionTreeRegressor
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_test_reg, df_train_reg
-import pandas as pd
+from nzpyida.analytics.predictive.two_step_clustering import TwoStepClustering
+
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CLUST
 import pytest
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
 @pytest.fixture(scope='module')
 def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
-    if idadb.exists_table(OUT_TABLE_CM):
-        idadb.drop_table(OUT_TABLE_CM)
+    if idadb.exists_table(OUT_TABLE_CLUST):
+        idadb.drop_table(OUT_TABLE_CLUST)
     yield
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
-    if idadb.exists_table(OUT_TABLE_CM):
-        idadb.drop_table(OUT_TABLE_CM)
-
-def test_regression_trees(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train_reg, tablename=TAB_NAME_TRAIN, clear_existing=True)
-    idf_test = idadb.as_idadataframe(df_test_reg, tablename=TAB_NAME_TEST, clear_existing=True)
-    assert idf_train
-    assert idf_test
+    if idadb.exists_table(OUT_TABLE_CLUST):
+        idadb.drop_table(OUT_TABLE_CLUST)
 
-    model = DecisionTreeRegressor(idadb, MOD_NAME)
+def test_bisecting_kmeans(idadb: IdaDataBase, mm: ModelManager, idf_train_clust,
+                          idf_test_clust, clear_up):
+    model = TwoStepClustering(idadb, MOD_NAME)
     assert model
     assert not mm.model_exists(MOD_NAME)
     
-    model.fit(idf_train, id_column="ID", target_column="B", min_improve=0.001, min_split=200)
+    model.fit(idf_train_clust, distance='euclidean', max_k=5, bins=10, node_capacity=10, 
+              leaf_capacity=10, max_leaves=100, rand_seed=4321, out_table=OUT_TABLE_CLUST)
     assert mm.model_exists(MOD_NAME)
 
-    pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
+    pred = model.predict(idf_test_clust, out_table=OUT_TABLE_PRED)
     assert pred
-    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
-    # assert any(round(x) == y for x, y in zip(list(pred.as_dataframe()['CLASS'].values),  [1, 4, 2223, -999, 11112]))
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
+    assert all(list(pred.head()[idadb.to_def_case('CLUSTER_ID')].values))
 
-    score = model.score(idf_test, id_column="ID", target_column="B")
+    score = model.score(idf_test_clust, target_column="A")
 
     assert score
-
-    mse, mae, rse, rae = model.score_all(idf_test, id_column='ID', target_column='B')
-    assert all([mse, mae, rse, rae])
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,416 +10,416 @@
 #-----------------------------------------------------------------------------
 
 import pytest
 import pandas as pd
 import numpy as np
 from nzpyida.base import IdaDataBase
 from nzpyida.analytics.exploration.relation_identification import *
-from nzpyida.analytics.tests.conftest import TAB_NAME_TRAIN
+from nzpyida.analytics.tests.conftest import TAB_NAME_TRAIN, OUT_TABLE_PRED
 
-TEST_TAB_NAME = "TEST_TAB_NAME"
+TAB_NAME = "TEST_TAB_NAME"
 
 @pytest.fixture(scope='module')
 def idf(idadb):
     df_train = pd.DataFrame.from_dict(
     {
         "ID": range(1000),
         "A": range(1,1001),
         "B": range(1000, 0, -1),
         "C": ['p','n']*500,
         "D": [1, 0]*500,
         "E": ['a']*500 + ['b']*500,
         "F": map(lambda l: l**2, range(1000))
     }
     )
-    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME_TRAIN, clear_existing=True)
+    idf = idadb.as_idadataframe(df_train, tablename=TAB_NAME, clear_existing=True)
     yield idf
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
+    if idadb.exists_table(TAB_NAME):
+        idadb.drop_table(TAB_NAME)
     
 @pytest.fixture(scope='function')
 def clean_up(idadb: IdaDataBase):
-    if idadb.exists_table_or_view(TEST_TAB_NAME):
-        idadb.drop_table(TEST_TAB_NAME)
+    if idadb.exists_table_or_view(OUT_TABLE_PRED):
+        idadb.drop_table(OUT_TABLE_PRED)
     yield
-    if idadb.exists_table_or_view(TEST_TAB_NAME):
-        idadb.drop_table(TEST_TAB_NAME)
+    if idadb.exists_table_or_view(OUT_TABLE_PRED):
+        idadb.drop_table(OUT_TABLE_PRED)
 
 class TestCorr:
     def test_strong_correlation(self, idadb, idf, clean_up):
-        out_df = corr(idf, in_column=["A", "B"], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = corr(idf, in_column=["A", "B"], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('CORRELATION'), "C"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case("CORRELATION")].head().values < -0.99)
 
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = corr(idf, in_column=["A", "D"], out_table=TEST_TAB_NAME)
+        out_df = corr(idf, in_column=["A", "D"], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['CORRELATION']))
         assert len(out_df) == 1
         assert 0.01 > out_df.head()[0] > -0.01
     
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = corr(idf, in_column=["A", "D"], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = corr(idf, in_column=["A", "D"], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('CORRELATION'), "C"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case("CORRELATION")].head().values == [0, 0])
 
 class TestCov:
     def test_strong_covariance(self, idadb, idf, clean_up):
-        out_df = cov(idf, in_column=['ID', 'A'], out_table=TEST_TAB_NAME)
+        out_df = cov(idf, in_column=['ID', 'A'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['COVARIANCE']))
         assert len(out_df) == 1
         max_cov = np.cov(range(1, 1001),range(1, 1001))[0][0]
         assert all(0.99*max_cov < out_df[idadb.to_def_case("COVARIANCE")].head().values < 1.01*max_cov)
     
     def test_weak_covariance(self, idadb, idf, clean_up):
-        out_df = cov(idf, in_column=['A', 'D'], out_table=TEST_TAB_NAME)
+        out_df = cov(idf, in_column=['A', 'D'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['COVARIANCE']))
         assert len(out_df) == 1
         assert np.abs(out_df[idadb.to_def_case("COVARIANCE")].head().values) < 0.5
 
 
     def test_no_covariance(self, idadb, idf, clean_up):
-        out_df = cov(idf, in_column=['A', 'D'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = cov(idf, in_column=['A', 'D'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('COVARIANCE'), "C"])
         assert len(out_df) == 2
         assert all( out_df[idadb.to_def_case("COVARIANCE")].head().values == [0, 0])
 
 class TestMutualInfo:
     def test_strong_corelation(self, idadb, idf, clean_up):
-        out_df = mutual_info(idf, ['A', 'B'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = mutual_info(idf, ['A', 'B'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('MUTUALINFO'), 'Over_C'])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case("MUTUALINFO")].head().values < 10)
     
     @pytest.mark.skip # "Attribute ... must be GROUPed or used in an aggregate function" error
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = mutual_info(idf, ['A', 'D'], out_table=TEST_TAB_NAME)
+        out_df = mutual_info(idf, ['A', 'D'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('MUTUALINFO'), 'Over_C'])
         assert len(out_df) == 1
 
     @pytest.mark.skip # "Attribute ... must be GROUPed or used in an aggregate function" error
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = mutual_info(idf, ['A', 'D'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = mutual_info(idf, ['A', 'D'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('MUTUALINFO'), 'Over_C'])
         assert len(out_df) == 2
 
 # TODO: poorly readable output
 class TestCovarianceMatrix:
     def test_strong_corelation(self, idadb, idf, clean_up):
-        out_df = covariance_matrix(idf, ['A', 'B'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = covariance_matrix(idf, ['A', 'B'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('COVARIANCE'), 'C'])
         assert len(out_df) == 2
     
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = covariance_matrix(idf, ['A', 'D'], out_table=TEST_TAB_NAME)
+        out_df = covariance_matrix(idf, ['A', 'D'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['COVARIANCE']))
         assert len(out_df) == 1
 
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = covariance_matrix(idf, ['A', 'D'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = covariance_matrix(idf, ['A', 'D'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('COVARIANCE'), 'C'])
         assert len(out_df) == 2
 
 class TestSpearmanCorr:
     def test_strong_corelation(self, idadb, idf, clean_up):
-        out_df = spearman_corr(idf, ['A', 'B'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = spearman_corr(idf, ['A', 'B'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['C', idadb.to_def_case('RHO'), idadb.to_def_case('N')])
         assert len(out_df) == 2
         assert all( out_df[idadb.to_def_case("RHO")].head().values == -1)
     
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = spearman_corr(idf, ['A', 'D'], out_table=TEST_TAB_NAME)
+        out_df = spearman_corr(idf, ['A', 'D'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['SPEARMAN_CORR']))
         assert len(out_df) == 1
         assert all(abs(out_df[idadb.to_def_case("SPEARMAN_CORR")].head().values) < 0.05)
         
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = spearman_corr(idf, ['A', 'D'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = spearman_corr(idf, ['A', 'D'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['C', idadb.to_def_case('RHO'), idadb.to_def_case('N')])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case("RHO")].head().values == 0)
 
 class TestChisq:
     # I believe last assertsion should be stronger (... > 0.95)
     def test_strong_correlation(self, idadb, idf, clean_up):
-        out_df = chisq(idf, ['A', 'B'], out_table=TEST_TAB_NAME)
+        out_df = chisq(idf, ['A', 'B'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'CHI2STATISTIC', 'DF', 'OVER_NO_GROUP']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] > 0.75
 
     @pytest.mark.skip # "Attribute ... must be GROUPed or used in an aggregate function" error
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = chisq(idf, ['A', 'D'], out_table=TEST_TAB_NAME)
+        out_df = chisq(idf, ['A', 'D'], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'CHI2STATISTIC', 'DF', 'OVER_NO_GROUP']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.05
     
     @pytest.mark.skip # "Attribute ... must be GROUPed or used in an aggregate function" error
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = chisq(idf, ['A', 'D'], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = chisq(idf, ['A', 'D'], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'CHI2STATISTIC', 'DF', 'OVER_NO_GROUP']))
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values == 0)
 
 
 class TestTMeTest:
     def test_linear_column_correct_value(self, idadb, idf, clean_up):
-        out_df = t_me_test(idf, in_column="A", mean_value=500, out_table=TEST_TAB_NAME)
+        out_df = t_me_test(idf, in_column="A", mean_value=500, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_ME_TEST']))
         assert len(out_df) == 1
         assert 0.05 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.95
     
     def test_linear_column_incorrect_value(self, idadb, idf, clean_up):
-        out_df = t_me_test(idf, in_column="A", mean_value=400, out_table=TEST_TAB_NAME)
+        out_df = t_me_test(idf, in_column="A", mean_value=400, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_ME_TEST']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] > 0.95
     
     def test_linear_column_incorrect_value_with_by_column(self, idadb, idf, clean_up):
-        out_df = t_me_test(idf, in_column="A", mean_value=550, by_column="C", out_table=TEST_TAB_NAME)
+        out_df = t_me_test(idf, in_column="A", mean_value=550, by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_ME_TEST']) + ["C"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values < 0.05)
     
     def test_constant_column(self, idadb, idf, clean_up):
-        out_df = t_me_test(idf, in_column="D", mean_value=1, by_column="C", out_table=TEST_TAB_NAME)
+        out_df = t_me_test(idf, in_column="D", mean_value=1, by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_ME_TEST']) + ["C"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values == None)
 
 class TestTUmdTest:
     def test_linear_column_correct_value(self, idadb, idf, clean_up):
-        out_df = t_umd_test(idf, in_column="A", class_column='C:p:n', out_table=TEST_TAB_NAME)
+        out_df = t_umd_test(idf, in_column="A", class_column='C:p:n', out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_UMD_TEST']))
         assert len(out_df) == 1
         assert 0.45 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.55
     
     def test_linear_column_incorrect_value(self, idadb, idf, clean_up):
-        out_df = t_umd_test(idf, in_column="A", class_column='E:a:b', by_column="C", out_table=TEST_TAB_NAME)
+        out_df = t_umd_test(idf, in_column="A", class_column='E:a:b', by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('PERCENTAGE'), idadb.to_def_case('T_UMD_TEST'), "C"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values < 0.05)
     
 class TestTPmdTest:
     def test_good_diff(self, idadb, idf, clean_up):
-        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], expected_diff=0, out_table=TEST_TAB_NAME)
+        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], expected_diff=0, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'TSTUDPAIREDMEANDIFF']))
         assert len(out_df) == 1
         assert 0.45 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.55
     
     def test_slightly_wrong_diff(self, idadb, idf, clean_up):
-        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], expected_diff=1, out_table=TEST_TAB_NAME)
+        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], expected_diff=1, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'TSTUDPAIREDMEANDIFF']))
         assert len(out_df) == 1
         assert 0.05 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.95
     
     def test_wrong_diff(self, idadb, idf, clean_up):
-        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], by_column="E", expected_diff=10, out_table=TEST_TAB_NAME)
+        out_df = t_pmd_test(idf, in_column=["A:X", "B:Y"], by_column="E", expected_diff=10, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('PERCENTAGE'), idadb.to_def_case('TSTUDPAIREDMEANDIFF'), "E"])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values == [0, 1])
 
 
 class TestTLsTest:
     @pytest.mark.skip # TODO: this function is failing, when slope is exactly right
     def test_good_slope(self, idadb, idf, clean_up):
-        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=-1, out_table=TEST_TAB_NAME)
+        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=-1, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_LS_TEST']))
         assert len(out_df) == 1
         assert 0.05 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.95
     
     def test_wrong_slope(self, idadb, idf, clean_up):
-        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=1, by_column="C", out_table=TEST_TAB_NAME)
+        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=1, by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('PERCENTAGE'), idadb.to_def_case('T_LS_TEST'), 'C'])
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PERCENTAGE')].head().values == 0)
 
     @pytest.mark.skip # TODO: this function is not working correctly, as slope close to correct value is treated as very bad one
     def test_slightly_wrong_slope(self, idadb, idf, clean_up):
-        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=-0.99999, out_table=TEST_TAB_NAME)
+        out_df = t_ls_test(idf, in_column=["A:X", "B:Y"], slope=-0.99999, out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['PERCENTAGE', 'T_LS_TEST']))
         assert len(out_df) == 1
         assert 0.05 < out_df[idadb.to_def_case('PERCENTAGE')].head().values[0] < 0.95
 
 
 class TestMwwTest:
     def test_linear_column_similar_values_with_by_column(self, idadb, idf, clean_up):
-        out_df = mww_test(idf, in_column="A", class_column="C", by_column="E", out_table=TEST_TAB_NAME)
+        out_df = mww_test(idf, in_column="A", class_column="C", by_column="E", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['E'] + idadb.to_def_case(['N', 'N1', 'N2', 'USTAT0', 'U2STAT0', 'ALPHASUM', 'NORM1',
                                       'USTAT1', 'NORM2', 'U2STAT1', 'MU_U1', 'SIGMA_U', 'ZSTAT', 'PP',
                                       'USTAT', 'U2STAT', 'MU_U', 'NOGROUPS', 'MESSAGE', 'LOWER']))
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PP')].head().values > 0.05)
         assert all(out_df[idadb.to_def_case('LOWER')].head().values == 'p')
     
     def test_linear_column_similar_values_without_by_column(self, idadb, idf, clean_up):
-        out_df = mww_test(idf, in_column="A", class_column="C", out_table=TEST_TAB_NAME)
+        out_df = mww_test(idf, in_column="A", class_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['USTAT', 'U2STAT', 'MUU', 'SIGMAU', 'ZSTAT', 'PP', 'LOWER'])
         assert len(out_df) == 1
         assert out_df['PP'].head().values[0] > 0.05
         assert out_df['LOWER'].head().values[0] == 'p'
     
     def test_linear_column_different_values_with_by_column(self, idadb, idf, clean_up):
-        out_df = mww_test(idf, in_column="A", class_column="E", by_column="C", out_table=TEST_TAB_NAME)
+        out_df = mww_test(idf, in_column="A", class_column="E", by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['C'] + idadb.to_def_case(['N', 'N1', 'N2', 'USTAT0', 'U2STAT0', 'ALPHASUM', 'NORM1',
                                       'USTAT1', 'NORM2', 'U2STAT1', 'MU_U1', 'SIGMA_U', 'ZSTAT', 'PP',
                                       'USTAT', 'U2STAT', 'MU_U', 'NOGROUPS', 'MESSAGE', 'LOWER']))
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PP')].head().values < 0.05)
         assert all(out_df[idadb.to_def_case('LOWER')].head().values == 'a')
 
 
 class TestWilcoxonTest:
     # function wrogly indicates column with lower values, need to change last assertions
     def test_similar_columns(self, idadb, idf, clean_up):
-        out_df = wilcoxon_test(idf, in_column=["A", "B"], out_table=TEST_TAB_NAME)
+        out_df = wilcoxon_test(idf, in_column=["A", "B"], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['SSTAT', 'WSTAT', 'ZSTAT', 'NOITEM', 'PP', 'LOWER'])
         assert len(out_df) == 1
         assert out_df['PP'].head().values[0] > 0.05
     
     # function wrogly indicates column with lower values, need to change last assertions
     def test_similar_columns_with_by_column(self, idadb, idf, clean_up):
-        out_df = wilcoxon_test(idf, in_column=["A", "B"], by_column="E", out_table=TEST_TAB_NAME)
+        out_df = wilcoxon_test(idf, in_column=["A", "B"], by_column="E", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['E'] + idadb.to_def_case(['N', 'SSTAT', 'WSTAT', 'ZSTAT', 'PP', 'LOWER']))
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PP')].head().values < 0.05)
         assert out_df[out_df["E"]=='a'][idadb.to_def_case("LOWER")].head().values[0] == '"B"'
         assert out_df[out_df["E"]=='b'][idadb.to_def_case("LOWER")].head().values[0] == '"A"'
     
     # function wrogly indicates column with lower values, need to change last assertion
     def test_different_columns(self, idadb, idf, clean_up):
-        out_df = wilcoxon_test(idf, in_column=["A", "D"], out_table=TEST_TAB_NAME)
+        out_df = wilcoxon_test(idf, in_column=["A", "D"], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == ['SSTAT', 'WSTAT', 'ZSTAT', 'NOITEM', 'PP', 'LOWER'])
         assert len(out_df) == 1
         assert out_df['PP'].head().values[0] < 0.05
         assert out_df['LOWER'].head().values[0] == '"A"'
 
 # TODO: poorly readable output
 class TestCanonicalCorr:
     def test_strong_correlation(self, idadb, idf, clean_up):
-        out_df = canonical_corr(idf, in_column=["A", "B"], out_table=TEST_TAB_NAME)
+        out_df = canonical_corr(idf, in_column=["A", "B"], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['CANONICAL_CORRELATION']))
         assert len(out_df) == 1
     
     def test_weak_correlation(self, idadb, idf, clean_up):
-        out_df = canonical_corr(idf, in_column=["A", "D"], out_table=TEST_TAB_NAME)
+        out_df = canonical_corr(idf, in_column=["A", "D"], out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['CANONICAL_CORRELATION']))
         assert len(out_df) == 1
     
     def test_no_correlation(self, idadb, idf, clean_up):
-        out_df = canonical_corr(idf, in_column=["A", "D"], by_column="C", out_table=TEST_TAB_NAME)
+        out_df = canonical_corr(idf, in_column=["A", "D"], by_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('CANONICAL_CORRELATION'), "C"])
         assert len(out_df) == 2
 
 
 class TestAnovaCrdTest:
     def test_simmilar_columns(self, idadb, idf, clean_up):
-        out_df = anova_crd_test(idf, in_column=['D'], treatment_column="E", out_table="TEST_TAB_NAME")
+        out_df = anova_crd_test(idf, in_column=['D'], treatment_column="E", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['TOTNO', 'TOTSU', 'TOTMEAN', 'TOTSS', 'SSCTOT', 'SSCBETWEEN', 
                                       'DFBETWEEN', 'SSCWITHIN', 'DFWITHIN', 'F', 'P']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('P')].head().values[0] < 0.95 
     
     def test_dfferent_columns(self, idadb, idf, clean_up):
-        out_df = anova_crd_test(idf, in_column=['A'], treatment_column="E", out_table="TEST_TAB_NAME")
+        out_df = anova_crd_test(idf, in_column=['A'], treatment_column="E", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['TOTNO', 'TOTSU', 'TOTMEAN', 'TOTSS', 'SSCTOT', 'SSCBETWEEN', 
                                       'DFBETWEEN', 'SSCWITHIN', 'DFWITHIN', 'F', 'P']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('P')].head().values[0] > 0.95
     
     def test_multiple_columns_with_by_column(self, idadb, idf, clean_up):
-        out_df = anova_crd_test(idf, in_column=['A', 'B'], treatment_column="E", by_column='C', out_table="TEST_TAB_NAME")
+        out_df = anova_crd_test(idf, in_column=['A', 'B'], treatment_column="E", by_column='C', out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == [idadb.to_def_case('INCOLUMN'), 'C'] + idadb.to_def_case(['TOTNO', 'TOTSU', 'TOTMEAN', 'TOTSS', 'SSCTOT', 
                                       'SSCBETWEEN', 'DFBETWEEN', 'SSCWITHIN', 'DFWITHIN', 'F', 'P']))
         assert len(out_df) == 4
 
 
 class TestAnovaRbdTest:
     def test_one_column(self, idadb, idf, clean_up):
-        out_df = anova_rbd_test(idf, in_column=['A'], treatment_column="E", block_column="C", out_table="TEST_TAB_NAME")
+        out_df = anova_rbd_test(idf, in_column=['A'], treatment_column="E", block_column="C", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['BLSSCBETWEEN', 'BLDFBETWEEN','SSCWITHIN', 'DFWITHIN', 'FBL', 'PBL', 
                                       'GRSSCBETWEEN', 'GRDFBETWEEN', 'FGR', 'PGR']))
         assert len(out_df) == 1
         assert out_df[idadb.to_def_case('PGR')].head().values[0] > 0.95  
         assert out_df[idadb.to_def_case('PBL')].head().values[0] < 0.95 
     
     def test_multiple_columns(self, idadb, idf, clean_up):
-        out_df = anova_rbd_test(idf, in_column=['A', 'B'], treatment_column="C", block_column='E', out_table="TEST_TAB_NAME")
+        out_df = anova_rbd_test(idf, in_column=['A', 'B'], treatment_column="C", block_column='E', out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['INCOLUMN', 'BLSSCBETWEEN', 'BLDFBETWEEN','SSCWITHIN', 'DFWITHIN', 
                                       'FBL', 'PBL', 'GRSSCBETWEEN', 'GRDFBETWEEN', 'FGR', 'PGR']))
         assert len(out_df) == 2
         assert all(out_df[idadb.to_def_case('PGR')].head().values < 0.95)
         assert all(out_df[idadb.to_def_case('PBL')].head().values > 0.95)
 
 class TestManovaOneWayTest:
     def test_idependent_columns(self, idadb, idf, clean_up):
         out_df = manova_one_way_test(idf, in_column=["A","D"], factor1_column="E", id_column="ID", 
-                                     table_type="columns", out_table="TEST_TAB_NAME")
+                                     table_type="columns", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['ID_TASK', 'ID_MATRIX', 'ROW', 'COL', 'VAL', 'EXPLANATION',
                                       'BONFERRONI_CORR', 'TASK_NAME', 'VARIABLE_NAME']))
         assert len(out_df) == 21
         assert len(set(out_df[idadb.to_def_case('ID_MATRIX')].as_dataframe().values)) == 4
     
     def test_correlated_columns(self, idadb, idf, clean_up):
         out_df = manova_one_way_test(idf, in_column=["A","F"], factor1_column="C", id_column="ID", 
-                                     table_type="columns", out_table="TEST_TAB_NAME")
+                                     table_type="columns", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['ID_TASK', 'ID_MATRIX', 'ROW', 'COL', 'VAL', 'EXPLANATION',
                                       'BONFERRONI_CORR', 'TASK_NAME', 'VARIABLE_NAME']))
         assert len(out_df) == 21
         assert len(set(out_df[idadb.to_def_case('ID_MATRIX')].as_dataframe().values)) == 4
 
 class TestManovaTwoWayTest:
     def test_correlated_columns(self, idadb, idf, clean_up):
         out_df = manova_two_way_test(idf, in_column=["A","F"], factor1_column="E", factor2_column="C", id_column="ID", 
-                                     table_type="columns", out_table="TEST_TAB_NAME")
+                                     table_type="columns", out_table=OUT_TABLE_PRED)
         assert out_df
         assert all(out_df.columns == idadb.to_def_case(['ID_TASK', 'ID_MATRIX', 'ROW', 'COL', 'VAL', 'EXPLANATION',
                                       'BONFERRONI_CORR', 'TASK_NAME', 'VARIABLE_NAME']))
         assert len(out_df) == 59
         assert len(set(out_df[idadb.to_def_case('ID_MATRIX')].as_dataframe().values)) == 8
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_timeseries.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_knn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,63 @@
+
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
 # Copyright (c) 2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
-from nzpyida.analytics.predictive.timeseries import TimeSeries
 from nzpyida.base import IdaDataBase
-from nzpyida.frame import IdaDataFrame
 from nzpyida.analytics.model_manager import ModelManager
+from nzpyida.analytics.predictive.knn import KNeighborsClassifier
+from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, OUT_TABLE_CM
 import pytest
-from nzpyida.analytics.tests.conftest import MOD_NAME, TAB_NAME_TRAIN, OUT_TABLE_PRED
-import pandas as pd
-from math import sin
-
 
 @pytest.fixture(scope='module')
 def mm(idadb: IdaDataBase):
     return ModelManager(idadb)
 
-@pytest.fixture
-def clean_up(idadb, mm):
+@pytest.fixture(scope='module')
+def clear_up(idadb: IdaDataBase, mm: ModelManager):
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
+    if idadb.exists_table(OUT_TABLE_CM):
+        idadb.drop_table(OUT_TABLE_CM)
     yield
     if mm.model_exists(MOD_NAME):
         mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
+    if idadb.exists_table(OUT_TABLE_CM):
+        idadb.drop_table(OUT_TABLE_CM)
 
-
-@pytest.fixture
-def idf_train(idadb: IdaDataBase):
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-
-    time_series = [sin(x)+x for x in range(200)]
-    df = pd.DataFrame.from_dict({
-        "TIME": range(200),
-        "VALUE": time_series
-    })
-    yield idadb.as_idadataframe(df, TAB_NAME_TRAIN)
-
-    if idadb.exists_table(TAB_NAME_TRAIN):
-        idadb.drop_table(TAB_NAME_TRAIN)
-
-
-def test_timeseries(idadb: IdaDataBase, mm: ModelManager, idf_train: IdaDataFrame, clean_up):
-    model = TimeSeries(idadb, MOD_NAME)
+def test_knn(idadb: IdaDataBase, mm: ModelManager, idf_train, idf_test, clear_up):
+    model = KNeighborsClassifier(idadb, MOD_NAME)
     assert model
-    assert not mm.model_exists(MOD_NAME) 
-
-    outtab = model.fit_predict(idf_train, time_column="TIME", target_column="VALUE", out_table=OUT_TABLE_PRED, 
-                       forecast_horizon='399')
-
-    assert mm.model_exists(MOD_NAME) 
-    assert outtab
-    assert len(outtab) == 200
-    assert round(outtab.head(10).iloc[-1]["VALUE"]) == round(sin(210)+210)
-    assert round(outtab.tail().iloc[-1]["VALUE"]) == round(sin(399)+399)
+    assert not mm.model_exists(MOD_NAME)
+    
+    model.fit(idf_train, id_column="ID", target_column="B")
+    assert mm.model_exists(MOD_NAME)
+
+    pred = model.predict(idf_test, id_column="ID", out_table=OUT_TABLE_PRED)
+    assert pred
+    assert all(pred.columns == idadb.to_def_case(['ID', 'CLASS']))
+    assert list(pred.head()[idadb.to_def_case('CLASS')].values) == ['p', 'n', 'n']
+
+    score = model.score(idf_test, id_column="ID", target_column="B")
+
+    assert score
+    assert 0.67 >= score >= 0.66
+
+    cm, acc, wacc = model.conf_matrix(idf_test, id_column='ID', target_column='B', out_matrix_table=OUT_TABLE_CM)
+    assert all([cm, acc, wacc])
+    assert all(cm.columns == idadb.to_def_case(['REAL', 'PREDICTION', 'CNT']))
+    assert len(cm) >= 3
+    assert sum(cm.as_dataframe()[idadb.to_def_case("CNT")].values) == 3
+    assert wacc == 0.75
+    assert 0.67 >= acc >= 0.66
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.9.4/nzpyida/analytics/tests/test_preparation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,78 @@
-
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
 # Copyright (c) 2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
-
-from nzpyida.frame import IdaDataFrame
-from nzpyida.base import IdaDataBase
-from nzpyida.analytics.model_manager import ModelManager
-from nzpyida.analytics.predictive.two_step_clustering import TwoStepClustering
-
-from nzpyida.analytics.tests.conftest import MOD_NAME, OUT_TABLE_PRED, TAB_NAME_TEST, \
-    TAB_NAME_TRAIN, df_train_clust, df_test_clust
-import pandas as pd
 import pytest
+from nzpyida.base import IdaDataBase
+from nzpyida.analytics.auto_delete_context import AutoDeleteContext
+from nzpyida.analytics.tests.conftest import OUT_TABLE_PRED
+from nzpyida.analytics.transform.preparation import std_norm, impute_data, \
+    random_sample, train_test_split
 
-OUT_TABLE_CLUST = "OUT_TABLE_CLUST"
+TAB_NAME_SPLIT_TRAIN = "TAB_NAME_SPLIT_TRAIN"
+TAB_NAME_SPLIT_TEST = "TAB_NAME_SPLIT_TEST"
 
-@pytest.fixture(scope='module')
-def mm(idadb: IdaDataBase):
-    return ModelManager(idadb)
-
-@pytest.fixture(scope='module')
-def clear_up(idadb: IdaDataBase, mm: ModelManager):
-    if mm.model_exists(MOD_NAME):
-        mm.drop_model(MOD_NAME)
+@pytest.fixture(scope='function')
+def clean_up(idadb: IdaDataBase):
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
-    if idadb.exists_table(OUT_TABLE_CLUST):
-        idadb.drop_table(OUT_TABLE_CLUST)
+    if idadb.exists_table(TAB_NAME_SPLIT_TRAIN):
+        idadb.drop_table(TAB_NAME_SPLIT_TRAIN)
+    if idadb.exists_table(TAB_NAME_SPLIT_TEST):
+        idadb.drop_table(TAB_NAME_SPLIT_TEST)
     yield
-    if mm.model_exists(MOD_NAME):
-        mm.drop_model(MOD_NAME)
     if idadb.exists_table(OUT_TABLE_PRED):
         idadb.drop_table(OUT_TABLE_PRED)
-    if idadb.exists_table(OUT_TABLE_CLUST):
-        idadb.drop_table(OUT_TABLE_CLUST)
+    if idadb.exists_table(TAB_NAME_SPLIT_TRAIN):
+        idadb.drop_table(TAB_NAME_SPLIT_TRAIN)
+    if idadb.exists_table(TAB_NAME_SPLIT_TEST):
+        idadb.drop_table(TAB_NAME_SPLIT_TEST)
+
+def test_std_norm(idadb: IdaDataBase, clean_up, idf_train):
+
+    out_df = std_norm(idf_train, in_column=['A:S'], by_column=['B'], 
+                      out_table=OUT_TABLE_PRED)
+    assert out_df
+    assert idadb.exists_table_or_view(OUT_TABLE_PRED)
+
+    assert all(out_df.columns == ['B', 'ID', 'std_A'])
+
+    assert len(out_df) == len(idf_train)
+
+
+def test_random_sample(idadb: IdaDataBase, idf_train, clean_up):
+    with AutoDeleteContext(idadb):
+        sample_df = random_sample(idf_train, size=100, by_column=["B"], rand_seed=123)
+        assert sample_df
+
+        assert all(sample_df.columns == [ 'ID', 'A', 'B'])
+
+        assert len(sample_df) == 100
+
+        sample_df2 = random_sample(idf_train, size=100, by_column=["B"], rand_seed=123)
+        sample_df3 = random_sample(idf_train, size=100, by_column=["B"])
+        assert all((sample_df.head(10) == sample_df2.head(10))['ID'])
+        assert not all((sample_df.head(10) == sample_df3.head(10))['ID'])
+
+@pytest.mark.skip
+def test_impute_data(idadb: IdaDataBase, idf_train, clean_up):
+    pass
+
 
-def test_bisecting_kmeans(idadb: IdaDataBase, mm: ModelManager, clear_up):
-    idf_train = idadb.as_idadataframe(df_train_clust, tablename=TAB_NAME_TRAIN, clear_existing=True, indexer='ID')
-    idf_test = idadb.as_idadataframe(df_test_clust, tablename=TAB_NAME_TEST, clear_existing=True, indexer='ID')
-    assert idf_train
-    assert idf_test
-
-    model = TwoStepClustering(idadb, MOD_NAME)
-    assert model
-    assert not mm.model_exists(MOD_NAME)
-    
-    model.fit(idf_train, distance='euclidean', max_k=5, bins=10, node_capacity=10, leaf_capacity=10,
-              max_leaves=100, rand_seed=4321, out_table=OUT_TABLE_CLUST)
-    assert mm.model_exists(MOD_NAME)
-
-    pred = model.predict(idf_test, out_table=OUT_TABLE_PRED)
-    assert pred
-    assert all(pred.columns == idadb.to_def_case(['ID', 'CLUSTER_ID', 'DISTANCE']))
-    assert all(list(pred.head()[idadb.to_def_case('CLUSTER_ID')].values))
+def test_train_test_split(idadb: IdaDataBase, idf_train, clean_up):
+    train_df, test_df = train_test_split(idf_train, TAB_NAME_SPLIT_TRAIN, 
+                                         TAB_NAME_SPLIT_TEST, fraction=0.8, id_column="ID")
+    assert test_df
+    assert test_df
+    assert round(len(train_df)/len(idf_train), 1) == 0.8
+    assert round(len(test_df)/len(idf_train), 1) == 0.2
 
-    score = model.score(idf_test, target_column="A")
+    train_pdf = train_df['ID'].as_dataframe()
+    assert not any(el in train_pdf.values for el in test_df["ID"].as_dataframe().values)
 
-    assert score
```

### Comparing `nzpyida-0.9.3/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.9.4/nzpyida/analytics/transform/discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.9.4/nzpyida/analytics/transform/preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/analytics/utils.py` & `nzpyida-0.9.4/nzpyida/analytics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     params['outtable'] = out_table
 
     params_s = map_to_props(params)
 
     try:
         out_query = in_df.ida_query(f'call NZA..{proc}(\'{params_s}\')')
     finally:
-        if need_delete:
+        if need_delete and in_df._idadb.exists_table_or_view(temp_view_name):
             in_df._idadb.drop_view(temp_view_name)
 
     if not in_df._idadb.exists_table_or_view(out_table):
         # stored procedure call was successful by did not produce a table
         return None, out_query
 
     if auto_delete_context:
```

### Comparing `nzpyida-0.9.3/nzpyida/base.py` & `nzpyida-0.9.4/nzpyida/base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/exceptions.py` & `nzpyida-0.9.4/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/__init__.py` & `nzpyida-0.9.4/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.9.4/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/entropy.py` & `nzpyida-0.9.4/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.9.4/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/gini.py` & `nzpyida-0.9.4/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.9.4/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/private.py` & `nzpyida-0.9.4/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.9.4/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/feature_selection/tstats.py` & `nzpyida-0.9.4/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/filtering.py` & `nzpyida-0.9.4/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/frame.py` & `nzpyida-0.9.4/nzpyida/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
 import nzpyida
 import nzpyida.statistics
 import nzpyida.indexing
 import nzpyida.aggregation
 import nzpyida.filtering
 import nzpyida.utils
+from nzpyida.groupby import IdaDataFrameGroupBy
 
 from nzpyida.utils import timed, chunklist
 from nzpyida.internals import InternalState
 from nzpyida.exceptions import IdaDataFrameError
 from nzpyida.internals import idadf_state
 
 
@@ -1228,16 +1229,40 @@
         return pivot_table(idadf=self, values=values, columns=columns,
                            max_entries=max_entries, sort=sort,
                            factor_threshold=factor_threshold,
                            interactive=interactive, aggfunc=aggfunc)
 
     @idadf_state
     def groupby(self, by):
-        # TODO: create an IdadataFrame groupby
-        raise NotImplementedError()
+        """
+        Creates the groupby object 
+        
+        Parameters
+        ----------
+        by : str
+            Column to group the Data Frame by
+        
+        Returns
+        ----------
+        IdaDataFrameGroupBy
+
+        Examples
+        --------
+        >>> ida_iris.groupby("CLASS")
+        <nzpyida.groupby.IdaDataFrameGroupBy at 0x11c288e10>
+        """
+        if by not in self.columns:
+            raise KeyError(by)
+        
+        columns_to_groupby = [col for col in self.columns if col != by]
+        
+        groupby_object = IdaDataFrameGroupBy(
+            self, columns_to_groupby, by)
+
+        return groupby_object
 
     @idadf_state
     def merge(self):
         raise NotImplementedError()
 
     @idadf_state
     def concat(self):
```

### Comparing `nzpyida-0.9.3/nzpyida/geo_frame.py` & `nzpyida-0.9.4/nzpyida/geo_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/geo_series.py` & `nzpyida-0.9.4/nzpyida/geo_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/indexing.py` & `nzpyida-0.9.4/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/internals.py` & `nzpyida-0.9.4/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/__init__.py` & `nzpyida-0.9.4/nzpyida/sampledata/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/iris.py` & `nzpyida-0.9.4/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/iris.txt` & `nzpyida-0.9.4/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/swiss.py` & `nzpyida-0.9.4/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/swiss.txt` & `nzpyida-0.9.4/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/titanic.py` & `nzpyida-0.9.4/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sampledata/titanic.txt` & `nzpyida-0.9.4/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/series.py` & `nzpyida-0.9.4/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/sql.py` & `nzpyida-0.9.4/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/statistics.py` & `nzpyida-0.9.4/nzpyida/statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/conftest.py` & `nzpyida-0.9.4/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_aggregation.py` & `nzpyida-0.9.4/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_association_rules.py` & `nzpyida-0.9.4/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_base.py` & `nzpyida-0.9.4/nzpyida/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.9.4/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_base_private.py` & `nzpyida-0.9.4/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.9.4/nzpyida/tests/test_base_table_manipulation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.9.4/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_filtering.py` & `nzpyida-0.9.4/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_frame.py` & `nzpyida-0.9.4/nzpyida/tests/test_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 import pandas
 import pytest
 import six
 
 import nzpyida
 from nzpyida import IdaDataBase
+from nzpyida.groupby import IdaDataFrameGroupBy
 
 
 class Test_OpenDataFrameObject(object):
 
     def test_idadf_attr_idadb(self, idadf):
         assert isinstance(idadf._idadb, IdaDataBase)
 
@@ -277,14 +278,15 @@
         pass
 
 
 class Test_DataExploration(object):
     ### head
     # For head and tail we do not test if the rows match because
     # the order is not guaranteed anyway
+    
     def test_idadf_head_default(self, idadb, idadf, df):
         sortkey = idadf.columns[0]
         if idadf._get_numerical_columns():
             sortkey = idadf._get_numerical_columns()[0]
 
         ida_head = idadf.head()
         assert isinstance(ida_head, pandas.core.frame.DataFrame)
@@ -429,10 +431,17 @@
 
     def test_idadf_pivot_table(self, idadf):
         pass
 
     def test_idadf_sort(self, idadf):
         pass
 
+    def test_groupby(self, idadf):
+        groupby_object = idadf.groupby("species")
+        assert isinstance(groupby_object, IdaDataFrameGroupBy)
+        grouped_idadf = groupby_object.mean()
+        assert isinstance(grouped_idadf, nzpyida.IdaDataFrame)
+        assert any([col.startswith("AVG_") for col in grouped_idadf.columns])
+
 # no test
 #__enter__
 #__exit__
```

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.9.4/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_frame_private.py` & `nzpyida-0.9.4/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_geo_frame.py` & `nzpyida-0.9.4/nzpyida/tests/test_geo_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_geo_series.py` & `nzpyida-0.9.4/nzpyida/tests/test_geo_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_indexing.py` & `nzpyida-0.9.4/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_internals.py` & `nzpyida-0.9.4/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_kmeans.py` & `nzpyida-0.9.4/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.9.4/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_series.py` & `nzpyida-0.9.4/nzpyida/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_sorting.py` & `nzpyida-0.9.4/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_statistics.py` & `nzpyida-0.9.4/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/tests/test_utils.py` & `nzpyida-0.9.4/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida/utils.py` & `nzpyida-0.9.4/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.9.3/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.9.4/nzpyida.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.9.3
+Version: 0.9.4
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Home-page: https://github.com/ibm/nzpyida
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Project-URL: Documentation, https://nzpyida.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/IBM/nzpyida
```

### Comparing `nzpyida-0.9.3/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.9.4/nzpyida.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 nzpyida/aggregation.py
 nzpyida/base.py
 nzpyida/exceptions.py
 nzpyida/filtering.py
 nzpyida/frame.py
 nzpyida/geo_frame.py
 nzpyida/geo_series.py
+nzpyida/groupby.py
 nzpyida/indexing.py
 nzpyida/internals.py
 nzpyida/series.py
 nzpyida/sql.py
 nzpyida/statistics.py
 nzpyida/utils.py
 nzpyida.egg-info/PKG-INFO
@@ -88,14 +89,15 @@
 nzpyida/analytics/tests/test_association_rules.py
 nzpyida/analytics/tests/test_auto_delete_context.py
 nzpyida/analytics/tests/test_bayesian_networks.py
 nzpyida/analytics/tests/test_bisecting_kmeans.py
 nzpyida/analytics/tests/test_cross_validation.py
 nzpyida/analytics/tests/test_decision_trees.py
 nzpyida/analytics/tests/test_discretization.py
+nzpyida/analytics/tests/test_distribution.py
 nzpyida/analytics/tests/test_glm.py
 nzpyida/analytics/tests/test_kmeans.py
 nzpyida/analytics/tests/test_knn.py
 nzpyida/analytics/tests/test_linear_regression.py
 nzpyida/analytics/tests/test_model_manager.py
 nzpyida/analytics/tests/test_naive_bayes.py
 nzpyida/analytics/tests/test_preparation.py
```

### Comparing `nzpyida-0.9.3/setup.py` & `nzpyida-0.9.4/setup.py`

 * *Files identical despite different names*

