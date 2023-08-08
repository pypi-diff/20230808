# Comparing `tmp/syngen-0.2.0rc0.tar.gz` & `tmp/syngen-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.2.0rc0.tar", last modified: Thu Aug  3 11:07:02 2023, max compression
+gzip compressed data, was "syngen-0.2.0rc1.tar", last modified: Fri Aug  4 14:47:53 2023, max compression
```

## Comparing `syngen-0.2.0rc0.tar` & `syngen-0.2.0rc1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20910 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.271280 syngen-0.2.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11674 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16303 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723170 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5183 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.271280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.279280 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    46130 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      391 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7731 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.283280 syngen-0.2.0rc0/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    36772 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24485 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10565 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11221 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5231 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.287280 syngen-0.2.0rc0/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11869 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-08-03 11:05:00.000000 syngen-0.2.0rc0/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 11:07:02.275280 syngen-0.2.0rc0/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-03 11:07:02.000000 syngen-0.2.0rc0/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-04 14:46:28.000000 syngen-0.2.0rc1/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-08-04 14:46:28.000000 syngen-0.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-08-04 14:46:28.000000 syngen-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20910 2023-08-04 14:46:28.000000 syngen-0.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.504159 syngen-0.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3495 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11144 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3476 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11674 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16303 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723170 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5183 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.504159 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46130 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.512159 syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6859 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7731 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36772 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24485 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10551 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11221 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5231 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.516159 syngen-0.2.0rc1/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11869 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-08-04 14:46:29.000000 syngen-0.2.0rc1/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 14:47:53.508159 syngen-0.2.0rc1/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21652 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-04 14:47:53.000000 syngen-0.2.0rc1/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.2.0rc0/LICENSE` & `syngen-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/PKG-INFO` & `syngen-0.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc0 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc1 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.2.0rc0/README.md` & `syngen-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/setup.cfg` & `syngen-0.2.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 packages = find:
 include_package_data = True
 python_requires = >3.7
 install_requires = 
 	category_encoders==2.5.*
 	click
 	ipython==8.4.*
-	keras==2.12.*
+	keras<2.14,>=2.13.1
 	lazy==1.4
 	loguru
 	matplotlib==3.5.*
 	numpy==1.22.*
 	pandas==1.3.*
 	pandavro==1.7.*
 	pathos==0.2.*
 	scikit_learn==1.1.*
 	scipy==1.7.*
 	seaborn==0.11.*
-	tensorflow==2.12.*
+	tensorflow==2.13.*
 	tqdm==4.64.*
 	PyYAML==6.*
 	MarkupSafe==2.0.1
 	Jinja2
 	avro
 	python-slugify[unidecode]>=7.0.0
 	pytest
```

### Comparing `syngen-0.2.0rc0/src/syngen/infer.py` & `syngen-0.2.0rc1/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/config/configurations.py` & `syngen-0.2.0rc1/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/context/context.py` & `syngen-0.2.0rc1/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/convertor/convertor.py` & `syngen-0.2.0rc1/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.2.0rc1/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/handlers/handlers.py` & `syngen-0.2.0rc1/src/syngen/ml/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/__init__.py` & `syngen-0.2.0rc1/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.2.0rc1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.2.0rc1/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.2.0rc1/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/metrics/utils.py` & `syngen-0.2.0rc1/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/reporters/reporters.py` & `syngen-0.2.0rc1/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/strategies/strategies.py` & `syngen-0.2.0rc1/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/utils/utils.py` & `syngen-0.2.0rc1/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.2.0rc1/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/vae/models/dataset.py` & `syngen-0.2.0rc1/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/vae/models/features.py` & `syngen-0.2.0rc1/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/vae/models/model.py` & `syngen-0.2.0rc1/src/syngen/ml/vae/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Activation,
 )
 from sklearn.mixture import BayesianGaussianMixture
 import numpy as np
 import pandas as pd
 from loguru import logger
 from IPython.display import SVG
-from keras.utils.vis_utils import model_to_dot
+from keras.utils import plot_model
 
 from syngen.ml.vae.models.custom_layers import FeatureLossLayer
 from syngen.ml.utils import slugify_parameters
 
 
 class CVAE:
     """
@@ -253,15 +253,15 @@
             for column in key_columns:
                 key_type = self.dataset.pk_uq_keys_types[column]
                 if key_type is float or self.__check_pk_numeric_convertability(column, key_type):
                     mapped_keys = np.arange(len(self.inverse_transformed_df[column])) + 1
                     self.inverse_transformed_df[column] = mapped_keys
 
     def show_model(self):
-        return SVG(model_to_dot(self.model).create(prog="dot", format="svg"))
+        return SVG(plot_model(self.model).create(prog="dot", format="svg"))
 
     def save_state(self, path: str):
         pth = Path(path)
 
         if self.model is not None:
             self.model.save_weights(str(pth / "vae.ckpt"))
```

### Comparing `syngen-0.2.0rc0/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.2.0rc1/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.2.0rc1/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/ml/worker/worker.py` & `syngen-0.2.0rc1/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen/train.py` & `syngen-0.2.0rc1/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.2.0rc0/src/syngen.egg-info/PKG-INFO` & `syngen-0.2.0rc1/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.2.0rc0
+Version: 0.2.0rc1
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc0 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.2.0rc1 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.2.0rc0/src/syngen.egg-info/SOURCES.txt` & `syngen-0.2.0rc1/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

