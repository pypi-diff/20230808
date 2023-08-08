# Comparing `tmp/TSInterpret-0.3.2.tar.gz` & `tmp/TSInterpret-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.3.2.tar", last modified: Wed Jul 19 13:06:00 2023, max compression
+gzip compressed data, was "TSInterpret-0.3.3.tar", last modified: Tue Aug  8 13:36:52 2023, max compression
```

## Comparing `TSInterpret-0.3.2.tar` & `TSInterpret-0.3.3.tar`

### file list

```diff
@@ -1,87 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.652955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:06:00.648954 TSInterpret-0.3.2/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 13:06:00.000000 TSInterpret-0.3.2/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 13:06:00.656955 TSInterpret-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-19 13:05:49.000000 TSInterpret-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.298654 TSInterpret-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:37.000000 TSInterpret-0.3.3/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-08 13:36:52.298654 TSInterpret-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16663 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/
+-rw-r--r--   0 runner    (1001) docker     (123)    17341 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12192 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.294654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.298654 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.298654 TSInterpret-0.3.3/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:36:52.290653 TSInterpret-0.3.3/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-08 13:36:52.000000 TSInterpret-0.3.3/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-08-08 13:36:52.000000 TSInterpret-0.3.3/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:36:52.000000 TSInterpret-0.3.3/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-08 13:36:52.000000 TSInterpret-0.3.3/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 13:36:52.000000 TSInterpret-0.3.3/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:36:52.298654 TSInterpret-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-08 13:36:38.000000 TSInterpret-0.3.3/setup.py
```

### Comparing `TSInterpret-0.3.2/ClassificationModels/CNN.py` & `TSInterpret-0.3.3/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/CNN_T.py` & `TSInterpret-0.3.3/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/DecisionTree.py` & `TSInterpret-0.3.3/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/LSTM.py` & `TSInterpret-0.3.3/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/LSTM_T.py` & `TSInterpret-0.3.3/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/ResNet.py` & `TSInterpret-0.3.3/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/ClassificationModels/utils.py` & `TSInterpret-0.3.3/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/LICENSE` & `TSInterpret-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/PKG-INFO` & `TSInterpret-0.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.3.2
+Version: 0.3.3
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -47,37 +47,18 @@
 
 ## 💈 Installation
 ```shell
 pip install TSInterpret
 ```
 You can install the latest development version from GitHub as so:
 ```shell
-pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
+pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/main.zip
 ```
 
-Or, through SSH:
-```shell
-pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
-```
-
-On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
 
-1. Set Enviroment Variable
-```shell
-set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
-```
-2. Install sklearn in advance 
-```shell
-pip install sklearn=0.0
-```
-
-3. Install TsIntrerpret
-```shell
-pip install TSInterpret
-```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.2 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.3 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
@@ -19,27 +19,20 @@
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
-github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
-through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
-known_installation_issue_due_to_the_sklearn_brownout_in_third_party
-dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
-are_fixed:_1._Set_Enviroment_Variable_```shell_set
-SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
-advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
-pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
-simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
-Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
-check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
-deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/
+main.zip_```_##_ð«_Quickstart_The_following_example_creates_a_simple_Neural
+Network_based_on_tensorflow_and_interprets_the_Classfier_with_Integrated
+Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples_check_out
+the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking_deep
+learning_interpretability_in_time_series_predictions."_Advances_in_neural
 information_processing_systems_33_(2020):_6441-6452._###_Import_```python
 import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
 as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
 ```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
 Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
 example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
```

### Comparing `TSInterpret-0.3.2/README.md` & `TSInterpret-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,37 +21,18 @@
 
 ## 💈 Installation
 ```shell
 pip install TSInterpret
 ```
 You can install the latest development version from GitHub as so:
 ```shell
-pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
+pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/main.zip
 ```
 
-Or, through SSH:
-```shell
-pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
-```
-
-On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
 
