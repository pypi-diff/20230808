# Comparing `tmp/mlflow_by_johnsnowlabs-2.8.0.tar.gz` & `tmp/mlflow_by_johnsnowlabs-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_by_johnsnowlabs-2.8.0.tar", last modified: Thu Jul 27 19:48:17 2023, max compression
+gzip compressed data, was "mlflow_by_johnsnowlabs-2.9.0.tar", last modified: Thu Jul 27 20:01:43 2023, max compression
```

## Comparing `mlflow_by_johnsnowlabs-2.8.0.tar` & `mlflow_by_johnsnowlabs-2.9.0.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/
--rw-rw-r--   0 root         (0) root         (0)    11382 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)      608 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10580 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     9817 2023-06-06 10:25:43.000000 mlflow_by_johnsnowlabs-2.8.0/README.rst
--rw-rw-r--   0 root         (0) root         (0)      949 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/README_SKINNY.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.222271 mlflow_by_johnsnowlabs-2.8.0/mlflow/
--rw-rw-r--   0 root         (0) root         (0)     6490 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       39 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     3668 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/_doctor.py
--rw-rw-r--   0 root         (0) root         (0)     9680 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/_spark_autologging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.222271 mlflow_by_johnsnowlabs-2.8.0/mlflow/artifacts/
--rw-rw-r--   0 root         (0) root         (0)     6485 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.222271 mlflow_by_johnsnowlabs-2.8.0/mlflow/azure/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/azure/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11647 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/azure/client.py
--rw-rw-r--   0 root         (0) root         (0)    15155 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/catboost.py
--rw-rw-r--   0 root         (0) root         (0)    24874 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/cli.py
--rw-rw-r--   0 root         (0) root         (0)      407 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/
--rw-rw-r--   0 root         (0) root         (0)     2477 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7022 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/artifact_dataset_sources.py
--rw-rw-r--   0 root         (0) root         (0)      946 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/code_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     4333 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset.py
--rw-rw-r--   0 root         (0) root         (0)     6297 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_registry.py
--rw-rw-r--   0 root         (0) root         (0)     3534 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     8270 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_source_registry.py
--rw-rw-r--   0 root         (0) root         (0)     3734 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/delta_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     4873 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/digest_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2598 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/filesystem_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     3929 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/http_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)    10462 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/huggingface_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     4008 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/huggingface_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     7966 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/numpy_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     6955 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/pandas_dataset.py
--rw-rw-r--   0 root         (0) root         (0)      897 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/pyfunc_dataset_mixin.py
--rw-rw-r--   0 root         (0) root         (0)     2800 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/schema.py
--rw-rw-r--   0 root         (0) root         (0)       13 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/sources.py
--rw-rw-r--   0 root         (0) root         (0)    15642 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_dataset.py
--rw-rw-r--   0 root         (0) root         (0)     2196 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_dataset_source.py
--rw-rw-r--   0 root         (0) root         (0)     3858 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_delta_utils.py
--rw-rw-r--   0 root         (0) root         (0)    11898 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/data/tensorflow_dataset.py
--rw-rw-r--   0 root         (0) root         (0)      881 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/
--rw-rw-r--   0 root         (0) root         (0)     3797 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15582 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/base.py
--rw-rw-r--   0 root         (0) root         (0)    15078 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/cli.py
--rw-rw-r--   0 root         (0) root         (0)     3825 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/interface.py
--rw-rw-r--   0 root         (0) root         (0)     5512 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/plugin_manager.py
--rw-rw-r--   0 root         (0) root         (0)      556 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/utils.py
--rw-rw-r--   0 root         (0) root         (0)    28178 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/diviner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/
--rw-rw-r--   0 root         (0) root         (0)     1211 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1414 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/_mlflow_object.py
--rw-rw-r--   0 root         (0) root         (0)     2118 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/dataset.py
--rw-rw-r--   0 root         (0) root         (0)     1510 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/dataset_input.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/experiment.py
--rw-rw-r--   0 root         (0) root         (0)      887 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/experiment_tag.py
--rw-rw-r--   0 root         (0) root         (0)     1215 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/file_info.py
--rw-rw-r--   0 root         (0) root         (0)      992 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/input_tag.py
--rw-rw-r--   0 root         (0) root         (0)     1242 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/lifecycle_stage.py
--rw-rw-r--   0 root         (0) root         (0)     1418 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/metric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/
--rw-rw-r--   0 root         (0) root         (0)      529 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      286 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/_model_registry_entity.py
--rw-rw-r--   0 root         (0) root         (0)     6435 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version.py
--rw-rw-r--   0 root         (0) root         (0)      831 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_stages.py
--rw-rw-r--   0 root         (0) root         (0)     1533 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_status.py
--rw-rw-r--   0 root         (0) root         (0)      933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_tag.py
--rw-rw-r--   0 root         (0) root         (0)     4933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model.py
--rw-rw-r--   0 root         (0) root         (0)     1053 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model_alias.py
--rw-rw-r--   0 root         (0) root         (0)      948 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model_tag.py
--rw-rw-r--   0 root         (0) root         (0)     1133 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/param.py
--rw-rw-r--   0 root         (0) root         (0)     2134 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run.py
--rw-rw-r--   0 root         (0) root         (0)     3032 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_data.py
--rw-rw-r--   0 root         (0) root         (0)     6182 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_info.py
--rw-rw-r--   0 root         (0) root         (0)     1258 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_inputs.py
--rw-rw-r--   0 root         (0) root         (0)     1550 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_status.py
--rw-rw-r--   0 root         (0) root         (0)      890 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_tag.py
--rw-rw-r--   0 root         (0) root         (0)     1212 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/source_type.py
--rw-rw-r--   0 root         (0) root         (0)     1826 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/view_type.py
--rw-rw-r--   0 root         (0) root         (0)    12114 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/environment_variables.py
--rw-rw-r--   0 root         (0) root         (0)     5020 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/experiments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/fastai/
--rw-rw-r--   0 root         (0) root         (0)    25449 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/fastai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5660 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/fastai/callback.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/gluon/
--rw-rw-r--   0 root         (0) root         (0)    19248 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/gluon/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2020 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/gluon/_autolog.py
--rw-rw-r--   0 root         (0) root         (0)    14185 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/h2o.py
--rw-rw-r--   0 root         (0) root         (0)    37137 2023-07-27 19:47:56.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/johnsnowlabs.py
--rw-rw-r--   0 root         (0) root         (0)      311 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/keras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/langchain/
--rw-rw-r--   0 root         (0) root         (0)    21279 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/langchain/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4898 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/langchain/api_request_parallel_processor.py
--rw-rw-r--   0 root         (0) root         (0)    38975 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/lightgbm.py
--rw-rw-r--   0 root         (0) root         (0)      180 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/llm.py
--rw-rw-r--   0 root         (0) root         (0)     5786 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/ml_package_versions.py
--rw-rw-r--   0 root         (0) root         (0)    13885 2023-06-11 09:09:54.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/mleap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/
--rw-rw-r--   0 root         (0) root         (0)     3637 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9803 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/
--rw-rw-r--   0 root         (0) root         (0)     9403 2023-07-20 22:36:07.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__pycache__/
--rw-rw-r--   0 root         (0) root         (0)     7287 2023-06-03 23:15:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 root         (0) root         (0)     7331 2023-07-27 18:58:20.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/scoring_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/scoring_server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      712 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/scoring_server/nginx.conf
--rw-rw-r--   0 root         (0) root         (0)      131 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/scoring_server/wsgi.py
--rw-rw-r--   0 root         (0) root         (0)     9886 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/docker_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/
--rw-rw-r--   0 root         (0) root         (0)      491 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3105 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/_shap_patch.py
--rw-rw-r--   0 root         (0) root         (0)     6769 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/artifacts.py
--rw-rw-r--   0 root         (0) root         (0)    64594 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/base.py
--rw-rw-r--   0 root         (0) root         (0)    52848 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/default_evaluator.py
--rw-rw-r--   0 root         (0) root         (0)     2036 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/evaluator_registry.py
--rw-rw-r--   0 root         (0) root         (0)     6223 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/lift_curve.py
--rw-rw-r--   0 root         (0) root         (0)    10946 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/validation.py
--rw-rw-r--   0 root         (0) root         (0)     3420 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/flavor_backend.py
--rw-rw-r--   0 root         (0) root         (0)     2354 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/flavor_backend_registry.py
--rw-rw-r--   0 root         (0) root         (0)    24997 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/model.py
--rw-rw-r--   0 root         (0) root         (0)    12595 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/signature.py
--rw-rw-r--   0 root         (0) root         (0)    39844 2023-07-27 17:01:27.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11707 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/models/wheeled_model.py
--rw-rw-r--   0 root         (0) root         (0)    24919 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/onnx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.226271 mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/
--rw-rw-r--   0 root         (0) root         (0)    23265 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12309 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/api_request_parallel_processor.py
--rw-rw-r--   0 root         (0) root         (0)     2936 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/retry.py
--rw-rw-r--   0 root         (0) root         (0)     2088 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/paddle/
--rw-rw-r--   0 root         (0) root         (0)    23859 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/paddle/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4792 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/paddle/_paddle_autolog.py
--rw-rw-r--   0 root         (0) root         (0)    17616 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pmdarima.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/
--rw-rw-r--   0 root         (0) root         (0)    17396 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11532 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/_project_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/
--rw-rw-r--   0 root         (0) root         (0)      271 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2210 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/abstract_backend.py
--rw-rw-r--   0 root         (0) root         (0)     1079 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/loader.py
--rw-rw-r--   0 root         (0) root         (0)    17277 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/local.py
--rw-rw-r--   0 root         (0) root         (0)    20228 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/databricks.py
--rw-rw-r--   0 root         (0) root         (0)     6402 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/docker.py
--rw-rw-r--   0 root         (0) root         (0)       94 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/env_type.py
--rw-rw-r--   0 root         (0) root         (0)     6379 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/kubernetes.py
--rw-rw-r--   0 root         (0) root         (0)     3574 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/submitted_run.py
--rw-rw-r--   0 root         (0) root         (0)    12237 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/utils.py
--rw-rw-r--   0 root         (0) root         (0)    14024 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/prophet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17261 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_artifacts_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14095 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    42316 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_uc_registry_messages_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    12471 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_uc_registry_service_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16146 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/facet_feature_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     1361 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/internal_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     8552 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/mlflow_artifacts_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    54475 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/model_registry_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/scalapb/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/scalapb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3307 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/scalapb/scalapb_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    53666 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/
--rw-rw-r--   0 root         (0) root         (0)    81981 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16573 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/backend.py
--rw-rw-r--   0 root         (0) root         (0)      901 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/mlserver.py
--rw-rw-r--   0 root         (0) root         (0)    15392 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/
--rw-rw-r--   0 root         (0) root         (0)    13926 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4222 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/client.py
--rw-rw-r--   0 root         (0) root         (0)      175 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/wsgi.py
--rw-rw-r--   0 root         (0) root         (0)     2124 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/spark_model_cache.py
--rw-rw-r--   0 root         (0) root         (0)     1001 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/stdin_server.py
--rw-rw-r--   0 root         (0) root         (0)  7380252 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pypi_package_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/
--rw-rw-r--   0 root         (0) root         (0)       50 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/
--rw-rw-r--   0 root         (0) root         (0)    55602 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2908 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/_autolog.py
--rw-rw-r--   0 root         (0) root         (0)     1886 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/log_model_allowlist.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/
--rw-rw-r--   0 root         (0) root         (0)    45559 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17568 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/_lightning_autolog.py
--rw-rw-r--   0 root         (0) root         (0)     2654 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/_pytorch_autolog.py
--rw-rw-r--   0 root         (0) root         (0)     2090 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/pickle_module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/
--rw-rw-r--   0 root         (0) root         (0)     1330 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6092 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/artifacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/
--rw-rw-r--   0 root         (0) root         (0)    10189 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4780 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/histogram_generator.py
--rw-rw-r--   0 root         (0) root         (0)    12548 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/pandas_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/templates/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/templates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3488 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/v1/
--rw-rw-r--   0 root         (0) root         (0)      122 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20462 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/v1/recipe.py
--rw-rw-r--   0 root         (0) root         (0)     2917 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cli.py
--rw-rw-r--   0 root         (0) root         (0)    18431 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/dag_help_strings.py
--rw-rw-r--   0 root         (0) root         (0)    17933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/recipe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/v1/
--rw-rw-r--   0 root         (0) root         (0)      114 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/v1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22495 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/v1/recipe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/resources/
--rw-rw-r--   0 root         (0) root         (0)    12211 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/resources/recipe_dag_template.html
--rw-rw-r--   0 root         (0) root         (0)    14841 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/automl/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/automl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6260 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/automl/flaml.py
--rw-rw-r--   0 root         (0) root         (0)    20666 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/evaluate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/ingest/
--rw-rw-r--   0 root         (0) root         (0)    11137 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/ingest/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    26390 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/ingest/datasets.py
--rw-rw-r--   0 root         (0) root         (0)    12140 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/predict.py
--rw-rw-r--   0 root         (0) root         (0)     7664 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/register.py
--rw-rw-r--   0 root         (0) root         (0)    19541 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/split.py
--rw-rw-r--   0 root         (0) root         (0)    59735 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/train.py
--rw-rw-r--   0 root         (0) root         (0)    10602 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/transform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.230271 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/
--rw-rw-r--   0 root         (0) root         (0)     6355 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28468 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/execution.py
--rw-rw-r--   0 root         (0) root         (0)     8990 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/metrics.py
--rw-rw-r--   0 root         (0) root         (0)     7680 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/step.py
--rw-rw-r--   0 root         (0) root         (0)    12316 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/tracking.py
--rw-rw-r--   0 root         (0) root         (0)     1748 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/wrapped_recipe_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/rfunc/
--rw-rw-r--   0 root         (0) root         (0)     1115 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/rfunc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3639 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/rfunc/backend.py
--rw-rw-r--   0 root         (0) root         (0)     2519 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/runs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/sagemaker/
--rw-rw-r--   0 root         (0) root         (0)   135083 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/sagemaker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12986 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/sagemaker/cli.py
--rw-rw-r--   0 root         (0) root         (0)    14450 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/sentence_transformers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/
--rw-rw-r--   0 root         (0) root         (0)     7077 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/
--rw-rw-r--   0 root         (0) root         (0)    28016 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      123 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/basic_auth.ini
--rw-rw-r--   0 root         (0) root         (0)     4689 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/client.py
--rw-rw-r--   0 root         (0) root         (0)      575 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/config.py
--rw-rw-r--   0 root         (0) root         (0)     4217 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/entities.py
--rw-rw-r--   0 root         (0) root         (0)     2673 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/logo.py
--rw-rw-r--   0 root         (0) root         (0)     1267 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/permissions.py
--rw-rw-r--   0 root         (0) root         (0)     1111 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/routes.py
--rw-rw-r--   0 root         (0) root         (0)    12648 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/sqlalchemy_store.py
--rw-rw-r--   0 root         (0) root         (0)    69738 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/handlers.py
--rw-rw-r--   0 root         (0) root         (0)      481 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/server/prometheus_exporter.py
--rw-rw-r--   0 root         (0) root         (0)    26647 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/shap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/sklearn/
--rw-rw-r--   0 root         (0) root         (0)    85689 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/sklearn/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    37469 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/sklearn/utils.py
--rw-rw-r--   0 root         (0) root         (0)    14259 2023-05-21 09:18:08.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/spacy.py
--rw-rw-r--   0 root         (0) root         (0)    45175 2023-06-11 09:09:54.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/spark.py
--rw-rw-r--   0 root         (0) root         (0)    24781 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/statsmodels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/
--rw-rw-r--   0 root         (0) root         (0)      227 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28656 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/rest_store.py
--rw-rw-r--   0 root         (0) root         (0)     5419 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10481 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5836 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/artifact_repository_registry.py
--rw-rw-r--   0 root         (0) root         (0)     8136 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/azure_blob_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5829 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5378 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/cli.py
--rw-rw-r--   0 root         (0) root         (0)    35001 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/databricks_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     9819 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/databricks_models_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)    10247 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/dbfs_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5234 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/ftp_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5873 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/gcs_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     9684 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/hdfs_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     3377 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/http_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5107 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/local_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/mlflow_artifacts_repo.py
--rw-rw-r--   0 root         (0) root         (0)     6757 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/models_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     6016 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/runs_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     9433 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/s3_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5455 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/sftp_artifact_repo.py
--rw-rw-r--   0 root         (0) root         (0)     5592 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3934 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/utils/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       71 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/base_sql_model.py
--rw-rw-r--   0 root         (0) root         (0)      221 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/db_types.py
--rw-rw-r--   0 root         (0) root         (0)    10567 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1634 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/alembic.ini
--rw-rw-r--   0 root         (0) root         (0)     2768 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/
--rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
--rw-rw-r--   0 root         (0) root         (0)      462 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
--rw-rw-r--   0 root         (0) root         (0)      924 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
--rw-rw-r--   0 root         (0) root         (0)     1059 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
--rw-rw-r--   0 root         (0) root         (0)     2624 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
--rw-rw-r--   0 root         (0) root         (0)     1375 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
--rw-rw-r--   0 root         (0) root         (0)     1433 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
--rw-rw-r--   0 root         (0) root         (0)     1201 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
--rw-rw-r--   0 root         (0) root         (0)      940 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
--rw-rw-r--   0 root         (0) root         (0)     1014 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
--rw-rw-r--   0 root         (0) root         (0)     3092 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
--rw-rw-r--   0 root         (0) root         (0)      476 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
--rw-rw-r--   0 root         (0) root         (0)     5716 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
--rw-rw-r--   0 root         (0) root         (0)     1666 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
--rw-rw-r--   0 root         (0) root         (0)      577 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      582 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
--rw-rw-r--   0 root         (0) root         (0)      637 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
--rw-rw-r--   0 root         (0) root         (0)     1295 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
--rw-rw-r--   0 root         (0) root         (0)      684 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
--rw-rw-r--   0 root         (0) root         (0)     2830 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
--rw-rw-r--   0 root         (0) root         (0)      904 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/entities/
--rw-rw-r--   0 root         (0) root         (0)       80 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/entities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      479 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/entities/paged_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.234271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/
--rw-rw-r--   0 root         (0) root         (0)      605 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11022 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/abstract_store.py
--rw-rw-r--   0 root         (0) root         (0)     1440 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/base_rest_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/dbmodels/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/dbmodels/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/dbmodels/models.py
--rw-rw-r--   0 root         (0) root         (0)    38833 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/file_store.py
--rw-rw-r--   0 root         (0) root         (0)    16920 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/rest_store.py
--rw-rw-r--   0 root         (0) root         (0)    50646 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/sqlalchemy_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/
--rw-rw-r--   0 root         (0) root         (0)     1154 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13534 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/abstract_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8315 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/initial_models.py
--rw-rw-r--   0 root         (0) root         (0)    21085 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/models.py
--rw-rw-r--   0 root         (0) root         (0)    52631 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/file_store.py
--rw-rw-r--   0 root         (0) root         (0)    12822 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/rest_store.py
--rw-rw-r--   0 root         (0) root         (0)    77913 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/sqlalchemy_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tensorflow/
--rw-rw-r--   0 root         (0) root         (0)    60208 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tensorflow/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8442 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tensorflow/_autolog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/
--rw-rw-r--   0 root         (0) root         (0)      995 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/
--rw-rw-r--   0 root         (0) root         (0)       41 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15534 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/client.py
--rw-rw-r--   0 root         (0) root         (0)     9641 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/fluent.py
--rw-rw-r--   0 root         (0) root         (0)     3152 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/registry.py
--rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    24289 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/client.py
--rw-rw-r--   0 root         (0) root         (0)     2335 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/registry.py
--rw-rw-r--   0 root         (0) root         (0)     9517 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/utils.py
--rw-rw-r--   0 root         (0) root         (0)     7540 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/artifact_utils.py
--rw-rw-r--   0 root         (0) root         (0)   142886 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1076 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/abstract_context.py
--rw-rw-r--   0 root         (0) root         (0)      520 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_cluster_context.py
--rw-rw-r--   0 root         (0) root         (0)      561 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_command_context.py
--rw-rw-r--   0 root         (0) root         (0)     1965 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_job_context.py
--rw-rw-r--   0 root         (0) root         (0)     1713 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_notebook_context.py
--rw-rw-r--   0 root         (0) root         (0)     1952 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_repo_context.py
--rw-rw-r--   0 root         (0) root         (0)     1020 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/default_context.py
--rw-rw-r--   0 root         (0) root         (0)      898 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/git_context.py
--rw-rw-r--   0 root         (0) root         (0)     3738 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/registry.py
--rw-rw-r--   0 root         (0) root         (0)      443 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/system_environment_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1703 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/abstract_context.py
--rw-rw-r--   0 root         (0) root         (0)     1718 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
--rw-rw-r--   0 root         (0) root         (0)     2300 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
--rw-rw-r--   0 root         (0) root         (0)     3173 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/registry.py
--rw-rw-r--   0 root         (0) root         (0)    78452 2023-06-06 10:07:33.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/fluent.py
--rw-rw-r--   0 root         (0) root         (0)     3404 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/llm_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2248 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/metric_value_conversion_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3515 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1077 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/abstract_request_header_provider.py
--rw-rw-r--   0 root         (0) root         (0)     1336 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/databricks_request_header_provider.py
--rw-rw-r--   0 root         (0) root         (0)      486 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/default_request_header_provider.py
--rw-rw-r--   0 root         (0) root         (0)     2867 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/registry.py
--rw-rw-r--   0 root         (0) root         (0)   110231 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/transformers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.238271 mlflow_by_johnsnowlabs-2.8.0/mlflow/types/
--rw-rw-r--   0 root         (0) root         (0)      299 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/types/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15035 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/types/schema.py
--rw-rw-r--   0 root         (0) root         (0)    18044 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/
--rw-rw-r--   0 root         (0) root         (0)     9365 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6589 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_capture_modules.py
--rw-rw-r--   0 root         (0) root         (0)     2274 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_capture_transformers_modules.py
--rw-rw-r--   0 root         (0) root         (0)     6387 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_spark_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5009 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/annotations.py
--rw-rw-r--   0 root         (0) root         (0)      400 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/arguments_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/
--rw-rw-r--   0 root         (0) root         (0)    27045 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    16642 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/client.py
--rw-rw-r--   0 root         (0) root         (0)    10937 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/events.py
--rw-rw-r--   0 root         (0) root         (0)    13381 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/logging_and_warnings.py
--rw-rw-r--   0 root         (0) root         (0)    47266 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/safety.py
--rw-rw-r--   0 root         (0) root         (0)     3570 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/versioning.py
--rw-rw-r--   0 root         (0) root         (0)      215 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/class_utils.py
--rw-rw-r--   0 root         (0) root         (0)     6431 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/cli_args.py
--rw-rw-r--   0 root         (0) root         (0)    13002 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/conda.py
--rw-rw-r--   0 root         (0) root         (0)      432 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/data_utils.py
--rw-rw-r--   0 root         (0) root         (0)    23803 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/databricks_utils.py
--rw-rw-r--   0 root         (0) root         (0)     9138 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/docstring_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1669 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/download_cloud_file_chunk.py
--rw-rw-r--   0 root         (0) root         (0)      192 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/env.py
--rw-rw-r--   0 root         (0) root         (0)      474 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/env_manager.py
--rw-rw-r--   0 root         (0) root         (0)    22714 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/environment.py
--rw-rw-r--   0 root         (0) root         (0)    30464 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/file_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2306 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/git_utils.py
--rw-rw-r--   0 root         (0) root         (0)    24178 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/gorilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/import_hooks/
--rw-rw-r--   0 root         (0) root         (0)    13645 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/import_hooks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2597 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/logging_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1298 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/mime_type_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4024 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/mlflow_tags.py
--rw-rw-r--   0 root         (0) root         (0)     8109 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/model_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5873 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/name_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2412 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/nfs_on_spark.py
--rw-rw-r--   0 root         (0) root         (0)      139 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/os.py
--rw-rw-r--   0 root         (0) root         (0)     5799 2023-06-12 03:19:23.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/process.py
--rw-rw-r--   0 root         (0) root         (0)    19909 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/proto_json_utils.py
--rw-rw-r--   0 root         (0) root         (0)     5560 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/request_utils.py
--rw-rw-r--   0 root         (0) root         (0)    20050 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/requirements_utils.py
--rw-rw-r--   0 root         (0) root         (0)    11987 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/rest_utils.py
--rw-rw-r--   0 root         (0) root         (0)    59666 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/search_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2368 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/server_cli_utils.py
--rw-rw-r--   0 root         (0) root         (0)     3805 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/string_utils.py
--rw-rw-r--   0 root         (0) root         (0)      512 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/time_utils.py
--rw-rw-r--   0 root         (0) root         (0)    14271 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/uri.py
--rw-rw-r--   0 root         (0) root         (0)    19435 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/validation.py
--rw-rw-r--   0 root         (0) root         (0)    16282 2023-07-27 18:58:37.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/virtualenv.py
--rw-rw-r--   0 root         (0) root         (0)      170 2023-07-27 19:48:03.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/mlflow/xgboost/
--rw-rw-r--   0 root         (0) root         (0)    37317 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/xgboost/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2908 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow/xgboost/_autolog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10580 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15074 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:36:33.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 19:48:17.000000 mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/
--rw-rw-r--   0 root         (0) root         (0)      614 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2234 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/errors.py
--rw-rw-r--   0 root         (0) root         (0)     4556 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/import_checker.py
--rw-rw-r--   0 root         (0) root         (0)      856 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/print_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/pytest_raises_checker/
--rw-rw-r--   0 root         (0) root         (0)     1546 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/pytest_raises_checker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      571 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/set_checker.py
--rw-rw-r--   0 root         (0) root         (0)      878 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/string_checker.py
--rw-rw-r--   0 root         (0) root         (0)      692 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/unittest_assert_raises.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/requirements/
--rw-rw-r--   0 root         (0) root         (0)      609 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.8.0/requirements/core-requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      297 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.8.0/requirements/gateway-requirements.txt
--rw-rw-r--   0 root         (0) root         (0)      481 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.8.0/requirements/skinny-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 19:48:17.242272 mlflow_by_johnsnowlabs-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     7281 2023-07-20 22:35:38.000000 mlflow_by_johnsnowlabs-2.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/
+-rw-rw-r--   0 root         (0) root         (0)    11382 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)      608 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10580 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     9817 2023-06-06 10:25:43.000000 mlflow_by_johnsnowlabs-2.9.0/README.rst
+-rw-rw-r--   0 root         (0) root         (0)      949 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/README_SKINNY.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/
+-rw-rw-r--   0 root         (0) root         (0)     6490 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     3668 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/_doctor.py
+-rw-rw-r--   0 root         (0) root         (0)     9680 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/_spark_autologging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/artifacts/
+-rw-rw-r--   0 root         (0) root         (0)     6485 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/azure/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/azure/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11647 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/azure/client.py
+-rw-rw-r--   0 root         (0) root         (0)    15155 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/catboost.py
+-rw-rw-r--   0 root         (0) root         (0)    24874 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/cli.py
+-rw-rw-r--   0 root         (0) root         (0)      407 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/
+-rw-rw-r--   0 root         (0) root         (0)     2477 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7022 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/artifact_dataset_sources.py
+-rw-rw-r--   0 root         (0) root         (0)      946 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/code_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4333 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     6297 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_registry.py
+-rw-rw-r--   0 root         (0) root         (0)     3534 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     8270 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_source_registry.py
+-rw-rw-r--   0 root         (0) root         (0)     3734 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/delta_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4873 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/digest_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2598 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/filesystem_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     3929 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/http_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10462 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/huggingface_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     4008 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/huggingface_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     7966 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/numpy_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     6955 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/pandas_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)      897 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/pyfunc_dataset_mixin.py
+-rw-rw-r--   0 root         (0) root         (0)     2800 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/schema.py
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/sources.py
+-rw-rw-r--   0 root         (0) root         (0)    15642 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     2196 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_dataset_source.py
+-rw-rw-r--   0 root         (0) root         (0)     3858 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_delta_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11898 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/data/tensorflow_dataset.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/
+-rw-rw-r--   0 root         (0) root         (0)     3797 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15582 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/base.py
+-rw-rw-r--   0 root         (0) root         (0)    15078 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/cli.py
+-rw-rw-r--   0 root         (0) root         (0)     3825 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/interface.py
+-rw-rw-r--   0 root         (0) root         (0)     5512 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/plugin_manager.py
+-rw-rw-r--   0 root         (0) root         (0)      556 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    28178 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/diviner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1211 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1414 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/_mlflow_object.py
+-rw-rw-r--   0 root         (0) root         (0)     2118 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/dataset.py
+-rw-rw-r--   0 root         (0) root         (0)     1510 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/dataset_input.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/experiment.py
+-rw-rw-r--   0 root         (0) root         (0)      887 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/experiment_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     1215 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/file_info.py
+-rw-rw-r--   0 root         (0) root         (0)      992 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/input_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     1242 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/lifecycle_stage.py
+-rw-rw-r--   0 root         (0) root         (0)     1418 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/metric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/
+-rw-rw-r--   0 root         (0) root         (0)      529 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      286 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/_model_registry_entity.py
+-rw-rw-r--   0 root         (0) root         (0)     6435 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version.py
+-rw-rw-r--   0 root         (0) root         (0)      831 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_stages.py
+-rw-rw-r--   0 root         (0) root         (0)     1533 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_status.py
+-rw-rw-r--   0 root         (0) root         (0)      933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     4933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model.py
+-rw-rw-r--   0 root         (0) root         (0)     1053 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model_alias.py
+-rw-rw-r--   0 root         (0) root         (0)      948 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     1133 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/param.py
+-rw-rw-r--   0 root         (0) root         (0)     2134 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run.py
+-rw-rw-r--   0 root         (0) root         (0)     3032 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6182 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1258 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_inputs.py
+-rw-rw-r--   0 root         (0) root         (0)     1550 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_status.py
+-rw-rw-r--   0 root         (0) root         (0)      890 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_tag.py
+-rw-rw-r--   0 root         (0) root         (0)     1212 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/source_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1826 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/view_type.py
+-rw-rw-r--   0 root         (0) root         (0)    12114 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/environment_variables.py
+-rw-rw-r--   0 root         (0) root         (0)     5020 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/experiments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/fastai/
+-rw-rw-r--   0 root         (0) root         (0)    25449 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/fastai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5660 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/fastai/callback.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/gluon/
+-rw-rw-r--   0 root         (0) root         (0)    19248 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/gluon/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2020 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/gluon/_autolog.py
+-rw-rw-r--   0 root         (0) root         (0)    14185 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/h2o.py
+-rw-rw-r--   0 root         (0) root         (0)    37149 2023-07-27 20:01:33.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/johnsnowlabs.py
+-rw-rw-r--   0 root         (0) root         (0)      311 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/keras.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/langchain/
+-rw-rw-r--   0 root         (0) root         (0)    21279 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/langchain/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4898 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/langchain/api_request_parallel_processor.py
+-rw-rw-r--   0 root         (0) root         (0)    38975 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/lightgbm.py
+-rw-rw-r--   0 root         (0) root         (0)      180 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/llm.py
+-rw-rw-r--   0 root         (0) root         (0)     5786 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/ml_package_versions.py
+-rw-rw-r--   0 root         (0) root         (0)    13885 2023-06-11 09:09:54.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/mleap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/
+-rw-rw-r--   0 root         (0) root         (0)     3637 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9803 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/
+-rw-rw-r--   0 root         (0) root         (0)     9403 2023-07-20 22:36:07.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__pycache__/
+-rw-rw-r--   0 root         (0) root         (0)     7287 2023-06-03 23:15:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 root         (0) root         (0)     7331 2023-07-27 18:58:20.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.872454 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/scoring_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/scoring_server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      712 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/scoring_server/nginx.conf
+-rw-rw-r--   0 root         (0) root         (0)      131 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/scoring_server/wsgi.py
+-rw-rw-r--   0 root         (0) root         (0)     9886 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/docker_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/
+-rw-rw-r--   0 root         (0) root         (0)      491 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3105 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/_shap_patch.py
+-rw-rw-r--   0 root         (0) root         (0)     6769 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/artifacts.py
+-rw-rw-r--   0 root         (0) root         (0)    64594 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/base.py
+-rw-rw-r--   0 root         (0) root         (0)    52848 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/default_evaluator.py
+-rw-rw-r--   0 root         (0) root         (0)     2036 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/evaluator_registry.py
+-rw-rw-r--   0 root         (0) root         (0)     6223 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/lift_curve.py
+-rw-rw-r--   0 root         (0) root         (0)    10946 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/validation.py
+-rw-rw-r--   0 root         (0) root         (0)     3420 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/flavor_backend.py
+-rw-rw-r--   0 root         (0) root         (0)     2354 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/flavor_backend_registry.py
+-rw-rw-r--   0 root         (0) root         (0)    24997 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/model.py
+-rw-rw-r--   0 root         (0) root         (0)    12595 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/signature.py
+-rw-rw-r--   0 root         (0) root         (0)    39844 2023-07-27 17:01:27.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11707 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/models/wheeled_model.py
+-rw-rw-r--   0 root         (0) root         (0)    24919 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/onnx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/
+-rw-rw-r--   0 root         (0) root         (0)    23265 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12309 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/api_request_parallel_processor.py
+-rw-rw-r--   0 root         (0) root         (0)     2936 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/retry.py
+-rw-rw-r--   0 root         (0) root         (0)     2088 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/paddle/
+-rw-rw-r--   0 root         (0) root         (0)    23859 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/paddle/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4792 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/paddle/_paddle_autolog.py
+-rw-rw-r--   0 root         (0) root         (0)    17616 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pmdarima.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/
+-rw-rw-r--   0 root         (0) root         (0)    17396 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11532 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/_project_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/
+-rw-rw-r--   0 root         (0) root         (0)      271 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2210 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/abstract_backend.py
+-rw-rw-r--   0 root         (0) root         (0)     1079 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/loader.py
+-rw-rw-r--   0 root         (0) root         (0)    17277 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/local.py
+-rw-rw-r--   0 root         (0) root         (0)    20228 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/databricks.py
+-rw-rw-r--   0 root         (0) root         (0)     6402 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/docker.py
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/env_type.py
+-rw-rw-r--   0 root         (0) root         (0)     6379 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/kubernetes.py
+-rw-rw-r--   0 root         (0) root         (0)     3574 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/submitted_run.py
+-rw-rw-r--   0 root         (0) root         (0)    12237 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    14024 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/prophet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17261 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_artifacts_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14095 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    42316 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_uc_registry_messages_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    12471 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_uc_registry_service_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16146 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/facet_feature_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1361 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/internal_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     8552 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/mlflow_artifacts_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    54475 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/model_registry_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/scalapb/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/scalapb/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3307 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/scalapb/scalapb_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    53666 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/
+-rw-rw-r--   0 root         (0) root         (0)    81981 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16573 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/backend.py
+-rw-rw-r--   0 root         (0) root         (0)      901 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/mlserver.py
+-rw-rw-r--   0 root         (0) root         (0)    15392 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/
+-rw-rw-r--   0 root         (0) root         (0)    13926 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4222 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/client.py
+-rw-rw-r--   0 root         (0) root         (0)      175 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/wsgi.py
+-rw-rw-r--   0 root         (0) root         (0)     2124 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/spark_model_cache.py
+-rw-rw-r--   0 root         (0) root         (0)     1001 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/stdin_server.py
+-rw-rw-r--   0 root         (0) root         (0)  7380252 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pypi_package_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/
+-rw-rw-r--   0 root         (0) root         (0)       50 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/
+-rw-rw-r--   0 root         (0) root         (0)    55602 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2908 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/_autolog.py
+-rw-rw-r--   0 root         (0) root         (0)     1886 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/log_model_allowlist.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/
+-rw-rw-r--   0 root         (0) root         (0)    45559 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17568 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/_lightning_autolog.py
+-rw-rw-r--   0 root         (0) root         (0)     2654 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/_pytorch_autolog.py
+-rw-rw-r--   0 root         (0) root         (0)     2090 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/pickle_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/
+-rw-rw-r--   0 root         (0) root         (0)     1330 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6092 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/artifacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/
+-rw-rw-r--   0 root         (0) root         (0)    10189 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4780 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/histogram_generator.py
+-rw-rw-r--   0 root         (0) root         (0)    12548 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/pandas_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/templates/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/templates/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3488 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/v1/
+-rw-rw-r--   0 root         (0) root         (0)      122 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    20462 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/v1/recipe.py
+-rw-rw-r--   0 root         (0) root         (0)     2917 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cli.py
+-rw-rw-r--   0 root         (0) root         (0)    18431 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/dag_help_strings.py
+-rw-rw-r--   0 root         (0) root         (0)    17933 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/recipe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/v1/
+-rw-rw-r--   0 root         (0) root         (0)      114 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/v1/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22495 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/v1/recipe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/resources/
+-rw-rw-r--   0 root         (0) root         (0)    12211 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/resources/recipe_dag_template.html
+-rw-rw-r--   0 root         (0) root         (0)    14841 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.876453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/automl/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/automl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6260 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/automl/flaml.py
+-rw-rw-r--   0 root         (0) root         (0)    20666 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/evaluate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/ingest/
+-rw-rw-r--   0 root         (0) root         (0)    11137 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/ingest/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    26390 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/ingest/datasets.py
+-rw-rw-r--   0 root         (0) root         (0)    12140 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/predict.py
+-rw-rw-r--   0 root         (0) root         (0)     7664 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/register.py
+-rw-rw-r--   0 root         (0) root         (0)    19541 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/split.py
+-rw-rw-r--   0 root         (0) root         (0)    59735 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/train.py
+-rw-rw-r--   0 root         (0) root         (0)    10602 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/transform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/
+-rw-rw-r--   0 root         (0) root         (0)     6355 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    28468 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/execution.py
+-rw-rw-r--   0 root         (0) root         (0)     8990 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/metrics.py
+-rw-rw-r--   0 root         (0) root         (0)     7680 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/step.py
+-rw-rw-r--   0 root         (0) root         (0)    12316 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/tracking.py
+-rw-rw-r--   0 root         (0) root         (0)     1748 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/wrapped_recipe_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/rfunc/
+-rw-rw-r--   0 root         (0) root         (0)     1115 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/rfunc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3639 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/rfunc/backend.py
+-rw-rw-r--   0 root         (0) root         (0)     2519 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/runs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/sagemaker/
+-rw-rw-r--   0 root         (0) root         (0)   135083 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/sagemaker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12986 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/sagemaker/cli.py
+-rw-rw-r--   0 root         (0) root         (0)    14450 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/sentence_transformers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/
+-rw-rw-r--   0 root         (0) root         (0)     7077 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/
+-rw-rw-r--   0 root         (0) root         (0)    28016 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      123 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/basic_auth.ini
+-rw-rw-r--   0 root         (0) root         (0)     4689 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/client.py
+-rw-rw-r--   0 root         (0) root         (0)      575 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/config.py
+-rw-rw-r--   0 root         (0) root         (0)     4217 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/entities.py
+-rw-rw-r--   0 root         (0) root         (0)     2673 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/logo.py
+-rw-rw-r--   0 root         (0) root         (0)     1267 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     1111 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/routes.py
+-rw-rw-r--   0 root         (0) root         (0)    12648 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/sqlalchemy_store.py
+-rw-rw-r--   0 root         (0) root         (0)    69738 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/handlers.py
+-rw-rw-r--   0 root         (0) root         (0)      481 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/server/prometheus_exporter.py
+-rw-rw-r--   0 root         (0) root         (0)    26647 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/shap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/sklearn/
+-rw-rw-r--   0 root         (0) root         (0)    85689 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/sklearn/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    37469 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/sklearn/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    14259 2023-05-21 09:18:08.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/spacy.py
+-rw-rw-r--   0 root         (0) root         (0)    45175 2023-06-11 09:09:54.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/spark.py
+-rw-rw-r--   0 root         (0) root         (0)    24781 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/statsmodels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/
+-rw-rw-r--   0 root         (0) root         (0)      227 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    28656 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/rest_store.py
+-rw-rw-r--   0 root         (0) root         (0)     5419 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10481 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5836 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/artifact_repository_registry.py
+-rw-rw-r--   0 root         (0) root         (0)     8136 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/azure_blob_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5829 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5378 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/cli.py
+-rw-rw-r--   0 root         (0) root         (0)    35001 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/databricks_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     9819 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/databricks_models_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)    10247 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/dbfs_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5234 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/ftp_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5873 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/gcs_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     9684 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/hdfs_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     3377 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/http_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5107 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/local_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/mlflow_artifacts_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     6757 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/models_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     6016 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/runs_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     9433 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/s3_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5455 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/sftp_artifact_repo.py
+-rw-rw-r--   0 root         (0) root         (0)     5592 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3934 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/utils/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/base_sql_model.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/db_types.py
+-rw-rw-r--   0 root         (0) root         (0)    10567 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1634 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/alembic.ini
+-rw-rw-r--   0 root         (0) root         (0)     2768 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/
+-rw-rw-r--   0 root         (0) root         (0)     1990 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py
+-rw-rw-r--   0 root         (0) root         (0)      462 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/0c779009ac13_add_deleted_time_field_to_runs_table.py
+-rw-rw-r--   0 root         (0) root         (0)      924 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py
+-rw-rw-r--   0 root         (0) root         (0)     1059 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py
+-rw-rw-r--   0 root         (0) root         (0)     2624 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py
+-rw-rw-r--   0 root         (0) root         (0)     1375 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py
+-rw-rw-r--   0 root         (0) root         (0)     1433 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py
+-rw-rw-r--   0 root         (0) root         (0)     1201 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py
+-rw-rw-r--   0 root         (0) root         (0)      940 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py
+-rw-rw-r--   0 root         (0) root         (0)     1014 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py
+-rw-rw-r--   0 root         (0) root         (0)     3092 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py
+-rw-rw-r--   0 root         (0) root         (0)      476 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/84291f40a231_add_run_link_to_model_version.py
+-rw-rw-r--   0 root         (0) root         (0)     5716 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py
+-rw-rw-r--   0 root         (0) root         (0)     1666 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py
+-rw-rw-r--   0 root         (0) root         (0)      577 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      582 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py
+-rw-rw-r--   0 root         (0) root         (0)      637 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py
+-rw-rw-r--   0 root         (0) root         (0)     1295 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py
+-rw-rw-r--   0 root         (0) root         (0)      684 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py
+-rw-rw-r--   0 root         (0) root         (0)     2830 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py
+-rw-rw-r--   0 root         (0) root         (0)      904 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.880453 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/entities/
+-rw-rw-r--   0 root         (0) root         (0)       80 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/entities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      479 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/entities/paged_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/
+-rw-rw-r--   0 root         (0) root         (0)      605 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11022 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/abstract_store.py
+-rw-rw-r--   0 root         (0) root         (0)     1440 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/base_rest_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/dbmodels/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/dbmodels/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/dbmodels/models.py
+-rw-rw-r--   0 root         (0) root         (0)    38833 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/file_store.py
+-rw-rw-r--   0 root         (0) root         (0)    16920 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/rest_store.py
+-rw-rw-r--   0 root         (0) root         (0)    50646 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/sqlalchemy_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/
+-rw-rw-r--   0 root         (0) root         (0)     1154 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13534 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/abstract_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8315 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/initial_models.py
+-rw-rw-r--   0 root         (0) root         (0)    21085 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/models.py
+-rw-rw-r--   0 root         (0) root         (0)    52631 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/file_store.py
+-rw-rw-r--   0 root         (0) root         (0)    12822 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/rest_store.py
+-rw-rw-r--   0 root         (0) root         (0)    77913 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/sqlalchemy_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tensorflow/
+-rw-rw-r--   0 root         (0) root         (0)    60208 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tensorflow/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8442 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tensorflow/_autolog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/
+-rw-rw-r--   0 root         (0) root         (0)      995 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/
+-rw-rw-r--   0 root         (0) root         (0)       41 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15534 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/client.py
+-rw-rw-r--   0 root         (0) root         (0)     9641 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/fluent.py
+-rw-rw-r--   0 root         (0) root         (0)     3152 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     7008 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    24289 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/client.py
+-rw-rw-r--   0 root         (0) root         (0)     2335 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/registry.py
+-rw-rw-r--   0 root         (0) root         (0)     9517 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     7540 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/artifact_utils.py
+-rw-rw-r--   0 root         (0) root         (0)   142886 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1076 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/abstract_context.py
+-rw-rw-r--   0 root         (0) root         (0)      520 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_cluster_context.py
+-rw-rw-r--   0 root         (0) root         (0)      561 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_command_context.py
+-rw-rw-r--   0 root         (0) root         (0)     1965 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_job_context.py
+-rw-rw-r--   0 root         (0) root         (0)     1713 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_notebook_context.py
+-rw-rw-r--   0 root         (0) root         (0)     1952 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_repo_context.py
+-rw-rw-r--   0 root         (0) root         (0)     1020 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/default_context.py
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/git_context.py
+-rw-rw-r--   0 root         (0) root         (0)     3738 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/registry.py
+-rw-rw-r--   0 root         (0) root         (0)      443 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/system_environment_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1703 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/abstract_context.py
+-rw-rw-r--   0 root         (0) root         (0)     1718 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py
+-rw-rw-r--   0 root         (0) root         (0)     2300 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py
+-rw-rw-r--   0 root         (0) root         (0)     3173 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/registry.py
+-rw-rw-r--   0 root         (0) root         (0)    78452 2023-06-06 10:07:33.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/fluent.py
+-rw-rw-r--   0 root         (0) root         (0)     3404 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/llm_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2248 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/metric_value_conversion_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3515 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1077 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/abstract_request_header_provider.py
+-rw-rw-r--   0 root         (0) root         (0)     1336 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/databricks_request_header_provider.py
+-rw-rw-r--   0 root         (0) root         (0)      486 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/default_request_header_provider.py
+-rw-rw-r--   0 root         (0) root         (0)     2867 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/registry.py
+-rw-rw-r--   0 root         (0) root         (0)   110231 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/transformers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.884454 mlflow_by_johnsnowlabs-2.9.0/mlflow/types/
+-rw-rw-r--   0 root         (0) root         (0)      299 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/types/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15035 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/types/schema.py
+-rw-rw-r--   0 root         (0) root         (0)    18044 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/
+-rw-rw-r--   0 root         (0) root         (0)     9365 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6589 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_capture_modules.py
+-rw-rw-r--   0 root         (0) root         (0)     2274 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_capture_transformers_modules.py
+-rw-rw-r--   0 root         (0) root         (0)     6387 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_spark_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5009 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/annotations.py
+-rw-rw-r--   0 root         (0) root         (0)      400 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/arguments_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/
+-rw-rw-r--   0 root         (0) root         (0)    27045 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16642 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/client.py
+-rw-rw-r--   0 root         (0) root         (0)    10937 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/events.py
+-rw-rw-r--   0 root         (0) root         (0)    13381 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/logging_and_warnings.py
+-rw-rw-r--   0 root         (0) root         (0)    47266 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/safety.py
+-rw-rw-r--   0 root         (0) root         (0)     3570 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/versioning.py
+-rw-rw-r--   0 root         (0) root         (0)      215 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/class_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6431 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/cli_args.py
+-rw-rw-r--   0 root         (0) root         (0)    13002 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/conda.py
+-rw-rw-r--   0 root         (0) root         (0)      432 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/data_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    23803 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/databricks_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     9138 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/docstring_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1669 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/download_cloud_file_chunk.py
+-rw-rw-r--   0 root         (0) root         (0)      192 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/env.py
+-rw-rw-r--   0 root         (0) root         (0)      474 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/env_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    22714 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/environment.py
+-rw-rw-r--   0 root         (0) root         (0)    30464 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/file_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2306 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/git_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    24178 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/gorilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/import_hooks/
+-rw-rw-r--   0 root         (0) root         (0)    13645 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/import_hooks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2597 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/logging_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1298 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/mime_type_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4024 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/mlflow_tags.py
+-rw-rw-r--   0 root         (0) root         (0)     8109 2023-05-21 08:45:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/model_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5873 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/name_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2412 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/nfs_on_spark.py
+-rw-rw-r--   0 root         (0) root         (0)      139 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/os.py
+-rw-rw-r--   0 root         (0) root         (0)     5799 2023-06-12 03:19:23.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/process.py
+-rw-rw-r--   0 root         (0) root         (0)    19909 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/proto_json_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     5560 2023-06-11 11:21:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/request_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    20050 2023-07-20 22:36:16.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/requirements_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11987 2023-06-13 16:35:00.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/rest_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    59666 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/search_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2368 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/server_cli_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     3805 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/string_utils.py
+-rw-rw-r--   0 root         (0) root         (0)      512 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/time_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    14271 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/uri.py
+-rw-rw-r--   0 root         (0) root         (0)    19435 2023-06-02 04:04:13.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/validation.py
+-rw-rw-r--   0 root         (0) root         (0)    16282 2023-07-27 18:58:37.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/virtualenv.py
+-rw-rw-r--   0 root         (0) root         (0)      170 2023-07-27 20:01:36.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/mlflow/xgboost/
+-rw-rw-r--   0 root         (0) root         (0)    37317 2023-06-04 16:58:45.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/xgboost/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2908 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow/xgboost/_autolog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10580 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15074 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:36:33.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-27 20:01:43.000000 mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/
+-rw-rw-r--   0 root         (0) root         (0)      614 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2234 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     4556 2023-05-31 07:59:21.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/import_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      856 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/print_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/pytest_raises_checker/
+-rw-rw-r--   0 root         (0) root         (0)     1546 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/pytest_raises_checker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      571 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/set_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      878 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/string_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      692 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/unittest_assert_raises.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/requirements/
+-rw-rw-r--   0 root         (0) root         (0)      609 2023-06-06 04:13:04.000000 mlflow_by_johnsnowlabs-2.9.0/requirements/core-requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      297 2023-06-08 09:49:57.000000 mlflow_by_johnsnowlabs-2.9.0/requirements/gateway-requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)      481 2023-05-18 21:19:46.000000 mlflow_by_johnsnowlabs-2.9.0/requirements/skinny-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 20:01:43.888454 mlflow_by_johnsnowlabs-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     7281 2023-07-20 22:35:38.000000 mlflow_by_johnsnowlabs-2.9.0/setup.py
```

### Comparing `mlflow_by_johnsnowlabs-2.8.0/LICENSE.txt` & `mlflow_by_johnsnowlabs-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/MANIFEST.in` & `mlflow_by_johnsnowlabs-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/PKG-INFO` & `mlflow_by_johnsnowlabs-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow_by_johnsnowlabs
-Version: 2.8.0
+Version: 2.9.0
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow_by_johnsnowlabs-2.8.0/README.rst` & `mlflow_by_johnsnowlabs-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/README_SKINNY.rst` & `mlflow_by_johnsnowlabs-2.9.0/README_SKINNY.rst`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/_doctor.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/_doctor.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/_spark_autologging.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/_spark_autologging.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/artifacts/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/azure/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/azure/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/catboost.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/catboost.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/artifact_dataset_sources.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/artifact_dataset_sources.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/code_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/code_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/dataset_source_registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/dataset_source_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/delta_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/delta_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/digest_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/digest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/filesystem_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/filesystem_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/http_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/http_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/huggingface_dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/huggingface_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/huggingface_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/numpy_dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/numpy_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/pandas_dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/pyfunc_dataset_mixin.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/pyfunc_dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/schema.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_dataset_source.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/spark_delta_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/spark_delta_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/data/tensorflow_dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/data/tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/db.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/db.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/base.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/base.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/interface.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/interface.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/plugin_manager.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/deployments/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/deployments/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/diviner.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/diviner.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/_mlflow_object.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/_mlflow_object.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/dataset.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/dataset_input.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/dataset_input.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/experiment.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/experiment_tag.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/experiment_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/file_info.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/file_info.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/input_tag.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/input_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/lifecycle_stage.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/lifecycle_stage.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/metric.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/metric.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_stages.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_stages.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_status.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_status.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/model_version_tag.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/model_version_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model_alias.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model_alias.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/model_registry/registered_model_tag.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/model_registry/registered_model_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/param.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/param.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_data.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_data.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_info.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_info.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_inputs.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_inputs.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_status.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_status.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/run_tag.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/run_tag.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/source_type.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/source_type.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/entities/view_type.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/entities/view_type.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/environment_variables.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/environment_variables.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/exceptions.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/experiments.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/fastai/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/fastai/callback.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/fastai/callback.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/gluon/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/gluon/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/gluon/_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/gluon/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/h2o.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/h2o.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/johnsnowlabs.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/johnsnowlabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,20 +109,20 @@
 _JOHNSNOWLABS_ENV_JSON_LICENSE_KEY = "JOHNSNOWLABS_LICENSE_JSON"
 _JOHNSNOWLABS_MODEL_PATH_SUB = "jsl-model"
 _logger = logging.getLogger(__name__)
 
 
 def _validate_env_vars():
     return True
-    if _JOHNSNOWLABS_ENV_JSON_LICENSE_KEY not in os.environ:
-        raise Exception(
-            f"Please set the {_JOHNSNOWLABS_ENV_JSON_LICENSE_KEY}"
-            f" environment variable as the raw license.json string from John Snow Labs"
-        )
-    _set_env_vars()
+    # if _JOHNSNOWLABS_ENV_JSON_LICENSE_KEY not in os.environ:
+    #     raise Exception(
+    #         f"Please set the {_JOHNSNOWLABS_ENV_JSON_LICENSE_KEY}"
+    #         f" environment variable as the raw license.json string from John Snow Labs"
+    #     )
+    # _set_env_vars()
 
 
 def _set_env_vars():
     # if json license is detected, we parse it and set the env vars
     loaded_license = json.loads(os.environ[_JOHNSNOWLABS_ENV_JSON_LICENSE_KEY])
     os.environ.update({k: str(v) for k, v in loaded_license.items() if v is not None})
```

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/langchain/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/langchain/api_request_parallel_processor.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/langchain/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/lightgbm.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/ml_package_versions.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/ml_package_versions.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/mleap.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/mleap.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__pycache__/__init__.cpython-310.pyc` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/__pycache__/__init__.cpython-39.pyc` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/container/scoring_server/nginx.conf` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/container/scoring_server/nginx.conf`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/docker_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/docker_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/_shap_patch.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/_shap_patch.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/artifacts.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/base.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/default_evaluator.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/default_evaluator.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/evaluator_registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/evaluator_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/lift_curve.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/lift_curve.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/evaluation/validation.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/evaluation/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/flavor_backend.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/flavor_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/flavor_backend_registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/flavor_backend_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/model.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/model.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/signature.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/signature.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/models/wheeled_model.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/models/wheeled_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/onnx.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/onnx.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/api_request_parallel_processor.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/api_request_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/retry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/retry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/openai/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/openai/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/paddle/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/paddle/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/paddle/_paddle_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/paddle/_paddle_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pmdarima.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pmdarima.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/_project_spec.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/_project_spec.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/abstract_backend.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/loader.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/loader.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/backend/local.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/backend/local.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/databricks.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/databricks.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/docker.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/docker.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/kubernetes.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/kubernetes.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/submitted_run.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/submitted_run.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/projects/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/projects/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/prophet.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/prophet.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_artifacts_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_uc_registry_messages_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_uc_registry_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/databricks_uc_registry_service_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/databricks_uc_registry_service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/facet_feature_statistics_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/facet_feature_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/internal_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/internal_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/mlflow_artifacts_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/mlflow_artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/model_registry_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/scalapb/scalapb_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/scalapb/scalapb_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/protos/service_pb2.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/protos/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/backend.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/mlserver.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/mlserver.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/model.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/model.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/scoring_server/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/scoring_server/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/spark_model_cache.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/spark_model_cache.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyfunc/stdin_server.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyfunc/stdin_server.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pypi_package_index.json` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pypi_package_index.json`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pyspark/ml/log_model_allowlist.txt` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pyspark/ml/log_model_allowlist.txt`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/_lightning_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/_lightning_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/_pytorch_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/_pytorch_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/pytorch/pickle_module.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/pytorch/pickle_module.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/artifacts.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/histogram_generator.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/histogram_generator.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/pandas_renderer.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/pandas_renderer.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cards/templates/base.html` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cards/templates/base.html`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/classification/v1/recipe.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/classification/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/dag_help_strings.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/dag_help_strings.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/recipe.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/regression/v1/recipe.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/regression/v1/recipe.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/resources/recipe_dag_template.html` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/resources/recipe_dag_template.html`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/step.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/step.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/automl/flaml.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/automl/flaml.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/evaluate.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/evaluate.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/ingest/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/ingest/datasets.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/ingest/datasets.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/predict.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/predict.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/register.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/register.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/split.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/split.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/train.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/train.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/steps/transform.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/steps/transform.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/execution.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/execution.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/metrics.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/step.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/step.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/tracking.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/recipes/utils/wrapped_recipe_model.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/recipes/utils/wrapped_recipe_model.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/rfunc/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/rfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/rfunc/backend.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/rfunc/backend.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/runs.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/runs.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/sagemaker/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/sagemaker/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/sagemaker/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/sentence_transformers.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/config.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/entities.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/entities.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/logo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/logo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/permissions.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/routes.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/routes.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/auth/sqlalchemy_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/auth/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/server/handlers.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/server/handlers.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/shap.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/shap.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/sklearn/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/sklearn/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/sklearn/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/spacy.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/spacy.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/spark.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/spark.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/statsmodels.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/statsmodels.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/rest_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/_unity_catalog/registry/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/_unity_catalog/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/artifact_repository_registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/artifact_repository_registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/azure_blob_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/azure_blob_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/azure_data_lake_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/cli.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/cli.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/databricks_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/databricks_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/databricks_models_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/databricks_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/dbfs_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/dbfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/ftp_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/ftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/gcs_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/gcs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/hdfs_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/hdfs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/http_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/http_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/local_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/local_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/mlflow_artifacts_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/mlflow_artifacts_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/models_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/runs_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/runs_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/s3_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/s3_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/sftp_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/sftp_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/unity_catalog_models_artifact_repo.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/artifact/utils/models.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/artifact/utils/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/alembic.ini` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/env.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/env.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/0a8213491aaa_drop_duplicate_killed_constraint.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/181f10493468_allow_nulls_for_metric_values.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/27a6a02d2cf1_add_model_version_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/2b4d017a5e9b_add_model_registry_tables_to_db.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/3500859a5d39_add_model_aliases_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/39d1c3be5f05_add_is_nan_constraint_for_metrics_tables_if_necessary.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/451aebb31d03_add_metric_step.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/728d730b5ebd_add_registered_model_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/7ac759974ad8_update_run_tags_with_larger_limit.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/7f2a7d5fae7d_add_datasets_inputs_input_tags_tables.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/89d4b8295536_create_latest_metrics_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/90e64c465722_migrate_user_column_to_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/97727af70f4d_creation_time_last_update_time_experiments.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/a8c4a736bde6_allow_nulls_for_run_id.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/bd07f7e963c5_create_index_on_run_uuid.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/c48cb773bb87_reset_default_value_for_is_nan_in_metrics_table_for_mysql.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/cc1f77228345_change_param_value_length_to_500.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/cfd24bdc0731_update_run_status_constraint_with_killed.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/db_migrations/versions/df50e92ffc5e_add_experiment_tags_table.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/abstract_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/base_rest_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/base_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/dbmodels/models.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/file_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/rest_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/model_registry/sqlalchemy_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/model_registry/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/abstract_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/abstract_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/initial_models.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/initial_models.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/dbmodels/models.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/dbmodels/models.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/file_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/file_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/rest_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/rest_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/store/tracking/sqlalchemy_store.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/store/tracking/sqlalchemy_store.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tensorflow/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tensorflow/_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tensorflow/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/fluent.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_model_registry/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_model_registry/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/_tracking_service/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/_tracking_service/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/artifact_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/abstract_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_cluster_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_cluster_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_command_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_command_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_job_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_job_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_notebook_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_notebook_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/databricks_repo_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/databricks_repo_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/default_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/default_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/git_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/git_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/context/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/context/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/abstract_context.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/abstract_context.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/databricks_job_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/databricks_notebook_experiment_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/default_experiment/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/default_experiment/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/fluent.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/fluent.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/llm_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/llm_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/metric_value_conversion_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/metric_value_conversion_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/abstract_request_header_provider.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/abstract_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/databricks_request_header_provider.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/databricks_request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/tracking/request_header/registry.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/tracking/request_header/registry.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/transformers.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/transformers.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/types/schema.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/types/schema.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/types/utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/types/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_capture_modules.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_capture_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_capture_transformers_modules.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_capture_transformers_modules.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/_spark_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/_spark_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/annotations.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/annotations.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/client.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/client.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/events.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/events.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/logging_and_warnings.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/logging_and_warnings.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/safety.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/safety.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/autologging_utils/versioning.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/autologging_utils/versioning.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/cli_args.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/cli_args.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/conda.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/conda.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/databricks_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/docstring_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/docstring_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/download_cloud_file_chunk.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/download_cloud_file_chunk.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/environment.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/environment.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/file_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/git_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/gorilla.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/gorilla.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/import_hooks/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/import_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/logging_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/mime_type_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/mime_type_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/mlflow_tags.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/mlflow_tags.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/model_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/name_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/name_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/nfs_on_spark.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/nfs_on_spark.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/process.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/process.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/proto_json_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/proto_json_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/request_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/requirements_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/requirements_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/rest_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/rest_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/search_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/server_cli_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/server_cli_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/string_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/time_utils.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/uri.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/uri.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/validation.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/utils/virtualenv.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/xgboost/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow/xgboost/_autolog.py` & `mlflow_by_johnsnowlabs-2.9.0/mlflow/xgboost/_autolog.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/PKG-INFO` & `mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-by-johnsnowlabs
-Version: 2.8.0
+Version: 2.9.0
 Summary: MLflow: A Platform for ML Development and Productionization
 Home-page: https://mlflow.org/
 Author: Databricks
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/mlflow/mlflow/issues
 Project-URL: Documentation, https://mlflow.org/docs/latest/index.html
 Project-URL: Source Code, https://github.com/mlflow/mlflow
```

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/SOURCES.txt` & `mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/mlflow_by_johnsnowlabs.egg-info/requires.txt` & `mlflow_by_johnsnowlabs-2.9.0/mlflow_by_johnsnowlabs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/errors.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/errors.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/import_checker.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/import_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/print_function.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/print_function.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/pytest_raises_checker/__init__.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/pytest_raises_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/set_checker.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/set_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/string_checker.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/string_checker.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/pylint_plugins/unittest_assert_raises.py` & `mlflow_by_johnsnowlabs-2.9.0/pylint_plugins/unittest_assert_raises.py`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/requirements/core-requirements.txt` & `mlflow_by_johnsnowlabs-2.9.0/requirements/core-requirements.txt`

 * *Files identical despite different names*

### Comparing `mlflow_by_johnsnowlabs-2.8.0/setup.py` & `mlflow_by_johnsnowlabs-2.9.0/setup.py`

 * *Files identical despite different names*

