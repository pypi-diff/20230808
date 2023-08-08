# Comparing `tmp/ProcessOptimizer-0.8.1.tar.gz` & `tmp/ProcessOptimizer-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessOptimizer-0.8.1.tar", last modified: Thu Jun 22 06:57:36 2023, max compression
+gzip compressed data, was "ProcessOptimizer-0.8.2.tar", last modified: Tue Aug  8 10:56:34 2023, max compression
```

## Comparing `ProcessOptimizer-0.8.1.tar` & `ProcessOptimizer-0.8.2.tar`

### file list

```diff
@@ -1,50 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/
--rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/AUTHORS_scikit_optimize.md
--rw-rw-rw-   0        0        0     1598 2023-02-14 09:41:21.000000 ProcessOptimizer-0.8.1/LICENSE.md
--rw-rw-rw-   0        0        0    10809 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.428574 ProcessOptimizer-0.8.1/ProcessOptimizer/
--rw-rw-rw-   0        0        0     1845 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/__init__.py
--rw-rw-rw-   0        0        0    11574 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/acquisition.py
--rw-rw-rw-   0        0        0    29142 2022-03-10 13:53:50.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/bokeh_plot.py
--rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.458753 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/
--rw-rw-rw-   0        0        0      425 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/__init__.py
--rw-rw-rw-   0        0        0    18835 2023-01-26 13:09:11.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/forest.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.480910 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/
--rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/__init__.py
--rw-rw-rw-   0        0        0    17518 2023-06-07 11:59:09.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/gpr.py
--rw-rw-rw-   0        0        0    15220 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/kernels.py
--rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gbrt.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.541304 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/
--rw-rw-rw-   0        0        0        0 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/__init__.py
--rw-rw-rw-   0        0        0     7547 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/benchmarks.py
--rw-rw-rw-   0        0        0      605 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/branin_hoo.py
--rw-rw-rw-   0        0        0     4455 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/model_system.py
--rw-rw-rw-   0        0        0     7440 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/noise_models.py
--rw-rw-rw-   0        0        0     1359 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.591637 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/
--rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/_NSGA2.py
--rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/__init__.py
--rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/base.py
--rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/dummy.py
--rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/forest.py
--rw-rw-rw-   0        0        0     6836 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gbrt.py
--rw-rw-rw-   0        0        0    10770 2023-05-16 08:56:50.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gp.py
--rw-rw-rw-   0        0        0    50046 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/optimizer.py
--rw-rw-rw-   0        0        0    89768 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/plots.py
--rw-rw-rw-   0        0        0    28205 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/searchcv.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.640006 ProcessOptimizer-0.8.1/ProcessOptimizer/space/
--rw-rw-rw-   0        0        0       71 2021-07-29 06:17:13.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/__init__.py
--rw-rw-rw-   0        0        0    41031 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/constraints.py
--rw-rw-rw-   0        0        0    30787 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/space.py
--rw-rw-rw-   0        0        0     5265 2023-05-02 07:34:39.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/transformers.py
--rw-rw-rw-   0        0        0    33016 2023-03-30 10:22:43.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.440656 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/
--rw-rw-rw-   0        0        0    10809 2023-06-22 06:57:34.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1449 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10361 2023-05-16 08:56:50.000000 ProcessOptimizer-0.8.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.943652 ProcessOptimizer-0.8.2/
+-rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/AUTHORS_scikit_optimize.md
+-rw-rw-rw-   0        0        0     1598 2023-02-14 09:41:21.000000 ProcessOptimizer-0.8.2/LICENSE.md
+-rw-rw-rw-   0        0        0    10786 2023-08-08 10:56:34.940569 ProcessOptimizer-0.8.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.467777 ProcessOptimizer-0.8.2/ProcessOptimizer/
+-rw-rw-rw-   0        0        0     1868 2023-08-08 10:41:30.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/__init__.py
+-rw-rw-rw-   0        0        0    11574 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/acquisition.py
+-rw-rw-rw-   0        0        0    29142 2022-03-10 13:53:50.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/bokeh_plot.py
+-rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.576212 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/
+-rw-rw-rw-   0        0        0      609 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/__init__.py
+-rw-rw-rw-   0        0        0     4461 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/cook_estimator.py
+-rw-rw-rw-   0        0        0    18829 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/forest.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.621343 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/
+-rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/__init__.py
+-rw-rw-rw-   0        0        0    17518 2023-06-07 11:59:09.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/gpr.py
+-rw-rw-rw-   0        0        0    15220 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/kernels.py
+-rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gbrt.py
+-rw-rw-rw-   0        0        0     1018 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/has_gradients.py
+-rw-rw-rw-   0        0        0     5785 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/learning/use_named_args.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.729210 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/
+-rw-rw-rw-   0        0        0      876 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/__init__.py
+-rw-rw-rw-   0        0        0     1579 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/benchmarks.py
+-rw-rw-rw-   0        0        0     1625 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/branin_hoo.py
+-rw-rw-rw-   0        0        0      799 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/gold_map.py
+-rw-rw-rw-   0        0        0     1650 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/hart3.py
+-rw-rw-rw-   0        0        0     2021 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/hart6.py
+-rw-rw-rw-   0        0        0     5149 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/model_system.py
+-rw-rw-rw-   0        0        0     8658 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/noise_models.py
+-rw-rw-rw-   0        0        0     1322 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/peaks.py
+-rw-rw-rw-   0        0        0     1186 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/poly2.py
+-rw-rw-rw-   0        0        0     1362 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.878703 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/
+-rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/_NSGA2.py
+-rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/__init__.py
+-rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/base.py
+-rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/dummy.py
+-rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/forest.py
+-rw-rw-rw-   0        0        0     6798 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/gbrt.py
+-rw-rw-rw-   0        0        0    10870 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/gp.py
+-rw-rw-rw-   0        0        0    49207 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0    89768 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/plots.py
+-rw-rw-rw-   0        0        0    28205 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/searchcv.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.930366 ProcessOptimizer-0.8.2/ProcessOptimizer/space/
+-rw-rw-rw-   0        0        0      127 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/space/__init__.py
+-rw-rw-rw-   0        0        0    41015 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/space/constraints.py
+-rw-rw-rw-   0        0        0     2582 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/space/normalize_dimensions.py
+-rw-rw-rw-   0        0        0    30914 2023-08-08 10:33:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/space/space.py
+-rw-rw-rw-   0        0        0     5265 2023-05-02 07:34:39.000000 ProcessOptimizer-0.8.2/ProcessOptimizer/space/transformers.py
+drwxrwxrwx   0        0        0        0 2023-08-08 10:56:34.500266 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/
+-rw-rw-rw-   0        0        0    10786 2023-08-08 10:56:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1804 2023-08-08 10:56:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 10:56:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-08-08 10:56:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-08 10:56:32.000000 ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10361 2023-05-16 08:56:50.000000 ProcessOptimizer-0.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-08 10:56:34.945634 ProcessOptimizer-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1580 2023-08-08 10:41:12.000000 ProcessOptimizer-0.8.2/setup.py
```

### Comparing `ProcessOptimizer-0.8.1/AUTHORS_scikit_optimize.md` & `ProcessOptimizer-0.8.2/AUTHORS_scikit_optimize.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/LICENSE.md` & `ProcessOptimizer-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/PKG-INFO` & `ProcessOptimizer-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.8.1
+Version: 0.8.2
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Description-Content-Type: text/markdown
-Provides-Extra: bokeh
 Provides-Extra: browniebee
 License-File: LICENSE.md
 License-File: AUTHORS_scikit_optimize.md
 
 <div align="center">
 <pre>
   _____                              ____        _   _           _
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.1 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.2 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Description-Content-Type: text/
-markdown Provides-Extra: bokeh Provides-Extra: browniebee License-File:
-LICENSE.md License-File: AUTHORS_scikit_optimize.md
+markdown Provides-Extra: browniebee License-File: LICENSE.md License-File:
+AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
 
        |  __ \                            / __ \      | | (_)         (_)
 
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __
 
    |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/__init__.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,32 @@
 from . import acquisition
 from .model_systems import benchmarks
 from . import callbacks
 from . import learning
 from . import optimizer
 
 from . import space
+from .learning import cook_estimator
 from .optimizer import dummy_minimize
 from .optimizer import forest_minimize
 from .optimizer import gbrt_minimize
 from .optimizer import gp_minimize
 from .optimizer import Optimizer
 from .searchcv import BayesSearchCV
 from .space import Space, space_factory
 from .utils import dump
 from .utils import expected_minimum
 from .utils import expected_minimum_random_sampling
 from .utils import load