-1. Set Enviroment Variable
-```shell
-set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
-```
-2. Install sklearn in advance 
-```shell
-pip install sklearn=0.0
-```
-
-3. Install TsIntrerpret
-```shell
-pip install TSInterpret
-```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
```

#### html2text {}

```diff
@@ -7,27 +7,20 @@
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
-github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
-through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
-known_installation_issue_due_to_the_sklearn_brownout_in_third_party
-dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
-are_fixed:_1._Set_Enviroment_Variable_```shell_set
-SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
-advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
-pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
-simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
-Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
-check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
-deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/
+main.zip_```_##_ð«_Quickstart_The_following_example_creates_a_simple_Neural
+Network_based_on_tensorflow_and_interprets_the_Classfier_with_Integrated
+Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples_check_out
+the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking_deep
+learning_interpretability_in_time_series_predictions."_Advances_in_neural
 information_processing_systems_33_(2020):_6441-6452._###_Import_```python
 import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
 as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
 ```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
 Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
 example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,56 +81,68 @@
         #    self.Grad = FeaturePermutation(model)
         elif method == "FA":
             self.Grad = FeatureAblation(model)
         elif method == "FO":
             self.Grad = Occlusion(model)
         self.device = device
 
-    def explain(self, item: np.ndarray, labels: int, TSR=None):
+    def explain(self, item: np.ndarray, labels: int, TSR=None, **kwargs):
         """Method to explain the model based on the item.
         Arguments:
             item np.array: item to get feature attribution for, if `mode = time`->`(1,time,feat)`  or `mode = feat`->`(1,feat,time)`
             labels int: label
             TSR bool: if True time series rescaling according to [1] is used, else plain (scaled) weights are returened
         Returns:
             np.array: feature attribution weights `mode = time`->`(time,feat)` or `mode = feat`->`(feat,time)`
         """
+
         mask = np.zeros((self.NumTimeSteps, self.NumFeatures), dtype=int)
         for i in range(self.NumTimeSteps):
             mask[i, :] = i
         rescaledGrad = np.zeros(item.shape)
         idx = 0
         item = np.array(item.tolist())  # , dtype=np.float64)
         input = torch.from_numpy(item)
 
         input = input.reshape(-1, self.NumTimeSteps, self.NumFeatures).to(self.device)
         input = Variable(input, volatile=False, requires_grad=True)
 
         batch_size = input.shape[0]
 
-        inputMask = np.zeros(input.shape)
-        inputMask[:, :, :] = mask
+        if "inputMask" in kwargs.keys():
+            inputMask = kwargs = ["inputMask"]
+        else:
+            inputMask = np.zeros(input.shape)
+            inputMask[:, :, :] = mask
         inputMask = torch.from_numpy(inputMask).to(self.device)
         mask_single = torch.from_numpy(mask).to(self.device)
         mask_single = mask_single.reshape(1, self.NumTimeSteps, self.NumFeatures).to(
             self.device
         )
         # input = samples.reshape(-1, args.NumTimeSteps, args.NumFeatures).to(device)
         if self.mode == "feat":
             input = input.reshape(-1, self.NumFeatures, self.NumTimeSteps)
-        baseline_single = (
-            torch.from_numpy(np.random.random(input.shape)).float().to(self.device)
-        )
-        baseline_multiple = (
-            torch.from_numpy(
-                np.random.random((input.shape[0] * 5, input.shape[1], input.shape[2]))
+        if "baseline_single" in kwargs.keys():
+            baseline_single = kwargs["baseline_single"]
+        else:
+            baseline_single = (
+                torch.from_numpy(np.random.random(input.shape)).float().to(self.device)
+            )  # random.random
+        if "baseline_multiple" in kwargs.keys():
+            baseline_multiple = kwargs["baseline_multiple"]
+        else:
+            baseline_multiple = (
+                torch.from_numpy(
+                    np.random.random(
+                        (input.shape[0] * 5, input.shape[1], input.shape[2])
+                    )
+                )
+                .float()
+                .to(self.device)
             )
-            .float()
-            .to(self.device)
-        )
         input = input.float()
         base = None
         has_sliding_window = None
         if self.method == "GRAD":
             attributions = self.Grad.attribute(input, target=labels)
         elif self.method == "IG":
             base = baseline_single
@@ -180,19 +192,24 @@
                 baselines=baseline_single,
             )
         if TSR is not None:
             self.tsr = TSR
 
         if self.tsr:
             # print('TSR', TSR)
+            if "assignment" in kwargs.keys():
+                assignment = kwargs["assignment"]
+            else:
+                assignment = None
             TSR_attributions = self._getTwoStepRescaling(
                 input,
                 labels,
                 hasBaseline=base,
                 hasSliding_window_shapes=has_sliding_window,
+                assignment=assignment,
             )
             # print('TSR Attribution', TSR_attributions.shape)
             TSR_saliency = self._givenAttGetRescaledSaliency(
                 TSR_attributions, isTensor=False
             )
             # print('TSR Saliency', TSR_saliency.shape)
             return TSR_saliency
@@ -208,23 +225,20 @@
     def _getTwoStepRescaling(
         self,
         input,
         TestingLabel,
         hasBaseline=None,
         hasFeatureMask=None,
         hasSliding_window_shapes=None,
+        assignment=None,
     ):
         sequence_length = self.NumTimeSteps
         input_size = self.NumFeatures
-        assignment = input[0, 0, 0]
-        # TODO IS THIS CORRECT TO BE PUT HERE
-        # if self.mode == "feat":
-        #    hasSliding_window_shapes = (1, self.NumFeatures)
-        # else:
-        #    hasSliding_window_shapes = (self.NumFeatures, 1)
+        if assignment is None:
+            assignment = input[0, 0, 0]
         timeGrad = np.zeros((1, sequence_length))
         inputGrad = np.zeros((input_size, 1))
         newGrad = np.zeros((input_size, sequence_length))
         # print("has Sliding Window", hasSliding_window_shapes)
         if self.mode == "time":
             input = input.reshape(-1, sequence_length, input_size)
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 import logging
 import multiprocessing
 import numbers
-import sys
 from typing import Tuple
 import numpy as np
 import pandas as pd
-
-# Workaround for mlrose package
-import six
 from sklearn.neighbors import KDTree
 from skopt import gbrt_minimize, gp_minimize
-
-sys.modules["sklearn.externals.six"] = six
-import mlrose
-
-from TSInterpret.InterpretabilityModels.counterfactual.CF import CF
-from TSInterpret.Models.PyTorchModel import PyTorchModel
-from TSInterpret.Models.SklearnModel import SklearnModel
-from TSInterpret.Models.TensorflowModel import TensorFlowModel
+from TSInterpret.InterpretabilityModels.counterfactual.COMTE.Problem import (
+    LossDiscreteState,
+    Problem,
+)
+from TSInterpret.InterpretabilityModels.counterfactual.COMTE.Optmization_helpers import (
+    random_hill_climb,
+)
 
 
 class BaseExplanation:
     def __init__(
         self,
         clf,
         timeseries,
@@ -87,17 +82,14 @@
 
     def _get_distractors(self, x_test, to_maximize, n_distractors=2):
         self.construct_per_class_trees()
         # to_maximize can be int, string or np.int64
         if isinstance(to_maximize, numbers.Integral):
             to_maximize = np.unique(self.labels)[to_maximize]
         distractors = []
-        # print('to_maximize',to_maximize)
-        # print('Class Tree',self.per_class_trees)
-        # print('Class Tree with id',self.per_class_trees[to_maximize])
         for idx in (
             self.per_class_trees[to_maximize]
             .query(x_test.T.flatten().reshape(1, -1), k=n_distractors)[1]
             .flatten()
         ):
             distractors.append(
                 self.timeseries[[self.per_class_node_indices[to_maximize][idx]], :, :]
@@ -328,66 +320,14 @@
                 explanation.append(best_column)
 
         other = modified
         target = np.argmax(self.clf(other), axis=1)
         return other, target
 
 
-class LossDiscreteState:
-    def __init__(
-        self,
-        label_idx,
-        clf,
-        x_test,
-        distractor,
-        cols_swap,
-        reg,
-        max_features=3,
-        maximize=True,
-    ):
-        self.target = label_idx
-        self.clf = clf
-        self.x_test = x_test
-        self.reg = reg
-        self.distractor = distractor
-        self.cols_swap = cols_swap  # Column names that we can swap
-        self.prob_type = "discrete"
-        self.max_features = 3 if max_features is None else max_features
-        self.maximize = maximize
-        self.window_size = x_test.shape[-1]
-        self.channels = x_test.shape[-2]
-
-    def __call__(self, feature_matrix):
-        return self.evaluate(feature_matrix)
-
-    def evaluate(self, feature_matrix):
-        new_case = self.x_test.copy()
-        assert len(self.cols_swap) == len(feature_matrix)
-
-        for col_replace, a in zip(self.cols_swap, feature_matrix):
-            if a == 1:
-                new_case[0][col_replace] = self.distractor[0][col_replace]
-
-        replaced_feature_count = np.sum(feature_matrix)
-
-        input_ = new_case.reshape(1, self.channels, self.window_size)
-        result = self.clf(input_)[0][self.target]
-        feature_loss = self.reg * np.maximum(
-            0, replaced_feature_count - self.max_features
-        )
-        loss_pred = np.square(np.maximum(0, 0.95 - result))
-
-        loss_pred = loss_pred + feature_loss
-        # print(loss_pred)
-        return -loss_pred if self.maximize else loss_pred
-
-    def get_prob_type(self):
-        return self.prob_type
-
-
 class OptimizedSearch(BaseExplanation):
     def __init__(
         self,
         clf,
         timeseries,
         labels,
         silent,
@@ -410,18 +350,16 @@
             x_test,
             dist,
             columns,
             reg=0.8,
             max_features=num_features,
             maximize=False,
         )
-        problem = mlrose.DiscreteOpt(
-            length=len(columns), fitness_fn=fitness_fn, maximize=False, max_val=2
-        )
-        best_state, best_fitness = mlrose.random_hill_climb(
+        problem = Problem(length=len(columns), loss=fitness_fn, max_val=2)
+        best_state, best_fitness = random_hill_climb(
             problem,
             max_attempts=self.max_attemps,
             max_iters=self.maxiter,
             init_state=init,
             restarts=5,
         )
 
@@ -465,17 +403,14 @@
         orig_preds = self.clf(input_)
 
         orig_label = np.argmax(orig_preds)
 
         if to_maximize is None:
             to_maximize = np.argsort(orig_preds)[0][-2:-1][0]
 
-        # print('Current may',np.argmax(orig_preds))
-        # print(to_maximize)
-
         if orig_label == to_maximize:
             print("Original and Target Label are identical !")
             return None, None
 
         explanation = self._get_explanation(x_test, to_maximize, num_features)
         tr, _ = explanation
         if tr is None:
@@ -490,14 +425,16 @@
 
         return best, target
 
     def _get_explanation(self, x_test, to_maximize, num_features):
         distractors = self._get_distractors(
             x_test, to_maximize, n_distractors=self.num_distractors
         )
+        # print('distracotr shape',np.array(distractors).shape)
+        # print('distracotr classification',np.argmax(self.clf(np.array(distractors).reshape(2,6,100)), axis=1))
 
         # Avoid constructing KDtrees twice
         self.backup.per_class_trees = self.per_class_trees
         self.backup.per_class_node_indices = self.per_class_node_indices
 
         best_explanation = set()
         best_explanation_score = 0
@@ -533,116 +470,18 @@
                 if c in explanation:
                     modified[0][c] = dist[0][c]
             input_ = modified.reshape(1, -1, self.window_size)
             probas = self.clf(input_)
 
             if not self.silent:
                 logging.info("Current probas: %s", probas)
-
             if np.argmax(probas) == to_maximize:
                 current_best = np.max(probas)
                 if current_best > best_explanation_score:
                     best_explanation = explanation
                     best_explanation_score = current_best
                     best_modified = modified
 
         if len(best_explanation) == 0:
             return None, None
 
         return best_modified, best_explanation
-
-
-class AtesCF(CF):
-    """Calculates and Visualizes Counterfactuals for Multivariate Time Series in accordance to the paper [1].
-
-    References
-    ----------
-     [1] Ates, Emre, et al.
-     "Counterfactual Explanations for Multivariate Time Series."
-     2021 International Conference on Applied Artificial Intelligence (ICAPAI). IEEE, 2021.
-    ----------
-    """
-
-    def __init__(
-        self,
-        model,
-        data,
-        backend,
-        mode,
-        method="opt",
-        number_distractors=2,
-        max_attempts=1000,
-        max_iter=1000,
-        silent=False,
-    ) -> None:
-        """
-        Arguments:
-            model [torch.nn.Module, Callable, tf.keras.model]: Model to be interpreted.
-            ref Tuple: Reference Dataset as Tuple (x,y).
-            backend str: desired Model Backend ('PYT', 'TF', 'SK').
-            mode str: Name of second dimension: `time` -> `(-1, time, feature)` or `feat` -> `(-1, feature, time)`
-            method str : 'opt' if optimized calculation, 'brute' for Brute Force
-            number_distractors int: number of distractore to be used
-            silent bool: logging.
-
-        """
-        super().__init__(model, mode)
-        self.backend = backend
-        test_x, test_y = data
-        shape = test_x.shape
-        if mode == "time":
-            # Parse test data into (1, feat, time):
-            change = True
-            self.ts_length = shape[-2]
-            test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
-        elif mode == "feat":
-            change = False
-            self.ts_length = shape[-1]
-
-        if backend == "PYT":
-            self.predict = PyTorchModel(model, change).predict
-        elif backend == "TF":
-            self.predict = TensorFlowModel(model, change).predict
-
-        elif backend == "SK":
-            self.predict = SklearnModel(model, change).predict
-        self.referenceset = (test_x, test_y)
-        self.method = method
-        self.silent = silent
-        self.number_distractors = number_distractors
-        self.max_attemps = max_attempts
-        self.max_iter = max_iter
-
-    def explain(
-        self, x: np.ndarray, orig_class: int = None, target: int = None
-    ) -> Tuple[np.ndarray, int]:
-        """
-        Calculates the Counterfactual according to Ates.
-        Arguments:
-            x (np.array): The instance to explain. Shape : `mode = time` -> `(1,time, feat)` or `mode = time` -> `(1,feat, time)`
-            target int: target class. If no target class is given, the class with the secon heighest classification probability is selected.
-
-        Returns:
-            ([np.array], int): Tuple of Counterfactual and Label. Shape of CF : `mode = time` -> `(time, feat)` or `mode = time` -> `(feat, time)`
-
-        """
-
-        if self.mode != "feat":
-            x = x.reshape(-1, x.shape[-1], x.shape[-2])
-        train_x, train_y = self.referenceset
-        if len(train_y.shape) > 1:
-            train_y = np.argmax(train_y, axis=1)
-        if self.method == "opt":
-            opt = OptimizedSearch(
-                self.predict,
-                train_x,
-                train_y,
-                silent=self.silent,
-                threads=1,
-                num_distractors=self.number_distractors,
-                max_attempts=self.max_attemps,
-                maxiter=self.max_iter,
-            )
-            return opt.explain(x, to_maximize=target)
-        elif self.method == "brute":
-            opt = BruteForceSearch(self.predict, train_x, train_y, threads=1)
-            return opt.explain(x, to_maximize=target)
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             exp np.array: returned explanation. Shape: `mode = time` -> `(time, feat)` or `mode = time` -> `(feat, time)`
             cf_label int: lebel of returned instance.
             figsize Tuple: Size of Figure (x,y).
             save_fig str: Path to Save the figure.
         """
         if self.mode == "time":
             item = item.reshape(item.shape[-1], item.shape[-2])
-            exp = exp.reshape(item.shape[-1], item.shape[-2])
+            exp = exp.reshape(exp.shape[-1], exp.shape[-2])
         else:
             item = item.reshape(item.shape[-2], item.shape[-1])
             exp = exp.reshape(item.shape[-2], item.shape[-1])
 
         # TODO This is new and needs to be testes
         ind = ""
         # print("Item Shape", item.shape[-2])
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,39 +152,40 @@
         individual = np.array(nun.tolist())  # , dtype=np.float64)
         out = self.predict(individual)
         return nun, np.argmax(out)
 
     def _findSubarray(
         self, a, k
     ):  # used to find the maximum contigious subarray of length k in the explanation weight vector
+        if len(a.shape) == 2:
+            a = a.reshape(-1)
         n = len(a)
+        a = a.tolist()
 
         vec = []
 
         # Iterate to find all the sub-arrays
         for i in range(n - k + 1):
             temp = []
 
             # Store the sub-array elements in the array
             for j in range(i, i + k):
                 temp.append(a[j])
 
             # Push the vector in the container
             vec.append(temp)
-
         sum_arr = []
         for v in vec:
             sum_arr.append(np.sum(v))
 
         return vec[np.argmax(sum_arr)]
 
     def _counterfactual_generator_swap(
         self, instance, label, subarray_length=1, max_iter=500
     ):
-        print(label)
         _, nun = self._native_guide_retrieval(instance, label, self.distance_measure, 1)
         if np.count_nonzero(nun.reshape(-1) - instance.reshape(-1)) == 0:
             print("Starting and nun are Identical !")
 
         test_x, test_y = self.data
         train_x = test_x
         individual = np.array(nun.tolist())  # , dtype=np.float64)
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,29 +262,34 @@
     # Define variables
     length = 1
     num_slices = 1
 
     # Set up dataframe for slices with start and end value
     slices_start_end_value = pd.DataFrame(columns=["Slice_number", "Start", "End"])
     # Include the first fourier band which should not be perturbed
-    new_row = {"Slice_number": 0, "Start": 0, "End": 1}
-    # append row to the dataframe
-    slices_start_end_value = slices_start_end_value.append(new_row, ignore_index=True)
+    new_row = pd.DataFrame(
+        [[0, 0, 1]], columns=["Slice_number", "Start", "End"]
+    )  # {"Slice_number": 0, "Start": 0, "End": 1}
+    slices_start_end_value = pd.concat(
+        [slices_start_end_value, new_row], ignore_index=True
+    )  # slices_start_end_value.append(new_row, ignore_index=True)
     start_idx = length
     end_idx = length
     while length < len_fourier:
         start_idx = length  # Start value
         end_idx = start_idx + num_slices**2  # End value
         end_idx = min(end_idx, len_fourier)
 
-        new_row = {"Slice_number": num_slices, "Start": start_idx, "End": end_idx}
+        new_row = pd.DataFrame(
+            [[num_slices, start_idx, end_idx]], columns=["Slice_number", "Start", "End"]
+        )  # new_row = {"Slice_number": num_slices, "Start": start_idx, "End": end_idx}
         # append row to the dataframe
-        slices_start_end_value = slices_start_end_value.append(
-            new_row, ignore_index=True
-        )
+        slices_start_end_value = pd.concat(
+            [slices_start_end_value, new_row], ignore_index=True
+        )  # slices_start_end_value.append( new_row, ignore_index=True)
 
         length = length + end_idx - start_idx
         num_slices = num_slices + 1
 
     feature = np.where(channels == 1)
     if len(feature[0]) != 0:
         # Select Feature to be changed
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -85,18 +85,18 @@
                 original_x.shape[0], original_x.shape[2], original_x.shape[1]
             )
         neighborhood = []
         if target_y is not None:
             if not type(target_y) == int:
                 target_y = np.argmax(original_y, axis=1)[0]
             reference_set = self.x[np.where(self.y == target_y)]
-        elif len(original_y) > 1:
-            reference_set = self.x[np.where(self.y != np.argmax(original_y, axis=1)[0])]
         elif type(original_y) is int:
             reference_set = self.x[np.where(self.y != original_y)]
+        elif len(original_y) > 1:
+            reference_set = self.x[np.where(self.y != np.argmax(original_y, axis=1)[0])]
         else:
             reference_set = self.x[np.where(self.y != original_y)]
 
         reference_set = reference_set.reshape(
             -1, original_x.shape[1], original_x.shape[2]
         )
         if len(reference_set.shape) == 2:
```

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.3.3/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.3.3/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.3.3/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.3.3/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret/Models/base_model.py` & `TSInterpret-0.3.3/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.3.2/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.3.3/TSInterpret.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.3.2
+Version: 0.3.3
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -47,37 +47,18 @@
 
 ## 💈 Installation
 ```shell
 pip install TSInterpret
 ```
 You can install the latest development version from GitHub as so:
 ```shell
-pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
+pip install https://github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/main.zip
 ```
 
