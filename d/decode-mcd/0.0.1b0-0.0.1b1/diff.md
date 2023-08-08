# Comparing `tmp/decode-mcd-0.0.1b0.tar.gz` & `tmp/decode-mcd-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decode-mcd-0.0.1b0.tar", last modified: Tue Jul 11 10:57:28 2023, max compression
+gzip compressed data, was "decode-mcd-0.0.1b1.tar", last modified: Tue Aug  8 05:48:56 2023, max compression
```

## Comparing `decode-mcd-0.0.1b0.tar` & `decode-mcd-0.0.1b1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.537698 decode-mcd-0.0.1b0/
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     1072 2023-05-21 10:38:32.000000 decode-mcd-0.0.1b0/LICENSE
--rw-rw-r--   0 yazan     (1000) yazan     (1000)    14412 2023-07-11 10:57:28.537698 decode-mcd-0.0.1b0/PKG-INFO
--rw-rw-r--   0 yazan     (1000) yazan     (1000)    12525 2023-07-11 10:56:11.000000 decode-mcd-0.0.1b0/README.md
--rw-rw-r--   0 yazan     (1000) yazan     (1000)      859 2023-07-11 10:41:50.000000 decode-mcd-0.0.1b0/pyproject.toml
--rw-rw-r--   0 yazan     (1000) yazan     (1000)       38 2023-07-11 10:57:28.541698 decode-mcd-0.0.1b0/setup.cfg
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.529698 decode-mcd-0.0.1b0/src/
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.533698 decode-mcd-0.0.1b0/src/decode_mcd/
--rw-rw-r--   0 yazan     (1000) yazan     (1000)      357 2023-07-11 10:39:51.000000 decode-mcd-0.0.1b0/src/decode_mcd/__init__.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)    19009 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b0/src/decode_mcd/counterfactuals_generator.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     8428 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b0/src/decode_mcd/data_package.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     7799 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b0/src/decode_mcd/design_targets.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)       95 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b0/src/decode_mcd/mcd_exceptions.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)    14393 2023-07-11 10:26:35.000000 decode-mcd-0.0.1b0/src/decode_mcd/multi_objective_problem.py
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.533698 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/
--rw-rw-r--   0 yazan     (1000) yazan     (1000)    14412 2023-07-11 10:57:28.000000 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/PKG-INFO
--rw-rw-r--   0 yazan     (1000) yazan     (1000)      957 2023-07-11 10:57:28.000000 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/SOURCES.txt
--rw-rw-r--   0 yazan     (1000) yazan     (1000)        1 2023-07-11 10:57:28.000000 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/dependency_links.txt
--rw-rw-r--   0 yazan     (1000) yazan     (1000)       24 2023-07-11 10:57:28.000000 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/requires.txt
--rw-rw-r--   0 yazan     (1000) yazan     (1000)       30 2023-07-11 10:57:28.000000 decode-mcd-0.0.1b0/src/decode_mcd.egg-info/top_level.txt
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.537698 decode-mcd-0.0.1b0/src/decode_mcd_private/
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     2750 2023-05-21 10:38:32.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/DPPsampling.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)        0 2023-06-16 10:57:18.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/__init__.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     2266 2023-06-27 11:04:35.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/calculate_dtai.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     1690 2023-06-19 04:49:26.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/classification_evaluator.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     2584 2023-06-06 05:17:07.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/stats_methods.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)      208 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b0/src/decode_mcd_private/validation_utils.py
-drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-07-11 10:57:28.537698 decode-mcd-0.0.1b0/tests/
--rw-rw-r--   0 yazan     (1000) yazan     (1000)      660 2023-06-27 11:04:35.000000 decode-mcd-0.0.1b0/tests/test_calculate_dtai.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     2390 2023-06-26 05:01:07.000000 decode-mcd-0.0.1b0/tests/test_classification_evaluator.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     5892 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b0/tests/test_counterfactuals_generator.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     8443 2023-07-11 10:20:54.000000 decode-mcd-0.0.1b0/tests/test_data_package.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     5117 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b0/tests/test_design_targets.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     8710 2023-07-10 05:37:04.000000 decode-mcd-0.0.1b0/tests/test_mcd_e2e.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     8969 2023-07-10 05:37:04.000000 decode-mcd-0.0.1b0/tests/test_multi_objective_problem.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     1722 2023-07-10 10:18:48.000000 decode-mcd-0.0.1b0/tests/test_quick_start.py
--rw-rw-r--   0 yazan     (1000) yazan     (1000)     5465 2023-06-26 05:01:07.000000 decode-mcd-0.0.1b0/tests/test_stats_methods.py
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     1072 2023-05-21 10:38:32.000000 decode-mcd-0.0.1b1/LICENSE
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)    14421 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/PKG-INFO
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)    12534 2023-07-16 13:12:22.000000 decode-mcd-0.0.1b1/README.md
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)      860 2023-08-08 05:48:50.000000 decode-mcd-0.0.1b1/pyproject.toml
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)       38 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/setup.cfg
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.828218 decode-mcd-0.0.1b1/src/
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.828218 decode-mcd-0.0.1b1/src/decode_mcd/
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)      357 2023-07-11 10:39:51.000000 decode-mcd-0.0.1b1/src/decode_mcd/__init__.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)    19009 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b1/src/decode_mcd/counterfactuals_generator.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     8428 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b1/src/decode_mcd/data_package.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     7799 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b1/src/decode_mcd/design_targets.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)       95 2023-07-11 10:26:36.000000 decode-mcd-0.0.1b1/src/decode_mcd/mcd_exceptions.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)    14430 2023-08-02 11:13:13.000000 decode-mcd-0.0.1b1/src/decode_mcd/multi_objective_problem.py
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)    14421 2023-08-08 05:48:56.000000 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/PKG-INFO
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)      957 2023-08-08 05:48:56.000000 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/SOURCES.txt
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)        1 2023-08-08 05:48:56.000000 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/dependency_links.txt
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)       24 2023-08-08 05:48:56.000000 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/requires.txt
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)       30 2023-08-08 05:48:56.000000 decode-mcd-0.0.1b1/src/decode_mcd.egg-info/top_level.txt
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/src/decode_mcd_private/
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     2750 2023-05-21 10:38:32.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/DPPsampling.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)        0 2023-06-16 10:57:18.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/__init__.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     2266 2023-06-27 11:04:35.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/calculate_dtai.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     1690 2023-06-19 04:49:26.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/classification_evaluator.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     2595 2023-08-02 11:16:28.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/stats_methods.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)      208 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b1/src/decode_mcd_private/validation_utils.py
+drwxrwxr-x   0 yazan     (1000) yazan     (1000)        0 2023-08-08 05:48:56.832218 decode-mcd-0.0.1b1/tests/
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)      660 2023-06-27 11:04:35.000000 decode-mcd-0.0.1b1/tests/test_calculate_dtai.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     2390 2023-06-26 05:01:07.000000 decode-mcd-0.0.1b1/tests/test_classification_evaluator.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     5892 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b1/tests/test_counterfactuals_generator.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     8443 2023-07-11 10:20:54.000000 decode-mcd-0.0.1b1/tests/test_data_package.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     5117 2023-07-10 10:53:35.000000 decode-mcd-0.0.1b1/tests/test_design_targets.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     8710 2023-07-10 05:37:04.000000 decode-mcd-0.0.1b1/tests/test_mcd_e2e.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     8969 2023-07-10 05:37:04.000000 decode-mcd-0.0.1b1/tests/test_multi_objective_problem.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     1722 2023-07-10 10:18:48.000000 decode-mcd-0.0.1b1/tests/test_quick_start.py
+-rw-rw-r--   0 yazan     (1000) yazan     (1000)     5465 2023-06-26 05:01:07.000000 decode-mcd-0.0.1b1/tests/test_stats_methods.py
```

### Comparing `decode-mcd-0.0.1b0/LICENSE` & `decode-mcd-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/PKG-INFO` & `decode-mcd-0.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decode-mcd
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: MCD generates counterfactuals that meet multiple, customizable objectives in both the feature and performance spaces.
 Author: Lyle Regenwetter & Yazan Abu Obaideh
 License: MIT License
         
         Copyright (c) 2023 Lyleregenwetter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -199,19 +199,19 @@
 from pymoo.core.variable import Real
 
 import numpy as np
 from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget
 
 x = np.random.random(100)
 x = x.reshape(100, 1)
