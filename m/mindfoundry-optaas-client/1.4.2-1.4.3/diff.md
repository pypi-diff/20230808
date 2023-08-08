# Comparing `tmp/mindfoundry-optaas-client-1.4.2.tar.gz` & `tmp/mindfoundry-optaas-client-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindfoundry-optaas-client-1.4.2.tar", last modified: Mon Mar 20 13:50:38 2023, max compression
+gzip compressed data, was "mindfoundry-optaas-client-1.4.3.tar", last modified: Tue Aug  8 09:04:54 2023, max compression
```

## Comparing `mindfoundry-optaas-client-1.4.2.tar` & `mindfoundry-optaas-client-1.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.349124 mindfoundry-optaas-client-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1984 2023-03-20 13:50:38.348124 mindfoundry-optaas-client-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.334122 mindfoundry-optaas-client-1.4.2/mindfoundry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.334122 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.340123 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    16515 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/expressions.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/goal.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/objective.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     4657 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/result.py
--rw-rw-rw-   0 root         (0) root         (0)     5780 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.342123 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.346124 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ada_boost.py
--rw-rw-rw-   0 root         (0) root         (0)     9718 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ica.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/k_neighbors.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/pca.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/svc.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/voting.py
--rw-rw-rw-   0 root         (0) root         (0)     2553 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)     8188 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/parameter_maker.py
--rw-rw-rw-   0 root         (0) root         (0)     5731 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/sklearn_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    25578 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/user_defined_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1847 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     6596 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 13:50:38.348124 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1984 2023-03-20 13:50:38.000000 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1931 2023-03-20 13:50:38.000000 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 13:50:38.000000 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-03-20 13:50:38.000000 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-20 13:50:38.000000 mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 13:50:38.349124 mindfoundry-optaas-client-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-03-20 13:50:35.000000 mindfoundry-optaas-client-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.998057 mindfoundry-optaas-client-1.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-08-08 09:04:53.998057 mindfoundry-optaas-client-1.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.991057 mindfoundry-optaas-client-1.4.3/mindfoundry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.991057 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.994057 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1864 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    16515 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/expressions.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/goal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/objective.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4657 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/result.py
+-rw-rw-rw-   0 root         (0) root         (0)     5780 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.995057 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.997057 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ada_boost.py
+-rw-rw-rw-   0 root         (0) root         (0)     9718 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ica.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/k_neighbors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/pca.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/svc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/voting.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)     8188 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/parameter_maker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/sklearn_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    25578 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1138 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/user_defined_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1847 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     6596 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:04:53.998057 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-08-08 09:04:53.000000 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-08-08 09:04:53.000000 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 09:04:53.000000 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-08-08 09:04:53.000000 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-08 09:04:53.000000 mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 09:04:53.998057 mindfoundry-optaas-client-1.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-08-08 09:04:52.000000 mindfoundry-optaas-client-1.4.3/setup.py
```

### Comparing `mindfoundry-optaas-client-1.4.2/LICENSE` & `mindfoundry-optaas-client-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/PKG-INFO` & `mindfoundry-optaas-client-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindfoundry-optaas-client
-Version: 1.4.2
+Version: 1.4.3
 Summary: Mind Foundry Optimization as a Service: Python Client
 Home-page: https://mindfoundry.ai/optaas
 Author: Mind Foundry Ltd
 Author-email: optaas@mindfoundry.ai
 License: MIT License
 Keywords: bayesian optimization,bayesian,optimization,machine learning,machine-learning,hyperparameter,hyper-parameters,model selection,model-selection
 Platform: Any
```

### Comparing `mindfoundry-optaas-client-1.4.2/README.md` & `mindfoundry-optaas-client-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/api_key.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/api_key.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/client.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/client.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/configuration.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/configuration.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/expressions.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/expressions.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/objective.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/objective.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/parameter.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/parameter.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/prediction.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/prediction.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/result.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/result.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/session.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             'Connection': 'keep-alive' if keep_alive else 'close'
         }
         self._disable_version_check = disable_version_check
 
     @staticmethod
     def _make_session(server_url: str, max_retries: int) -> Session:
         session = Session()
-        retry = Retry(total=max_retries, connect=max_retries, backoff_factor=0.5, method_whitelist=None,
+        retry = Retry(total=max_retries, connect=max_retries, backoff_factor=0.5, allowed_methods=False,
                       status_forcelist=RETRY_STATUS_CODES)
         session.mount(server_url, HTTPAdapter(max_retries=retry))
         return session
 
     def post(self, endpoint: str, body: dict, timeout: float = DEFAULT_TIMEOUT) -> OPTaaSResponse:
         """Make a POST request to OPTaaS with a JSON body.
```

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ada_boost.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ada_boost.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ensemble.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ensemble.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/ica.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/ica.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/k_neighbors.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/k_neighbors.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/linear_model.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/linear_model.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/pca.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/pca.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/svc.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/svc.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/voting.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/voting.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/estimators/xgboost.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/estimators/xgboost.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/mixin.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/mixin.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/parameter_maker.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/parameter_maker.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/sklearn_task.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/sklearn_task.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/sklearn_pipelines/utils.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/sklearn_pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/task.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/task.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/user_defined_configuration.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/user_defined_configuration.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/utils.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/utils.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/version_check.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/version_check.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry/optaas/client/viz.py` & `mindfoundry-optaas-client-1.4.3/mindfoundry/optaas/client/viz.py`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/PKG-INFO` & `mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindfoundry-optaas-client
-Version: 1.4.2
+Version: 1.4.3
 Summary: Mind Foundry Optimization as a Service: Python Client
 Home-page: https://mindfoundry.ai/optaas
 Author: Mind Foundry Ltd
 Author-email: optaas@mindfoundry.ai
 License: MIT License
 Keywords: bayesian optimization,bayesian,optimization,machine learning,machine-learning,hyperparameter,hyper-parameters,model selection,model-selection
 Platform: Any
```

### Comparing `mindfoundry-optaas-client-1.4.2/mindfoundry_optaas_client.egg-info/SOURCES.txt` & `mindfoundry-optaas-client-1.4.3/mindfoundry_optaas_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindfoundry-optaas-client-1.4.2/setup.py` & `mindfoundry-optaas-client-1.4.3/setup.py`

 * *Files identical despite different names*