-Or, through SSH:
-```shell
-pip install git@github.com:fzi-forschungszentrum-informatik/TSInterpret.git --upgrade
-```
-
-On Windows with Anaconda there is a known installation issue due to the <a href='https://github.com/scikit-learn/sklearn-pypi-package'>sklearn brownout</a> in third party dependencies. The workaround (working for python 3.9) till all the dependencies are fixed: 
 
-1. Set Enviroment Variable
-```shell
-set SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True
-```
-2. Install sklearn in advance 
-```shell
-pip install sklearn=0.0
-```
-
-3. Install TsIntrerpret
-```shell
-pip install TSInterpret
-```
 
 ## 🍫 Quickstart
 The following example creates a simple Neural Network based on tensorflow and interprets the Classfier with Integrated Gradients and Temporal Saliency Rescaling [1].
 For further examples check out the <a href="https://fzi-forschungszentrum-informatik.github.io/TSInterpret/">Documentation</a>.
 
 [1] Ismail, Aya Abdelsalam, et al. "Benchmarking deep learning interpretability in time series predictions." Advances in neural information processing systems 33 (2020): 6441-6452.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.2 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.3.3 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
@@ -19,27 +19,20 @@
 The Framework supports Sklearn, Tensorflow, Torch and in some cases predict
 functions. A listing of implemented algorithms and supported frameworks can be
 found in our Documentation. More information on our framework can be found in
 our
 paper
 ._##_ð_Installation_```shell_pip_install_TSInterpret_```_You_can_install_the
 latest_development_version_from_GitHub_as_so:_```shell_pip_install_https://
-github.com/fzi-forschungszentrum-informatik/TSInterpret.git_--upgrade_```_Or,
-through_SSH:_```shell_pip_install_git@github.com:fzi-forschungszentrum-
-informatik/TSInterpret.git_--upgrade_```_On_Windows_with_Anaconda_there_is_a
-known_installation_issue_due_to_the_sklearn_brownout_in_third_party
-dependencies._The_workaround_(working_for_python_3.9)_till_all_the_dependencies
-are_fixed:_1._Set_Enviroment_Variable_```shell_set
-SKLEARN_ALLOW_DEPRECATED_SKLEARN_PACKAGE_INSTALL=True_```_2._Install_sklearn_in
-advance_```shell_pip_install_sklearn=0.0_```_3._Install_TsIntrerpret_```shell
-pip_install_TSInterpret_```_##_ð«_Quickstart_The_following_example_creates_a
-simple_Neural_Network_based_on_tensorflow_and_interprets_the_Classfier_with
-Integrated_Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples
-check_out_the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking
-deep_learning_interpretability_in_time_series_predictions."_Advances_in_neural
+github.com/fzi-forschungszentrum-informatik/TSInterpret/archive/refs/heads/
+main.zip_```_##_ð«_Quickstart_The_following_example_creates_a_simple_Neural
+Network_based_on_tensorflow_and_interprets_the_Classfier_with_Integrated
+Gradients_and_Temporal_Saliency_Rescaling_[1]._For_further_examples_check_out
+the_Documentation._[1]_Ismail,_Aya_Abdelsalam,_et_al._"Benchmarking_deep
+learning_interpretability_in_time_series_predictions."_Advances_in_neural
 information_processing_systems_33_(2020):_6441-6452._###_Import_```python
 import_pickle_import_numpy_as_np_import_matplotlib.pyplot_as_plt_import_seaborn
 as_snst_from_tslearn.datasets_import_UCR_UEA_datasets_import_tensorflow_as_tf
 ```_###_Create_Classifcation_Model_This_Section_uses_a_pretrained
 Classification_Model_to_illustrate_the_use_of_our_package._For_running_the
 example,_please_clone_our_repository_and_comment_the_variable
 PATH_TO_YOUR_CLASSIFICATION_MODEL_in._The_code_in_this_section_can_also_be
```

