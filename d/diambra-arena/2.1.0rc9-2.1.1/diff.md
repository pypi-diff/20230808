# Comparing `tmp/diambra-arena-2.1.0rc9.tar.gz` & `tmp/diambra-arena-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-arena-2.1.0rc9.tar", last modified: Sun Jun 11 18:27:28 2023, max compression
+gzip compressed data, was "diambra-arena-2.1.1.tar", last modified: Tue Aug  8 11:35:04 2023, max compression
```

## Comparing `diambra-arena-2.1.0rc9.tar` & `diambra-arena-2.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16903 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/arena/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/arena_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/arena_imitation_learning_gym.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.655247 diambra-arena-2.1.0rc9/diambra/arena/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/engine/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/env_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/make_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/make_ray_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/make_sb_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/sb_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/p2_wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.659247 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/make_sb3_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/sb3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.663248 diambra-arena-2.1.0rc9/diambra/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/.splash_screen.gif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/engine_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/gym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14509 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/integratedGames.json
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/utils/splash_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.667248 diambra-arena-2.1.0rc9/diambra/arena/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/arena_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper_hardcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.667248 diambra-arena-2.1.0rc9/diambra_arena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17868 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 18:27:28.000000 diambra-arena-2.1.0rc9/diambra_arena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:27:28.671248 diambra-arena-2.1.0rc9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_gym_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_imitation_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_integration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_recording_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-11 18:27:04.000000 diambra-arena-2.1.0rc9/tests/test_wrappers_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.609248 diambra-arena-2.1.1/diambra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21897 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/arena_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16522 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/arena_imitation_learning_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/engine/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/env_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/make_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/ray_rllib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/ray_rllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/ray_rllib/make_ray_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.613248 diambra-arena-2.1.1/diambra/arena/stable_baselines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/make_sb_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/sb_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.617248 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/p2_wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.617248 diambra-arena-2.1.1/diambra/arena/stable_baselines3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/make_sb3_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/stable_baselines3/sb3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   167633 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/.splash_screen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39134 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/engine_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/gym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14111 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/integratedGames.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/utils/splash_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra/arena/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/arena_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper_hardcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.621248 diambra-arena-2.1.1/diambra_arena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-08 11:35:04.000000 diambra-arena-2.1.1/diambra_arena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 11:35:04.625249 diambra-arena-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_gym_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_imitation_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5084 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_recording_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-08 11:34:49.000000 diambra-arena-2.1.1/tests/test_wrappers_settings.py
```

### Comparing `diambra-arena-2.1.0rc9/LICENSE.txt` & `diambra-arena-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/PKG-INFO` & `diambra-arena-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc9
+Version: 2.1.1
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -115,20 +115,26 @@
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
+- Install specific `wheel` and `setuptools` versions (temporary workaround to handle `gym v0.21` incompatibility with newest `pip` versions*):
+
+  `python3 -m pip install wheel==0.38.4 setuptools==66.0.0`
+
 - Install DIAMBRA Command Line Interface: `python3 -m pip install diambra`
 
 - Install DIAMBRA Arena: `python3 -m pip install diambra-arena`
 
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
+*We are already working to support `gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This breaking change will happen very soon.
+
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc9 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.1 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -86,23 +86,28 @@
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
 possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
 our_website, it requires just a few clicks and is 100% free - Install Docker
-Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
-`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
-install diambra-arena` **Using a virtual environment to isolate your python
-packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
-Arena usage follows the standard RL interaction framework: the agent sends an
-action to the environment, which process it and performs a transition
-accordingly, from the starting state to the new state, returning the
-observation and the reward to the agent to close the interaction loop. The
-figure below shows this typical interaction scheme and data flow.
+Desktop: Linux | Windows | MacOS - Install specific `wheel` and `setuptools`
+versions (temporary workaround to handle `gym v0.21` incompatibility with
+newest `pip` versions*): `python3 -m pip install wheel==0.38.4
+setuptools==66.0.0` - Install DIAMBRA Command Line Interface: `python3 -m pip
+install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
+arena` **Using a virtual environment to isolate your python packages
+installation is strongly suggested** *We are already working to support
+`gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This
+breaking change will happen very soon. ## Quickstart & Examples DIAMBRA Arena
+usage follows the standard RL interaction framework: the agent sends an action
+to the environment, which process it and performs a transition accordingly,
+from the starting state to the new state, returning the observation and the
+reward to the agent to close the interaction loop. The figure below shows this
+typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check out available games: ```
 diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
 ++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
 name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
 japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
```