-y = x * 100 + random.random()
+y = x * 100
 
 
 def predict(_x):
-    return _x * 100
+    return _x * 100 + random.random()
 
 
 data_package = DataPackage(features_dataset=x,
                            predictions_dataset=y,
                            query_x=x[0].reshape(1, 1),
                            design_targets=DesignTargets([ContinuousTarget(label=0,
                                                                           lower_bound=25,
@@ -238,14 +238,15 @@
 
 
 <!-- USAGE EXAMPLES -->
 
 [//]: # (## I-Got-Time Guide)
 
 [//]: # ()
+
 [//]: # (1. Either install MCD with pip as shown in the Quick-Start Guide, or fork the repo with)
 
 [//]: # (   ```git clone git@github.com:Lyleregenwetter/Multiobjective-Counterfactuals-for-Design.git```)
 
 [//]: # (2. Now, customize the code below to fit your datasets and model. The template below assumes the following:)
 
 [//]: # (    * The features_dataset _X_ has 4 columns: R1, R2, C1, in order. R1 and R2 are real variables)
@@ -257,28 +258,31 @@
 [//]: # (      O_C1 is a categorical/choice variable. O_P1 and O_P2 represent the probabilities of belonging to classes A and B,)
 
 [//]: # (      respectively, where a design can belong to either class A or B and nothing else.)
 
 [//]: # (    *)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (from pymoo.core.variable import Real, Choice)
 
 [//]: # (from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget)
 
 [//]: # ()
+
 [//]: # (x, y = ...  # load your data)
 
 [//]: # (model = ...  # load your model)
 
 [//]: # (query_x = ...  # define the initial design or starting point)
 
 [//]: # ()
+
 [//]: # (data_package = DataPackage&#40;features_dataset=x,)
 
 [//]: # (                           predictions_dataset=y,)
 
 [//]: # (                           query_x=query_x,)
 
 [//]: # (                           design_targets=DesignTargets&#40;[ContinuousTarget&#40;label=0,)
@@ -302,30 +306,33 @@
 [//]: # (                           # datasets_validity=...,)
 
 [//]: # (                           # datasets_scores=...,)
 
 [//]: # (                           &#41;)
 
 [//]: # ()
+
 [//]: # (problem = MultiObjectiveProblem&#40;data_package=data_package,)
 
 [//]: # (                                prediction_function=lambda design: model.predict&#40;design&#41;,)
 
 [//]: # (                                constraint_functions=[]&#41;)
 
 [//]: # ()
+
 [//]: # (generator = CounterfactualsGenerator&#40;problem=problem,)
 
 [//]: # (                                     pop_size=10,)
 
 [//]: # (                                     initialize_from_dataset=False,)
 
 [//]: # (                                     verbose=True&#41;)
 
 [//]: # ()
+
 [//]: # (generator.generate&#40;n_generations=10&#41;)
 
 [//]: # (counterfactuals = generator.sample_with_dtai&#40;num_samples=10, gower_weight=1,)
 
 [//]: # (                                             avg_gower_weight=1, cfc_weight=1,)
 
 [//]: # (                                             diversity_weight=50&#41;)
@@ -334,17 +341,15 @@
 
 [//]: # (```)
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
-- [ ] We are currently working on support gradient-based optimization
-
-
+- [ ] We are currently working on support for gradient-based optimization
 
 See the [open issues](https://github.com/Lyleregenwetter/Multiobjective-Counterfactuals-for-Design/issues) for a full
 list of proposed features (and
 known issues).
 
 [//]: # (<p align="right">&#40;<a href="#readme-top">back to top</a>&#41;</p>)
 
@@ -408,14 +413,14 @@
 
 [python-url]: https://www.python.org/
 
 [pandas-badge-url]: https://img.shields.io/badge/framework-pandas-red
 
 [pandas-url]: https://pandas.pydata.org/
 
-[numpy-badge-url]: https://img.shields.io/badge/frameowrk-numpy-green
+[numpy-badge-url]: https://img.shields.io/badge/framework-numpy-green
 
 [numpy-url]: https://numpy.org/
 
 [pymoo-badge-url]: https://img.shields.io/badge/framework-pymoo-blue
 
 [pymoo-url]: https://pymoo.org/
```

### Comparing `decode-mcd-0.0.1b0/README.md` & `decode-mcd-0.0.1b1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -163,19 +163,19 @@
 from pymoo.core.variable import Real
 
 import numpy as np
 from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget
 
 x = np.random.random(100)
 x = x.reshape(100, 1)
-y = x * 100 + random.random()
+y = x * 100
 
 
 def predict(_x):
-    return _x * 100
+    return _x * 100 + random.random()
 
 
 data_package = DataPackage(features_dataset=x,
                            predictions_dataset=y,
                            query_x=x[0].reshape(1, 1),
                            design_targets=DesignTargets([ContinuousTarget(label=0,
                                                                           lower_bound=25,
@@ -202,14 +202,15 @@
 
 
 <!-- USAGE EXAMPLES -->
 
 [//]: # (## I-Got-Time Guide)
 
 [//]: # ()
+
 [//]: # (1. Either install MCD with pip as shown in the Quick-Start Guide, or fork the repo with)
 
 [//]: # (   ```git clone git@github.com:Lyleregenwetter/Multiobjective-Counterfactuals-for-Design.git```)
 
 [//]: # (2. Now, customize the code below to fit your datasets and model. The template below assumes the following:)
 
 [//]: # (    * The features_dataset _X_ has 4 columns: R1, R2, C1, in order. R1 and R2 are real variables)
@@ -221,28 +222,31 @@
 [//]: # (      O_C1 is a categorical/choice variable. O_P1 and O_P2 represent the probabilities of belonging to classes A and B,)
 
 [//]: # (      respectively, where a design can belong to either class A or B and nothing else.)
 
 [//]: # (    *)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (from pymoo.core.variable import Real, Choice)
 
 [//]: # (from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget)
 
 [//]: # ()
+
 [//]: # (x, y = ...  # load your data)
 
 [//]: # (model = ...  # load your model)
 
 [//]: # (query_x = ...  # define the initial design or starting point)
 
 [//]: # ()
+
 [//]: # (data_package = DataPackage&#40;features_dataset=x,)
 
 [//]: # (                           predictions_dataset=y,)
 
 [//]: # (                           query_x=query_x,)
 
 [//]: # (                           design_targets=DesignTargets&#40;[ContinuousTarget&#40;label=0,)
@@ -266,30 +270,33 @@
 [//]: # (                           # datasets_validity=...,)
 
 [//]: # (                           # datasets_scores=...,)
 
 [//]: # (                           &#41;)
 
 [//]: # ()
+
 [//]: # (problem = MultiObjectiveProblem&#40;data_package=data_package,)
 
 [//]: # (                                prediction_function=lambda design: model.predict&#40;design&#41;,)
 
 [//]: # (                                constraint_functions=[]&#41;)
 
 [//]: # ()
+
 [//]: # (generator = CounterfactualsGenerator&#40;problem=problem,)
 
 [//]: # (                                     pop_size=10,)
 
 [//]: # (                                     initialize_from_dataset=False,)
 
 [//]: # (                                     verbose=True&#41;)
 
 [//]: # ()
+
 [//]: # (generator.generate&#40;n_generations=10&#41;)
 
 [//]: # (counterfactuals = generator.sample_with_dtai&#40;num_samples=10, gower_weight=1,)
 
 [//]: # (                                             avg_gower_weight=1, cfc_weight=1,)
 
 [//]: # (                                             diversity_weight=50&#41;)
@@ -298,17 +305,15 @@
 
 [//]: # (```)
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
-- [ ] We are currently working on support gradient-based optimization
-
-
+- [ ] We are currently working on support for gradient-based optimization
 
 See the [open issues](https://github.com/Lyleregenwetter/Multiobjective-Counterfactuals-for-Design/issues) for a full
 list of proposed features (and
 known issues).
 
 [//]: # (<p align="right">&#40;<a href="#readme-top">back to top</a>&#41;</p>)
 
@@ -372,14 +377,14 @@
 
 [python-url]: https://www.python.org/
 
 [pandas-badge-url]: https://img.shields.io/badge/framework-pandas-red
 
 [pandas-url]: https://pandas.pydata.org/
 
-[numpy-badge-url]: https://img.shields.io/badge/frameowrk-numpy-green
+[numpy-badge-url]: https://img.shields.io/badge/framework-numpy-green
 
 [numpy-url]: https://numpy.org/
 
 [pymoo-badge-url]: https://img.shields.io/badge/framework-pymoo-blue
 
 [pymoo-url]: https://pymoo.org/
```

### Comparing `decode-mcd-0.0.1b0/pyproject.toml` & `decode-mcd-0.0.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decode-mcd"
-version = "0.0.1b"
+version = "0.0.1b1"
 description = "MCD generates counterfactuals that meet multiple, customizable objectives in both the feature and performance spaces."
 readme = "README.md"
 authors = [{ name = "Lyle Regenwetter & Yazan Abu Obaideh" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd/counterfactuals_generator.py` & `decode-mcd-0.0.1b1/src/decode_mcd/counterfactuals_generator.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd/data_package.py` & `decode-mcd-0.0.1b1/src/decode_mcd/data_package.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd/design_targets.py` & `decode-mcd-0.0.1b1/src/decode_mcd/design_targets.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd/multi_objective_problem.py` & `decode-mcd-0.0.1b1/src/decode_mcd/multi_objective_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         return self._calculate_mixed_constraint_satisfaction(x_full, y, x_constraint_functions, design_targets)
 
     def _calculate_mixed_constraint_satisfaction(self,
                                                  x_full: pd.DataFrame,
                                                  y: pd.DataFrame,
                                                  x_constraint_functions: list,
                                                  design_targets: DesignTargets):
-        n_total_constraints = design_targets.count_constrained_labels()
+        n_total_constraints = design_targets.count_constrained_labels() + len(x_constraint_functions)
         n_rows = x_full.shape[0]
         result = np.zeros(shape=(n_rows, n_total_constraints))
 
         self._append_x_constraint_satisfaction(result, x_full, x_constraint_functions, n_total_constraints)
         self._append_proba_satisfaction(result, y, design_targets)
         self._append_satisfaction(result, self._evaluate_regression_satisfaction, y, design_targets,
                                   design_targets.get_continuous_labels())
@@ -240,15 +240,15 @@
 
     def _append_x_constraint_satisfaction(self, result: np.ndarray,
                                           x_full: pd.DataFrame,
                                           x_constraint_functions: List[callable],
                                           n_total_constraints: int):
         for i in range(len(x_constraint_functions)):
             # TODO: discuss this change with Lyle
-            result[:, n_total_constraints - 1 - i] = x_constraint_functions[i](x_full).flatten()
+            result[:, n_total_constraints - 1 - i] = x_constraint_functions[i](x_full).values.flatten()
 
     def _evaluate_categorical_satisfaction(self, y: pd.DataFrame, y_category_constraints: DesignTargets):
         actual = y.loc[:, y_category_constraints.get_classification_labels()]
         # dtype=object is needed, otherwise the operation is deprecated
         targets = np.array([[i for i in j] for j in y_category_constraints.get_desired_classes()], dtype=object)
         return ClassificationEvaluator().evaluate_categorical(actual, targets=targets)
```

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd.egg-info/PKG-INFO` & `decode-mcd-0.0.1b1/src/decode_mcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decode-mcd
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: MCD generates counterfactuals that meet multiple, customizable objectives in both the feature and performance spaces.
 Author: Lyle Regenwetter & Yazan Abu Obaideh
 License: MIT License
         
         Copyright (c) 2023 Lyleregenwetter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -199,19 +199,19 @@
 from pymoo.core.variable import Real
 
 import numpy as np
 from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget
 
 x = np.random.random(100)
 x = x.reshape(100, 1)
-y = x * 100 + random.random()
+y = x * 100
 
 
 def predict(_x):
-    return _x * 100
+    return _x * 100 + random.random()
 
 
 data_package = DataPackage(features_dataset=x,
                            predictions_dataset=y,
                            query_x=x[0].reshape(1, 1),
                            design_targets=DesignTargets([ContinuousTarget(label=0,
                                                                           lower_bound=25,
@@ -238,14 +238,15 @@
 
 
 <!-- USAGE EXAMPLES -->
 
 [//]: # (## I-Got-Time Guide)
 
 [//]: # ()
+
 [//]: # (1. Either install MCD with pip as shown in the Quick-Start Guide, or fork the repo with)
 
 [//]: # (   ```git clone git@github.com:Lyleregenwetter/Multiobjective-Counterfactuals-for-Design.git```)
 
 [//]: # (2. Now, customize the code below to fit your datasets and model. The template below assumes the following:)
 
 [//]: # (    * The features_dataset _X_ has 4 columns: R1, R2, C1, in order. R1 and R2 are real variables)
@@ -257,28 +258,31 @@
 [//]: # (      O_C1 is a categorical/choice variable. O_P1 and O_P2 represent the probabilities of belonging to classes A and B,)
 
 [//]: # (      respectively, where a design can belong to either class A or B and nothing else.)
 
 [//]: # (    *)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (from pymoo.core.variable import Real, Choice)
 
 [//]: # (from decode_mcd import DesignTargets, DataPackage, MultiObjectiveProblem, CounterfactualsGenerator, ContinuousTarget)
 
 [//]: # ()
+
 [//]: # (x, y = ...  # load your data)
 
 [//]: # (model = ...  # load your model)
 
 [//]: # (query_x = ...  # define the initial design or starting point)
 
 [//]: # ()
+
 [//]: # (data_package = DataPackage&#40;features_dataset=x,)
 
 [//]: # (                           predictions_dataset=y,)
 
 [//]: # (                           query_x=query_x,)
 
 [//]: # (                           design_targets=DesignTargets&#40;[ContinuousTarget&#40;label=0,)
@@ -302,30 +306,33 @@
 [//]: # (                           # datasets_validity=...,)
 
 [//]: # (                           # datasets_scores=...,)
 
 [//]: # (                           &#41;)
 
 [//]: # ()
+
 [//]: # (problem = MultiObjectiveProblem&#40;data_package=data_package,)
 
 [//]: # (                                prediction_function=lambda design: model.predict&#40;design&#41;,)
 
 [//]: # (                                constraint_functions=[]&#41;)
 
 [//]: # ()
+
 [//]: # (generator = CounterfactualsGenerator&#40;problem=problem,)
 
 [//]: # (                                     pop_size=10,)
 
 [//]: # (                                     initialize_from_dataset=False,)
 
 [//]: # (                                     verbose=True&#41;)
 
 [//]: # ()
+
 [//]: # (generator.generate&#40;n_generations=10&#41;)
 
 [//]: # (counterfactuals = generator.sample_with_dtai&#40;num_samples=10, gower_weight=1,)
 
 [//]: # (                                             avg_gower_weight=1, cfc_weight=1,)
 
 [//]: # (                                             diversity_weight=50&#41;)
@@ -334,17 +341,15 @@
 
 [//]: # (```)
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
-- [ ] We are currently working on support gradient-based optimization
-
-
+- [ ] We are currently working on support for gradient-based optimization
 
 See the [open issues](https://github.com/Lyleregenwetter/Multiobjective-Counterfactuals-for-Design/issues) for a full
 list of proposed features (and
 known issues).
 
 [//]: # (<p align="right">&#40;<a href="#readme-top">back to top</a>&#41;</p>)
 
@@ -408,14 +413,14 @@
 
 [python-url]: https://www.python.org/
 
 [pandas-badge-url]: https://img.shields.io/badge/framework-pandas-red
 
 [pandas-url]: https://pandas.pydata.org/
 
-[numpy-badge-url]: https://img.shields.io/badge/frameowrk-numpy-green
+[numpy-badge-url]: https://img.shields.io/badge/framework-numpy-green
 
 [numpy-url]: https://numpy.org/
 
 [pymoo-badge-url]: https://img.shields.io/badge/framework-pymoo-blue
 
 [pymoo-url]: https://pymoo.org/
```

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd.egg-info/SOURCES.txt` & `decode-mcd-0.0.1b1/src/decode_mcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd_private/DPPsampling.py` & `decode-mcd-0.0.1b1/src/decode_mcd_private/DPPsampling.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd_private/calculate_dtai.py` & `decode-mcd-0.0.1b1/src/decode_mcd_private/calculate_dtai.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd_private/classification_evaluator.py` & `decode-mcd-0.0.1b1/src/decode_mcd_private/classification_evaluator.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/src/decode_mcd_private/stats_methods.py` & `decode-mcd-0.0.1b1/src/decode_mcd_private/stats_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,14 @@
 
 
 def changed_features_ratio(designs_dataframe: pd.DataFrame,
                            reference_dataframe: pd.DataFrame,
                            n_features: int):
     designs = designs_dataframe.values
     reference = reference_dataframe.iloc[0].values
-    changes = np.count_nonzero((designs - reference), axis=1)
+    changes = np.count_nonzero(np.not_equal(designs, reference), axis=1)
     return changes / n_features
 
 
 def to_dataframe(numpy_array: np.ndarray):
     dummy_columns = [_ for _ in range(numpy_array.shape[1])]
     return pd.DataFrame(numpy_array, columns=dummy_columns)
```

### Comparing `decode-mcd-0.0.1b0/tests/test_calculate_dtai.py` & `decode-mcd-0.0.1b1/tests/test_calculate_dtai.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_classification_evaluator.py` & `decode-mcd-0.0.1b1/tests/test_classification_evaluator.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_counterfactuals_generator.py` & `decode-mcd-0.0.1b1/tests/test_counterfactuals_generator.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_data_package.py` & `decode-mcd-0.0.1b1/tests/test_data_package.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_design_targets.py` & `decode-mcd-0.0.1b1/tests/test_design_targets.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_mcd_e2e.py` & `decode-mcd-0.0.1b1/tests/test_mcd_e2e.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_multi_objective_problem.py` & `decode-mcd-0.0.1b1/tests/test_multi_objective_problem.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_quick_start.py` & `decode-mcd-0.0.1b1/tests/test_quick_start.py`

 * *Files identical despite different names*

### Comparing `decode-mcd-0.0.1b0/tests/test_stats_methods.py` & `decode-mcd-0.0.1b1/tests/test_stats_methods.py`

 * *Files identical despite different names*

