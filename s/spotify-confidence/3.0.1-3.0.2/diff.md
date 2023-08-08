# Comparing `tmp/spotify-confidence-3.0.1.tar.gz` & `tmp/spotify-confidence-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/confidence/confidence/dist/.tmp-at_5yb94/spotify-confidence-3.0.1.tar", last modified: Fri Apr 21 12:14:39 2023, max compression
+gzip compressed data, was "/home/runner/work/confidence/confidence/dist/.tmp-dy4vhops/spotify-confidence-3.0.2.tar", last modified: Tue Aug  8 12:28:08 2023, max compression
```

## Comparing `spotify-confidence-3.0.1.tar` & `spotify-confidence-3.0.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-21 12:14:24.000000 spotify-confidence-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/confidence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chartify_grapher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chi_squared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/multiple_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/nims_and_mdes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_ratio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_size_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sequential_bound_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/t_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test_linreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/chartgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33000 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/spotify_confidence/samplesize/sample_size_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/spotify_confidence.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/bayesian/
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/bayesian/test_betabinomial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/frequentist/
--rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_chisquared.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_freqsamplesizecalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    34292 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)   132810 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ztest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/frequentist/test_ztest_linreg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/outputs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/outputs/precision/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/outputs/precision/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:14:39.000000 spotify-confidence-3.0.1/tests/samplesize/
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/samplesize/test_samplesizecalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-21 12:14:25.000000 spotify-confidence-3.0.1/tests/test_plot_precision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/bayesian_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30877 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/bayesian_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/confidence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25819 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/chartify_grapher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/chi_squared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27499 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17379 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14286 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/multiple_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/nims_and_mdes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sample_ratio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sample_size_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sequential_bound_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/t_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/z_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/z_test_linreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/chartgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence/samplesize/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/samplesize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33000 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/spotify_confidence/samplesize/sample_size_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/spotify_confidence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/bayesian/test_betabinomial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/frequentist/
+-rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_chisquared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_freqsamplesizecalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34292 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132810 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_ztest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/frequentist/test_ztest_linreg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/outputs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/outputs/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/outputs/precision/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:28:08.000000 spotify-confidence-3.0.2/tests/samplesize/
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/samplesize/test_samplesizecalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-08-08 12:27:56.000000 spotify-confidence-3.0.2/tests/test_plot_precision.py
```

### Comparing `spotify-confidence-3.0.1/LICENSE` & `spotify-confidence-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/PKG-INFO` & `spotify-confidence-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-confidence
-Version: 3.0.1
+Version: 3.0.2
 Summary: Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 Home-page: https://github.com/spotify/confidence
 Author: Per Sillren
 Author-email: pers@spotify.com
 Project-URL: Bug Tracker, https://github.com/spotify/confidence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,26 +14,26 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
