# Comparing `tmp/NeuralPlayground-0.0.3.tar.gz` & `tmp/NeuralPlayground-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralPlayground-0.0.3.tar", last modified: Fri Jul 28 12:56:09 2023, max compression
+gzip compressed data, was "NeuralPlayground-0.0.4.tar", last modified: Tue Aug  8 17:28:20 2023, max compression
```

## Comparing `NeuralPlayground-0.0.3.tar` & `NeuralPlayground-0.0.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.all-contributorsrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.772187 NeuralPlayground-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 12:56:09.000000 NeuralPlayground-0.0.3/NeuralPlayground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/citation.cff
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/contributors.md
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/licence.md
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/road_map.md
--rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/documents/style_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/neuralplayground/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.776187 NeuralPlayground-0.0.3/neuralplayground/agents/
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/agent_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/stachenfeld_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/weber_2018.py
--rw-r--r--   0 runner    (1001) docker     (123)    22858 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)    66462 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/arenas/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/arena_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/connected_rooms.py
--rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/discritized_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/hafting_2008.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/sargolini_2006.py
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/simple2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/arenas/wernle_2018.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/default_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/simulation_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/backend/training_loops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/comparison/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/comparison/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/config/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/main_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/config/plot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/experiment_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/hafting_2008_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/sargolini_2006_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/experiments/wernle_2018_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/neuralplayground/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/plotting/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/neuralplayground/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 12:56:09.784187 NeuralPlayground-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 12:56:09.780187 NeuralPlayground-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/agent_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tests/arena_exp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-28 12:55:57.000000 NeuralPlayground-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/.all-contributorsrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.232653 NeuralPlayground-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.240653 NeuralPlayground-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.240653 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-08-08 17:28:19.000000 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-08 17:28:20.000000 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 17:28:19.000000 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-08 17:28:19.000000 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 17:28:19.000000 NeuralPlayground-0.0.4/NeuralPlayground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.244654 NeuralPlayground-0.0.4/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/contributors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/licence.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/road_map.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20474 2023-08-08 17:28:07.000000 NeuralPlayground-0.0.4/documents/style_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.244654 NeuralPlayground-0.0.4/neuralplayground/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.244654 NeuralPlayground-0.0.4/neuralplayground/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/agent_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/stachenfeld_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/weber_2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22858 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.248654 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66462 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20416 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.248654 NeuralPlayground-0.0.4/neuralplayground/arenas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/arena_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/connected_rooms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/discritized_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/hafting_2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/sargolini_2006.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/simple2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/arenas/wernle_2018.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/neuralplayground/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/backend/default_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/backend/simulation_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/backend/training_loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/neuralplayground/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22109 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/comparison/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/neuralplayground/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/config/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/config/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/config/main_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/config/plot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/neuralplayground/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/experiment_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/hafting_2008_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/sargolini_2006_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/experiments/wernle_2018_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/neuralplayground/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/plotting/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/neuralplayground/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 17:28:20.256654 NeuralPlayground-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:20.252653 NeuralPlayground-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/tests/agent_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/tests/arena_exp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 17:28:08.000000 NeuralPlayground-0.0.4/tox.ini
```

### Comparing `NeuralPlayground-0.0.3/.all-contributorsrc` & `NeuralPlayground-0.0.4/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/.gitignore` & `NeuralPlayground-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/.pre-commit-config.yaml` & `NeuralPlayground-0.0.4/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
           - id: check-toml
           - id: end-of-file-fixer
           - id: mixed-line-ending
             args: [--fix=lf]
           - id: requirements-txt-fixer
           - id: trailing-whitespace
             exclude: 'README.md'
-    - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.280
+    - repo: https://github.com/astral-sh/ruff-pre-commit
+      rev: v0.0.282
       hooks:
         - id: ruff
     - repo: https://github.com/psf/black
       rev: 23.7.0
       hooks:
           - id: black
```

### Comparing `NeuralPlayground-0.0.3/LICENSE` & `NeuralPlayground-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/NeuralPlayground.egg-info/PKG-INFO` & `NeuralPlayground-0.0.4/NeuralPlayground.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.3
+Version: 0.0.4
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
 Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
 Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
```

### Comparing `NeuralPlayground-0.0.3/NeuralPlayground.egg-info/SOURCES.txt` & `NeuralPlayground-0.0.4/NeuralPlayground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/PKG-INFO` & `NeuralPlayground-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralPlayground
-Version: 0.0.3
+Version: 0.0.4
 Summary: The standardised environment for the hippocampus and entorhinal cortex models
 Author: Clementine Domine
 Author-email: Rodrigo Carrasco-Davis <rodrigo.carrasco.davis@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ClementineDomine/NeuralPlayground
 Project-URL: Bug tracker, https://github.com/ClementineDomine/NeuralPlayground/issues
 Project-URL: Documentation, https://github.com/ClementineDomine/NeuralPlayground
