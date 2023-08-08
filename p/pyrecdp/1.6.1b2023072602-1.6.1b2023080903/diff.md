# Comparing `tmp/pyrecdp-1.6.1b2023072602.tar.gz` & `tmp/pyrecdp-1.6.1b2023080903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrecdp-1.6.1b2023072602.tar", last modified: Wed Jul 26 05:27:16 2023, max compression
+gzip compressed data, was "pyrecdp-1.6.1b2023080903.tar", last modified: Tue Aug  8 19:55:25 2023, max compression
```

## Comparing `pyrecdp-1.6.1b2023072602.tar` & `pyrecdp-1.6.1b2023080903.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/LICENSE
--rw-r--r--   0 root         (0) root         (0)      205 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.763441 pyrecdp-1.6.1b2023072602/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.763441 pyrecdp-1.6.1b2023072602/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      559 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1142 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.765441 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-26 04:18:12.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    15830 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4812 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3114 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.766441 pyrecdp-1.6.1b2023072602/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      908 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)      901 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/parallel_iterator.py
--rw-r--r--   0 root         (0) root         (0)     6642 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     7159 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.767441 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.767441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.768441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-07-07 05:24:39.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.770441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     2043 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1636 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-07-10 02:55:58.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/group_category.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4448 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.771441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     5807 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     9106 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.772441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      317 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/cluster_infer.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/distribution_infer.py
--rw-r--r--   0 root         (0) root         (0)     5752 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     1732 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/time_series_infer.py
--rw-r--r--   0 root         (0) root         (0)     5346 2023-07-26 05:14:55.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.773441 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54072 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8328 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     9032 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.774441 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.774441 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 08:03:34.000000 pyrecdp-1.6.1b2023072602/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.764441 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8824 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-26 05:27:16.000000 pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1521 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:27:16.776441 pyrecdp-1.6.1b2023072602/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_autofe.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_dataconversion.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_estimator.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_profiler.py
--rw-r--r--   0 root         (0) root         (0)     3316 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_feature_wrangler.py
--rw-r--r--   0 root         (0) root         (0)     4911 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_individual_method.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_pipeline_json.py
--rw-r--r--   0 root         (0) root         (0)     2260 2023-07-26 02:03:03.000000 pyrecdp-1.6.1b2023072602/tests/test_relational_builder.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-06-08 08:03:35.000000 pyrecdp-1.6.1b2023072602/tests/test_spark_dataprocessor.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-26 05:27:02.000000 pyrecdp-1.6.1b2023072602/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023080903/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.604094 pyrecdp-1.6.1b2023080903/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.604094 pyrecdp-1.6.1b2023080903/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      908 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/parallel_iterator.py
+-rw-r--r--   0 root         (0) root         (0)     6816 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.608095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.612095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-07-18 01:09:39.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-07-10 18:45:18.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     5856 2023-08-02 02:48:14.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-08-02 02:48:14.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4792 2023-08-02 02:48:14.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/group_category.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-08-02 02:48:14.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.612095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-11 09:02:53.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     9106 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      980 2023-08-08 02:22:12.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-07-24 20:42:56.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.612095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      317 2023-07-18 01:09:39.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-18 01:09:39.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/cluster_infer.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-18 01:09:39.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/distribution_infer.py
+-rw-r--r--   0 root         (0) root         (0)     5752 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-07-18 01:09:39.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/time_series_infer.py
+-rw-r--r--   0 root         (0) root         (0)     6198 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.612095 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54072 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-07-11 09:02:53.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9032 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.604094 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8824 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      202 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 19:55:25.616095 pyrecdp-1.6.1b2023080903/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 06:07:34.000000 pyrecdp-1.6.1b2023080903/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/tests/test_autofe.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-07-11 09:02:53.000000 pyrecdp-1.6.1b2023080903/tests/test_dataconversion.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/tests/test_feature_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-27 23:05:53.000000 pyrecdp-1.6.1b2023080903/tests/test_feature_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-08-01 09:46:06.000000 pyrecdp-1.6.1b2023080903/tests/test_feature_wrangler.py
+-rw-r--r--   0 root         (0) root         (0)     6004 2023-08-07 21:57:28.000000 pyrecdp-1.6.1b2023080903/tests/test_individual_method.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/tests/test_pipeline_json.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2023-07-18 15:05:20.000000 pyrecdp-1.6.1b2023080903/tests/test_relational_builder.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-27 22:00:24.000000 pyrecdp-1.6.1b2023080903/tests/test_spark_dataprocessor.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-08-08 19:55:25.000000 pyrecdp-1.6.1b2023080903/version
```

### Comparing `pyrecdp-1.6.1b2023072602/LICENSE` & `pyrecdp-1.6.1b2023080903/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/PKG-INFO` & `pyrecdp-1.6.1b2023080903/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023072602
+Version: 1.6.1b2023080903
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023072602/README.md` & `pyrecdp-1.6.1b2023080903/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/spark-env.sh` & `pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/spark-env.sh`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.6.1b2023080903/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/__init__.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/AutoFE.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/BasePipeline.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -359,18 +359,18 @@
                 spark_master = kwargs["spark_master"]
                 spark_mode = 'standalone'
             else:
                 spark_master = "local[*]"
                 spark_mode = 'local'
             self.rdp = SparkDataProcessor(spark_mode=spark_mode, spark_master=spark_master)
         ret = self.execute(engine_type = engine_type, no_cache = no_cache, data = data, trans_type = 'transform')
+        self.transformed_cache = ret
         if engine_type == "spark":
             del self.rdp
             self.rdp = None
-        self.transformed_cache = ret
         return ret
 
     def get_transformed_cache(self):
         if hasattr(self, 'transformed_cache') and self.transformed_cache is not None:
             return self.transformed_cache
         else:
             print("No transformed data detected.")
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureEstimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureProfiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/core/dataframe.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/core/di_graph.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/core/parallel_iterator.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/core/parallel_iterator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/core/schema.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,21 @@
 
     @property
     def group_id_list(self):
         if 'group_id' in self.config:
             return self.config["group_id"]
         else:
             return []
+    
+    @property
+    def datetime_ft_list(self):
+        if 'datetime_ft' in self.config:
+            return self.config["datetime_ft"]
+        else:
+            return []
 
 
 class DataFrameSchema(list):
     def __init__(self, df):
         for s_name in df.columns:
             s = df[s_name]
             super().append(SeriesSchema(s))
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/core/utils.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/base_api.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,77 +7,80 @@
 class LabelEncodeFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         feature_in_out = {}
         folder = 'pipeline_default'
         for idx, pa_field in enumerate(pa_schema):
             if pa_field.is_string and pa_field.is_label:
                 feature = pa_field.name
                 config = {}
                 config = pa_field.copy_config_to(config)
                 config['is_string'] = False
                 out_schema = SeriesSchema(f"{feature}", int)
                 out_schema.copy_config_from(config)
                 feature_in_out[feature] = (f"{folder}/{feature}_categorify_dict", feature)
                 is_useful = True
-                pa_schema[idx] = out_schema
+                ret_pa_schema[idx] = out_schema
         if is_useful:
             cur_idx = max_idx + 1
             config = feature_in_out
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'categorify', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'categorify', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
 
 class OneHotFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.feature_in = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         config = {}
         for pa_field in pa_schema:
             if pa_field.is_onehot:
                 feature = pa_field.name
                 out_schema = [SeriesSchema(f"{feature}__{key}", int) for key in pa_field.config["is_onehot"]]
                 config[pa_field.name] = pa_field.config["is_onehot"]
                 is_useful = True
-                pa_schema.extend(out_schema)
+                ret_pa_schema.extend(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'onehot_encode', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'onehot_encode', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
         
 class ListOneHotFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.feature_in = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         config = {}
         for pa_field in pa_schema:
             if pa_field.is_list_string:
                 feature = pa_field.name
                 out_schema = [SeriesSchema(f"{feature}_{key}", int) for key in pa_field.config["is_list_string"][1] if key != None or key != ""]
                 config[pa_field.name] = pa_field.config["is_list_string"]
                 is_useful = True
-                pa_schema.extend(out_schema)
+                ret_pa_schema.extend(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'list_onehot_encode', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'list_onehot_encode', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
         
 class TargetEncodeFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from .base import BaseFeatureGenerator as super_class
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
+import copy
 
 class FeaturetoolsBasedFeatureGenerator(super_class):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.feature_in = []
         self.feature_in_out_map = {}
         self.op_name = 'featuretools'
     
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for in_feat_name in self.feature_in:
             is_useful = True
             self.feature_in_out_map[in_feat_name] = []
             for op in self.op_list:
                 op_clz = op
                 op = op_clz()
                 out_feat_name = f"{in_feat_name}__{op.name}"
                 out_feat_type = op.return_type
                 out_schema = SeriesSchema(out_feat_name, out_feat_type)
-                pa_schema.append(out_schema)
+                ret_pa_schema.append(out_schema)
                 self.feature_in_out_map[in_feat_name].append((out_schema.name, op_clz))
         if is_useful:
             cur_idx = max_idx + 1
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = self.op_name, config = self.feature_in_out_map)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = self.op_name, config = self.feature_in_out_map)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/geograph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from .base import BaseFeatureGenerator as super_class
 from .featuretools_adaptor import FeaturetoolsBasedFeatureGenerator
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
 from featuretools.primitives import Haversine
+import copy
 
 class GeoFeatureGenerator(FeaturetoolsBasedFeatureGenerator):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.op_list = [Haversine]
         self.op_name = 'haversine'
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
             if pa_field.is_coordinates:
                 self.feature_in.append(pa_field.name)
                 is_useful = True
         if len(self.feature_in) == 2:
             # we assume we can calculate distance between them
             out_feat_name = f"haversine_{'_'.join(self.feature_in)}"
             op = self.op_list[0]()
             out_feat_type = op.return_type
             out_schema = SeriesSchema(out_feat_name, out_feat_type)
             self.feature_in_out_map[str(self.feature_in)] = (out_schema.name, self.op_list[0])
-            pa_schema.append(out_schema)
+            ret_pa_schema.append(out_schema)
 
         if is_useful:
             cur_idx = max_idx + 1
             config = self.feature_in_out_map
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'haversine', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'haversine', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
 
 
 class Point:
     def __init__(self, prefix = None, longitude = None, latitude = None):
@@ -65,27 +67,28 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.points = []
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for field in pa_schema:
             if self.is_coor_related_name_and_set(field.name):
                 is_useful = True
         for p in self.points:
             out_schema = SeriesSchema(p.get_feature_name(), p.get_feature_type()) 
-            pa_schema.append(out_schema)
+            ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx
             child = children[0]
             for p in self.points:
                 cur_idx = cur_idx + 1
                 config = p.get_config()
-                pipeline[cur_idx] = Operation(cur_idx, [child], pa_schema, op = 'tuple', config = config)
+                pipeline[cur_idx] = Operation(cur_idx, [child], ret_pa_schema, op = 'tuple', config = config)
                 child = cur_idx
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
     
     def is_coor_related_name_and_set(self, f_name):
             coor_related_names = ["longitude", "latitude", "coordinates", "point", "latlong", "longlat"]
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/group_category.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/group_category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/nlp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .featuretools_adaptor import FeaturetoolsBasedFeatureGenerator
 from pyrecdp.core import SeriesSchema
 from pyrecdp.primitives.operations import Operation
 from pyrecdp.core.schema import TextDtype
 
 from featuretools.primitives.base import TransformPrimitive
+import copy
 
 class BertTokenizerDecode(TransformPrimitive):
     name = "decoded"
     return_type = TextDtype()
 
     def __init__(self, pretrained_model = 'bert-base-multilingual-cased', case_sensitive = False):
         self.pretrained_model = pretrained_model
@@ -33,32 +34,33 @@
             BertTokenizerDecode
         ]
         self.op_name = 'bert_decode'
 
     def fit_prepare(self, pipeline, children, max_idx):
         is_useful = False
         pa_schema = pipeline[children[0]].output
+        ret_pa_schema = copy.deepcopy(pa_schema)
         for pa_field in pa_schema:
             if pa_field.is_text and pa_field.is_encoded:
                 in_feat_name = pa_field.name
                 is_useful = True
                 self.feature_in.append(in_feat_name)
         for in_feat_name in self.feature_in:
             self.feature_in_out_map[in_feat_name] = []
             for op in self.op_list:
                 op_clz = op
                 op = op_clz()
                 out_feat_name = f"{in_feat_name}__{op.name}"
                 out_schema = SeriesSchema(out_feat_name, op.return_type, {'is_text': True})
                 self.feature_in_out_map[in_feat_name].append((out_schema.name, op_clz))
-                pa_schema.append(out_schema)
+                ret_pa_schema.append(out_schema)
         if is_useful:
             cur_idx = max_idx + 1
             config = self.feature_in_out_map
-            pipeline[cur_idx] = Operation(cur_idx, children, pa_schema, op = 'bert_decode', config = config)
+            pipeline[cur_idx] = Operation(cur_idx, children, ret_pa_schema, op = 'bert_decode', config = config)
             return pipeline, cur_idx, cur_idx
         else:
             return pipeline, children[0], max_idx
  
 class TextFeatureGenerator(FeaturetoolsBasedFeatureGenerator):
     def __init__(self):
         super().__init__()
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/data.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/drop.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,18 @@
         self.support_spark_rdd = True
         self.fast_without_dpp = True
 
     def get_function_pd(self, trans_type = 'fit_transform'):
         feature_in = copy.deepcopy(self.feature_in)
 
         def drop_useless_feature(df):
-            for i in df.columns:
-                if i not in feature_in and is_unique(df[i]):
-                    feature_in.append(i)
             return df.drop(columns = feature_in)
+            # for i in df.columns:
+            #     if i not in feature_in and is_unique(df[i]):
+            #         feature_in.append(i)
+            # return df.drop(columns = feature_in)
         return drop_useless_feature
     
     def get_function_spark(self, rdp, trans_type = 'fit_transform'):
         def drop_feature(df):
             return df.drop(*self.feature_in)
         return drop_feature
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/cluster_infer.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/cluster_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/distribution_infer.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/distribution_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/statics.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/time_series_infer.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/time_series_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/profilers/type_infer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyrecdp.core import SeriesSchema
+from pyrecdp.core.utils import is_unique 
 from pyrecdp.primitives.operations import Operation
 import pandas as pd
 import numpy as np
 from pandas.api import types as pdt
 import copy
 from featuretools.primitives.base import TransformPrimitive
 from tqdm import tqdm
@@ -39,14 +40,32 @@
         result = pd.to_datetime(result, errors='coerce')
         if result.isnull().mean() > 0.8:  # If over 80% of the rows are NaN
             return False
         else:
             return True
     except:
         return False
+    
+def get_datetime_potential_features(s):
+    if len(s) > 5000:
+        # Sample to speed-up type inference
+        result = s.sample(n=5000, random_state=0)
+    result = pd.to_datetime(result, errors='coerce')
+    ret = []
+    if not is_unique(result.dt.day):
+        ret.append('day')
+    if not is_unique(result.dt.month):
+        ret.append('month')
+    if not is_unique(result.dt.year):
+        ret.append('year')
+    if not is_unique(result.dt.weekday):
+        ret.append('weekday')
+    if not is_unique(result.dt.hour):
+        ret.append('hour')    
+    return ret
 
 def try_re_numeric(s):
     if s.isnull().all():
         return True
     try:
         if len(s) > 500:
             # Sample to speed-up type inference
@@ -124,20 +143,23 @@
             config = {}
             # Add y_label to y column
             if feature_name == y:
                 config['is_label'] = True
                 if pa_field.is_string:
                     config['is_categorical_label'] = True
             else:
-                if feature_name == ts:
+                if isinstance(ts, str) and feature_name == ts:
+                    config['is_timeseries'] = True
+                if isinstance(ts, list) and feature_name in ts:
                     config['is_timeseries'] = True
                 if pa_field.is_text and is_encoded(df[feature_name]):
                     config['is_encoded'] = True
                 if try_datetime(df[feature_name]):
                     config['is_datetime'] = True
+                    config['datetime_ft'] = get_datetime_potential_features(df[feature_name])
                 if try_category(df[feature_name]):
                     config['is_categorical'] = True
                 if try_numeric(df[feature_name]):
                     config['is_numeric'] = True
                 elif try_re_numeric(df[feature_name]):
                     config['is_re_numeric'] = True
                     config['is_categorical'] = False
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/scripts.html` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.6.1b2023080903/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.6.1b2023072602
+Version: 1.6.1b2023080903
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrecdp-1.6.1b2023072602/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.6.1b2023080903/pyrecdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/setup.py` & `pyrecdp-1.6.1b2023080903/setup.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_dataconversion.py` & `pyrecdp-1.6.1b2023080903/tests/test_dataconversion.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_feature_estimator.py` & `pyrecdp-1.6.1b2023080903/tests/test_feature_estimator.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_feature_profiler.py` & `pyrecdp-1.6.1b2023080903/tests/test_feature_profiler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_feature_wrangler.py` & `pyrecdp-1.6.1b2023080903/tests/test_feature_wrangler.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 print(pathlib)
 try:
     import pyrecdp
 except:
     print("Not detect system installed pyrecdp, using local one")
     sys.path.append(pathlib)
 from pyrecdp.autofe import FeatureWrangler