-from .utils import cook_estimator, create_result, y_coverage
+from .utils import create_result, y_coverage
 from .plots import plot_objective, plot_objectives
 from .plots import plot_evaluations, plot_convergence
 from .plots import plot_Pareto, plot_expected_minimum_convergence
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 
 __all__ = (
     "acquisition",
     "benchmarks",
     "callbacks",
     "learning",
@@ -64,9 +65,9 @@
     "space_factory",
     "plot_objective",
     "plot_objectives",
     "plot_evaluations",
     "plot_convergence",
     "plot_Pareto",
     "y_coverage",
-    "plot_expected_minimum_convergence"
+    "plot_expected_minimum_convergence",
 )
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/acquisition.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/acquisition.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/bokeh_plot.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/callbacks.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/callbacks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/forest.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/learning/forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     References
     ----------
     .. [1] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
     """
 
     def __init__(self, n_estimators=10, criterion='squared_error', max_depth=None,
                  min_samples_split=2, min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0, max_features='auto',
+                 min_weight_fraction_leaf=0.0, max_features=1.0,
                  max_leaf_nodes=None, bootstrap=True, oob_score=False,
                  n_jobs=1, random_state=None, verbose=0, warm_start=False,
                  min_variance=0.0):
         self.min_variance = min_variance
         super(RandomForestRegressor, self).__init__(
             n_estimators=n_estimators, criterion=criterion,
             max_depth=max_depth,
@@ -368,15 +368,15 @@
     References
     ----------
     .. [1] L. Breiman, "Random Forests", Machine Learning, 45(1), 5-32, 2001.
     """
 
     def __init__(self, n_estimators=10, criterion='squared_error', max_depth=None,
                  min_samples_split=2, min_samples_leaf=1,
-                 min_weight_fraction_leaf=0.0, max_features='auto',
+                 min_weight_fraction_leaf=0.0, max_features=1.0,
                  max_leaf_nodes=None, bootstrap=False, oob_score=False,
                  n_jobs=1, random_state=None, verbose=0, warm_start=False,
                  min_variance=0.0):
         self.min_variance = min_variance
         super(ExtraTreesRegressor, self).__init__(
             n_estimators=n_estimators, criterion=criterion,
             max_depth=max_depth,
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/gpr.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/kernels.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gaussian_process/kernels.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gbrt.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/learning/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/noise_models.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/noise_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,136 @@
 from abc import ABC, abstractmethod
 from typing import Callable, List, Union, Optional
 
 import numpy as np
 
+
 class NoiseModel(ABC):
     """
     Abstract class that is the basis for noise models.
     """
+
     def __init__(
         self,
         noise_size: Optional[float],
         seed: Optional[int] = 42,
     ):
-        """        
+        """
         Parameters
         ----------
-        * `noise_size` [Optional[float]]: 
+        * `noise_size` [Optional[float]]:
             The size (magnitude) of the noise. If ´None´, it signifies that
-            the class is compound, and should not have its own noise signal, 
-            but refer to its compounding NoiseModels instead. An example is 
+            the class is compound, and should not have its own noise signal,
+            but refer to its compounding NoiseModels instead. An example is
             SumNoise, which sums the noise of a list of noise models, but does
             not add any noise by itself.
-        
+
         * `seed` [Optional[int], default=42]:
             Seed to pass forward to the numpy random number generator that is
             used when providing samples with noise.
         """
         # We could just set noise_dist and let that have a size, but being able to
         # directly set the size is more intuitive, and that would be complicated if it
         # was just one variable.
         # Note that this has the potential for problems if _noise_distribution does not
         # have "size" 1, but as long as it is only set by set_noise_type(), it should be
         # safe.
         self.noise_size = noise_size
         self._rng = np.random.default_rng(seed)
+        # Change this to ..utils.get_random_genertor once the pull request with that have been merged
         self.set_noise_type("normal")
-        self._noise_distribution: Callable[[], float]
 
     @abstractmethod
     def get_noise(self, X, Y: float) -> float:
         pass
-    
+
     @property
     def _sample_noise(self) -> float:
         """A raw noise value, to be used in the get_noise() function."""
         if self.noise_size is None:
-            raise TypeError("Method \"raw_noise()\" for NoiseModel class "
-                            f"{self.__class__.__name__} is not supposed to be called.")
-            
-        return self._noise_distribution()*self.noise_size
-    
+            raise TypeError(
+                'Method "raw_noise()" for NoiseModel class '
+                f"{self.__class__.__name__} is not supposed to be called."
+            )
+
+        return self._noise_distribution() * self.noise_size
+
     def set_noise_type(self, noise_type: str):
-        if noise_type in ["normal", "Gaussian", "norm"]:
+        if noise_type in ["normal", "Gaussian", "norm", "uniform"]:
             self.noise_type = noise_type
-            self._noise_distribution = self._rng.normal
-        elif noise_type == "uniform":
-            self.noise_type = noise_type
-            self._noise_distribution = lambda: self._rng.uniform(low=-1, high=1)
         else:
-            raise ValueError(f"Noise distribution \"{noise_type}\" not recognised.")
-    
+            raise ValueError(f'Noise distribution "{noise_type}" not recognised.')
+
     def set_seed(self, seed: Optional[int]):
         # Instantiate the random number generator again
         self._rng = np.random.default_rng(seed)
-        # Make sure to do the same for the noise distribution
+
+    @property
+    def _noise_distribution(self) -> Callable[[], float]:
         if self.noise_type in ["normal", "Gaussian", "norm"]:
-            self._noise_distribution = self._rng.normal
+            return self._rng.normal
         elif self.noise_type == "uniform":
-            self._noise_distribution = lambda: self._rng.uniform(low=-1, high=1)
+            return lambda: self._rng.uniform(low=-1, high=1)
+        else:
+            raise ValueError(f'Noise distribution "{self.noise_type}" not recognised.')
+
 
 class ConstantNoise(NoiseModel):
     """
     Noise model for noise that is independent of both the sampled point and the
     resulting score; The noise is constant. Another name is "additive noise", as the
     same noise is added to the score. This is typical for many measurements.
 
     Parameters
     ----------
-    * `noise_size` [float, default=1]: 
-        The size (magnitude) of the noise. 
+    * `noise_size` [float, default=1]:
+        The size (magnitude) of the noise.
     """
+
     def __init__(self, noise_size: float = 1, **kwargs):
         super().__init__(noise_size=noise_size, **kwargs)
 
     def get_noise(self, _, Y: float) -> float:
         return self._sample_noise
 
-    
+
 class ProportionalNoise(NoiseModel):
     """
     Noise model for noise proportional to the signal, but independent of the sampled
     point. Another name is "multiplicative noise", as the same noise is multiplied with
     the score. This is typical of some electronic measurements.
 
     Parameters
     ----------
-    * `noise_size` [float, default=0.1]: 
+    * `noise_size` [float, default=0.1]:
         The size of the noise relative to the signal.
     """
-    def __init__(self, noise_size : float = 0.1, **kwargs):
+
+    def __init__(self, noise_size: float = 0.1, **kwargs):
         super().__init__(noise_size=noise_size, **kwargs)
-    
+
     def get_noise(self, _, Y: float) -> float:
-        return self._sample_noise*Y
-    
+        return self._sample_noise * Y
+
 
 class DataDependentNoise(NoiseModel):
     """
     Noise model for noise that depends on the input parameters.
 
     Parameters
     ----------
-    * `noise_function` [(parameters) -> NoiseModel]: 
-        A function that takes a set of parameters, and returns a noise model to 
+    * `noise_function` [(parameters) -> NoiseModel]:
+        A function that takes a set of parameters, and returns a noise model to
         apply.
+    * `overwrite_rng` [bool, default=True]:
+        Whether to overwrite the random number generator of underlying noise models.
+        This is necessary if the underlying noise models are created each time
+        `noise_function()` is called, since they will otherwise have the same random
+        seed. If the underlying noise models are created once, this can be set to
+        False to not mess with the underlying noise models.
 
     Examples
     --------
     To make additive noise proportional to the input parameter (not to the score):
     ```
     noise_choice = lambda X: ConstantNoise(noise_size=X)
     noise_model = DataDependentNoise(noise_function=noise_choice)
@@ -125,69 +138,103 @@
 
     To add constant noise except if X[0] is 0:
     ```
     noise_choice = lambda X: ZeroNoise() if X[0]==0 else ConstantNoise()
     noise_model = DataDependentNoise(noise_function=noise_choice)
     ```
     """
-    def __init__(self, noise_function: Callable[..., NoiseModel], **kwargs):
-        self.noise_function = noise_function
+
+    def __init__(
+        self,
+        noise_function: Callable[..., NoiseModel],
+        overwrite_rng: bool = True,
+        **kwargs,
+    ):
         super().__init__(noise_size=None, **kwargs)
-    
+        self.noise_function = noise_function
+        self.overwrite_rng = overwrite_rng
+
     def get_noise(self, X, Y: float) -> float:
-        return self.noise_function(X).get_noise(X, Y)           
-    
+        noise_model = self.noise_function(X)
+        if self.overwrite_rng:
+            noise_model._rng = self._rng
+        return noise_model.get_noise(X, Y)
+
+
 class ZeroNoise(NoiseModel):
     """
     Noise model for zero noise. Doesn't take any arguments. Exist for consistency,
     and to be used in data dependent noise models.
     """
+
     def __init__(self):
         super().__init__(noise_size=0)
 
     def get_noise(self, _, Y: float) -> float:
         return 0
 
+
 class SumNoise(NoiseModel):
     """
     Noise model that returns the sum of two or more noise models. Can be used if the
     total noise is a sum of constant and proportional noise.
 
     Parameters
     ----------
-    * `noise_model_list` [List[Union[dict, NoiseModel]]]: 
-        List of either noise models, or dicts containing at least the type of 
+    * `noise_model_list` [List[Union[dict, NoiseModel]]]:
+        List of either noise models, or dicts containing at least the type of
         noise model to create.
+    * `overwrite_rng` [bool, default=True]:
+        Whether to overwrite the random number generator of underlying noise models.
+        This is necessary if the underlying noise models are created with the same seed,
+        which they are by default, since they will otherwise give correlated noise.
 
     """
-    def __init__(self,noise_model_list: List[Union[str,dict,NoiseModel]], **kwargs):
-        super().__init__(noise_size = None,**kwargs)
+
+    def __init__(
+        self,
+        noise_model_list: List[Union[str, dict, NoiseModel]],
+        overwrite_rng: bool = True,
+        **kwargs,
+    ):
+        super().__init__(noise_size=None, **kwargs)
         self.noise_model_list: List[NoiseModel]
+        self.overwrite_rng = overwrite_rng
         self.set_noise_model_list(noise_model_list=noise_model_list)
 
-    def set_noise_model_list(self, noise_model_list: List[Union[dict, NoiseModel]]):
+    def set_noise_model_list(
+        self, noise_model_list: List[Union[str, dict, NoiseModel]]
+    ):
         self.noise_model_list = []
         for model_description in noise_model_list:
             self.noise_model_list.append(parse_noise_model(model_description))
+        if self.overwrite_rng:
+            for model in self.noise_model_list:
+                model._rng = self._rng
 
     def get_noise(self, X, Y: float) -> float:
         noise_list = [model.get_noise(X, Y) for model in self.noise_model_list]
         return sum(noise_list)
 
 
-def parse_noise_model(model: Union[str, dict, NoiseModel], **kwargs) -> NoiseModel:
+def parse_noise_model(
+    model: Union[str, dict, NoiseModel, None], **kwargs
+) -> NoiseModel:
     if isinstance(model, NoiseModel):
         return model
-    elif type(model) == str:
+    elif isinstance(model, str):
         return noise_model_factory(model_type=model, **kwargs)
+    elif model is None:
+        return noise_model_factory(model_type="zero")
     else:
         return noise_model_factory(**model)
 
+
 def noise_model_factory(model_type: str, **kwargs) -> NoiseModel:
     if model_type == "constant":
         return ConstantNoise(**kwargs)
     elif model_type == "proportional":
         return ProportionalNoise(**kwargs)
-    elif model_type == "zero":
+    elif model_type in ["zero", "none"]:
         return ZeroNoise()
     else:
-        raise ValueError(f"Noise model of type '{model_type}' not recognised")
+        raise ValueError(f"Noise model of type '{model_type}' not recognised")
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/second_order_polynomial_2d.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/model_systems/second_order_polynomial_2d.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import numpy as np
 from ProcessOptimizer.model_systems import ModelSystem
 from ProcessOptimizer.model_systems.benchmarks import poly_2d
 from ProcessOptimizer.space import Real
 
+
 # This system is intended to run in the domain x[0] in [-1,1] and x[1] in [-1,1]. This function
-# has its minimum in this domain at (0.6667,-0.4833), with a value of 
+# has its minimum in this domain at (0.6667,-0.4833), with a value of
 # about -2.0512, and its maximum in this domain at (-1,-1) with a value of -1.27
 def score(x, rng=np.random.default_rng(), noise_std=0.02):
     """Calculate the score of the model system
 
     Parameters:
     * x [array of length 2 containing numbers between -1 and 1]:
-        The point in the parameter space at which to calculate the score. 
+        The point in the parameter space at which to calculate the score.
     * rng [np.random Generator]:
-        Random number generator used to generate noise. 
-    * noise_std [float]: 
-        Standard deviation of the noise which is added to the result of the polynomial. 
+        Random number generator used to generate noise.
+    * noise_std [float]:
+        Standard deviation of the noise which is added to the result of the polynomial.
     """
     value = poly_2d(x) + rng.normal(scale=noise_std)
     return value
 
+
 # The location of the minimum in the parameter space:
-true_min_loc = [2/3, -0.4833]
+true_min_loc = [2 / 3, -0.4833]
 # The true minimum value
 true_min = score(true_min_loc, noise_std=0)
 
 # Define a the domain as a Space object
 space = []
-space += [Real(-1, 1, name='x1')]
-space += [Real(-1, 1, name='x2')]
+space += [Real(-1, 1, name="x1")]
+space += [Real(-1, 1, name="x2")]
 
 # Create model system
-polynomial_system_2d = ModelSystem(score, space, true_min)
+polynomial_system_2d = ModelSystem(score, space, true_min)
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/_NSGA2.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/_NSGA2.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/base.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/dummy.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/dummy.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/forest.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gbrt.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/gbrt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,31 @@
-
 from sklearn.utils import check_random_state
 
 from .base import base_minimize
-from ..utils import cook_estimator
+from ..learning import cook_estimator
 
 
-def gbrt_minimize(func, dimensions, base_estimator=None,
-                  n_calls=100, n_random_starts=10,
-                  acq_func="EI", acq_optimizer="auto",
-                  x0=None, y0=None, random_state=None, verbose=False,
-                  callback=None, n_points=10000, xi=0.01, kappa=1.96,
-                  n_jobs=1):
+def gbrt_minimize(
+    func,
+    dimensions,
+    base_estimator=None,
+    n_calls=100,
+    n_random_starts=10,
+    acq_func="EI",
+    acq_optimizer="auto",
+    x0=None,
+    y0=None,
+    random_state=None,
+    verbose=False,
+    callback=None,
+    n_points=10000,
+    xi=0.01,
+    kappa=1.96,
+    n_jobs=1,
+):
     """Sequential optimization using gradient boosted trees.
 
     Gradient boosted regression trees are used to model the (very)
     expensive to evaluate function `func`. The model is improved
     by sequentially evaluating the expensive function at the next
     best point. Thereby finding the minimum of `func` with as
     few evaluations as possible.
@@ -139,15 +150,25 @@
         For more details related to the OptimizeResult object, refer
         http://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.OptimizeResult.html
     """
     # Check params
     rng = check_random_state(random_state)
 
     if base_estimator is None:
-        base_estimator = cook_estimator("GBRT", random_state=rng,
-                                        n_jobs=n_jobs)
-    return base_minimize(func, dimensions, base_estimator,
-                         n_calls=n_calls, n_points=n_points,
-                         n_random_starts=n_random_starts,
-                         x0=x0, y0=y0, random_state=random_state, xi=xi,
-                         kappa=kappa, acq_func=acq_func, verbose=verbose,
-                         callback=callback, acq_optimizer="sampling")
+        base_estimator = cook_estimator("GBRT", random_state=rng, n_jobs=n_jobs)
+    return base_minimize(
+        func,
+        dimensions,
+        base_estimator,
+        n_calls=n_calls,
+        n_points=n_points,
+        n_random_starts=n_random_starts,
+        x0=x0,
+        y0=y0,
+        random_state=random_state,
+        xi=xi,
+        kappa=kappa,
+        acq_func=acq_func,
+        verbose=verbose,
+        callback=callback,
+        acq_optimizer="sampling",
+    )
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gp.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 """Gaussian process-based minimization algorithms."""
 
 import numpy as np
 
 from sklearn.utils import check_random_state
 
 from .base import base_minimize
-from ..utils import cook_estimator
-from ..utils import normalize_dimensions
+from ..learning import cook_estimator
+from ..space import normalize_dimensions
 
 
-def gp_minimize(func, dimensions, base_estimator=None,
-                n_calls=100, n_random_starts=10,
-                acq_func="EI", acq_optimizer="auto", x0=None, y0=None,
-                random_state=None, verbose=False, callback=None,
-                n_points=10000, n_restarts_optimizer=5, xi=0.01, kappa=1.96,
-                noise="gaussian", n_jobs=1):
+def gp_minimize(
+    func,
+    dimensions,
+    base_estimator=None,
+    n_calls=100,
+    n_random_starts=10,
+    acq_func="EI",
+    acq_optimizer="auto",
+    x0=None,
+    y0=None,
+    random_state=None,
+    verbose=False,
+    callback=None,
+    n_points=10000,
+    n_restarts_optimizer=5,
+    xi=0.01,
+    kappa=1.96,
+    noise="gaussian",
+    n_jobs=1,
+):
     """Bayesian optimization using Gaussian Processes.
 
     If every function evaluation is expensive, for instance
     when the parameters are the hyperparameters of a neural network
     and the function evaluation is the mean cross-validation score across
     ten folds, optimizing the hyperparameters by standard optimization
     routines would take for ever!
@@ -211,21 +225,32 @@
     """
     # Check params
     rng = check_random_state(random_state)
     space = normalize_dimensions(dimensions)
 
     if base_estimator is None:
         base_estimator = cook_estimator(
-            "GP", space=space, random_state=rng.randint(
-              0, np.iinfo(np.int32).max
-              ),
-            noise=noise
-            )
+            "GP",
+            space=space,
+            random_state=rng.randint(0, np.iinfo(np.int32).max),
+            noise=noise,
+        )
 
     return base_minimize(
-        func, space, base_estimator=base_estimator,
+        func,
+        space,
+        base_estimator=base_estimator,
         acq_func=acq_func,
-        xi=xi, kappa=kappa, acq_optimizer=acq_optimizer, n_calls=n_calls,
-        n_points=n_points, n_random_starts=n_random_starts,
+        xi=xi,
+        kappa=kappa,
+        acq_optimizer=acq_optimizer,
+        n_calls=n_calls,
+        n_points=n_points,
+        n_random_starts=n_random_starts,
         n_restarts_optimizer=n_restarts_optimizer,
-        x0=x0, y0=y0, random_state=rng, verbose=verbose,
-        callback=callback, n_jobs=n_jobs)
+        x0=x0,
+        y0=y0,
+        random_state=rng,
+        verbose=verbose,
+        callback=callback,
+        n_jobs=n_jobs,
+    )
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/optimizer.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/optimizer/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,40 @@
 from sklearn.base import clone
 from sklearn.base import is_regressor
 from sklearn.multioutput import MultiOutputRegressor
 from sklearn.utils import check_random_state
 
 from ..acquisition import _gaussian_acquisition
 from ..acquisition import gaussian_acquisition_1D
-from ..learning import GaussianProcessRegressor
+from ..learning import cook_estimator, GaussianProcessRegressor, has_gradients
 from ..space import Categorical
-from ..space import Space
+from ..space import Space, normalize_dimensions
 from ..space.constraints import Constraints, SumEquals
 from ..utils import check_x_in_space
-from ..utils import cook_estimator
 from ..utils import create_result
-from ..utils import has_gradients
 from ..utils import is_listlike
 from ..utils import is_2Dlistlike
-from ..utils import normalize_dimensions
 
 from ..learning.gaussian_process.gpr import _param_for_white_kernel_in_Sum
 from ..learning.gaussian_process.kernels import WhiteKernel
 
 
 class Optimizer(object):
     """Run bayesian optimisation loop.
 
     An `Optimizer` represents the steps of a bayesian optimisation loop. To
     use it you need to provide your own loop mechanism. The various
     optimisers provided by `ProcessOptimizer` use this class under the hood.
 
     Use this class directly if you want to control the iterations of your
     bayesian optimisation loop.
-    
+
     In default behavior, the optimizer will reset the modelled experimental
     noise between each refitting (read: while adding new data). This is
-    described in Rasmussen and Williams chapter 2. 
+    described in Rasmussen and Williams chapter 2.
     Some users might want to plot, predict or sample from a model that includes
     the modelling of the experimental noise: in that case, two helper methods
     can "switch" the noise "on/off". Functions are called 'add_modelled_noise'
     and 'remove_modelled_noise'.
 
     Parameters
     ----------
@@ -78,16 +75,16 @@
     * `n_initial_points` [int, default=10]:
         Number of evaluations of `func` with initialization points
         before approximating it with `base_estimator`. Points provided as
         `x0` count as initialization points. If len(x0) < n_initial_points
         additional points are sampled at random.
 
     * `lhs` [bool, default = True]:
-        If set to True, the optimizer will use latin hypercube sampling for the 
-        first n_initial_points. If set to False, the optimizer will return 
+        If set to True, the optimizer will use latin hypercube sampling for the
+        first n_initial_points. If set to False, the optimizer will return
         random points
 
     * `acq_func` [string, default=`"EI"`]:
         Function to minimize over the posterior distribution. Can be either
 
         - `"LCB"` for lower confidence bound.
         - `"EI"` for negative expected improvement.
@@ -137,17 +134,17 @@
     * `acq_optimizer_kwargs` [dict]:
         Additional arguments to be passed to the acquistion optimizer.
         options are:
         - "length_scale_bounds" [list] a list of tuples with lower and upper bound
         -  "length_scale" [list] a list of floats
         - "n_restarts_optimizer" [int]
         - "n_jobs" [int]
-        
+
     * `n_objectives` [int, default=1]:
-        Number of objectives to be optimized. 
+        Number of objectives to be optimized.
         When n_objectives>1 the optimizer will fit models for each objective and the Pareto front can be approximated using NSGA2
 
 
 
     Attributes
     ----------
     * `Xi` [list]:
@@ -207,18 +204,15 @@
         self.eta = acq_func_kwargs.get("eta", 1.0)
 
         # Configure counters of points
 
         # Check `n_random_starts` deprecation first
         if n_random_starts is not None:
             warnings.warn(
-                (
-                    "n_random_starts will be removed in favour of "
-                    "n_initial_points."
-                ),
+                ("n_random_starts will be removed in favour of " "n_initial_points."),
                 DeprecationWarning,
             )
             n_initial_points = n_random_starts
 
         if n_initial_points < 0:
             raise ValueError(
                 "Expected `n_initial_points` >= 0, got %d" % n_initial_points
@@ -231,17 +225,15 @@
             acq_optimizer_kwargs = dict()
 
         self._length_scale_bounds = acq_optimizer_kwargs.get(
             "length_scale_bounds", None
         )
         self._length_scale = acq_optimizer_kwargs.get("length_scale", None)
         self.n_points = acq_optimizer_kwargs.get("n_points", 10000)
-        self.n_restarts_optimizer = acq_optimizer_kwargs.get(
-            "n_restarts_optimizer", 5
-        )
+        self.n_restarts_optimizer = acq_optimizer_kwargs.get("n_restarts_optimizer", 5)
         n_jobs = acq_optimizer_kwargs.get("n_jobs", 1)
         self.n_jobs = n_jobs
         self.acq_optimizer_kwargs = acq_optimizer_kwargs
 
         # Configure estimator
         self._check_length_scale_bounds(dimensions, self._length_scale_bounds)
         # build base_estimator if doesn't exist
@@ -276,18 +268,15 @@
 
         if acq_optimizer not in ["lbfgs", "sampling"]:
             raise ValueError(
                 "Expected acq_optimizer to be 'lbfgs' or "
                 "'sampling', got {0}".format(acq_optimizer)
             )
 
-        if (
-            not has_gradients(self.base_estimator_)
-            and acq_optimizer != "sampling"
-        ):
+        if not has_gradients(self.base_estimator_) and acq_optimizer != "sampling":
             raise ValueError(
                 "The regressor {0} should run with "
                 "acq_optimizer"
                 "='sampling'.".format(type(base_estimator))
             )
         self.acq_optimizer = acq_optimizer
 
@@ -381,23 +370,23 @@
             parallel, and thus obtain more objective function evaluations per
             unit of time.
 
         * `strategy` [string, default=`stbr_fill`]:
             Method to use to sample multiple points (see also `n_points`
             description). This parameter is ignored if n_points = None.
             Supported options are `"cl_min"`, `"cl_mean"` or `"cl_max"`.
-            
+
             -if set to `"stbr_fill"` then Steinerberger sampling is used
               after first point.
             -if set to `"stbr_full"` then Steinerberger sampling is used
-              from first point.   
-              
+              from first point.
+
              For details on the Steinerberger method see:
              https://arxiv.org/abs/1902.03269
-             
+
             - If set to `"cl_min"`, then constant liar strategy is used
                with lie objective value being minimum of observed objective
                values. `"cl_mean"` and `"cl_max"` means mean and max of values
                respectively. For details on this strategy see:
 
                https://hal.archives-ouvertes.fr/hal-00732512/document
 
@@ -412,40 +401,35 @@
                 is returning the expected value of the next_x before asking for
                 the next_next_x. Implementation is still experimental.
                 For use of KB, see:
                 https://www.nature.com/articles/s41586-021-03213-y
 
         """
 
-        if not (
-            (isinstance(n_points, int) and n_points > 0) or n_points is None
-        ):
-            raise ValueError(
-                "n_points should be int > 0, got " + str(n_points)
-            )
+        if not ((isinstance(n_points, int) and n_points > 0) or n_points is None):
+            raise ValueError("n_points should be int > 0, got " + str(n_points))
         # These are the only filling strategies which are supported
         supported_strategies = [
             "cl_min",
             "cl_mean",
             "cl_max",
             "stbr_fill",
             "stbr_full",
-            "KB"
+            "KB",
         ]
 
         if strategy not in supported_strategies:
             raise ValueError(
                 "Expected parallel_strategy to be one of "
                 + str(supported_strategies)
                 + ", "
                 + "got %s" % strategy
             )
 
         if strategy == "stbr_full" and self._n_initial_points < 1:
-
             # Steienerberger sampling can not be used from an empty Xi set
             if self.Xi == []:
                 raise ValueError(
                     "Steinerberger sampling requires initial points but got [] "
                 )
 
             if n_points is None:
@@ -463,25 +447,19 @@
         # are provided to the ask, the cache_ is not used.
         if (n_points, strategy) in self.cache_:
             return self.cache_[(n_points, strategy)]
 
         # Copy of the optimizer is made in order to manage the
         # deletion of points with "lie" objective (the copy of
         # optimizer is simply discarded)
-        opt = self.copy(
-            random_state=self.rng.randint(0, np.iinfo(np.int32).max)
-        )
+        opt = self.copy(random_state=self.rng.randint(0, np.iinfo(np.int32).max))
 
         X = []
         for i in range(n_points):
-            if (
-                i > 0
-                and strategy == "stbr_fill"
-                and self._n_initial_points < 1
-            ):
+            if i > 0 and strategy == "stbr_fill" and self._n_initial_points < 1:
                 x = opt.stbr_scipy()[0]
             else:
                 x = opt._ask()
             X.append(x)
 
             ti_available = "ps" in self.acq_func and len(opt.yi) > 0
             ti = [t for (_, t) in opt.yi] if ti_available else None
@@ -500,39 +478,33 @@
                 y_lie = (
                     np.min(opt.yi, axis=0).tolist()
                     if opt.yi
                     else np.zeros(opt.n_objectives).tolist()
                 )  # CL-min lie
                 if opt.n_objectives == 1 and not opt.yi:
                     y_lie = y_lie[0]
-                t_lie = (
-                    np.min(ti) if ti is not None else log(sys.float_info.max)
-                )
+                t_lie = np.min(ti) if ti is not None else log(sys.float_info.max)
             elif strategy == "cl_mean":
                 y_lie = (
                     np.mean(opt.yi, axis=0).tolist()
                     if opt.yi
                     else np.zeros(opt.n_objectives).tolist()
                 )  # CL-mean lie
                 if opt.n_objectives == 1 and not opt.yi:
                     y_lie = y_lie[0]
-                t_lie = (
-                    np.mean(ti) if ti is not None else log(sys.float_info.max)
-                )
+                t_lie = np.mean(ti) if ti is not None else log(sys.float_info.max)
             else:
                 y_lie = (
                     np.max(opt.yi, axis=0).tolist()
                     if opt.yi
                     else np.zeros(opt.n_objectives).tolist()
                 )  # CL-max lie
                 if opt.n_objectives == 1 and not opt.yi:
                     y_lie = y_lie[0]
-                t_lie = (
-                    np.max(ti) if ti is not None else log(sys.float_info.max)
-                )
+                t_lie = np.max(ti) if ti is not None else log(sys.float_info.max)
 
             # Lie to the optimizer.
             if "ps" in self.acq_func:
                 # Use `_tell()` instead of `tell()` to prevent repeated
                 # log transformations of the computation times.
                 opt._tell(x, (y_lie, t_lie))
             else:
@@ -563,41 +535,39 @@
                 return self.space.rvs(random_state=self.rng)[0]
 
             if self._constraints:
                 # Use one sampling strategy for SumEquals constraints
                 if len(self._constraints.sum_equals) > 0:
                     # Create a consistent list of points n_initial_points long
                     sum_equals_list = self._constraints.sumequal_sampling(
-                        n_samples=self.n_initial_points_,
-                        random_state=self.rng
+                        n_samples=self.n_initial_points_, random_state=self.rng
                     )
                     # The samples are returned one at a time from this list
-                    return sum_equals_list[self.n_initial_points_ - self._n_initial_points]
+                    return sum_equals_list[
+                        self.n_initial_points_ - self._n_initial_points
+                    ]
                 else:
                     # We use random value sampling for other constraint types
                     return self._constraints.rvs(random_state=self.rng)[0]
             elif self._lhs:
                 # The samples are evaluated starting form lhs_samples[0]
                 return self._lhs_samples[
                     len(self._lhs_samples) - self._n_initial_points
                 ]
             else:
                 return self.space.rvs(random_state=self.rng)[0]
         else:
             if not self.models:
                 raise RuntimeError(
-                    "Random evaluations exhausted and no "
-                    "model has been fit."
+                    "Random evaluations exhausted and no " "model has been fit."
                 )
 
             next_x = self._next_x
 
-            min_delta_x = min(
-                [self.space.distance(next_x, xi) for xi in self.Xi]
-            )
+            min_delta_x = min([self.space.distance(next_x, xi) for xi in self.Xi])
 
             if abs(min_delta_x) <= 1e-8:
                 warnings.warn(
                     "The objective has been evaluated " "at this point before."
                 )
 
             # return point computed from last call to tell()
@@ -691,25 +661,20 @@
             )
 
         # optimizer learned something new - discard cache
         self.cache_ = {}
 
         # after being "told" n_initial_points we switch from sampling
         # random points to using a surrogate model(s)
-        if (
-            fit
-            and self._n_initial_points <= 0
-            and self.base_estimator_ is not None
-        ):
+        if fit and self._n_initial_points <= 0 and self.base_estimator_ is not None:
             transformed_bounds = np.array(self.space.transformed_bounds)
             est = clone(self.base_estimator_)
 
             # If the problem containts multiblie objectives a model has to be fitted for each objective
             if self.n_objectives > 1:
-
                 # fit an estimator to each objective
                 obj_models = []
                 for i in range(self.n_objectives):
                     est = clone(self.base_estimator_)
                     y_list = [item[i] for item in self.yi]
                     with warnings.catch_warnings():
                         warnings.simplefilter("ignore")
@@ -724,21 +689,19 @@
                 prob_stbr = 0.25
 
                 # Simulate a random number
                 random_uniform_number = np.random.uniform()
 
                 # The random number decides what strategy to use for the next point
                 if random_uniform_number < prob_stbr:
-
                     # self._next_x is found via stbr_scipy
                     next_x = self.stbr_scipy()
                     self._next_x = next_x[0]
 
                 else:
-
                     # The Pareto front is approximated using the NSGAII algorithm
                     pop, logbook, front = self.NSGAII()
 
                     # The best point in the Pareto front is found (the point furthest from existing measurements)
                     next_x = self.best_Pareto_point(pop, front)
                     self._next_x = self.space.inverse_transform(
                         next_x.reshape((1, -1))
@@ -759,27 +722,25 @@
                     # If the constraint is of the SumEquals type, create samples
                     # that respect this
                     if isinstance(self._constraints.constraints_list[0], SumEquals):
                         X = self.space.transform(
                             self._constraints.sumequal_sampling(
                                 n_samples=self.n_points, random_state=self.rng
                             )
-                        )                    
+                        )
                     # For all other constraints we use random sampling
                     else:
                         X = self.space.transform(
                             self._constraints.rvs(
                                 n_samples=self.n_points, random_state=self.rng
                             )
                         )
                 else:
                     X = self.space.transform(
-                        self.space.rvs(
-                            n_samples=self.n_points, random_state=self.rng
-                        )
+                        self.space.rvs(n_samples=self.n_points, random_state=self.rng)
                     )
 
                 self.next_xs_ = []
                 for cand_acq_func in self.cand_acq_funcs_:
                     values = _gaussian_acquisition(
                         X=X,
                         model=est,
@@ -833,29 +794,23 @@
                     self.next_xs_.append(next_x)
 
                 if self.acq_func == "gp_hedge":
                     logits = np.array(self.gains_)
                     logits -= np.max(logits)
                     exp_logits = np.exp(self.eta * logits)
                     probs = exp_logits / np.sum(exp_logits)
-                    next_x = self.next_xs_[
-                        np.argmax(self.rng.multinomial(1, probs))
-                    ]
+                    next_x = self.next_xs_[np.argmax(self.rng.multinomial(1, probs))]
                 else:
                     next_x = self.next_xs_[0]
 
                 # note the need for [0] at the end
-                self._next_x = self.space.inverse_transform(
-                    next_x.reshape((1, -1))
-                )[0]
+                self._next_x = self.space.inverse_transform(next_x.reshape((1, -1)))[0]
         # Pack results
 
-        return create_result(
-            self.Xi, self.yi, self.space, self.rng, models=self.models
-        )
+        return create_result(self.Xi, self.yi, self.space, self.rng, models=self.models)
 
     def _check_y_is_valid(self, x, y):
         """Check if the shape and types of x and y are consistent."""
 
         if "ps" in self.acq_func:
             if is_2Dlistlike(x):
                 if not (np.ndim(y) == 2 and np.shape(y)[1] == 2):
@@ -869,17 +824,15 @@
             for y_values in y:
                 if not len(y_values) == self.n_objectives:
                     raise ValueError(
                         "y does not have the correct number of objective scores"
                     )
                 for y_value in y_values:
                     if not isinstance(y_value, Number):
-                        raise ValueError(
-                            "expected y to be a list of lists of scalars"
-                        )
+                        raise ValueError("expected y to be a list of lists of scalars")
 
         # Check batch tell with single objective
         elif is_listlike(y) and is_2Dlistlike(x) and self.n_objectives == 1:
             for y_value in y:
                 if not isinstance(y_value, Number):
                     raise ValueError("expected y to be a list of scalars")
 
@@ -908,20 +861,18 @@
 
     def run(self, func, n_iter=1):
         """Execute ask() + tell() `n_iter` times"""
         for _ in range(n_iter):
             x = self.ask()
             self.tell(x, func(x))
 
-        return create_result(
-            self.Xi, self.yi, self.space, self.rng, models=self.models
-        )
+        return create_result(self.Xi, self.yi, self.space, self.rng, models=self.models)
 
     def set_constraints(self, constraints):
-        """ Sets the constraints for the optimizer
+        """Sets the constraints for the optimizer
 
         Parameters
         ----------
         * `constraints` [list] or [Constraints]:
             Can either be a list of Constraint objects or a Constraints object
         """
         if self._n_initial_points > 0 and self._lhs:
@@ -938,41 +889,39 @@
                 self._constraints = Constraints(constraints, self.space)
         else:
             self._constraints = None
 
         self.update_next()
 
     def remove_constraints(self):
-        """ Sets constraints to None"""
+        """Sets constraints to None"""
         self.set_constraints(None)
 
     def get_constraints(self):
         """Returns constraints"""
         return self._constraints
 
     def update_next(self):
-        """ Updates the value returned by opt.ask(). Useful if a parameter was updated after ask was called."""
+        """Updates the value returned by opt.ask(). Useful if a parameter was updated after ask was called."""
         self.cache_ = {}
         # Ask for a new next_x. Usefull if new constraints have been added or lenght_scale has been tweaked.
         # We only need to overwrite _next_x if it exists.
         if hasattr(self, "_next_x"):
             opt = self.copy(random_state=self.rng)
             self._next_x = opt._next_x
 
     def get_result(self):
         """Returns the same result that would be returned by opt.tell()
         but without calling tell.
         In the case of multiobejective optimization, a list of results are
         returned."""
-        return create_result(
-            self.Xi, self.yi, self.space, self.rng, models=self.models
-        )
+        return create_result(self.Xi, self.yi, self.space, self.rng, models=self.models)
 
     def _check_length_scale_bounds(self, dimensions, bounds):
-        """ Checks if length scale bounds are of in correct format"""
+        """Checks if length scale bounds are of in correct format"""
         space = Space(dimensions)
         n_dims = space.n_dims
         if bounds:
             if isinstance(bounds, list):
                 # Check that number of bounds is the same as number of dimensions
                 if not len(bounds) == n_dims:
                     raise ValueError(
@@ -988,16 +937,15 @@
                     if not len(bounds[i]) == 2:
                         raise ValueError(
                             "Each bound-tuple must have length 2, got %s"
                             % (len(bounds[i]))
                         )
             else:
                 raise TypeError(
-                    "Expected bounds to be of type list, got %s"
-                    % (type(bounds))
+                    "Expected bounds to be of type list, got %s" % (type(bounds))
                 )
 
     def stbr_scipy(self, n_points=1):
         from scipy.optimize import minimize
 
         # Suggestion for improvemenet. Seperate categorical and real/integer space.
         # Only solve Steinerberger minimization in real/integer sub space.
@@ -1039,34 +987,30 @@
             for j in range(len(x0)):
                 res = minimize(copy.stbr_fun, x0=x0[j], bounds=bounds)
                 loc_min.append(res.x)
                 fun_val.append(res.fun)
 
             # Decide the global minimum as the local minimum with the lowest function value
             glob_min = loc_min[np.argmin(fun_val)]
-            next_X = np.asarray(glob_min).reshape(
-                1, copy.space.transformed_n_dims
-            )
+            next_X = np.asarray(glob_min).reshape(1, copy.space.transformed_n_dims)
             # Transform back to original space
             next_X = copy.space.inverse_transform(next_X)
 
             # This deals with categorical variables, since they are not suited for Steinerberger
             for dim, n in zip(self.space.dimensions, range(self.space.n_dims)):
                 # Check if dimension is categorical
                 if isinstance(dim, Categorical):
                     # Make array with categories for that dimension
                     categories = dim.categories
                     # Make array with all instances of categories observed
                     instances = np.array(copy.Xi)[:, n]
                     # Calculate the number of instances of each category
                     cat_population = np.zeros(len(categories))
                     for category, i in zip(categories, range(len(categories))):
-                        cat_population[i] = (instances.tolist()).count(
-                            category
-                        )
+                        cat_population[i] = (instances.tolist()).count(category)
                     # Find the category with the lowest population
                     least_populated = categories[np.argmin(cat_population)]
                     # Set the category to the lowest populated category
                     next_X[0][n] = least_populated
 
             # Append point to list of new Steinerberger points
             X.append(next_X[0])
@@ -1074,15 +1018,15 @@
             copy.Xi.append(next_X[0])
 
         return X
 
     # This function returns the Steinerberger sum for a given x
     def stbr_fun(self, x):
         # parameter to ensure that log argument is non-zero
-        eta = 10 ** -8
+        eta = 10**-8
         # Initialize Steinerberger sum
         stbr_sum = 0
         # Transform initial points to [0,1]^d space
         Xi = self.space.transform(self.Xi)
         # for loop over all existing points
         for i in range(len(Xi)):
             # Calculate the factors in the Steinerberger term in each dimension
@@ -1092,37 +1036,34 @@
             # Add term to Steinerberger sum
             stbr_sum = stbr_sum + stbr_term
 
         return stbr_sum
 
     # This function returns the objective scores at x estimated by the models
     def __ObjectiveGP(self, x):
-
         # Fator = 1.0e10
         F = [None] * self.n_objectives
         xx = np.asarray(x).reshape(1, -1)
 
         # Constraints = 0.0
         # for cons in self.constraints:
         #    y = cons['fun'](x)
         #    if cons['type'] == 'eq':
         #        Constraints += np.abs(y)
         #    elif cons['type'] == 'ineq':
         #        if y < 0:
         #            Constraints -= y
 
         for i in range(self.n_objectives):
-
             F[i] = self.models[-1][i].predict(xx)[0]
 
         return F
 
     # This function returns the point in the Pareto front, which is deemed the best (furthest away from existing observations)
     def best_Pareto_point(self, pop, front, q=0.5):
-
         Population = np.asarray(pop)
 
         IndexF, FatorF = self.__LargestOfLeast(front, self.yi)
 
         IndexPop, FatorPop = self.__LargestOfLeast(
             Population, self.space.transform(self.Xi).tolist()
         )
@@ -1165,48 +1106,62 @@
             Dist = np.sqrt(Dist)
             if Dist < DistMin:
                 DistMin = Dist
         return DistMin
 
     # This function calls NSGAII to estimate the Pareto Front
     def NSGAII(self, MU=40):
-
         from ._NSGA2 import NSGAII
 
         pop, logbook, front = NSGAII(
             self.n_objectives,
             self.__ObjectiveGP,
             np.array(self.space.transformed_bounds),
             MU=MU,
         )
 
         return pop, logbook, front
-    
+
     # This function adds the modelled white noise to the regressor to allow predictions including noise
     def add_modelled_noise(self):
-        '''
+        """
         This method will add the noise that has been modelled to fit the data. (The noise is disabled
         by default to reflect description in book on gaussian processes for Machine Learning
         This has been described in Eq 2.24 of
         http://www.gaussianprocess.org/gpml/chapters/RW2.pdf)
-        '''
-        if isinstance(self.models[-1].noise, str) and self.models[-1].noise != "gaussian":
-            raise ValueError("expected noise to be 'gaussian', got %s"
-                             % self.models[-1].noise)
+        """
+        if (
+            isinstance(self.models[-1].noise, str)
+            and self.models[-1].noise != "gaussian"
+        ):
+            raise ValueError(
+                "Expected noise to be 'gaussian', got %s" % self.models[-1].noise
+            )
         noise_estimate = self.models[-1].noise_
-        white_present, white_param = _param_for_white_kernel_in_Sum(self.models[-1].kernel_)
+        white_present, white_param = _param_for_white_kernel_in_Sum(
+            self.models[-1].kernel_
+        )
         if white_present:
-            self.models[-1].kernel_.set_params(**{white_param: WhiteKernel(noise_level=noise_estimate)})
-    
+            self.models[-1].kernel_.set_params(
+                **{white_param: WhiteKernel(noise_level=noise_estimate)}
+            )
+
     def remove_modelled_noise(self):
-        '''
+        """
         This method resets the noise levels to only include the "true" uncertaincy of the main kernel
-        used for fitting and predicting. This method can be used in conjunction with the 
+        used for fitting and predicting. This method can be used in conjunction with the
         'add_modelled_noise()'
-        '''
-        if isinstance(self.models[-1].noise, str) and self.models[-1].noise != "gaussian":
-            raise ValueError("expected noise to be 'gaussian', got %s"
-                             % self.models[-1].noise)
-        white_present, white_param = _param_for_white_kernel_in_Sum(self.models[-1].kernel_)
+        """
+        if (
+            isinstance(self.models[-1].noise, str)
+            and self.models[-1].noise != "gaussian"
+        ):
+            raise ValueError(
+                "expected noise to be 'gaussian', got %s" % self.models[-1].noise
+            )
+        white_present, white_param = _param_for_white_kernel_in_Sum(
+            self.models[-1].kernel_
+        )
         if white_present:
-            self.models[-1].kernel_.set_params(**{white_param: WhiteKernel(noise_level=0.0)})
-    
+            self.models[-1].kernel_.set_params(
+                **{white_param: WhiteKernel(noise_level=0.0)}
+            )
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/plots.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/plots.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/searchcv.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/searchcv.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/space/constraints.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/space/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,24 +88,23 @@
         n_samples_candidates = 0
 
         # We keep sampling until all samples a valid with regard to the
         # constraints:
         while len(rows) < n_samples:
             columns = []
             # Iterate through all dimensions:
+            random_samples = self.space.rvs(n_samples=n_samples, random_state=rng)
             for i in range(self.space.n_dims):
-                dim = self.space.dimensions[i]
                 # If a dimension has a "Single"-type constraint we just sample
                 # that value:
                 if self.single[i]:
                     column = np.full(n_samples, self.single[i].value)
                 else:  # Using the default rvs() for the given dimension
                     try:
-                        column = (dim.rvs(n_samples=n_samples, 
-                                          random_state=rng))
+                        column = [sample[i] for sample in random_samples]
                     except Exception as error:
                         print(f'''Caught an error while making random points in
                          constrained space, error is: {error}''')
                 columns.append(column)
 
             # Transpose
             for i in range(n_samples):
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/space/space.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/space/space.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,48 @@
-from typing import List, Union
+from abc import ABC, abstractmethod
+from typing import Iterable, List, Union
 
 import numbers
 import numpy as np
 import yaml
 
-from scipy.stats.distributions import randint
-from scipy.stats.distributions import rv_discrete
-from scipy.stats.distributions import uniform
-
-from sklearn.utils import check_random_state
-from sklearn.utils.fixes import sp_version
 
 from .transformers import CategoricalEncoder
 from .transformers import Normalize
 from .transformers import Identity
 from .transformers import Log10
 from .transformers import Pipeline
+from ..utils import get_random_generator
 
 # helper class to be able to print [1, ..., 4] instead of [1, '...', 4]
 
 
 class _Ellipsis:
     def __repr__(self):
-        return '...'
+        return "..."
 
 
 def space_factory(input: Union["Space", List]) -> "Space":
     """Transforms a list of dimension definitions into a Space
 
     If the input is already a Space, that is returned.
 
     Parameters:
     * `input` (List, Space): The list of Dimension definitions. For more details,
         see documentation for check_dimensions.
 
     Returns:
     * `space`: The resulting Space.
     """
-    if isinstance(input,Space):
+    if isinstance(input, Space):
         return input
     else:
         return Space(input)
 
+
 def check_dimension(dimension, transform=None):
     """Turn a provided dimension description into a dimension object.
 
     Checks that the provided dimension falls into one of the
     supported types. For a list of supported types, look at
     the documentation of ``dimension`` below.
 
@@ -95,67 +92,56 @@
     # to define subspaces that fix one value, e.g. to choose the
     # model type, see "sklearn-gridsearchcv-replacement.ipynb"
     # for examples.
     if len(dimension) == 1:
         return Categorical(dimension, transform=transform)
 
     if len(dimension) == 2:
-        if any([isinstance(d, (str, bool)) or isinstance(d, np.bool_)
-                for d in dimension]):
+        if any(
+            [isinstance(d, (str, bool)) or isinstance(d, np.bool_) for d in dimension]
+        ):
             return Categorical(dimension, transform=transform)
         elif all([isinstance(dim, numbers.Integral) for dim in dimension]):
             return Integer(*dimension, transform=transform)
         elif any([isinstance(dim, numbers.Real) for dim in dimension]):
             return Real(*dimension, transform=transform)
         else:
-            raise ValueError("Invalid dimension {}. Read the documentation for"
-                             " supported types.".format(dimension))
+            raise ValueError(
+                "Invalid dimension {}. Read the documentation for"
+                " supported types.".format(dimension)
+            )
 
     if len(dimension) == 3:
-        if (any([isinstance(dim, (float, int)) for dim in dimension[:2]]) and
-                dimension[2] in ["uniform", "log-uniform"]):
+        if (any([isinstance(dim, (float, int)) for dim in dimension[:2]])
+            and dimension[2] in ["uniform", "log-uniform"]):
             return Real(*dimension, transform=transform)
         else:
             return Categorical(dimension, transform=transform)
 
     if len(dimension) > 3:
         return Categorical(dimension, transform=transform)
 
-    raise ValueError("Invalid dimension {}. Read the documentation for "
-                     "supported types.".format(dimension))
+    raise ValueError(
+        "Invalid dimension {}. Read the documentation for "
+        "supported types.".format(dimension)
+    )
 
 
-class Dimension(object):
+class Dimension(ABC):
     """Base class for search space dimensions."""
 
     prior = None
 
-    def rvs(self, n_samples=1, random_state=None):
-        """Draw random samples.
-
-        Parameters
-        ----------
-        * `n_samples` [int or None]:
-            The number of samples to be drawn.
-
-        * `random_state` [int, RandomState instance, or None (default)]:
-            Set random state to something other than None for reproducible
-            results.
-        """
-        rng = check_random_state(random_state)
-        samples = self._rvs.rvs(size=n_samples, random_state=rng)
-        return self.inverse_transform(samples)
-
     def transform(self, X):
         """Transform samples form the original space to a warped space."""
         return self.transformer.transform(X)
 
     def inverse_transform(self, Xt):
         """Inverse transform samples from the warped space back into the
-           original space.
+        original space.
         """
         return self.transformer.inverse_transform(Xt)
 
     @property
     def size(self):
         return 1
 
@@ -178,20 +164,63 @@
     @name.setter
     def name(self, value):
         if isinstance(value, str) or value is None:
             self._name = value
         else:
             raise ValueError("Dimension's name must be either string or None.")
 
+    def sample(
+        self, points: Union[float, Iterable[float]], allow_duplicates: bool = True
+    ) -> np.ndarray:
+        """Draw points from the dimension.
 
-def _uniform_inclusive(loc=0.0, scale=1.0):
-    # like scipy.stats.distributions but inclusive of `high`
-    # XXX scale + 1. might not actually be a float after scale if
-    # XXX scale is very large.
-    return uniform(loc=loc, scale=np.nextafter(scale, scale + 1.))
+
+
+        Parameters
+        ----------
+        * `points` [float or list[float]]:
+            A single point or a list of points to sample. All must be between 0 and 1.
+
+        * `allow_duplicates` [bool, default=True]:
+            If True, the output will have the same size as `points`. If False, each
+            point in the output will be unique. This means that the output can be
+            shorter than `points`.
+        """
+        if isinstance(points, (int, float)):  # If a single point is given, convert it
+            # to a list.
+            points = [points]
+        if any([point < 0 or point > 1 for point in points]):
+            raise ValueError("Sample points must be between 0 and 1.")
+        sampled_points = self._sample(points)
+        if not allow_duplicates:
+            # np.unique sorts the inputs, which we do not want, so we have to reinvent
+            # the wheel.
+            seen = set()
+            unique_points = []
+            for point in sampled_points:
+                if point not in seen:
+                    unique_points.append(point)
+                    seen.add(point)
+            sampled_points = unique_points
+        return np.array(sampled_points)
+
+    @abstractmethod
+    def _sample(self, points: Iterable[float]) -> np.array:
+        """A reasonable mapping from the interval [0, 1] to the dimension, whatever that
+        may mean. For example, for an integer dimension, the sampling should be give a
+        higher integer for a higher value of the point, and each integer should be
+        mapped to from an equally large interval.
+
+        The mapping should be monotonic, but it does not have to be strictly monotonic.
+
+        The mapping should respect (informative) priors. For example, if the prior is
+        log-uniform, the mapping should be logarithmic, so that the interval that maps
+        to [0.1, 1] is the same size as the interval that maps to [1, 10].
+        """
+        pass
 
 
 class Real(Dimension):
     def __init__(self, low, high, prior="uniform", transform=None, name=None):
         """Search space dimension that can take on any real value.
 
         Parameters
@@ -217,73 +246,69 @@
             - "normalize", the transformed space is scaled to be between
               0 and 1.
 
         * `name` [str or None]:
             Name associated with the dimension, e.g., "learning rate".
         """
         if high <= low:
-            raise ValueError("the lower bound {} has to be less than the"
-                             " upper bound {}".format(low, high))
+            raise ValueError(
+                "the lower bound {} has to be less than the"
+                " upper bound {}".format(low, high)
+            )
         self.low = low
         self.high = high
         self.prior = prior
         self.name = name
 
         if transform is None:
             transform = "identity"
 
         self.transform_ = transform
 
         if self.transform_ not in ["normalize", "identity"]:
-            raise ValueError("transform should be 'normalize' or 'identity'"
-                             " got {}".format(self.transform_))
+            raise ValueError(
+                "transform should be 'normalize' or 'identity'"
+                " got {}".format(self.transform_)
+            )
 
-        # Define _rvs and transformer spaces.
-        # XXX: The _rvs is for sampling in the transformed space.
-        # The rvs on Dimension calls inverse_transform on the points sampled
-        # using _rvs
         if self.transform_ == "normalize":
             # set upper bound to next float after 1. to make the numbers
             # inclusive of upper edge
-            self._rvs = _uniform_inclusive(0., 1.)
             if self.prior == "uniform":
-                self.transformer = Pipeline(
-                    [Identity(), Normalize(low, high)])
+                self.transformer = Pipeline([Identity(), Normalize(low, high)])
             else:
                 self.transformer = Pipeline(
                     [Log10(), Normalize(np.log10(low), np.log10(high))]
                 )
         else:
             if self.prior == "uniform":
-                self._rvs = _uniform_inclusive(self.low, self.high - self.low)
                 self.transformer = Identity()
             else:
-                self._rvs = _uniform_inclusive(
-                    np.log10(self.low),
-                    np.log10(self.high) - np.log10(self.low))
                 self.transformer = Log10()
 
     def __eq__(self, other):
-        return (type(self) is type(other) and
-                np.allclose([self.low], [other.low]) and
-                np.allclose([self.high], [other.high]) and
-                self.prior == other.prior and
-                self.transform_ == other.transform_)
+        return (
+            type(self) is type(other)
+            and np.allclose([self.low], [other.low])
+            and np.allclose([self.high], [other.high])
+            and self.prior == other.prior
+            and self.transform_ == other.transform_
+        )
 
     def __repr__(self):
         return "Real(low={}, high={}, prior='{}', transform='{}')".format(
-            self.low, self.high, self.prior, self.transform_)
+            self.low, self.high, self.prior, self.transform_
+        )
 
     def inverse_transform(self, Xt):
         """Inverse transform samples from the warped space back into the
-           orignal space.
+        orignal space.
         """
         return np.clip(
-            super(Real, self).inverse_transform(Xt).astype(float),
-            self.low, self.high
+            super(Real, self).inverse_transform(Xt).astype(float), self.low, self.high
         )
 
     @property
     def bounds(self):
         return (self.low, self.high)
 
     def __contains__(self, point):
@@ -296,45 +321,43 @@
         else:
             if self.prior == "uniform":
                 return self.low, self.high
             else:
                 return np.log10(self.low), np.log10(self.high)
 
     def distance(self, a, b):
-
         """Compute distance between point `a` and `b`.
 
         Parameters
         ----------
         * `a` [float]
             First point.
 
         * `b` [float]
             Second point.
         """
         if not (a in self and b in self):
-            raise RuntimeError("Can only compute distance for values within "
-                               "the space, not %s and %s." % (a, b))
+            raise RuntimeError(
+                "Can only compute distance for values within "
+                "the space, not %s and %s." % (a, b)
+            )
         return abs(a - b)
 
-    def lhs_arange(self, n):
-        """ Returns an evenly distributed numpy array of samples to use with latin hypercube sampling.
-
-        Parameters
-        -----------
-        * `n` [int]
-            Number of samples.
-        """
-        # Generate sample points by splitting the space 0 to 1 into n pieces
-        # and picking the middle of each piece. Samples are spaced 1/n apart
-        # inside the interval with a buffer of half a step size to the extremes
-        samples = (np.arange(n)+0.5)/n
-
-        # Transform the samples to the range used for this dimension
-        return samples*(self.high - self.low) + self.low
+    def _sample(self, point_list: Iterable[float]) -> np.ndarray:
+        if self.prior == "uniform":
+            sampled_points = [
+                point * (self.high - self.low) + self.low for point in point_list
+            ]
+        else:
+            log_sampled_points = [
+                point * np.log(self.high / self.low) + np.log(self.low)
+                for point in point_list
+            ]
+            sampled_points = np.exp(log_sampled_points)
+        return sampled_points
 
 
 class Integer(Dimension):
     def __init__(self, low, high, transform=None, name=None):
         """Search space dimension that can take on integer values.
 
         Parameters
@@ -353,49 +376,50 @@
             - "normalize", the transformed space is scaled to be between
               0 and 1.
 
         * `name` [str or None]:
             Name associated with dimension, e.g., "number of trees".
         """
         if high <= low:
-            raise ValueError("the lower bound {} has to be less than the"
-                             " upper bound {}".format(low, high))
+            raise ValueError(
+                "The lower bound {} has to be less than the "
+                "upper bound {}".format(low, high)
+            )
         self.low = low
         self.high = high
         self.name = name
 
         if transform is None:
             transform = "identity"
 
         self.transform_ = transform
 
         if transform not in ["normalize", "identity"]:
-            raise ValueError("transform should be 'normalize' or 'identity'"
-                             " got {}".format(self.transform_))
+            raise ValueError(
+                "Transform should be 'normalize' or 'identity' "
+                "got {}".format(self.transform_)
+            )
         if transform == "normalize":
-            self._rvs = uniform(0, 1)
             self.transformer = Normalize(low, high, is_int=True)
         else:
-            self._rvs = randint(self.low, self.high + 1)
             self.transformer = Identity()
 
-    def update_samplingspace(self, new_space):
-        self._rvs = new_space
-
     def __eq__(self, other):
-        return (type(self) is type(other) and
-                np.allclose([self.low], [other.low]) and
-                np.allclose([self.high], [other.high]))
+        return (
+            type(self) is type(other)
+            and np.allclose([self.low], [other.low])
+            and np.allclose([self.high], [other.high])
+        )
 
     def __repr__(self):
         return "Integer(low={}, high={})".format(self.low, self.high)
 
     def inverse_transform(self, Xt):
         """Inverse transform samples from the warped space back into the
-           orignal space.
+        orignal space.
         """
         # The concatenation of all transformed dimensions makes Xt to be
         # of type float, hence the required cast back to int.
         return super(Integer, self).inverse_transform(Xt).astype(np.int64)
 
     @property
     def bounds(self):
@@ -419,37 +443,25 @@
         * `a` [int]
             First point.
 
         * `b` [int]
             Second point.
         """
         if not (a in self and b in self):
-            raise RuntimeError("Can only compute distance for values within "
-                               "the space, not %s and %s." % (a, b))
+            raise RuntimeError(
+                "Can only compute distance for values within "
+                "the space, not %s and %s." % (a, b)
+            )
         return abs(a - b)
 
-    def lhs_arange(self, n):
-        """ Returns an evenly distributed list of samples to use with latin hypercube sampling.
-
-        Parameters
-        -----------
-        * `n` [int]
-            Number of samples.
-        """
-        # Generate sample points by splitting the space 0 to 1 into n pieces
-        # and picking the middle of each piece. Samples are spaced 1/n apart
-        # inside the interval with a buffer of half a step size to the extremes
-        samples = (np.arange(n)+0.5)/n
-        # Transform the samples to the range used for this dimension and then 
-        # round them back to integers. If your space is less than n wide, some 
-        # of your samples will be rounded to the same number
-        samples = np.round(samples*(self.high - self.low) + self.low)
-        
-        # Convert samples to a list of integers
-        return samples.astype(int)
+    def _sample(self, point_list: Iterable[float]) -> np.ndarray:
+        point_list = [
+            point * (self.high + 1 - self.low) + self.low for point in point_list
+        ]
+        return np.floor(point_list).astype(int)
 
 
 class Categorical(Dimension):
     def __init__(self, categories, prior=None, transform=None, name=None):
         """Search space dimension that can take on categorical values.
 
         Parameters
@@ -466,71 +478,62 @@
               space.
             - "onehot", the transformed space is a one-hot encoded
               representation of the original space.
 
         * `name` [str or None]:
             Name associated with dimension, e.g., "colors".
         """
-        if transform == 'identity':
+        if transform == "identity":
             self.categories = tuple([str(c) for c in categories])
         else:
             self.categories = tuple(categories)
 
         self.name = name
 
         if transform is None:
             transform = "onehot"
         self.transform_ = transform
         if transform not in ["identity", "onehot"]:
-            raise ValueError("Expected transform to be 'identity' or 'onehot' "
-                             "got {}".format(transform))
+            raise ValueError(
+                "Expected transform to be 'identity' or 'onehot' "
+                "got {}".format(transform)
+            )
         if transform == "onehot":
             self.transformer = CategoricalEncoder()
             self.transformer.fit(self.categories)
         else:
             self.transformer = Identity(dtype=type(categories[0]))
 
         self.prior = prior
 
         if prior is None:
-            self.prior_ = np.tile(1. / len(self.categories),
-                                  len(self.categories))
+            self.prior_ = np.tile(1.0 / len(self.categories), len(self.categories))
         else:
             self.prior_ = prior
 
-        # XXX check that sum(prior) == 1
-        self._rvs = rv_discrete(
-            values=(range(len(self.categories)), self.prior_)
-        )
-
     def __eq__(self, other):
-        return (type(self) is type(other) and
-                self.categories == other.categories and
-                np.allclose(self.prior_, other.prior_))
+        return (
+            type(self) is type(other)
+            and self.categories == other.categories
+            and np.allclose(self.prior_, other.prior_)
+        )
 
     def __repr__(self):
         if len(self.categories) > 7:
-            cats = self.categories[:3] + (_Ellipsis(), ) + self.categories[-3:]
+            cats = self.categories[:3] + (_Ellipsis(),) + self.categories[-3:]
         else:
             cats = self.categories
 
         if self.prior is not None and len(self.prior) > 7:
             prior = self.prior[:3] + [_Ellipsis()] + self.prior[-3:]
         else:
             prior = self.prior
 
         return "Categorical(categories={}, prior={})".format(cats, prior)
 
-    def rvs(self, n_samples=None, random_state=None):
-        choices = self._rvs.rvs(size=n_samples, random_state=random_state)
-        if isinstance(choices, numbers.Integral):
-            return self.categories[choices]
-        else:
-            return [self.categories[c] for c in choices]
-
     @property
     def transformed_size(self):
         if self.transform_ == "onehot":
             size = len(self.categories)
             # when len(categories) == 2, CategoricalEncoder outputs a
             # single value
             return size if size != 2 else 1
@@ -561,33 +564,27 @@
         * `a` [category]
             First category.
 
         * `b` [category]
             Second category.
         """
         if not (a in self and b in self):
-            raise RuntimeError("Can only compute distance for values within"
-                               " the space, not {} and {}.".format(a, b))
+            raise RuntimeError(
+                "Can only compute distance for values within "
+                "the space, not {} and {}.".format(a, b)
+            )
         return 1 if a != b else 0
 
-    def lhs_arange(self, n):
-        """ Returns an evenly distributed list of samples to use with latin hypercube sampling.
-
-        Parameters
-        -----------
-        * `n` [int]
-            Number of samples.
-        """
-
-        s = []
-        l = len(self.categories)  # Number of categories
-        for i in range(n):
-            # Loop through all categories by using the modulus.
-            s.append(self.categories[i % l])
-        return s
+    def _sample(self, point_list: Iterable[float]) -> np.ndarray:
+        # XXX check that sum(prior) == 1
+        cummulative_prior = np.cumsum(self.prior_)
+        # For each point in point_list, find the index of the first element in cummulative_prior that is greater than the point
+        # This is the index of the category that the point corresponds to
+        category_index = [np.argmax(cummulative_prior > point) for point in point_list]
+        return np.array([self.categories[index] for index in category_index])
 
 
 class Space(object):
     """Search space."""
 
     def __init__(self, dimensions):
         """Initialize a search space from given specifications.
@@ -615,15 +612,15 @@
         return all([a == b for a, b in zip(self.dimensions, other.dimensions)])
 
     def __repr__(self):
         if len(self.dimensions) > 31:
             dims = self.dimensions[:15] + [_Ellipsis()] + self.dimensions[-15:]
         else:
             dims = self.dimensions
-        return "Space([{}])".format(',\n       '.join(map(str, dims)))
+        return "Space([{}])".format(",\n       ".join(map(str, dims)))
 
     def __iter__(self):
         return iter(self.dimensions)
 
     @property
     def is_real(self):
         """
@@ -656,31 +653,33 @@
              namespace if not provided
 
         Returns
         -------
         * `space` [Space]:
            Instantiated Space object
         """
-        with open(yml_path, 'rb') as f:
+        with open(yml_path, "rb") as f:
             config = yaml.safe_load(f)
 
-        dimension_classes = {'real': Real,
-                             'integer': Integer,
-                             'categorical': Categorical}
+        dimension_classes = {
+            "real": Real,
+            "integer": Integer,
+            "categorical": Categorical,
+        }
 
         # Extract space options for configuration file
         if isinstance(config, dict):
             if namespace is None:
                 options = next(iter(config.values()))
             else:
                 options = config[namespace]
         elif isinstance(config, list):
             options = config
         else:
-            raise TypeError('YaML does not specify a list or dictionary')
+            raise TypeError("YaML does not specify a list or dictionary")
 
         # Populate list with Dimension objects
         dimensions = []
         for option in options:
             key = next(iter(option.keys()))
             # Make configuration case insensitive
             dimension_class = key.lower()
@@ -690,41 +689,48 @@
                 dimension = dimension_classes[dimension_class](**values)
                 dimensions.append(dimension)
 
         space = cls(dimensions=dimensions)
 
         return space
 
-    def rvs(self, n_samples=1, random_state=None):
+    def rvs(
+        self,
+        n_samples=1,
+        random_state: Union[
+            int, np.random.RandomState, np.random.Generator, None
+        ] = None,
+    ):
         """Draw random samples.
 
         The samples are in the original space. They need to be transformed
         before being passed to a model or minimizer by `space.transform()`.
 
         Parameters
         ----------
         * `n_samples` [int, default=1]:
             Number of samples to be drawn from the space.
 
-        * `random_state` [int, RandomState instance, or None (default)]:
+        * `random_state` [int, np.random.RandomState, np.random.Generator, or None, default=None]:
             Set random state to something other than None for reproducible
             results.
 
         Returns
         -------
         * `points`: [list of lists, shape=(n_points, n_dims)]
            Points sampled from the space.
         """
 
-        rng = check_random_state(random_state)
+        rng = get_random_generator(random_state)
 
         columns = []
 
         for dim in self.dimensions:
-            columns.append(dim.rvs(n_samples=n_samples, random_state=rng))
+            index_array = rng.uniform(size=n_samples)
+            columns.append(dim.sample(index_array))
 
         # Transpose
         rows = []
         for i in range(n_samples):
             r = []
             for j in range(self.n_dims):
                 r.append(columns[j][i])
@@ -788,16 +794,15 @@
         for j in range(self.n_dims):
             dim = self.dimensions[j]
             offset = dim.transformed_size
 
             if offset == 1:
                 columns.append(dim.inverse_transform(Xt[:, start]))
             else:
-                columns.append(
-                    dim.inverse_transform(Xt[:, start:start+offset]))
+                columns.append(dim.inverse_transform(Xt[:, start : start + offset]))
 
             start += offset
 
         # Transpose
         rows = []
 
         for i in range(len(Xt)):
@@ -827,20 +832,22 @@
         for dim in self.dimensions:
             if dim.size == 1:
                 b.append(dim.bounds)
             else:
                 b.extend(dim.bounds)
 
         return b
-    
+
     @property
     def names(self):
-        '''The names of the dimensions if given. Otherwise [X1, X2, ... Xn]'''
-        labels = ["$X_{%i}$" % i if d.name is None else d.name
-            for i, d in enumerate(self.dimensions)]
+        """The names of the dimensions if given. Otherwise [X1, X2, ... Xn]"""
+        labels = [
+            "$X_{%i}$" % i if d.name is None else d.name
+            for i, d in enumerate(self.dimensions)
+        ]
         return labels
 
     def __contains__(self, point):
         """Check that `point` is within the bounds of the space."""
         for component, dim in zip(point, self.dimensions):
             if component not in dim:
                 return False
@@ -866,52 +873,65 @@
 
     @property
     def is_partly_categorical(self):
         """Space contains any categorical dimensions"""
         return any([isinstance(dim, Categorical) for dim in self.dimensions])
 
     def distance(self, point_a, point_b):
-        """Compute distance between two points in this space.
+        """Compute the L1 (Manhattan or taxicab) distance between two points in this space.
 
         Parameters
         ----------
         * `a` [array]
             First point.
 
         * `b` [array]
             Second point.
         """
-        distance = 0.
+        distance = 0.0
         if len(self.dimensions) > 1:
             for a, b, dim in zip(point_a, point_b, self.dimensions):
                 distance += dim.distance(a, b)
-                
+
         if len(self.dimensions) == 1:
-             distance +=  self.dimensions[0].distance(point_a[0], point_b[0])
+            distance += self.dimensions[0].distance(point_a[0], point_b[0])
 
         return distance
 
-    def lhs(self, n):
-        """ Returns n latin hypercube samples as a list of lists
-        """
+    def lhs(
+        self,
+        n: int,
+        seed: Union[int, float, np.random.RandomState, np.random.Generator, None] = 42,
+    ):
+        """Returns n latin hypercube samples as a list of lists
+
+        Parameters
+        ----------
+        * `n` [int]: The number of samples to generate.
 
+        * `seed`
+            [int, float, np.random.RandomState, np.random.Generator, or None, default=42]:
+            The seed used by the random number generator. If None, the results are not reproducible.
+        """
+        rng = get_random_generator(seed)
         samples = []
         for i in range(self.n_dims):
             lhs_perm = []
             # Get evenly distributed samples from one dimension
-            lhs_aranged = self.dimensions[i].lhs_arange(n)
-            perm = np.random.RandomState(seed=42 + i).permutation(n)
+            sample_indices = (np.arange(n) + 0.5) / n
+            lhs_aranged = self.dimensions[i].sample(sample_indices)
+            perm = rng.permutation(n)
             for p in perm:  # Random permutate the order of the samples
                 lhs_perm.append(lhs_aranged[p])
             samples.append(lhs_perm)
         # Now we have a list of lists with samples for each dimension.
         # We need to transpose this so that we get a list of lists with
         # samples for all the dimensions
         transposed_samples = []
         for i in range(n):
             row = []
             for j in range(self.n_dims):
                 row.append(samples[j][i])
             transposed_samples.append(row)
         return transposed_samples
-    
+
     # TODO: Add a R1 QRS sampling method here
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer/space/transformers.py` & `ProcessOptimizer-0.8.2/ProcessOptimizer/space/transformers.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/PKG-INFO` & `ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.8.1
+Version: 0.8.2
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
 Description-Content-Type: text/markdown
-Provides-Extra: bokeh
 Provides-Extra: browniebee
 License-File: LICENSE.md
 License-File: AUTHORS_scikit_optimize.md
 
 <div align="center">
 <pre>
   _____                              ____        _   _           _
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.1 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.2 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
 Research & Early Development License: BSD Description-Content-Type: text/
-markdown Provides-Extra: bokeh Provides-Extra: browniebee License-File:
-LICENSE.md License-File: AUTHORS_scikit_optimize.md
+markdown Provides-Extra: browniebee License-File: LICENSE.md License-File:
+AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
 
        |  __ \                            / __ \      | | (_)         (_)
 
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __
 
    |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \
```

### Comparing `ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/SOURCES.txt` & `ProcessOptimizer-0.8.2/ProcessOptimizer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,45 @@
 setup.py
 ProcessOptimizer/__init__.py
 ProcessOptimizer/acquisition.py
 ProcessOptimizer/bokeh_plot.py
 ProcessOptimizer/callbacks.py
 ProcessOptimizer/plots.py
 ProcessOptimizer/searchcv.py
-ProcessOptimizer/utils.py
 ProcessOptimizer.egg-info/PKG-INFO
 ProcessOptimizer.egg-info/SOURCES.txt
 ProcessOptimizer.egg-info/dependency_links.txt
 ProcessOptimizer.egg-info/requires.txt
 ProcessOptimizer.egg-info/top_level.txt
 ProcessOptimizer/learning/__init__.py
+ProcessOptimizer/learning/cook_estimator.py
 ProcessOptimizer/learning/forest.py
 ProcessOptimizer/learning/gbrt.py
+ProcessOptimizer/learning/has_gradients.py
+ProcessOptimizer/learning/use_named_args.py
 ProcessOptimizer/learning/gaussian_process/__init__.py
 ProcessOptimizer/learning/gaussian_process/gpr.py
 ProcessOptimizer/learning/gaussian_process/kernels.py
 ProcessOptimizer/model_systems/__init__.py
 ProcessOptimizer/model_systems/benchmarks.py
 ProcessOptimizer/model_systems/branin_hoo.py
+ProcessOptimizer/model_systems/gold_map.py
+ProcessOptimizer/model_systems/hart3.py
+ProcessOptimizer/model_systems/hart6.py
 ProcessOptimizer/model_systems/model_system.py
 ProcessOptimizer/model_systems/noise_models.py
+ProcessOptimizer/model_systems/peaks.py
+ProcessOptimizer/model_systems/poly2.py
 ProcessOptimizer/model_systems/second_order_polynomial_2d.py
 ProcessOptimizer/optimizer/_NSGA2.py
 ProcessOptimizer/optimizer/__init__.py
 ProcessOptimizer/optimizer/base.py
 ProcessOptimizer/optimizer/dummy.py
 ProcessOptimizer/optimizer/forest.py
 ProcessOptimizer/optimizer/gbrt.py
 ProcessOptimizer/optimizer/gp.py
 ProcessOptimizer/optimizer/optimizer.py
 ProcessOptimizer/space/__init__.py
 ProcessOptimizer/space/constraints.py
+ProcessOptimizer/space/normalize_dimensions.py
 ProcessOptimizer/space/space.py
 ProcessOptimizer/space/transformers.py
```

### Comparing `ProcessOptimizer-0.8.1/README.md` & `ProcessOptimizer-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.1/setup.py` & `ProcessOptimizer-0.8.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ProcessOptimizer',
-      version='0.8.1',
+      version='0.8.2',
       description='Sequential model-based optimization toolbox \
     (forked from scikit-optimize)',
       url='https://github.com/novonordisk-research/ProcessOptimizer',
       license='BSD',
       author='Novo Nordisk, Research & Early Development',
       packages=[
           'ProcessOptimizer',
           'ProcessOptimizer.learning',
           'ProcessOptimizer.model_systems',
           'ProcessOptimizer.optimizer',
           'ProcessOptimizer.space',
           'ProcessOptimizer.learning.gaussian_process'
           ],
-      install_requires=['numpy', 'matplotlib', 'scipy',
+      install_requires=['numpy', 'matplotlib', 'scipy', 'bokeh',
                         'scikit-learn>=0.24.2', 'six', 'deap', 'pyYAML'],
       extras_require={
-          "bokeh": ['bokeh', 'tornado'],
           "browniebee": ['numpy==1.23.3',
                          'matplotlib==3.5.3',
                          'scipy==1.9.1',
                          'scikit-learn==1.1.2',
                          'six==1.16.0',
                          'deap==1.3.3',
                          'pyYAML==6.0',
```