```

### Comparing `NeuralPlayground-0.0.3/README.md` & `NeuralPlayground-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/citation.cff` & `NeuralPlayground-0.0.4/documents/citation.cff`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/code_of_conduct.md` & `NeuralPlayground-0.0.4/documents/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/contributors.md` & `NeuralPlayground-0.0.4/documents/contributors.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/licence.md` & `NeuralPlayground-0.0.4/documents/licence.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/road_map.md` & `NeuralPlayground-0.0.4/documents/road_map.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/documents/style_guide.md` & `NeuralPlayground-0.0.4/documents/style_guide.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Style Guide 
 
 We are following to the best of our abilities the [PEP8](https://www.python.org/dev/peps/pep-0008/) and [numpy docstring](https://numpydoc.readthedocs.io/en/latest/format.html) style convention. Note: Pycharm has an inbuild checking framework that will help you follow the style guide. 
+The pre-commit bot will enforces these style guide requierements. 
 
 The General convention is as follows:
 
 > Class variable: NameOfClass
 
 > Function/Methods/Variable: 
         Private: _name_private_function
```

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/README.md` & `NeuralPlayground-0.0.4/neuralplayground/agents/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/agent_core.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/agent_core.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/stachenfeld_2018.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/stachenfeld_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/weber_2018.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/weber_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_analyse.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_analyse.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_model.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_model.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_parameters.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_parameters.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/agents/whittington_2020_extras/whittington_2020_utils.py` & `NeuralPlayground-0.0.4/neuralplayground/agents/whittington_2020_extras/whittington_2020_utils.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/README.md` & `NeuralPlayground-0.0.4/neuralplayground/arenas/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/arena_core.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/arena_core.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/batch_environment.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/batch_environment.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/connected_rooms.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/connected_rooms.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/discritized_objects.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/discritized_objects.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/hafting_2008.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/hafting_2008.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/sargolini_2006.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/sargolini_2006.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/simple2d.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/simple2d.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/arenas/wernle_2018.py` & `NeuralPlayground-0.0.4/neuralplayground/arenas/wernle_2018.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/backend/default_simulation.py` & `NeuralPlayground-0.0.4/neuralplayground/backend/default_simulation.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/backend/simulation_manager.py` & `NeuralPlayground-0.0.4/neuralplayground/backend/simulation_manager.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/backend/training_loops.py` & `NeuralPlayground-0.0.4/neuralplayground/backend/training_loops.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/comparison/metrics.py` & `NeuralPlayground-0.0.4/neuralplayground/comparison/metrics.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/config/default_config.yaml` & `NeuralPlayground-0.0.4/neuralplayground/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/config/load_config.py` & `NeuralPlayground-0.0.4/neuralplayground/config/load_config.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/config/main_config.py` & `NeuralPlayground-0.0.4/neuralplayground/config/main_config.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/config/plot_config.py` & `NeuralPlayground-0.0.4/neuralplayground/config/plot_config.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/datasets.py` & `NeuralPlayground-0.0.4/neuralplayground/datasets.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/experiments/README.md` & `NeuralPlayground-0.0.4/neuralplayground/experiments/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/experiments/hafting_2008_data.py` & `NeuralPlayground-0.0.4/neuralplayground/experiments/hafting_2008_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/experiments/sargolini_2006_data.py` & `NeuralPlayground-0.0.4/neuralplayground/experiments/sargolini_2006_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/experiments/wernle_2018_data.py` & `NeuralPlayground-0.0.4/neuralplayground/experiments/wernle_2018_data.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/plotting/plot_utils.py` & `NeuralPlayground-0.0.4/neuralplayground/plotting/plot_utils.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/neuralplayground/utils.py` & `NeuralPlayground-0.0.4/neuralplayground/utils.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/pyproject.toml` & `NeuralPlayground-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
   "ipython",
   "matplotlib",
   "deepdiff",
   "opencv-python",
   "gymnasium",
   "scikit-image",
   "pooch",
+  "colorama",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ClementineDomine/NeuralPlayground"
 "Bug tracker" = "https://github.com/ClementineDomine/NeuralPlayground/issues"
 "Documentation" = "https://github.com/ClementineDomine/NeuralPlayground"
 "Source code" = "https://github.com/ClementineDomine/NeuralPlayground"
```

### Comparing `NeuralPlayground-0.0.3/tests/README.md` & `NeuralPlayground-0.0.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/tests/agent_test.py` & `NeuralPlayground-0.0.4/tests/agent_test.py`

 * *Files identical despite different names*

### Comparing `NeuralPlayground-0.0.3/tests/arena_exp_test.py` & `NeuralPlayground-0.0.4/tests/arena_exp_test.py`

 * *Files identical despite different names*