+from pyrecdp.core.utils import Timer
 from IPython.display import display
 
 
 class TestFeatureWranglerPandasBased(unittest.TestCase):
 
     def test_nyc_taxi(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_nyc_taxi_fare.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="fare_amount")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         # test with shape
         display(ret_df)
+    
+    def test_nyc_taxi_perf(self):
+        train_data = pd.read_csv(f"/home/vmagent/app/dataset/nyc_taxi/train.csv")
+        with Timer("NYC taxi performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="fare_amount")
+            ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        display(ret_df)
         
     def test_twitter_recsys(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_twitter_recsys.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="reply")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         # test with shape
         display(ret_df)
@@ -37,31 +45,52 @@
         display(ret_df)
         
     def test_frauddetect(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="Is Fraud?")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         display(ret_df)
+    
+    def test_frauddetect_perf(self):
+        train_data = pd.read_csv(f"/home/vmagent/app/dataset/fraud_detect/card_transaction.v1.csv")
+        with Timer("Fraud detect performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="Is Fraud?")
+            ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        display(ret_df)
 
     def test_ppdt(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/recsys2023_train.parquet")
         #train_data = train_data[:10000]
         pipeline = FeatureWrangler(dataset=train_data, label="is_installed", time_series = 'f_1')
         # pipeline.export(f"{pathlib}/tests/ppdt_pipeline.json")
         ret_df = pipeline.fit_transform(engine_type = 'pandas')
         display(ret_df)
+    
+    def test_recsys2023_perf(self):
+        train_data = pd.read_parquet(f"/home/vmagent/app/dataset/recsys2023/recsys2023_train.parquet")
+        with Timer("Recsys2023 performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="is_installed", time_series = 'f_1')
+            ret_df = pipeline.fit_transform(engine_type = 'pandas')
+        display(ret_df)
         
 class TestFeatureWranglerSparkBased(unittest.TestCase):
 
     def test_nyc_taxi(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_nyc_taxi_fare.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="fare_amount")
         ret_df = pipeline.fit_transform(engine_type = 'spark')
         # test with shape
         display(ret_df)
+    
+    def test_nyc_taxi_perf(self):
+        train_data = pd.read_csv(f"/home/vmagent/app/dataset/nyc_taxi/train.csv")
+        with Timer("NYC taxi performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="fare_amount")
+            ret_df = pipeline.fit_transform(engine_type = 'spark')
+        display(ret_df)
         
     def test_twitter_recsys(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_twitter_recsys.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="reply")
         ret_df = pipeline.fit_transform(engine_type = 'spark')
         # test with shape
         display(ret_df)
@@ -74,7 +103,29 @@
         display(ret_df)
 
     def test_frauddetect(self):
         train_data = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
         pipeline = FeatureWrangler(dataset=train_data, label="Is Fraud?")
         ret_df = pipeline.fit_transform(engine_type = 'spark')
         display(ret_df)
+
+    def test_frauddetect_perf(self):
+        train_data = pd.read_csv(f"/home/vmagent/app/dataset/fraud_detect/card_transaction.v1.csv")
+        with Timer("Fraud detect performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="Is Fraud?")
+            ret_df = pipeline.fit_transform(engine_type = 'spark')
+        display(ret_df)
+    
+    def test_ppdt(self):
+        train_data = pd.read_parquet(f"{pathlib}/tests/data/recsys2023_train.parquet")
+        #train_data = train_data[:10000]
+        pipeline = FeatureWrangler(dataset=train_data, label="is_installed", time_series = 'f_1')
+        # pipeline.export(f"{pathlib}/tests/ppdt_pipeline.json")
+        ret_df = pipeline.fit_transform(engine_type = 'spark')
+        display(ret_df)
+    
+    def test_recsys2023_perf(self):
+        train_data = pd.read_parquet(f"/home/vmagent/app/dataset/recsys2023/recsys2023_train.parquet")
+        with Timer("Recsys2023 performance test"):
+            pipeline = FeatureWrangler(dataset=train_data, label="is_installed", time_series = 'f_1')
+            ret_df = pipeline.fit_transform(engine_type = 'spark')
+        display(ret_df)
```

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_individual_method.py` & `pyrecdp-1.6.1b2023080903/tests/test_individual_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pyrecdp.core import DataFrameSchema, DiGraph
 from pyrecdp.primitives.operations import Operation
 
 
 class TestUnitMethod(unittest.TestCase):
     def setUp(self):
         self.df = pd.read_parquet(f"{pathlib}/tests/data/recsys2023_train.parquet")
+        self.fraud_detect_df = pd.read_parquet(f"{pathlib}/tests/data/test_frdtct.parquet")
         self.pipeline = DiGraph()
         self.pipeline[0] = Operation(
             0, None, output = DataFrameSchema(self.df), op = 'DataFrame', config = 'main')
 
     def test_distribution_infer(self):
         from pyrecdp.primitives.profilers import DistributionInferFeatureProfiler
         DistributionInferFeatureProfiler().fit_prepare(self.pipeline, [0], 0, self.df, y = None)
@@ -44,14 +45,37 @@
         ret_test = pd.DataFrame()
         ret_test['f_1'] = test_df['f_1']
         ret_test['f_2'] = test_df['f_2']
         ret_test['f_2_idx'] = CategorifyOperation.label_encode_transform(item)
         display(ret_train)
         display(ret_test)
         
+    def test_Time_categorify(self):
+        from pyrecdp.primitives.operations.category import CategorifyOperation
+        feature = ['Time']
+        df = self.fraud_detect_df
+        df['Time'] = pd.to_datetime(df['Time'])
+        train_df = df[df['Year'] < 2018].reset_index(drop=True)
+        test_df = df[df['Year'] > 2018].reset_index(drop=True)
+        df_x_1 = train_df[feature]
+        df_x_2 = test_df[feature]
+        dict_path = f"{feature[0]}_cat.pkl"
+        feature_out = f"{feature[0]}_idx"
+        item = (feature, df_x_1, dict_path, feature_out)
+        ret_train = pd.DataFrame()
+        ret_train['Time'] = train_df['Time']
+        ret_train[feature_out] = CategorifyOperation.label_encode(item)
+        
+        item = (feature, df_x_2, dict_path, feature_out)
+        ret_test = pd.DataFrame()
+        ret_test['Time'] = test_df['Time']
+        ret_test[feature_out] = CategorifyOperation.label_encode_transform(item)
+        display(ret_train)
+        display(ret_test)
+        
     def test_group_categorify(self):
         from pyrecdp.primitives.operations.category import GroupCategorifyOperation
         grouped_features = ['f_1', 'f_2']
         train_df = self.df[self.df['f_1'] < 66]
         test_df = self.df[self.df['f_1'] == 66]
         df_x_1 = train_df[grouped_features]
         df_x_2 = test_df[grouped_features]
```

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_pipeline_json.py` & `pyrecdp-1.6.1b2023080903/tests/test_pipeline_json.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_relational_builder.py` & `pyrecdp-1.6.1b2023080903/tests/test_relational_builder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.6.1b2023072602/tests/test_spark_dataprocessor.py` & `pyrecdp-1.6.1b2023080903/tests/test_spark_dataprocessor.py`

 * *Files identical despite different names*