### Comparing `TSInterpret-0.3.2/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.3.3/TSInterpret.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -24,19 +24,23 @@
 TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
 TSInterpret/InterpretabilityModels/GradCam/__init__.py
 TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
 TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
 TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
 TSInterpret/InterpretabilityModels/Saliency/TSR.py
 TSInterpret/InterpretabilityModels/Saliency/__init__.py
-TSInterpret/InterpretabilityModels/counterfactual/Ates.py
 TSInterpret/InterpretabilityModels/counterfactual/CF.py
+TSInterpret/InterpretabilityModels/counterfactual/COMTECF.py
 TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
 TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
 TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization.py
+TSInterpret/InterpretabilityModels/counterfactual/COMTE/Optimization_helpers.py
+TSInterpret/InterpretabilityModels/counterfactual/COMTE/Problem.py
+TSInterpret/InterpretabilityModels/counterfactual/COMTE/__init__.py
 TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
 TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
 TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
 TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
 TSInterpret/InterpretabilityModels/leftist/__init__.py
 TSInterpret/InterpretabilityModels/leftist/leftist.py
 TSInterpret/InterpretabilityModels/leftist/neighbors.py
```

### Comparing `TSInterpret-0.3.2/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.3.3/TSInterpret.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 scikit-learn==1.3.0
-torch<2.0,>=1.13.0
-pandas~=1.3.2
+torch<3.0,>=1.13.0
+pandas<=3.0.0
 numpy<2.0,>=1.21.6
 tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
