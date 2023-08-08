# Comparing `tmp/diambra-arena-2.1.1.tar.gz` & `tmp/diambra-arena-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.1.tar", last modified: Tue Aug  8 11:35:04 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.2.tar", last modified: Tue Aug  8 13:12:24 2023, max compression
```

## Comparing `diambra-arena-2.1.1.tar` & `diambra-arena-2.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.609248 diambra-arena-2.1.1/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.617248 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.617248 diambra-arena-2.1.1/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/.splash_screen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/engine_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.100445 diambra-arena-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 13:12:24.100445 diambra-arena-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.088445 diambra-arena-2.1.2/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.088445 diambra-arena-2.1.2/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.088445 diambra-arena-2.1.2/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.088445 diambra-arena-2.1.2/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.088445 diambra-arena-2.1.2/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.092445 diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.092445 diambra-arena-2.1.2/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.096445 diambra-arena-2.1.2/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/.splash_screen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/engine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.096445 diambra-arena-2.1.2/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.100445 diambra-arena-2.1.2/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 13:12:24.000000 diambra-arena-2.1.2/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 13:12:24.000000 diambra-arena-2.1.2/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:12:24.000000 diambra-arena-2.1.2/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 13:12:24.000000 diambra-arena-2.1.2/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 13:12:24.000000 diambra-arena-2.1.2/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:12:24.100445 diambra-arena-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:12:24.100445 diambra-arena-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-08 13:12:05.000000 diambra-arena-2.1.2/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.1/LICENSE.txt` & `diambra-arena-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/PKG-INFO` & `diambra-arena-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.1
+Version: 2.1.2
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.1 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.2 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `diambra-arena-2.1.1/README.md` & `diambra-arena-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/arena_gym.py` & `diambra-arena-2.1.2/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.2/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/engine/interface.py` & `diambra-arena-2.1.2/diambra/arena/engine/interface.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/env_settings.py` & `diambra-arena-2.1.2/diambra/arena/env_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/make_env.py` & `diambra-arena-2.1.2/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.2/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines/sb_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra-arena-2.1.2/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/.splash_screen.gif` & `diambra-arena-2.1.2/diambra/arena/utils/.splash_screen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/controller.py` & `diambra-arena-2.1.2/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/engine_mock.py` & `diambra-arena-2.1.2/diambra/arena/utils/engine_mock.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.2/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/integratedGames.json` & `diambra-arena-2.1.2/diambra/arena/utils/integratedGames.json`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/policies.py` & `diambra-arena-2.1.2/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.2/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.2/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.2/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.2/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.2/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.2/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.2/diambra_arena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.1
+Version: 2.1.2
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.1 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.2 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
```

### Comparing `diambra-arena-2.1.1/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.2/diambra_arena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/setup.py` & `diambra-arena-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_gym_settings.py` & `diambra-arena-2.1.2/tests/test_gym_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_imitation_learning.py` & `diambra-arena-2.1.2/tests/test_imitation_learning.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_integration.py` & `diambra-arena-2.1.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_random.py` & `diambra-arena-2.1.2/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_recording_settings.py` & `diambra-arena-2.1.2/tests/test_recording_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_speed.py` & `diambra-arena-2.1.2/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.1/tests/test_wrappers_settings.py` & `diambra-arena-2.1.2/tests/test_wrappers_settings.py`

 * *Files identical despite different names*

