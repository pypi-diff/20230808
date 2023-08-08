# Comparing `tmp/popgym-1.0.2.tar.gz` & `tmp/popgym-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popgym-1.0.2.tar", last modified: Sun Apr  9 17:17:30 2023, max compression
+gzip compressed data, was "popgym-1.0.3.tar", last modified: Tue Aug  8 14:24:46 2023, max compression
```

## Comparing `popgym-1.0.2.tar` & `popgym-1.0.3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.196375 popgym-1.0.2/
--rw-r--r--   0 smorad     (501) staff       (20)     1069 2023-01-26 13:50:44.000000 popgym-1.0.2/LICENSE.md
--rw-r--r--   0 smorad     (501) staff       (20)     7729 2023-04-09 17:17:30.196493 popgym-1.0.2/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     7375 2023-04-09 16:55:40.000000 popgym-1.0.2/README.md
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.180017 popgym-1.0.2/popgym/
--rw-r--r--   0 smorad     (501) staff       (20)       73 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.181192 popgym-1.0.2/popgym/baselines/
--rw-r--r--   0 smorad     (501) staff       (20)       85 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/__init__.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.182964 popgym-1.0.2/popgym/baselines/models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.2/popgym/baselines/models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)      992 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/aggregations.py
--rw-r--r--   0 smorad     (501) staff       (20)     9855 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/embeddings.py
--rw-r--r--   0 smorad     (501) staff       (20)     1834 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/baselines/models/fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2046 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     2450 2022-09-22 16:05:05.000000 popgym-1.0.2/popgym/baselines/models/linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)    10069 2022-09-27 16:44:40.000000 popgym-1.0.2/popgym/baselines/models/lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)    60700 2022-10-08 11:28:47.000000 popgym-1.0.2/popgym/baselines/models/s4d.py
--rw-r--r--   0 smorad     (501) staff       (20)     7318 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/baselines/ppo.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.186283 popgym-1.0.2/popgym/baselines/ray_models/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.2/popgym/baselines/ray_models/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)    12303 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/base_model.py
--rw-r--r--   0 smorad     (501) staff       (20)     5407 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_diffnc.py
--rw-r--r--   0 smorad     (501) staff       (20)     2367 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_elman.py
--rw-r--r--   0 smorad     (501) staff       (20)     2343 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_frameconv.py
--rw-r--r--   0 smorad     (501) staff       (20)     3689 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_framestack.py
--rw-r--r--   0 smorad     (501) staff       (20)     3543 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_fwp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2493 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_gru.py
--rw-r--r--   0 smorad     (501) staff       (20)     2359 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_indrnn.py
--rw-r--r--   0 smorad     (501) staff       (20)     3772 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_linear_attention.py
--rw-r--r--   0 smorad     (501) staff       (20)     2269 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_lmu.py
--rw-r--r--   0 smorad     (501) staff       (20)     2617 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_lstm.py
--rw-r--r--   0 smorad     (501) staff       (20)     1441 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_mlp.py
--rw-r--r--   0 smorad     (501) staff       (20)     2704 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/baselines/ray_models/ray_s4d.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.187461 popgym-1.0.2/popgym/core/
--rw-r--r--   0 smorad     (501) staff       (20)       56 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/core/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     9714 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      863 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/env.py
--rw-r--r--   0 smorad     (501) staff       (20)     5507 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/maze.py
--rw-r--r--   0 smorad     (501) staff       (20)      590 2023-01-26 13:50:44.000000 popgym-1.0.2/popgym/core/observability.py
--rw-r--r--   0 smorad     (501) staff       (20)      785 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/core/wrapper.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.190517 popgym-1.0.2/popgym/envs/
--rw-r--r--   0 smorad     (501) staff       (20)     9576 2023-04-09 16:59:46.000000 popgym-1.0.2/popgym/envs/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3594 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)     5123 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     6837 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     5489 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     3526 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     2072 2023-04-09 16:52:16.000000 popgym-1.0.2/popgym/envs/labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     2419 2023-04-09 16:52:13.000000 popgym-1.0.2/popgym/envs/labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     4742 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)     2357 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)     1625 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/noisy_stateless_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     1597 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/envs/noisy_stateless_pendulum.py
--rw-r--r--   0 smorad     (501) staff       (20)     2465 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     3060 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     2860 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/stateless_cartpole.py
--rw-r--r--   0 smorad     (501) staff       (20)     2622 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/envs/stateless_pendulum.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.190824 popgym-1.0.2/popgym/util/
--rw-r--r--   0 smorad     (501) staff       (20)       33 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/util/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     6140 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/util/benchmark.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.192227 popgym-1.0.2/popgym/wrappers/
--rw-r--r--   0 smorad     (501) staff       (20)      313 2023-03-11 17:40:45.000000 popgym-1.0.2/popgym/wrappers/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3459 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/antialias.py
--rw-r--r--   0 smorad     (501) staff       (20)     3008 2023-03-09 21:24:36.000000 popgym-1.0.2/popgym/wrappers/flatten.py
--rw-r--r--   0 smorad     (501) staff       (20)     2109 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/markovian.py
--rw-r--r--   0 smorad     (501) staff       (20)     5570 2023-03-08 15:29:35.000000 popgym-1.0.2/popgym/wrappers/previous_action.py
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.180790 popgym-1.0.2/popgym.egg-info/
--rw-r--r--   0 smorad     (501) staff       (20)     7729 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/PKG-INFO
--rw-r--r--   0 smorad     (501) staff       (20)     2488 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/SOURCES.txt
--rw-r--r--   0 smorad     (501) staff       (20)        1 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/dependency_links.txt
--rw-r--r--   0 smorad     (501) staff       (20)      103 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/requires.txt
--rw-r--r--   0 smorad     (501) staff       (20)       13 2023-04-09 17:17:30.000000 popgym-1.0.2/popgym.egg-info/top_level.txt
--rw-r--r--   0 smorad     (501) staff       (20)       80 2023-01-26 13:50:44.000000 popgym-1.0.2/pyproject.toml
--rw-r--r--   0 smorad     (501) staff       (20)      652 2023-04-09 17:17:30.196885 popgym-1.0.2/setup.cfg
-drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-04-09 17:17:30.196203 popgym-1.0.2/tests/
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/__init__.py
--rw-r--r--   0 smorad     (501) staff       (20)     3391 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/base_env_test.py
--rw-r--r--   0 smorad     (501) staff       (20)      907 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/compute_framerate.py
--rw-r--r--   0 smorad     (501) staff       (20)      351 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/notest_bipedal_walker.py
--rw-r--r--   0 smorad     (501) staff       (20)     1013 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_autoencode.py
--rw-r--r--   0 smorad     (501) staff       (20)      217 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_bandits.py
--rw-r--r--   0 smorad     (501) staff       (20)     3216 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_battleship.py
--rw-r--r--   0 smorad     (501) staff       (20)     4160 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_concentration.py
--rw-r--r--   0 smorad     (501) staff       (20)     1602 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_count_recall.py
--rw-r--r--   0 smorad     (501) staff       (20)     2091 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/test_deck.py
--rw-r--r--   0 smorad     (501) staff       (20)      267 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_envs.py
--rw-r--r--   0 smorad     (501) staff       (20)      909 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_higher_lower.py
--rw-r--r--   0 smorad     (501) staff       (20)     1637 2023-04-09 16:58:11.000000 popgym-1.0.2/tests/test_labyrinth_escape.py
--rw-r--r--   0 smorad     (501) staff       (20)     2068 2023-04-09 16:58:11.000000 popgym-1.0.2/tests/test_labyrinth_explore.py
--rw-r--r--   0 smorad     (501) staff       (20)     1570 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_minesweeper.py
--rw-r--r--   0 smorad     (501) staff       (20)      972 2023-03-08 15:29:35.000000 popgym-1.0.2/tests/test_multiarmed_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.2/tests/test_nonstationary_bandit.py
--rw-r--r--   0 smorad     (501) staff       (20)      674 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_repeat_first.py
--rw-r--r--   0 smorad     (501) staff       (20)     1936 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_repeat_previous.py
--rw-r--r--   0 smorad     (501) staff       (20)     3660 2023-03-11 17:40:45.000000 popgym-1.0.2/tests/test_wrappers.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.709656 popgym-1.0.3/
+-rw-r--r--   0 smorad     (501) staff       (20)     1069 2023-01-26 13:50:44.000000 popgym-1.0.3/LICENSE.md
+-rw-r--r--   0 smorad     (501) staff       (20)     7745 2023-08-08 14:24:46.709774 popgym-1.0.3/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     7391 2023-06-12 09:32:13.000000 popgym-1.0.3/README.md
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.693825 popgym-1.0.3/popgym/
+-rw-r--r--   0 smorad     (501) staff       (20)       73 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.695367 popgym-1.0.3/popgym/baselines/
+-rw-r--r--   0 smorad     (501) staff       (20)       85 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/__init__.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.697048 popgym-1.0.3/popgym/baselines/models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.3/popgym/baselines/models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)      992 2022-09-22 16:05:05.000000 popgym-1.0.3/popgym/baselines/models/aggregations.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9855 2022-09-22 16:05:05.000000 popgym-1.0.3/popgym/baselines/models/embeddings.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2702 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/baselines/models/fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2046 2022-09-22 16:05:05.000000 popgym-1.0.3/popgym/baselines/models/indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3214 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/baselines/models/linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)    10069 2022-09-27 16:44:40.000000 popgym-1.0.3/popgym/baselines/models/lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)    60700 2022-10-08 11:28:47.000000 popgym-1.0.3/popgym/baselines/models/s4d.py
+-rw-r--r--   0 smorad     (501) staff       (20)     7441 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/baselines/ppo.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.699711 popgym-1.0.3/popgym/baselines/ray_models/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2023-03-08 13:39:50.000000 popgym-1.0.3/popgym/baselines/ray_models/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)    12303 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/base_model.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5407 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_diffnc.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2367 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_elman.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2343 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_frameconv.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3689 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_framestack.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5019 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_fwp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2493 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_gru.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2359 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_indrnn.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5368 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_linear_attention.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2269 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_lmu.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2617 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_lstm.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1441 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_mlp.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2704 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/baselines/ray_models/ray_s4d.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.700922 popgym-1.0.3/popgym/core/
+-rw-r--r--   0 smorad     (501) staff       (20)       56 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/core/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     9714 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/core/deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      863 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/core/env.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5507 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/core/maze.py
+-rw-r--r--   0 smorad     (501) staff       (20)      590 2023-01-26 13:50:44.000000 popgym-1.0.3/popgym/core/observability.py
+-rw-r--r--   0 smorad     (501) staff       (20)      785 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/core/wrapper.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.703769 popgym-1.0.3/popgym/envs/
+-rw-r--r--   0 smorad     (501) staff       (20)     9576 2023-06-12 09:32:13.000000 popgym-1.0.3/popgym/envs/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3594 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5123 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6837 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5489 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3526 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2072 2023-04-09 16:52:16.000000 popgym-1.0.3/popgym/envs/labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2419 2023-04-09 16:52:13.000000 popgym-1.0.3/popgym/envs/labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4742 2023-08-01 16:49:39.000000 popgym-1.0.3/popgym/envs/minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2357 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/envs/multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1625 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/envs/noisy_stateless_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1597 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/envs/noisy_stateless_pendulum.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2465 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3060 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2860 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/stateless_cartpole.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2622 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/envs/stateless_pendulum.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.704060 popgym-1.0.3/popgym/util/
+-rw-r--r--   0 smorad     (501) staff       (20)       33 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/util/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     6140 2023-03-11 17:40:45.000000 popgym-1.0.3/popgym/util/benchmark.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.705612 popgym-1.0.3/popgym/wrappers/
+-rw-r--r--   0 smorad     (501) staff       (20)      390 2023-08-08 13:48:45.000000 popgym-1.0.3/popgym/wrappers/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3459 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/wrappers/antialias.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1756 2023-08-08 14:12:01.000000 popgym-1.0.3/popgym/wrappers/discrete_action.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3145 2023-08-01 16:47:26.000000 popgym-1.0.3/popgym/wrappers/flatten.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2109 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/wrappers/markovian.py
+-rw-r--r--   0 smorad     (501) staff       (20)     5570 2023-03-08 15:29:35.000000 popgym-1.0.3/popgym/wrappers/previous_action.py
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.694978 popgym-1.0.3/popgym.egg-info/
+-rw-r--r--   0 smorad     (501) staff       (20)     7745 2023-08-08 14:24:46.000000 popgym-1.0.3/popgym.egg-info/PKG-INFO
+-rw-r--r--   0 smorad     (501) staff       (20)     2523 2023-08-08 14:24:46.000000 popgym-1.0.3/popgym.egg-info/SOURCES.txt
+-rw-r--r--   0 smorad     (501) staff       (20)        1 2023-08-08 14:24:46.000000 popgym-1.0.3/popgym.egg-info/dependency_links.txt
+-rw-r--r--   0 smorad     (501) staff       (20)      103 2023-08-08 14:24:46.000000 popgym-1.0.3/popgym.egg-info/requires.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       13 2023-08-08 14:24:46.000000 popgym-1.0.3/popgym.egg-info/top_level.txt
+-rw-r--r--   0 smorad     (501) staff       (20)       80 2023-01-26 13:50:44.000000 popgym-1.0.3/pyproject.toml
+-rw-r--r--   0 smorad     (501) staff       (20)      652 2023-08-08 14:24:46.710206 popgym-1.0.3/setup.cfg
+drwxr-xr-x   0 smorad     (501) staff       (20)        0 2023-08-08 14:24:46.709305 popgym-1.0.3/tests/
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.3/tests/__init__.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3391 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/base_env_test.py
+-rw-r--r--   0 smorad     (501) staff       (20)      907 2022-09-22 16:05:05.000000 popgym-1.0.3/tests/compute_framerate.py
+-rw-r--r--   0 smorad     (501) staff       (20)      351 2022-09-22 16:05:05.000000 popgym-1.0.3/tests/notest_bipedal_walker.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1013 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_autoencode.py
+-rw-r--r--   0 smorad     (501) staff       (20)      217 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_bandits.py
+-rw-r--r--   0 smorad     (501) staff       (20)     3216 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_battleship.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4160 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_concentration.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1602 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_count_recall.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2091 2022-09-22 16:05:05.000000 popgym-1.0.3/tests/test_deck.py
+-rw-r--r--   0 smorad     (501) staff       (20)      267 2023-03-11 17:40:45.000000 popgym-1.0.3/tests/test_envs.py
+-rw-r--r--   0 smorad     (501) staff       (20)      909 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_higher_lower.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1637 2023-06-12 09:32:13.000000 popgym-1.0.3/tests/test_labyrinth_escape.py
+-rw-r--r--   0 smorad     (501) staff       (20)     2068 2023-06-12 09:32:13.000000 popgym-1.0.3/tests/test_labyrinth_explore.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1570 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_minesweeper.py
+-rw-r--r--   0 smorad     (501) staff       (20)      972 2023-03-08 15:29:35.000000 popgym-1.0.3/tests/test_multiarmed_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)        0 2022-09-22 16:05:05.000000 popgym-1.0.3/tests/test_nonstationary_bandit.py
+-rw-r--r--   0 smorad     (501) staff       (20)      674 2023-03-11 17:40:45.000000 popgym-1.0.3/tests/test_repeat_first.py
+-rw-r--r--   0 smorad     (501) staff       (20)     1936 2023-03-11 17:40:45.000000 popgym-1.0.3/tests/test_repeat_previous.py
+-rw-r--r--   0 smorad     (501) staff       (20)     4080 2023-08-08 14:10:20.000000 popgym-1.0.3/tests/test_wrappers.py
```

### Comparing `popgym-1.0.2/LICENSE.md` & `popgym-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/PKG-INFO` & `popgym-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: popgym
-Version: 1.0.2
-Summary: A collection of partially-observable procedural gym environments
-Author: Steven Morad
-License: MIT
-Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
-Description-Content-Type: text/markdown
-Provides-Extra: navigation
-Provides-Extra: baselines
-License-File: LICENSE.md
-
 # POPGym: Partially Observable Process Gym
 ![tests](https://github.com/smorad/popgym/actions/workflows/python-app.yml/badge.svg)
 [![codecov](https://codecov.io/gh/smorad/popgym/branch/master/graph/badge.svg?token=I47IDFZXSV)](https://codecov.io/gh/smorad/popgym)
 
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. 
 
 ## Quickstart Install
@@ -22,15 +10,15 @@
 pip install popgym # base environments only, only requires numpy and gymnasium
 pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
-POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
+POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnaisum) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
 |---------------------------------------------------------------------------------------------------------|-------------------|-------------------|-------------------|---------------------------|
 | [Battleship](#battleship) [(Code)](popgym/envs/battleship.py)                                           |Game               |None               |  117,158          |  235,402                  |
 | [Concentration](#concentration) [(Code)](popgym/envs/concentration.py)                                  |Game               |Weak               |  47,515           |  157,217                  |
 | [Higher Lower](#higher-lower) [(Code)](popgym/envs/higher_lower.py)                                     |Game, Noisy        |None               |  24,312           |  76,903                   |
 | [Labyrinth Escape](#labyrinth-escape) [(Code)](popgym/envs/labyrinth_escape.py)                         |Navigation         |Strong             |  1,399            |  41,122                   |
```

### Comparing `popgym-1.0.2/README.md` & `popgym-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: popgym
+Version: 1.0.3
+Summary: A collection of partially-observable procedural gym environments
+Author: Steven Morad
+License: MIT
+Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
+Description-Content-Type: text/markdown
+Provides-Extra: navigation
+Provides-Extra: baselines
+License-File: LICENSE.md
+
 # POPGym: Partially Observable Process Gym
 ![tests](https://github.com/smorad/popgym/actions/workflows/python-app.yml/badge.svg)
 [![codecov](https://codecov.io/gh/smorad/popgym/branch/master/graph/badge.svg?token=I47IDFZXSV)](https://codecov.io/gh/smorad/popgym)
 
 POPGym is designed to benchmark memory in deep reinforcement learning. It contains a set of [environments](#popgym-environments) and a collection of [memory model baselines](#popgym-baselines). The full paper is available on [OpenReview](https://openreview.net/forum?id=chDrutUTs0K). Please see the [documentation](https://popgym.readthedocs.io/en/latest/) for advanced installation instructions and examples. 
 
 ## Quickstart Install
@@ -10,15 +22,15 @@
 pip install popgym # base environments only, only requires numpy and gymnasium
 pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
-POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
+POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnaisum) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
 |---------------------------------------------------------------------------------------------------------|-------------------|-------------------|-------------------|---------------------------|
 | [Battleship](#battleship) [(Code)](popgym/envs/battleship.py)                                           |Game               |None               |  117,158          |  235,402                  |
 | [Concentration](#concentration) [(Code)](popgym/envs/concentration.py)                                  |Game               |Weak               |  47,515           |  157,217                  |
 | [Higher Lower](#higher-lower) [(Code)](popgym/envs/higher_lower.py)                                     |Game, Noisy        |None               |  24,312           |  76,903                   |
 | [Labyrinth Escape](#labyrinth-escape) [(Code)](popgym/envs/labyrinth_escape.py)                         |Navigation         |Strong             |  1,399            |  41,122                   |
```

### Comparing `popgym-1.0.2/popgym/baselines/models/aggregations.py` & `popgym-1.0.3/popgym/baselines/models/aggregations.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/models/embeddings.py` & `popgym-1.0.3/popgym/baselines/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/models/fwp.py` & `popgym-1.0.3/popgym/baselines/models/fwp.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,38 +5,56 @@
 
 
 class FWPBlock(nn.Module):
     """
     The building block in the fast weight transformers paper. This is
     a form of linear transformer.
 
+    Note that this is a "simplified" version of FWP without the delta
+    update rule and DPFP. We use ReLU instead of DPFP.
+
     Inputs:
         input_size: Size of input feature dim
         hidden_size: Size of key/query/value space
         aggregator: Which type of aggregation to use
         sum_normalization: Whether to use the sum normalization described
             in the paper
+        feed_forward: Whether to apply a perceptron to the output
+        residual: Whether to apply a residual connection from input to output
     """
 
     def __init__(
         self,
         input_size,
         hidden_size,
         aggregator="sum",
         sum_normalization=True,
+        feed_forward=True,
+        residual=True,
     ):
         super().__init__()
         self.key = nn.Linear(input_size, hidden_size, bias=False)
         self.query = nn.Linear(input_size, hidden_size, bias=False)
         self.value = nn.Linear(input_size, hidden_size, bias=False)
         self.norm = nn.LayerNorm(input_size)
         self.sum_normalization = sum_normalization
+        self.feed_forward = feed_forward
+        self.residual = residual
         self.aggregator = get_aggregator(aggregator)(
             max_len=1024, d_model=hidden_size**2
         )
+        if self.feed_forward:
+            self.ff = nn.Sequential(
+                nn.Linear(hidden_size, hidden_size),
+                nn.ReLU(inplace=True),
+                nn.Linear(hidden_size, hidden_size),
+                nn.ReLU(inplace=True)
+            )
+        if self.residual:
+            self.shortcut = nn.Linear(input_size, hidden_size)
 
     def forward(self, x: torch.Tensor, state: torch.Tensor) -> torch.Tensor:
         """
         Inputs:
             x: [B, T, F]
             state: [B, 1, F]
         Outputs:
@@ -51,9 +69,14 @@
             K = K / (1e-5 + K.sum(dim=-1, keepdim=True))
             Q = Q / (1e-5 + Q.sum(dim=-1, keepdim=True))
 
         kv = torch.einsum("bti, btj -> btij", V, K)
         shape = kv.shape
         state = self.aggregator(kv.flatten(-2), state.flatten(-2)).reshape(shape)
 
-        y = torch.einsum("btij, bti -> btj", state, Q)
+        y = torch.einsum("btij, btj -> bti", state, Q)
+        if self.feed_forward:
+            y = self.ff(y)
+
+        if self.residual:
+            y = y + self.shortcut(x)
         return y, state
```

### Comparing `popgym-1.0.2/popgym/baselines/models/indrnn.py` & `popgym-1.0.3/popgym/baselines/models/indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/models/linear_attention.py` & `popgym-1.0.3/popgym/baselines/models/linear_attention.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,31 +17,47 @@
     a form of linear transformer.
 
     Inputs:
         input_size: Size of input feature dim
         hidden_size: Size of key/query/value space
         S_aggregator: Which type of aggregation to use for the numerator (S term)
         Z_aggregator: Which type of aggregation to use for the denominator (Z term)
+        feed_forward: Whether to apply a perceptron to the output
+        residual: Whether to apply a residual connection from input to output
     """
 
     def __init__(
         self,
         input_size: int,
         hidden_size: int,
         S_aggregator: str = "sum",
         Z_aggregator: str = "sum",
+        feed_forward=True,
+        residual=True,
     ):
         super().__init__()
         self.key = nn.Linear(input_size, hidden_size, bias=False)
         self.query = nn.Linear(input_size, hidden_size, bias=False)
         self.value = nn.Linear(input_size, hidden_size, bias=False)
         self.norm = nn.LayerNorm(input_size)
         self.phi = Phi()
         self.S_aggregator = get_aggregator(S_aggregator)()
         self.Z_aggregator = get_aggregator(Z_aggregator)()
+        self.feed_forward = feed_forward
+        self.residual = residual
+
+        if self.feed_forward:
+            self.ff = nn.Sequential(
+                nn.Linear(hidden_size, hidden_size),
+                nn.ReLU(inplace=True),
+                nn.Linear(hidden_size, hidden_size),
+                nn.ReLU(inplace=True)
+            )
+        if self.residual:
+            self.shortcut = nn.Linear(input_size, hidden_size)
 
     def forward(
         self, x: torch.Tensor, state: List[torch.Tensor]
     ) -> Tuple[torch.Tensor, List[torch.Tensor]]:
         """
         Input:
             x: [B, T, F]
@@ -74,10 +90,16 @@
         # numerator = Q^T S
         numerator = torch.einsum("bti, btil -> btl", Q, S)
         # denominator = Q^T Z
         denominator = torch.einsum("bti, btl -> bt", Q, Z).reshape(B, T, 1) + 1e-5
         # output = (Q^T S) / (Q^T Z)
         output = numerator / denominator
 
+        if self.feed_forward:
+            output = self.ff(output)
+
+        if self.residual:
+            output = output + self.shortcut(x)
+
         state = [S, Z]
 
         return output, state
```

### Comparing `popgym-1.0.2/popgym/baselines/models/lmu.py` & `popgym-1.0.3/popgym/baselines/models/lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/models/s4d.py` & `popgym-1.0.3/popgym/baselines/models/s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ppo.py` & `popgym-1.0.3/popgym/baselines/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 
 import popgym  # noqa: F401
 from popgym import wrappers
 from popgym.baselines.ray_models.ray_diffnc import DiffNC  # noqa: F401
 from popgym.baselines.ray_models.ray_elman import Elman
 from popgym.baselines.ray_models.ray_frameconv import Frameconv
 from popgym.baselines.ray_models.ray_framestack import Framestack
-from popgym.baselines.ray_models.ray_fwp import FastWeightProgrammer
+from popgym.baselines.ray_models.ray_fwp import (
+    DeepFastWeightProgrammer,
+    FastWeightProgrammer,
+)
 from popgym.baselines.ray_models.ray_gru import GRU
 from popgym.baselines.ray_models.ray_indrnn import IndRNN
-from popgym.baselines.ray_models.ray_linear_attention import LinearAttention
+from popgym.baselines.ray_models.ray_linear_attention import LinearAttention, DeepLinearAttention
 from popgym.baselines.ray_models.ray_lmu import LMU
 from popgym.baselines.ray_models.ray_lstm import LSTM
 from popgym.baselines.ray_models.ray_mlp import MLP, BasicMLP
 from popgym.baselines.ray_models.ray_s4d import S4D
 from popgym.core.env import POPGymEnv
 
 
 def main():
     env_names: List[Any] = []
 
-    env_types = os.environ.get("POPGYM_EXPERIMENT", "ALL_ENVS")
+    env_types = os.environ.get("POPGYM_EXPERIMENT", "ALL")
     desired_models = os.environ.get("POPGYM_MODELS", "ALL")
     num_splits = int(os.environ.get("POPGYM_NUM_SPLITS", 1))
     split_id = int(os.environ.get("POPGYM_SPLIT_ID", 0))
     project_id = os.environ.get("POPGYM_PROJECT", "popgym-debug")
     gpu_per_worker = float(os.environ.get("POPGYM_GPU", 0.25))
-    max_steps = int(os.environ.get("POPGYM_STEPS", 10e6))
+    max_steps = int(os.environ.get("POPGYM_STEPS", 15e6))
     storage_path = os.environ.get("POPGYM_STORAGE", "/tmp/ray_results")
     num_samples = int(os.environ.get("POPGYM_SAMPLES", 1))
 
     # Used for testing
     # Maximum episode length and backprop thru time truncation length
     bptt_cutoff = int(os.environ.get("POPGYM_BPTT_CUTOFF", 1024))
     num_workers = int(os.environ.get("POPGYM_WORKERS", 4))
@@ -52,39 +55,41 @@
     h_memory = 256
     train_batch_size = bptt_cutoff * max(num_workers, 1) * num_envs_per_worker
 
     def wrap(env: POPGymEnv) -> POPGymEnv:
         return wrappers.Antialias(wrappers.PreviousAction(env))
 
     # Register all envs with ray
-    envs = popgym.ALL_ENVS
+    envs = popgym.envs.ALL
     for cls, info in envs.items():
         env_name = info["id"]
         register_env(env_name, lambda x: wrap(cls()))
 
     # Of the registered envs, pick out the ones we actually want to run
     env_names = []
     for e in env_types.split(","):
         # getattr will either return a dict of {class: info[name}}
         # or just a class
-        res = getattr(popgym, e)
+        res = getattr(popgym.envs, e)
         if isinstance(res, dict):
             desired_envs = list(res.keys())
         else:
             desired_envs = [res]
 
         for d in desired_envs:
             env_names.append(envs[d]["id"])
 
     env_names = env_names[split_id::num_splits]
 
     # Setup the models we want to train
     attn_models = [
         LinearAttention,
         FastWeightProgrammer,
+        DeepFastWeightProgrammer,
+        DeepLinearAttention,
     ]
     rnn_models = [LSTM, GRU, Elman, LMU, IndRNN, DiffNC]
     conv_models = [S4D]
     basic_models = [
         BasicMLP,
         MLP,
         Framestack,
```

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/base_model.py` & `popgym-1.0.3/popgym/baselines/ray_models/base_model.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_diffnc.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_diffnc.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_elman.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_elman.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_frameconv.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_frameconv.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_framestack.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_framestack.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_gru.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_gru.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_indrnn.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_indrnn.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_lmu.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_lmu.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_lstm.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_lstm.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_mlp.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_mlp.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/baselines/ray_models/ray_s4d.py` & `popgym-1.0.3/popgym/baselines/ray_models/ray_s4d.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/core/deck.py` & `popgym-1.0.3/popgym/core/deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/core/env.py` & `popgym-1.0.3/popgym/core/env.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/core/maze.py` & `popgym-1.0.3/popgym/core/maze.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/core/observability.py` & `popgym-1.0.3/popgym/core/observability.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/core/wrapper.py` & `popgym-1.0.3/popgym/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/__init__.py` & `popgym-1.0.3/popgym/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/autoencode.py` & `popgym-1.0.3/popgym/envs/autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/battleship.py` & `popgym-1.0.3/popgym/envs/battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/concentration.py` & `popgym-1.0.3/popgym/envs/concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/count_recall.py` & `popgym-1.0.3/popgym/envs/count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/higher_lower.py` & `popgym-1.0.3/popgym/envs/higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/labyrinth_escape.py` & `popgym-1.0.3/popgym/envs/labyrinth_escape.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/labyrinth_explore.py` & `popgym-1.0.3/popgym/envs/labyrinth_explore.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/minesweeper.py` & `popgym-1.0.3/popgym/envs/minesweeper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/multiarmed_bandit.py` & `popgym-1.0.3/popgym/envs/multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/noisy_stateless_cartpole.py` & `popgym-1.0.3/popgym/envs/noisy_stateless_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/noisy_stateless_pendulum.py` & `popgym-1.0.3/popgym/envs/noisy_stateless_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/repeat_first.py` & `popgym-1.0.3/popgym/envs/repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/repeat_previous.py` & `popgym-1.0.3/popgym/envs/repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/stateless_cartpole.py` & `popgym-1.0.3/popgym/envs/stateless_cartpole.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/envs/stateless_pendulum.py` & `popgym-1.0.3/popgym/envs/stateless_pendulum.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/util/benchmark.py` & `popgym-1.0.3/popgym/util/benchmark.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/wrappers/antialias.py` & `popgym-1.0.3/popgym/wrappers/antialias.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/wrappers/flatten.py` & `popgym-1.0.3/popgym/wrappers/flatten.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-from gettext import npgettext
 from typing import Tuple
+
 import gymnasium as gym
+import numpy as np
 from gymnasium.core import ActType, ObsType
+
 from popgym.core.env import POPGymEnv
 from popgym.core.wrapper import POPGymWrapper
-import numpy as np
+
 
 class Flatten(POPGymWrapper):
     """
     Wrapper that flattens the observation and action spaces
     to make them compatible with neural networks.
     """
 
-    def __init__(self, env: POPGymEnv, flatten_action: bool=True, flatten_observation: bool=True):
+    def __init__(
+        self,
+        env: POPGymEnv,
+        flatten_action: bool = True,
+        flatten_observation: bool = True,
+    ):
         super().__init__(env)
         self.need_flatten_action = False
         self.need_flatten_obs = False
         if flatten_action:
             # Check that spaces are either all continuous or all discrete
             self.continuous(self.env.action_space)
-            self.need_flatten_action = isinstance(self.env.action_space, gym.spaces.Tuple) or isinstance(self.env.action_space, gym.spaces.Dict)
+            self.need_flatten_action = isinstance(
+                self.env.action_space, gym.spaces.Tuple
+            ) or isinstance(self.env.action_space, gym.spaces.Dict)
             if self.need_flatten_action:
-                self.action_space = gym.spaces.utils.flatten_space(self.env.action_space)
+                self.action_space = gym.spaces.utils.flatten_space(
+                    self.env.action_space
+                )
         if flatten_observation:
-            self.continuous(self.env.observation_space)
-            self.need_flatten_obs = isinstance(self.env.action_space, gym.spaces.Tuple) or isinstance(self.env.action_space, gym.spaces.Dict)
+            self.need_flatten_obs = isinstance(
+                self.env.observation_space, gym.spaces.Tuple
+            ) or isinstance(self.env.observation_space, gym.spaces.Dict)
             if self.need_flatten_obs:
-                self.observation_space = gym.spaces.utils.flatten_space(self.env.observation_space)
+                self.observation_space = gym.spaces.utils.flatten_space(
+                    self.env.observation_space
+                )
 
-    
     def step(self, action: ActType) -> Tuple[ObsType, float, bool, bool, dict]:
         if self.need_flatten_action:
             flat_action = gym.spaces.utils.unflatten(self.env.action_space, action)
         else:
             flat_action = action
 
         obs, reward, terminated, truncated, info = self.env.step(flat_action)
@@ -49,19 +62,22 @@
 
     def continuous(self, space: gym.spaces.Space) -> bool:
         if isinstance(space, gym.spaces.Box):
             if np.issubdtype(space.dtype, np.integer):
                 return False
             else:
                 return True
-        elif isinstance(space, (gym.spaces.Discrete, gym.spaces.MultiDiscrete, gym.spaces.MultiBinary)):
+        elif isinstance(
+            space,
+            (gym.spaces.Discrete, gym.spaces.MultiDiscrete, gym.spaces.MultiBinary),
+        ):
             return False
         elif isinstance(space, gym.spaces.Tuple):
             res = [self.continuous(s) for s in space.spaces]
             assert all(res) or not any(res), "Cannot mix continuous and discrete spaces"
             return any(res)
         elif isinstance(space, gym.spaces.Dict):
             res = [self.continuous(s) for s in space.spaces.values()]
             assert all(res) or not any(res), "Cannot mix continuous and discrete spaces"
             return any(res)
         else:
-            raise NotImplementedError(f"Unknown space: {space}")
+            raise NotImplementedError(f"Unknown space: {space}")
```

### Comparing `popgym-1.0.2/popgym/wrappers/markovian.py` & `popgym-1.0.3/popgym/wrappers/markovian.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym/wrappers/previous_action.py` & `popgym-1.0.3/popgym/wrappers/previous_action.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/popgym.egg-info/PKG-INFO` & `popgym-1.0.3/popgym.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popgym
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of partially-observable procedural gym environments
 Author: Steven Morad
 License: MIT
 Keywords: gym,gymnasium,pomdp,partially observable,reinforcement learning,rl
 Description-Content-Type: text/markdown
 Provides-Extra: navigation
 Provides-Extra: baselines
@@ -22,15 +22,15 @@
 pip install popgym # base environments only, only requires numpy and gymnasium
 pip install "popgym[navigation]" # also include navigation environments, which require mazelib
 pip install "popgym[baselines]" # environments and memory baselines
 ```
 
 ## POPGym Environments
 
-POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Openai Gym](https://github.com/openai/gym) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
+POPGym contains Partially Observable Markov Decision Process (POMDP) environments following the [Gymnasium](https://github.com/Farama-Foundation/Gymnaisum) interface. POPGym environments have minimal dependencies and fast enough to solve on a laptop CPU in less than a day. We provide the following environments:
 
 | Environment                                                                                             |         Tags      | Temporal Ordering | Colab FPS         | Macbook Air (2020) FPS    |
 |---------------------------------------------------------------------------------------------------------|-------------------|-------------------|-------------------|---------------------------|
 | [Battleship](#battleship) [(Code)](popgym/envs/battleship.py)                                           |Game               |None               |  117,158          |  235,402                  |
 | [Concentration](#concentration) [(Code)](popgym/envs/concentration.py)                                  |Game               |Weak               |  47,515           |  157,217                  |
 | [Higher Lower](#higher-lower) [(Code)](popgym/envs/higher_lower.py)                                     |Game, Noisy        |None               |  24,312           |  76,903                   |
 | [Labyrinth Escape](#labyrinth-escape) [(Code)](popgym/envs/labyrinth_escape.py)                         |Navigation         |Strong             |  1,399            |  41,122                   |
```

### Comparing `popgym-1.0.2/popgym.egg-info/SOURCES.txt` & `popgym-1.0.3/popgym.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 popgym/envs/repeat_previous.py
 popgym/envs/stateless_cartpole.py
 popgym/envs/stateless_pendulum.py
 popgym/util/__init__.py
 popgym/util/benchmark.py
 popgym/wrappers/__init__.py
 popgym/wrappers/antialias.py
+popgym/wrappers/discrete_action.py
 popgym/wrappers/flatten.py
 popgym/wrappers/markovian.py
 popgym/wrappers/previous_action.py
 tests/__init__.py
 tests/base_env_test.py
 tests/compute_framerate.py
 tests/notest_bipedal_walker.py
```

### Comparing `popgym-1.0.2/setup.cfg` & `popgym-1.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = popgym
 description = A collection of partially-observable procedural gym environments
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Steven Morad
-version = 1.0.2
+version = 1.0.3
 license = MIT
 readme = README.md
-requires-python = >=3.7 <=3.10 # Remove 3.10 limit when mazelib fixes its build process
+requires_python = >=3.7 <=3.10 # Remove 3.10 limit when mazelib fixes its build process
 keywords = gym, gymnasium, pomdp, partially observable, reinforcement learning, rl
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	gymnasium
```

### Comparing `popgym-1.0.2/tests/base_env_test.py` & `popgym-1.0.3/tests/base_env_test.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/compute_framerate.py` & `popgym-1.0.3/tests/compute_framerate.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_autoencode.py` & `popgym-1.0.3/tests/test_autoencode.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_battleship.py` & `popgym-1.0.3/tests/test_battleship.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_concentration.py` & `popgym-1.0.3/tests/test_concentration.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_count_recall.py` & `popgym-1.0.3/tests/test_count_recall.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_deck.py` & `popgym-1.0.3/tests/test_deck.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_higher_lower.py` & `popgym-1.0.3/tests/test_higher_lower.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_labyrinth_escape.py` & `popgym-1.0.3/tests/test_labyrinth_escape.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_labyrinth_explore.py` & `popgym-1.0.3/tests/test_labyrinth_explore.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_minesweeper.py` & `popgym-1.0.3/tests/test_minesweeper.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_multiarmed_bandit.py` & `popgym-1.0.3/tests/test_multiarmed_bandit.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_repeat_first.py` & `popgym-1.0.3/tests/test_repeat_first.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_repeat_previous.py` & `popgym-1.0.3/tests/test_repeat_previous.py`

 * *Files identical despite different names*

### Comparing `popgym-1.0.2/tests/test_wrappers.py` & `popgym-1.0.3/tests/test_wrappers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from gymnasium.utils.env_checker import check_env
 
 from popgym import envs
 from popgym.core.observability import OBS, STATE, Observability
 from popgym.wrappers.antialias import Antialias
+from popgym.wrappers.discrete_action import DiscreteAction
 from popgym.wrappers.flatten import Flatten
 from popgym.wrappers.markovian import Markovian
 from popgym.wrappers.previous_action import PreviousAction
 
 
 def check_space(space, data):
     valid = space.contains(data)
@@ -102,7 +103,16 @@
 
 @pytest.mark.parametrize("env", envs.ALL.keys())
 def test_flatten_step(env):
     wrapped_aa = Flatten(env())
     obs, _ = wrapped_aa.reset()
     assert wrapped_aa.observation_space.contains(obs)
     check_env(wrapped_aa, skip_render_check=True)
+
+
+@pytest.mark.parametrize("env", envs.ALL.keys())
+def test_discrete_action(env):
+    if issubclass(env, (envs.StatelessPendulum, envs.NoisyStatelessPendulum)):
+        pytest.skip("StatelessPendulum does not support discrete action space")
+    wrapped = DiscreteAction(Flatten(env()))
+    _, _ = wrapped.reset()
+    wrapped.step(wrapped.action_space.sample())
```