### Comparing `diambra-arena-2.1.0rc9/README.md` & `diambra-arena-2.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,20 +90,26 @@
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
+- Install specific `wheel` and `setuptools` versions (temporary workaround to handle `gym v0.21` incompatibility with newest `pip` versions*):
+
+  `python3 -m pip install wheel==0.38.4 setuptools==66.0.0`
+
 - Install DIAMBRA Command Line Interface: `python3 -m pip install diambra`
 
 - Install DIAMBRA Arena: `python3 -m pip install diambra-arena`
 
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
+*We are already working to support `gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This breaking change will happen very soon.
+
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
```

#### html2text {}

```diff
@@ -74,23 +74,28 @@
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
 possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
 our_website, it requires just a few clicks and is 100% free - Install Docker
-Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
-`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
-install diambra-arena` **Using a virtual environment to isolate your python
-packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
-Arena usage follows the standard RL interaction framework: the agent sends an
-action to the environment, which process it and performs a transition
-accordingly, from the starting state to the new state, returning the
-observation and the reward to the agent to close the interaction loop. The
-figure below shows this typical interaction scheme and data flow.
+Desktop: Linux | Windows | MacOS - Install specific `wheel` and `setuptools`
+versions (temporary workaround to handle `gym v0.21` incompatibility with
+newest `pip` versions*): `python3 -m pip install wheel==0.38.4
+setuptools==66.0.0` - Install DIAMBRA Command Line Interface: `python3 -m pip
+install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
+arena` **Using a virtual environment to isolate your python packages
+installation is strongly suggested** *We are already working to support
+`gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This
+breaking change will happen very soon. ## Quickstart & Examples DIAMBRA Arena
+usage follows the standard RL interaction framework: the agent sends an action
+to the environment, which process it and performs a transition accordingly,
+from the starting state to the new state, returning the observation and the
+reward to the agent to close the interaction loop. The figure below shows this
+typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check out available games: ```
 diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
 ++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
 name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
 japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
```

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/arena_gym.py` & `diambra-arena-2.1.1/diambra/arena/arena_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/arena_imitation_learning_gym.py` & `diambra-arena-2.1.1/diambra/arena/arena_imitation_learning_gym.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/engine/interface.py` & `diambra-arena-2.1.1/diambra/arena/engine/interface.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/env_settings.py` & `diambra-arena-2.1.1/diambra/arena/env_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/make_env.py` & `diambra-arena-2.1.1/diambra/arena/make_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/ray_rllib/make_ray_env.py` & `diambra-arena-2.1.1/diambra/arena/ray_rllib/make_ray_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/make_sb_env.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines/make_sb_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/sb_utils.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines/sb_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/add_obs_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/p2_wrap.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/p2_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines/wrappers/tektag_rew_wrap.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/make_sb3_env.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines3/make_sb3_env.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/stable_baselines3/sb3_utils.py` & `diambra-arena-2.1.1/diambra/arena/stable_baselines3/sb3_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/.splash_screen.gif` & `diambra-arena-2.1.1/diambra/arena/utils/.splash_screen.gif`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/controller.py` & `diambra-arena-2.1.1/diambra/arena/utils/controller.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/engine_mock.py` & `diambra-arena-2.1.1/diambra/arena/utils/engine_mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,14 @@
         self.ram_states["SideP1"][3] = self.side_p1
         self.ram_states["SideP2"][3] = self.side_p2
         self.ram_states["WinsP1"][3] = self.n_rounds_won
         self.ram_states["WinsP2"][3] = self.n_rounds_lost
 
         self.ram_states["CharP1"][3] = self.char_p1
         self.ram_states["CharP2"][3] = self.char_p2
-        self.ram_states["Char1P1"][3] = self.char_p1
-        self.ram_states["Char1P2"][3] = self.char_p2
 
         if self.game_data["number_of_chars_per_round"] == 1:
             self.ram_states["HealthP1"][3] = self.health_p1
             self.ram_states["HealthP2"][3] = self.health_p2
         else:
             for idx in range(self.game_data["number_of_chars_per_round"]):
                 self.ram_states["Health{}P1".format(idx+1)][3] = self.health_p1
```

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/gym_utils.py` & `diambra-arena-2.1.1/diambra/arena/utils/gym_utils.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/integratedGames.json` & `diambra-arena-2.1.1/diambra/arena/utils/integratedGames.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966258804601197%*

 * *Differences: {"'doapp'": "{'ram_states': {delete: ['Char1P1', 'Char1P2']}}",*

 * * "'kof98umh'": "{'ram_states': {delete: ['ActiveCharP1', 'ActiveCharP2']}}",*

 * * "'samsh5sp'": "{'stages_per_game': 7, 'ram_states': {'WinsP1': {insert: [(2, 3)], delete: [2]}, "*

 * *               "'WinsP2': {insert: [(2, 3)], delete: [2]}, 'stage': {insert: [(2, 7)], delete: "*

 * *               "[2]}, delete: ['Char1P1', 'Char1P2']}}",*

 * * "'sfiii3n'": "{'ram_states': {delete: ['Char1P1', 'Char1P2']}}",*

 * * "'umk3'": "{'ram_states': {delete: ['Char1P1', 'Cha […]*

```diff
@@ -55,24 +55,14 @@
         "nvram_save": "at28c16",
         "original_rom_name": "doapp.zip",
         "outfits": [
             1,
             4
         ],
         "ram_states": {
-            "Char1P1": [
-                2,
-                0,
-                10
-            ],
-            "Char1P2": [
-                2,
-                0,
-                10
-            ],
             "CharP1": [
                 2,
                 0,
                 10
             ],
             "CharP2": [
                 2,
@@ -220,24 +210,14 @@
         "nvram_save": "",
         "original_rom_name": "kof98umh.zip",
         "outfits": [
             1,
             4
         ],
         "ram_states": {
-            "ActiveCharP1": [
-                1,
-                0,
-                2
-            ],
-            "ActiveCharP2": [
-                1,
-                0,
-                2
-            ],
             "BarTypeP1": [
                 2,
                 0,
                 7
             ],
             "BarTypeP2": [
                 2,
@@ -427,24 +407,14 @@
         "nvram_save": "",
         "original_rom_name": "samsh5sp.zip",
         "outfits": [
             1,
             4
         ],
         "ram_states": {
-            "Char1P1": [
-                2,
-                0,
-                27
-            ],
-            "Char1P2": [
-                2,
-                0,
-                27
-            ],
             "CharP1": [
                 2,
                 0,
                 27
             ],
             "CharP2": [
                 2,
@@ -540,36 +510,36 @@
                 0,
                 0,
                 1
             ],
             "WinsP1": [
                 1,
                 0,
-                2
+                3
             ],
             "WinsP2": [
                 1,
                 0,
-                2
+                3
             ],
             "stage": [
                 1,
                 1,
-                9
+                7
             ]
         },
         "rounds_per_stage": 2,
         "search_keywords": [
             "SAMURAI SHODOWN V SPECIAL",
             "samurai-shodown-v-special",
             "100347",
             "wowroms"
         ],
         "sha256": "adf33d8a02f3d900b4aa95e62fb21d9278fb920b179665b12a489bd39a6c103d",
-        "stages_per_game": 9
+        "stages_per_game": 7
     },
     "sfiii3n": {
         "cfg": {
             "HK": "But6",
             "HP": "But5",
             "LK": "But3",
             "LP": "But4",
@@ -639,24 +609,14 @@
         "nvram_save": "",
         "original_rom_name": "sfiii3n.zip",
         "outfits": [
             1,
             7
         ],
         "ram_states": {
-            "Char1P1": [
-                2,
-                0,
-                19
-            ],
-            "Char1P2": [
-                2,
-                0,
-                19
-            ],
             "CharP1": [
                 2,
                 0,
                 19
             ],
             "CharP2": [
                 2,
@@ -1055,24 +1015,14 @@
                 48
             ],
             "AggressorBarP2": [
                 1,
                 0,
                 48
             ],
-            "Char1P1": [
-                2,
-                0,
-                25
-            ],
-            "Char1P2": [
-                2,
-                0,
-                25
-            ],
             "CharP1": [
                 2,
                 0,
                 25
             ],
             "CharP2": [
                 2,
```

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/policies.py` & `diambra-arena-2.1.1/diambra/arena/utils/policies.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/utils/splash_screen.py` & `diambra-arena-2.1.1/diambra/arena/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/wrappers/arena_wrappers.py` & `diambra-arena-2.1.1/diambra/arena/wrappers/arena_wrappers.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper.py` & `diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/wrappers/obs_wrapper_hardcore.py` & `diambra-arena-2.1.1/diambra/arena/wrappers/obs_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper.py` & `diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py` & `diambra-arena-2.1.1/diambra/arena/wrappers/traj_rec_wrapper_hardcore.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/diambra_arena.egg-info/PKG-INFO` & `diambra-arena-2.1.1/diambra_arena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-arena
-Version: 2.1.0rc9
+Version: 2.1.1
 Summary: DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments
 Home-page: https://github.com/diambra/arena
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
@@ -115,20 +115,26 @@
 
 ## Installation
 
 - <a href="https://diambra.ai/register/" target="_blank">Create an account on our website</a>, it requires just a few clicks and is 100% free
 
 - Install Docker Desktop: <a href="https://docs.docker.com/desktop/install/linux-install/" target="_blank">Linux</a> | <a href="https://docs.docker.com/desktop/windows/install/" target="_blank">Windows</a> | <a href="https://docs.docker.com/desktop/mac/install/" target="_blank">MacOS</a>
 
+- Install specific `wheel` and `setuptools` versions (temporary workaround to handle `gym v0.21` incompatibility with newest `pip` versions*):
+
+  `python3 -m pip install wheel==0.38.4 setuptools==66.0.0`
+
 - Install DIAMBRA Command Line Interface: `python3 -m pip install diambra`
 
 - Install DIAMBRA Arena: `python3 -m pip install diambra-arena`
 
 **Using a virtual environment to isolate your python packages installation is strongly suggested**
 
+*We are already working to support `gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This breaking change will happen very soon.
+
 ## Quickstart & Examples
 
 DIAMBRA Arena usage follows the standard RL interaction framework: the agent sends an action to the environment, which process it and performs a transition accordingly, from the starting state to the new state, returning the observation and the reward to the agent to close the interaction loop. The figure below shows this typical interaction scheme and data flow.
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/diambra/arena/main/img/basicUsage.png" alt="rlScheme" width="75%"/>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.0rc9 Summary: DIAMBRAâ¢
+Metadata-Version: 2.1 Name: diambra-arena Version: 2.1.1 Summary: DIAMBRAâ¢
 Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular
 video games into Reinforcement Learning environments Home-page: https://
 github.com/diambra/arena Author: DIAMBRA Team Author-email: info@diambra.ai
 License: Custom Classifier: Development Status :: 3 - Alpha Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
@@ -86,23 +86,28 @@
 It features a public global leaderboard where users are ranked by the best
 score achieved by their agents in our different environments. It also offers
 you the possibility to unlock cool achievements depending on the performances
 of your agent. Submitted agents are evaluated and their episodes are streamed
 on our Twitch channel. We aimed at making the submission process as smooth as
 possible, **join_us_and_try_it_now!** ## Installation - Create_an_account_on
 our_website, it requires just a few clicks and is 100% free - Install Docker
-Desktop: Linux | Windows | MacOS - Install DIAMBRA Command Line Interface:
-`python3 -m pip install diambra` - Install DIAMBRA Arena: `python3 -m pip
-install diambra-arena` **Using a virtual environment to isolate your python
-packages installation is strongly suggested** ## Quickstart & Examples DIAMBRA
-Arena usage follows the standard RL interaction framework: the agent sends an
-action to the environment, which process it and performs a transition
-accordingly, from the starting state to the new state, returning the
-observation and the reward to the agent to close the interaction loop. The
-figure below shows this typical interaction scheme and data flow.
+Desktop: Linux | Windows | MacOS - Install specific `wheel` and `setuptools`
+versions (temporary workaround to handle `gym v0.21` incompatibility with
+newest `pip` versions*): `python3 -m pip install wheel==0.38.4
+setuptools==66.0.0` - Install DIAMBRA Command Line Interface: `python3 -m pip
+install diambra` - Install DIAMBRA Arena: `python3 -m pip install diambra-
+arena` **Using a virtual environment to isolate your python packages
+installation is strongly suggested** *We are already working to support
+`gymnasium>=0.26.3` to solve all `gym v0.21` compatibility issues. This
+breaking change will happen very soon. ## Quickstart & Examples DIAMBRA Arena
+usage follows the standard RL interaction framework: the agent sends an action
+to the environment, which process it and performs a transition accordingly,
+from the starting state to the new state, returning the observation and the
+reward to the agent to close the interaction loop. The figure below shows this
+typical interaction scheme and data flow.
                                   [rlScheme]
 #### Download Game ROM(s) and Check Validity Check out available games: ```
 diambra arena list-roms ``` Output extract: ```shell [...] Title: Dead Or Alive
 ++ - GameId: doapp Difficulty levels: Min 1 - Max 4 SHA256 sum:
 d95855c7d8596a90f0b8ca15725686567d767a9a3f93a8896b489a160e705c4e Original ROM
 name: doapp.zip Search keywords: ['DEAD OR ALIVE ++ [JAPAN]', 'dead-or-alive-
 japan', '80781', 'wowroms'] Characters list: ['Kasumi', 'Zack', 'Hayabusa',
```

### Comparing `diambra-arena-2.1.0rc9/diambra_arena.egg-info/SOURCES.txt` & `diambra-arena-2.1.1/diambra_arena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/setup.py` & `diambra-arena-2.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     description="DIAMBRA™ Arena. Built with OpenAI Gym Python interface, easy to use, transforms popular video games into Reinforcement Learning environments",
     long_description = (Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     license='Custom',
     install_requires=[
             'pip>=21',
             'importlib-metadata<=4.12.0; python_version <= "3.7"', # problem with gym for importlib-metadata==5.0.0 and python <=3.7
-            'wheel==0.38.4', # Required until we can upgrade to gym >= 0.22.0
-            'setuptools',
+            'setuptools<=66.0.0', # Required until we can upgrade to gym >= 0.22.0
             'distro>=1',
             'gym<=0.21.0',
             'inputs',
             'screeninfo',
             'tk',
             'opencv-python>=4.4.0.42',
             'grpcio',
```

### Comparing `diambra-arena-2.1.0rc9/tests/test_gym_settings.py` & `diambra-arena-2.1.1/tests/test_gym_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_imitation_learning.py` & `diambra-arena-2.1.1/tests/test_imitation_learning.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_integration.py` & `diambra-arena-2.1.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_random.py` & `diambra-arena-2.1.1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_recording_settings.py` & `diambra-arena-2.1.1/tests/test_recording_settings.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_speed.py` & `diambra-arena-2.1.1/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `diambra-arena-2.1.0rc9/tests/test_wrappers_settings.py` & `diambra-arena-2.1.1/tests/test_wrappers_settings.py`

 * *Files identical despite different names*