+![Latest release](https://img.shields.io/badge/release-3.0.2-green.svg "Latest release: 3.0.2")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
-Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
+Spotify Confidence provides convenience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
 With Spotify Confidence it's easy to compute several p-values and confidence bounds in one go, e.g. one for each country or for each date. 
 Each function comes in two versions: 
  - one that return a pandas dataframe,
  - one that returns a [Chartify](https://github.com/spotify/chartify) chart.
 
 Spotify Confidence has support calculating p-values and confidence intervals using Z-statistics, Student's T-statistics 
 (or more exactly [Welch's T-test](https://en.wikipedia.org/wiki/Welch%27s_t-test)), as well as Chi-squared statistics.
```

### Comparing `spotify-confidence-3.0.1/README.md` & `spotify-confidence-3.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
+![Latest release](https://img.shields.io/badge/release-3.0.2-green.svg "Latest release: 3.0.2")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
-Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
+Spotify Confidence provides convenience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
 With Spotify Confidence it's easy to compute several p-values and confidence bounds in one go, e.g. one for each country or for each date. 
 Each function comes in two versions: 
  - one that return a pandas dataframe,
  - one that returns a [Chartify](https://github.com/spotify/chartify) chart.
 
 Spotify Confidence has support calculating p-values and confidence intervals using Z-statistics, Student's T-statistics 
 (or more exactly [Welch's T-test](https://en.wikipedia.org/wiki/Welch%27s_t-test)), as well as Chi-squared statistics.
```

### Comparing `spotify-confidence-3.0.1/setup.cfg` & `spotify-confidence-3.0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spotify-confidence
-version = 3.0.1
+version = 3.0.2
 author = Per Sillren
 author_email = pers@spotify.com
 description = Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spotify/confidence
 project_urls =
```

### Comparing `spotify-confidence-3.0.1/spotify_confidence/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_computer_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/abstract_base_classes/confidence_grapher_abc.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_base.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/bayesian_base.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/bayesian/bayesian_models.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/bayesian/bayesian_models.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/confidence_utils.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/confidence_utils.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/constants.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/constants.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chartify_grapher.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/chartify_grapher.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/chi_squared.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/chi_squared.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/bootstrap_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/chi_squared_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/confidence_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/sample_size_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/t_test_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/z_test_computer.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/confidence_computers/z_test_linreg_computer.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,18 @@
     XX0[0, 1 : (k + 1)] = col_sum(df[kwargs[FEATURE]])
     XX0[1 : (k + 1), 0] = col_sum(df[kwargs[FEATURE]])
 
     Xy0 = np.zeros((k + 1, 1))
     Xy0[0,] = col_sum(df[kwargs[NUMERATOR]])
     Xy0[1 : (k + 1),] = np.atleast_2d(col_sum(df[kwargs[FEATURE_CROSS]])).reshape(-1, 1)
 
-    b = np.matmul(np.linalg.inv(XX0), Xy0)
+    try:
+        b = np.matmul(np.linalg.inv(XX0), Xy0)
+    except np.linalg.LinAlgError:
+        b = np.zeros((k + 1, 1))
     out = b[1 : (k + 1)]
     if out.size == 1:
         out = out.item()
 
     outseries = Series(index=df.index, dtype=df[kwargs[FEATURE]].dtype)
     df[REGRESSION_PARAM] = outseries.apply(lambda x: out)
     return df
@@ -84,17 +87,19 @@
     variance3 = -2 * np.matmul(np.transpose(b), sample_cov).item()
 
     return variance2 + variance3
 
 
 def variance(df: DataFrame, **kwargs) -> Series:
     variance1 = z_test_computer.variance(df, **kwargs)
-
     if kwargs[FEATURE] in df:
-        return variance1 + df.apply(lin_reg_variance_delta, axis=1, **kwargs)
+        computed_variances = variance1 + df.apply(lin_reg_variance_delta, axis=1, **kwargs)
+        if (computed_variances < 0).any():
+            raise ValueError("Computed variance is negative, please check sufficient " "statistics.")
+        return computed_variances
     else:
         return variance1
 
 
 def add_point_estimate_ci(df: DataFrame, **kwargs: Dict) -> DataFrame:
     return z_test_computer.add_point_estimate_ci(df, **kwargs)
```

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/experiment.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/experiment.py`

 * *Files 27% similar despite different names*

```diff
@@ -29,14 +29,45 @@
 )
 from ..constants import BONFERRONI, NIM_TYPE, METHODS
 from ..frequentist.sample_ratio_test import sample_ratio_test
 from ...chartgrid import ChartGrid
 
 
 class Experiment(ConfidenceABC):
+    """
+    This class represents an experiment which might include several metrics and treatment groups, as well as other
+    dimensions to break down the results by. It provides several methods to analyze and visualize the results of the
+    experiment. The experiment is based on data provided as a DataFrame with sufficient statistics, such as information
+    the numerator, and denominator (number of units in the experiment) of the tested metrics and their grouping columns.
+
+    Attributes:
+        data_frame (DataFrame): DataFrame that contains the experimental data.
+        numerator_column (str): Name of the DataFrame column that contains the numerator of the tested metric.
+        numerator_sum_squares_column (Union[str, None]): Name of the DataFrame column that contains the sum of squares
+        of the numerator.
+        denominator_column (str): Name of the DataFrame column that contains the denominator of the tested metric.
+        categorical_group_columns (Union[str, Iterable]): Column(s) that categorically group the data.
+        ordinal_group_column (Union[str, None]): Column that ordinally group the data. Values need to be of
+        types int or datetime
+        interval_size (float): Size of the confidence interval. Defaults to 0.95.
+        correction_method (str): Method for correction. Defaults to "bonferroni".
+        confidence_computer (ConfidenceComputerABC): ConfidenceComputerABC object to compute confidence intervals.
+        confidence_grapher (ConfidenceGrapherABC): ConfidenceGrapherABC object to plot confidence intervals.
+        method_column (str): Column that contains the statistical test method, e.g. "z-test", "t-test".
+        bootstrap_samples_column (str): Column that contains the bootstrap samples when method is "bootstrap".
+        metric_column (str): Column that contain the names of metrics.
+        treatment_column (str): Column that contains the names of treatment and control groups.
+        power (float): Desired statistical power. Defaults to 0.8.
+        feature_column (str): Column that contains the features when method is "z-test-linreg".
+        feature_sum_squares_column (str): Column that contains the sum of squares of the features method is
+        "z-test-linreg".
+        feature_cross_sum_column (str): Column that contains the cross product sum of the features method is
+        "z-test-linreg".
+    """
+
     def __init__(
         self,
         data_frame: DataFrame,
         numerator_column: str,
         numerator_sum_squares_column: Union[str, None],
         denominator_column: str,
         categorical_group_columns: Union[str, Iterable],
```

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/multiple_comparison.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/multiple_comparison.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/nims_and_mdes.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/nims_and_mdes.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_ratio_test.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sample_ratio_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sample_size_calculator.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sample_size_calculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/sequential_bound_solver.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/sequential_bound_solver.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/t_test.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/t_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/z_test.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/analysis/frequentist/z_test_linreg.py` & `spotify-confidence-3.0.2/spotify_confidence/analysis/frequentist/z_test_linreg.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/chartgrid.py` & `spotify-confidence-3.0.2/spotify_confidence/chartgrid.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/examples.py` & `spotify-confidence-3.0.2/spotify_confidence/examples.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/options.py` & `spotify-confidence-3.0.2/spotify_confidence/options.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/samplesize/__init__.py` & `spotify-confidence-3.0.2/spotify_confidence/samplesize/__init__.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence/samplesize/sample_size_calculator.py` & `spotify-confidence-3.0.2/spotify_confidence/samplesize/sample_size_calculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/spotify_confidence.egg-info/PKG-INFO` & `spotify-confidence-3.0.2/spotify_confidence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-confidence
-Version: 3.0.1
+Version: 3.0.2
 Summary: Package for calculating and visualising confidence intervals, e.g. for A/B test analysis.
 Home-page: https://github.com/spotify/confidence
 Author: Per Sillren
 Author-email: pers@spotify.com
 Project-URL: Bug Tracker, https://github.com/spotify/confidence/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,26 +14,26 @@
 License-File: LICENSE
 License-File: AUTHORS.md
 
 Spotify Confidence
 ========
 
 ![Status](https://img.shields.io/badge/Status-Beta-blue.svg)
-![Latest release](https://img.shields.io/badge/release-3.0.1-green.svg "Latest release: 3.0.1")
+![Latest release](https://img.shields.io/badge/release-3.0.2-green.svg "Latest release: 3.0.2")
 ![Python](https://img.shields.io/badge/Python-3.7-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.8-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.9-blue.svg "Python")
 ![Python](https://img.shields.io/badge/Python-3.10-blue.svg "Python")
 
 Python library for AB test analysis.
 
 Why use Spotify Confidence?
 -----------------
 
-Spotify Confidence provides convinience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
+Spotify Confidence provides convenience wrappers around statsmodel's various functions for computing p-values and confidence intervalls. 
 With Spotify Confidence it's easy to compute several p-values and confidence bounds in one go, e.g. one for each country or for each date. 
 Each function comes in two versions: 
  - one that return a pandas dataframe,
  - one that returns a [Chartify](https://github.com/spotify/chartify) chart.
 
 Spotify Confidence has support calculating p-values and confidence intervals using Z-statistics, Student's T-statistics 
 (or more exactly [Welch's T-test](https://en.wikipedia.org/wiki/Welch%27s_t-test)), as well as Chi-squared statistics.
```

### Comparing `spotify-confidence-3.0.1/spotify_confidence.egg-info/SOURCES.txt` & `spotify-confidence-3.0.2/spotify_confidence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/bayesian/test_betabinomial.py` & `spotify-confidence-3.0.2/tests/bayesian/test_betabinomial.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_bounds.py` & `spotify-confidence-3.0.2/tests/frequentist/test_bounds.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_chisquared.py` & `spotify-confidence-3.0.2/tests/frequentist/test_chisquared.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_experiment.py` & `spotify-confidence-3.0.2/tests/frequentist/test_experiment.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_freqsamplesizecalculator.py` & `spotify-confidence-3.0.2/tests/frequentist/test_freqsamplesizecalculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_ttest.py` & `spotify-confidence-3.0.2/tests/frequentist/test_ttest.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_ztest.py` & `spotify-confidence-3.0.2/tests/frequentist/test_ztest.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/frequentist/test_ztest_linreg.py` & `spotify-confidence-3.0.2/tests/frequentist/test_ztest_linreg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+import pytest
 
 import spotify_confidence
 from spotify_confidence.analysis.constants import REGRESSION_PARAM, DECREASE_PREFFERED, METHOD_COLUMN_NAME
 
 
 class TestUnivariateSingleMetric(object):
     def setup(self):
@@ -506,9 +507,108 @@
         )
         assert (
             np.ceil(diff["required_sample_size"][0] * diff_linreg["variance_1"][0] / diff["variance_1"][0])
             == diff_linreg["required_sample_size"][0]
         )
 
 
-# TODO: Test for sequential data (w/ ordinal column)
-# TODO: Test for segmentation
+class TestUnivariateSingleMetricWithBadPreExposureData(object):
+    def setup(self):
+        np.random.seed(123)
+        n = 10000
+        d = np.random.randint(2, size=n)
+        y = 0.5 * d + np.random.standard_normal(size=n)
+        data = pd.DataFrame({"variation_name": list(map(str, d)), "y": y})
+        data = (
+            data.assign(y2=y**2)
+            .groupby(["variation_name"])
+            .agg({"y": ["sum", "count"], "y2": "sum"})
+            .assign(**{"x_sum": 0.0, "x2_sum": 0.0, "xy_sum": 0.0})
+            .reset_index()
+        )
+
+        data.columns = data.columns.map("_".join).str.strip("_")
+        data = data.assign(**{"metric_name": "metricA"})
+        self.n = n
+        self.y = y
+        self.d = d
+        self.data = data
+
+        self.test = spotify_confidence.ZTestLinreg(
+            data_frame=data,
+            numerator_column="y_sum",
+            numerator_sum_squares_column="y2_sum",
+            denominator_column="y_count",
+            categorical_group_columns=["variation_name"],
+            feature_column="x_sum",
+            feature_sum_squares_column="x2_sum",
+            feature_cross_sum_column="xy_sum",
+            interval_size=0.99,
+            correction_method="bonferroni",
+            metric_column="metric_name",
+        )
+
+    def test_summary(self):
+        summary_df = self.test.summary(verbose=True)
+        print(summary_df)
+        assert len(summary_df) == len(self.data)
+
+    def test_parameters_univariate(self):
+        summary_df = self.test.summary(verbose=True)
+        assert np.allclose(0.0, summary_df[REGRESSION_PARAM][0], rtol=0.0001)
+
+        diff = self.test.difference(level_1="0", level_2="1", verbose=True, groupby="metric_name")
+        y = self.y
+        d = self.d
+        assert np.allclose(y[d == 1].mean() - y[d == 0].mean(), diff["difference"])
+
+        v0 = np.var(y[d == 0])
+        v1 = np.var(y[d == 1])
+        n0 = y[d == 0].size
+        n1 = y[d == 1].size
+        assert np.allclose(diff["std_err"], np.sqrt(v0 / n0 + v1 / n1), rtol=1e-3)
+
+
+class TestUnivariateSingleMetricNegativeVariance(object):
+    def setup(self):
+        self.data = pd.DataFrame(
+            [
+                {
+                    "group": "1",
+                    "count": 17512,
+                    "sum": 16544,
+                    "sum_of_squares": 16044,
+                    "sum_2": 6625,
+                    "sum_of_squares_2": 6455,
+                    "sum_of_squares_x": 3513,
+                    "metric_name": "metricA",
+                },
+                {
+                    "group": "2",
+                    "count": 159142,
+                    "sum": 150364,
+                    "sum_of_squares": 145794,
+                    "sum_2": 60540,
+                    "sum_of_squares_2": 59047,
+                    "sum_of_squares_x": 32398,
+                    "metric_name": "metricA",
+                },
+            ]
+        )
+
+        self.test = spotify_confidence.ZTestLinreg(
+            data_frame=self.data,
+            numerator_column="sum",
+            numerator_sum_squares_column="sum_of_squares",
+            denominator_column="count",
+            categorical_group_columns=["group"],
+            feature_column="sum_2",
+            feature_sum_squares_column="sum_of_squares_2",
+            feature_cross_sum_column="sum_of_squares_x",
+            interval_size=0.99,
+            correction_method="bonferroni",
+            metric_column="metric_name",
+        )
+
+    def test_setup_that_will_fail_with_negative_variance(self):
+        with pytest.raises(ValueError):
+            self.test.summary(verbose=True)
```

### Comparing `spotify-confidence-3.0.1/tests/samplesize/test_samplesizecalculator.py` & `spotify-confidence-3.0.2/tests/samplesize/test_samplesizecalculator.py`

 * *Files identical despite different names*

### Comparing `spotify-confidence-3.0.1/tests/test_plot_precision.py` & `spotify-confidence-3.0.2/tests/test_plot_precision.py`

 * *Files identical despite different names*