@@ -27,16 +27,16 @@
 wheel
 
 [:python_version == '3.8']
 dataclasses
 
 [all]
 scikit-learn==1.3.0
-torch<2.0,>=1.13.0
-pandas~=1.3.2
+torch<3.0,>=1.13.0
+pandas<=3.0.0
 numpy<2.0,>=1.21.6
 tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
@@ -80,16 +80,16 @@
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [dev]
 scikit-learn==1.3.0
-torch<2.0,>=1.13.0
-pandas~=1.3.2
+torch<3.0,>=1.13.0
+pandas<=3.0.0
 numpy<2.0,>=1.21.6
 tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
@@ -135,16 +135,16 @@
 nbconvert==6.4.2
 numpydoc==1.2
 spacy==3.2.2
 jinja2==3.0.3
 
 [test]
 scikit-learn==1.3.0
-torch<2.0,>=1.13.0
-pandas~=1.3.2
+torch<3.0,>=1.13.0
+pandas<=3.0.0
 numpy<2.0,>=1.21.6
 tqdm<4.66.0,>=4.61.2
 h5py==3.7.0
 joblib<2.0,>=1.0.1
 Markdown<4.0,==3.3.4
 matplotlib<4.0,>=3.3.4
 partd==1.2.0
```

### Comparing `TSInterpret-0.3.2/setup.py` & `TSInterpret-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 # Package requirements.
 base_packages = [
     #"mlrose @ https://github.com/gkhayes/mlrose/archive/refs/heads/master.zip",
     #"mlrose>=1.3.0,< 2.0",
     "scikit-learn==1.3.0",
     # "scikit-surprise==1.1.1",
-    "torch>=1.13.0,<2.0",
-    "pandas~=1.3.2",
+    "torch>=1.13.0,<3.0",
+    "pandas<=3.0.0",
     "numpy>=1.21.6,< 2.0",
     "tqdm>=4.61.2, < 4.66.0",
     "h5py==3.7.0", # todo add version
     "joblib>=1.0.1,< 2.0",
     #"lime==0.2.0.1",
     "Markdown==3.3.4,< 4.0",
     "matplotlib>=3.3.4,< 4.0",
```

