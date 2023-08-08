# Comparing `tmp/slingshot_ai-0.0.17.tar.gz` & `tmp/slingshot_ai-0.0.18rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.17.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.18rc1.tar", max compression
```

## Comparing `slingshot_ai-0.0.17.tar` & `slingshot_ai-0.0.18rc1.tar`

### file list

```diff
@@ -1,79 +1,81 @@
--rw-r--r--   0        0        0      831 2023-07-20 17:43:37.505854 slingshot_ai-0.0.17/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.17/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.17/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17378 2023-07-19 17:55:36.034054 slingshot_ai-0.0.17/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     1982 2023-07-13 15:57:24.531070 slingshot_ai-0.0.17/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     6431 2023-07-12 21:00:50.132623 slingshot_ai-0.0.17/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     5916 2023-06-20 21:48:49.557285 slingshot_ai-0.0.17/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5263 2023-06-27 15:26:50.737721 slingshot_ai-0.0.17/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.17/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.17/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.17/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.17/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.17/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0     1234 2023-06-08 13:51:24.735333 slingshot_ai-0.0.17/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1123 2023-07-03 01:17:17.281267 slingshot_ai-0.0.17/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     5323 2023-07-05 13:59:49.265273 slingshot_ai-0.0.17/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.17/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.17/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2759 2023-07-04 04:36:55.756325 slingshot_ai-0.0.17/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     3011 2023-07-12 21:00:50.133568 slingshot_ai-0.0.17/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.17/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     8920 2023-07-07 20:43:45.117337 slingshot_ai-0.0.17/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.17/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3845 2023-07-04 04:36:55.756967 slingshot_ai-0.0.17/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.17/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6260 2023-06-20 21:48:49.557743 slingshot_ai-0.0.17/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7036 2023-07-12 21:00:50.134070 slingshot_ai-0.0.17/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.17/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      191 2023-06-08 13:51:24.738326 slingshot_ai-0.0.17/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     6183 2023-07-18 01:03:50.455195 slingshot_ai-0.0.17/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.17/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.17/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.17/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.17/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.17/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.17/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.17/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.17/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.17/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26686 2023-07-20 17:22:15.000000 slingshot_ai-0.0.17/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.17/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10181 2023-06-27 15:26:50.747432 slingshot_ai-0.0.17/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    15314 2023-07-19 17:55:36.035248 slingshot_ai-0.0.17/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    19863 2023-07-19 17:55:36.035584 slingshot_ai-0.0.17/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0      125 2023-07-06 14:31:59.119085 slingshot_ai-0.0.17/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    48950 2023-07-19 17:56:27.919660 slingshot_ai-0.0.17/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.17/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     2073 2023-06-27 15:26:50.749266 slingshot_ai-0.0.17/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     2007 2023-07-13 02:14:29.104748 slingshot_ai-0.0.17/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.17/src/slingshot/sdk/data_collector.py
--rw-r--r--   0        0        0     5394 2023-07-19 17:56:27.920088 slingshot_ai-0.0.17/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-08 13:51:24.743943 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    18486 2023-07-14 18:10:49.055701 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3671 2023-06-08 13:51:24.745123 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5247 2023-06-27 15:26:50.751307 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2416 2023-07-07 20:43:45.118845 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     3578 2023-06-08 13:51:24.745899 slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.17/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    48581 2023-07-19 17:56:27.920680 slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    52327 2023-07-20 13:33:03.423585 slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     7010 2023-07-18 16:49:57.082909 slingshot_ai-0.0.17/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2862 2023-06-08 13:51:24.747244 slingshot_ai-0.0.17/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     4149 2023-07-13 15:57:24.533800 slingshot_ai-0.0.17/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.17/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.17/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.17/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     6753 2023-07-12 21:00:50.142218 slingshot_ai-0.0.17/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-07-20 17:44:29.983945 slingshot_ai-0.0.17/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.17/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.17/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     1090 2023-06-08 13:51:24.748859 slingshot_ai-0.0.17/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.17/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 slingshot_ai-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      795 2023-08-08 03:19:43.773858 slingshot_ai-0.0.18rc1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.18rc1/src/slingshot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.18rc1/src/slingshot/cli/__init__.py
+-rw-r--r--   0        0        0    17826 2023-08-01 14:47:02.806869 slingshot_ai-0.0.18rc1/src/slingshot/cli/add.py
+-rw-r--r--   0        0        0     1328 2023-08-07 17:29:08.858475 slingshot_ai-0.0.18rc1/src/slingshot/cli/apply.py
+-rw-r--r--   0        0        0     5931 2023-07-28 21:27:30.614734 slingshot_ai-0.0.18rc1/src/slingshot/cli/apps.py
+-rw-r--r--   0        0        0     8225 2023-08-02 14:52:04.657063 slingshot_ai-0.0.18rc1/src/slingshot/cli/artifact.py
+-rw-r--r--   0        0        0     5388 2023-07-21 18:05:09.101272 slingshot_ai-0.0.18rc1/src/slingshot/cli/auth.py
+-rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.18rc1/src/slingshot/cli/code.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.18rc1/src/slingshot/cli/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.18rc1/src/slingshot/cli/config/py.typed
+-rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.18rc1/src/slingshot/cli/config/sentry_setup.py
+-rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.18rc1/src/slingshot/cli/config/slingshot_cli.py
+-rw-r--r--   0        0        0      899 2023-08-07 21:17:35.138494 slingshot_ai-0.0.18rc1/src/slingshot/cli/dev.py
+-rw-r--r--   0        0        0     1422 2023-07-28 21:27:30.615238 slingshot_ai-0.0.18rc1/src/slingshot/cli/environment.py
+-rw-r--r--   0        0        0     4778 2023-07-28 21:27:30.615824 slingshot_ai-0.0.18rc1/src/slingshot/cli/inference.py
+-rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.18rc1/src/slingshot/cli/logs.py
+-rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.18rc1/src/slingshot/cli/machine.py
+-rw-r--r--   0        0        0     2731 2023-08-07 17:00:07.297121 slingshot_ai-0.0.18rc1/src/slingshot/cli/main.py
+-rw-r--r--   0        0        0     3085 2023-08-07 17:00:07.297512 slingshot_ai-0.0.18rc1/src/slingshot/cli/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.18rc1/src/slingshot/cli/py.typed
+-rw-r--r--   0        0        0     8170 2023-07-28 21:27:30.616461 slingshot_ai-0.0.18rc1/src/slingshot/cli/run.py
+-rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.18rc1/src/slingshot/cli/secret.py
+-rw-r--r--   0        0        0     3846 2023-07-21 18:05:09.101837 slingshot_ai-0.0.18rc1/src/slingshot/cli/session.py
+-rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/__init__.py
+-rw-r--r--   0        0        0     6582 2023-07-21 18:05:09.102433 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/code_sync.py
+-rw-r--r--   0        0        0     7036 2023-07-12 21:00:50.134070 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/py.typed
+-rw-r--r--   0        0        0      200 2023-08-07 16:59:44.189969 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/settings.py
+-rw-r--r--   0        0        0     7527 2023-08-01 14:47:02.809069 slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/utils.py
+-rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.18rc1/src/slingshot/cli/volume.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.18rc1/src/slingshot/code/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.18rc1/src/slingshot/code/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.18rc1/src/slingshot/code/py.typed
+-rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.18rc1/src/slingshot/inference_model/__init__.py
+-rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.18rc1/src/slingshot/inference_model/inference_model.py
+-rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.18rc1/src/slingshot/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.18rc1/src/slingshot/schemas/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.18rc1/src/slingshot/schemas/generated/py.typed
+-rw-r--r--   0        0        0    26165 2023-08-08 03:31:35.000000 slingshot_ai-0.0.18rc1/src/slingshot/schemas/generated/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.18rc1/src/slingshot/schemas/py.typed
+-rw-r--r--   0        0        0    10081 2023-08-07 21:53:29.033623 slingshot_ai-0.0.18rc1/src/slingshot/schemas/schema_extensions.py
+-rw-r--r--   0        0        0    17610 2023-08-07 21:54:30.413533 slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot-schema.config.json
+-rw-r--r--   0        0        0    22943 2023-08-07 21:53:50.709395 slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot_schema.py
+-rw-r--r--   0        0        0      155 2023-07-28 16:35:47.947662 slingshot_ai-0.0.18rc1/src/slingshot/sdk/__init__.py
+-rw-r--r--   0        0        0    33767 2023-08-07 20:05:38.093697 slingshot_ai-0.0.18rc1/src/slingshot/sdk/apply.py
+-rw-r--r--   0        0        0     4193 2023-08-07 21:32:16.535851 slingshot_ai-0.0.18rc1/src/slingshot/sdk/apply_diff.py
+-rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.18rc1/src/slingshot/sdk/auth.py
+-rw-r--r--   0        0        0     3070 2023-08-07 21:40:49.398817 slingshot_ai-0.0.18rc1/src/slingshot/sdk/config.py
+-rw-r--r--   0        0        0     2953 2023-08-08 03:18:11.866437 slingshot_ai-0.0.18rc1/src/slingshot/sdk/config_utils.py
+-rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.18rc1/src/slingshot/sdk/data_collector.py
+-rw-r--r--   0        0        0     6805 2023-08-07 16:59:44.195575 slingshot_ai-0.0.18rc1/src/slingshot/sdk/errors.py
+-rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/__init__.py
+-rw-r--r--   0        0        0     3100 2023-08-07 16:59:46.676999 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/base_graphql.py
+-rw-r--r--   0        0        0    19980 2023-08-08 03:11:35.470733 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/fragments.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/py.typed
+-rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/__init__.py
+-rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/apps.py
+-rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/deployment.py
+-rw-r--r--   0        0        0     3674 2023-08-07 16:59:44.196853 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/environment.py
+-rw-r--r--   0        0        0     5272 2023-08-07 16:59:44.197122 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/project.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/py.typed
+-rw-r--r--   0        0        0     2418 2023-08-07 16:59:44.197383 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/run.py
+-rw-r--r--   0        0        0     4362 2023-08-07 16:59:46.677767 slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/storage.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.18rc1/src/slingshot/sdk/py.typed
+-rw-r--r--   0        0        0    51039 2023-08-07 20:35:18.480908 slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_api.py
+-rw-r--r--   0        0        0    54502 2023-08-07 17:00:07.299389 slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_sdk.py
+-rw-r--r--   0        0        0     7008 2023-08-01 14:47:02.813054 slingshot_ai-0.0.18rc1/src/slingshot/sdk/sync.py
+-rw-r--r--   0        0        0     2904 2023-08-01 14:47:02.814359 slingshot_ai-0.0.18rc1/src/slingshot/sdk/upload_download_utils.py
+-rw-r--r--   0        0        0     4583 2023-08-07 16:59:44.201251 slingshot_ai-0.0.18rc1/src/slingshot/sdk/utils.py
+-rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.18rc1/src/slingshot/sdk/web_path_util.py
+-rw-r--r--   0        0        0     6934 2023-08-07 17:00:07.299685 slingshot_ai-0.0.18rc1/src/slingshot/sdk/wrapped_diff.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.18rc1/src/slingshot/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.18rc1/src/slingshot/shared/py.typed
+-rw-r--r--   0        0        0     7416 2023-08-07 20:36:47.135606 slingshot_ai-0.0.18rc1/src/slingshot/shared/utils.py
+-rw-r--r--   0        0        0       26 2023-08-08 03:36:04.100984 slingshot_ai-0.0.18rc1/src/slingshot/slingshot_version.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.18rc1/src/slingshot/templates/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.18rc1/src/slingshot/templates/inference_template.py
+-rw-r--r--   0        0        0     3582 2023-08-07 16:59:44.203536 slingshot_ai-0.0.18rc1/src/slingshot/templates/label_studio_data_export_template.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.18rc1/src/slingshot/templates/py.typed
+-rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 slingshot_ai-0.0.18rc1/PKG-INFO
```

### Comparing `slingshot_ai-0.0.17/pyproject.toml` & `slingshot_ai-0.0.18rc1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [project]
 name = "slingshot-ai"
-version = "0.0.17"
+version = "0.0.18rc1"
 
 [tool.poetry]
 name = "slingshot-ai"
-version = "0.0.17"
+version = "0.0.18rc1"
 description = ""
 authors = ["Slingshot AI <service-account@slingshot.xyz>"]
 packages = [ { include = "slingshot", from = "src" } ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = "~=3.8.1"
-urllib3 = "~=1.26.11"
-pydantic = "<=1.10.11"
-typer = {extras = ["all"], version = "~0.7.0"}
-requests = "~=2.28.1"
-sh = "~=1.14.3"
-pyyaml = "~=6.0"
-"ruamel.yaml" = "~=0.17.0"
-simple-term-menu = "~=1.6.0"
-deepdiff = "~=6.3.0"
-fastapi = "~=0.88.0"
-uvicorn = {extras = ["standard"], version = "~=0.22.0"}
-tqdm = "~=4.63.0"
-sentry-sdk = "~=1.16.0"
-backoff = "~=2.0.0"
-openai = "~=0.27.8"
+aiohttp = ">=3.8.1"
+urllib3 = ">=1.26.11"
+pydantic = ">=2.0.0,<3"
+pydantic-settings = ">=2.0.0,<3"
+typer = {extras = ["all"], version = ">=0.7.0"}
+requests = ">=2.28.1"
+sh = ">=1.14.3"
+pyyaml = ">=6.0"
+"ruamel.yaml" = ">=0.17.0"
+simple-term-menu = ">=1.6.0"
+deepdiff = ">=6.3.0"
+tqdm = ">=4.63.0"
+sentry-sdk = ">=1.16.0"
+backoff = ">=2.0.0"
+openai = ">=0.27.8"
 
 [tool.poetry.scripts]
 slingshot = "slingshot.cli.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/add.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,20 @@
     alphanumeric_hyphen_underscore = re.sub(r"[^a-z0-9-_]", "", single_hyphen)
     return alphanumeric_hyphen_underscore
 
 
 async def _create_project(sdk: SlingshotSDK) -> str:
     new_id = None
     display_name = typer.prompt("Enter a name for your project")
-    project_id_default = _display_name_to_id(display_name) + "-" + uuid.uuid4().hex[:4]
+
+    # Use the display name to generate a project ID and append UUID if it's not available
+    project_id_default = _display_name_to_id(display_name)
+    if not await sdk._api.project_id_available(project_id_default):
+        project_id_default = f"{project_id_default}-{uuid.uuid4().hex[:4]}"
+
     while True:
         # Replace multiple spaces with a single space and spaces with hyphens
         new_id = new_id or typer.prompt(
             "Enter a slug for your project (unique ID used for URLs)", default=project_id_default
         )
         try:
             project_response = await sdk.create_project(new_id, display_name=display_name)
@@ -86,15 +91,15 @@
 
     # Check if the slingshot.yaml exists
     if client_settings.slingshot_config_path.exists() and client_settings.slingshot_config_path.stat().st_size > 0:
         console.print(
             "This project already has a `slingshot yaml`. You can add components to it with [bold]slingshot add[/bold]"
         )
         if not typer.confirm("Do you want to reinitialize this project from scratch?"):
-            await sdk.apply_project(and_wait=True)
+            await sdk.apply_project()
             return
 
     create_empty_project_manifest(client_settings.slingshot_config_path)
 
     first = True
     while True:
         prompt = "Do you want to add another component?" if not first else "Do you want to add a component?"
@@ -216,73 +221,77 @@
         console.print(f"App '{app_name}' added", style="green")
     return app_name
 
 
 def _create_label_studio() -> None:
     current = load_slingshot_project_config()
 
-    # Add a new label-studio environment if it doesn't already exist
-    env_name = "label-studio"
-    if env_name in current.environments:
-        console.print(f"Environment '{env_name}' already exists, skipping creation", style="yellow")
-    else:
-        environment = slingshot_yaml_schemas.EnvironmentSpec(
-            python_packages=["label-studio==1.7.1", "label-studio-sdk"]
-        )
-        current.environments[env_name] = environment
-        with edit_slingshot_yaml() as doc:
-            doc["environments"][env_name] = pydantic_to_dict(environment)
-        console.print(f"Environment '{env_name}' added", style="green")
+    # Add a new label studio app environment if it doesn't already exist
+    app_env_name = "label-studio-env"
+    _insert_env_if_not_exists(env_name=app_env_name, python_packages=["label-studio==1.8.0"], current_manifest=current)
 
-    # Add a new label-studio app if it doesn't already exist
+    # Add a new label studio app if it doesn't already exist
     app_name = "label-studio"
     if any(existing_app.name == app_name for existing_app in current.apps):
         console.print(f"App '{app_name}' already exists, skipping creation", style="yellow")
     else:
         # TODO ENG-1184
         ls_app = schemas.SlingshotCustomAppSpec(
             name=app_name,
-            environment=env_name,  # Guaranteed to exist since we just added it
+            environment=app_env_name,  # Guaranteed to exist since we just added it
             cmd=(
                 "label-studio start slingshot_ls_project --init "
                 "--username slingshot --password slingshot --user-token slingshot"
             ),
             port=8080,
             # TODO: include a volume so we automatically can persist data across app restarts
         )
         current.apps.append(ls_app)
         with edit_slingshot_yaml() as doc:
             if not doc.get("apps"):
                 doc["apps"] = []
             doc["apps"].append(pydantic_to_dict(ls_app))
         console.print(f"App '{app_name}' added", style="green")
 
+    # Add a new label studio run environment if it doesn't already exist
+    run_env_name = "label-studio-run-env"
+    _insert_env_if_not_exists(
+        env_name=run_env_name, python_packages=["label-studio-sdk==0.0.29", "slingshot-ai"], current_manifest=current
+    )
+
     # Add a new label-studio-export run if it doesn't already exist and create template file
     run_name = "label-studio-export"
     if any(existing_run.name == run_name for existing_run in current.runs):
         console.print(f"Run '{run_name}' already exists, skipping creation", style="yellow")
     else:
-        ls_run = schemas.RunSpec(
-            name=run_name,
-            # TODO: support mounting an empty download mount to export data and append to an existing artifact
-            mounts=[schemas.UploadMountSpec(path="/mnt/data", mode="UPLOAD", tag="dataset")],
-            cmd="python label_studio_data_export.py",
-            environment="label-studio",
-        )
+        ls_run = schemas.RunSpec(name=run_name, cmd="python label_studio_data_export.py", environment=run_env_name)
         current.runs.append(ls_run)
         with edit_slingshot_yaml() as doc:
             if not doc.get("runs"):
                 doc["runs"] = []
             doc["runs"].append(pydantic_to_dict(ls_run))
         console.print(f"Run '{run_name}' added", style="green")
 
         if prompt_confirm("Do you want to use template code for this run?", default=True):
             _copy_template_to_user_dir("label_studio_data_export_template.py", "label_studio_data_export.py")
 
 
+def _insert_env_if_not_exists(
+    env_name: str, python_packages: list[str], current_manifest: schemas.ProjectManifest
+) -> None:
+    if env_name in current_manifest.environments:
+        console.print(f"Environment '{env_name}' already exists, skipping creation", style="yellow")
+    else:
+        environment = slingshot_yaml_schemas.EnvironmentSpec(python_packages=python_packages)
+        current_manifest.environments[env_name] = environment
+        with edit_slingshot_yaml() as doc:
+            doc["environments"][env_name] = pydantic_to_dict(environment)
+        console.print(f"Environment '{env_name}' added", style="green")
+
+
 def _choose_or_create_environment(
     env_names: list[str], *, new_env_name: str, new_env_auto_packages: list[str] | None = None
 ) -> str:
     if len(env_names) == 1:
         env_name = list(env_names)[0]
         console.print(f"Defaulting to '{env_name}' as the environment", style="yellow")
         return env_name
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 async def start_app(
     *,
     sdk: SlingshotSDK,
     name: Optional[str] = typer.Argument(None, help="App name"),
     sessions: bool = typer.Option(False, "--sessions", "-s", help="Only show sessions"),
 ) -> str:
     """Start a Slingshot app"""
-    applied, await_env_specs = await sdk.apply_project()
+    applied = await sdk.apply_project()
     source_code_id = await prompt_push_code(sdk)
 
     if not name:
         filter_fn = filter_for_sessions if sessions else filter_for_apps
         id_and_name_or_none = await prompt_for_app_spec(
             sdk, filter_fn, app_display_name='session' if sessions else 'app', raise_if_missing=False
         )
@@ -58,22 +58,14 @@
             raise typer.Exit(1)
 
     assert sdk.project
     app_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
     if not app_spec:
         raise SlingshotException(f"No run found with the name '{name}'")
 
-    await_env_spec_names = [spec.execution_environment_spec_name for spec in await_env_specs]
-    if app_spec.execution_environment_spec.execution_environment_spec_name in await_env_spec_names:
-        console.print(
-            "Waiting for environment "
-            f"'{app_spec.execution_environment_spec.execution_environment_spec_name}' to compile"
-        )
-        await sdk._wait_for_env_compile(app_spec.execution_environment_spec.execution_environment, should_print=True)
-
     app_instance = await sdk.start_app(app_name=name, source_code_id=source_code_id)
     url = await sdk.web_path_util.app(app_spec=app_instance.app_spec_id)
     console.print(f"Starting app '{name}'. See details here: {url}")
 
     console.print(f"Following logs. Ctrl-C to stop, and run 'slingshot logs {name} --follow' to follow again")
     status = await follow_app_logs_until_ready(sdk, app_instance.app_spec_id)
     if status == schemas.AppInstanceStatus.ERROR:
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     will be used (usually ~/.ssh)."""
 
     await _set_ssh_public_key(sdk, filename)
 
 
 async def set_ssh_public_key_if_not_set(sdk: SlingshotSDK) -> None:
     """Set the SSH public key for the logged-in user if it's not set"""
-
     me = await sdk.me()
     if not (user := me and me.user):
         return None
     if not user.ssh_public_key:
         console.print(
             "You don't have an SSH public key set. Without it you won't be able to use the sync functionality."
         )
@@ -130,10 +129,11 @@
         raise typer.BadParameter("SSH public key file must end with .pub")
 
     with open(filename) as f:
         key = f.read()
 
     await sdk.set_ssh(key)
     console.print(
-        f"[green]Success[/green]: SSH public key has been set to {key}"
+        f"[green]Success[/green]: SSH public key has been set to {key}\n"
+        f"Note: Please make sure your SSH key is added to the SSH agent. You can do this by running 'ssh-add {filename}'\n"
         f"[yellow]Warning[/yellow]: Sessions that have already started won't get the updated key."
     )
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/code.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/dev.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional
 
 import typer
 
 from slingshot.sdk.config import global_config
 
-from ..sdk import SlingshotSDK
 from ..sdk.utils import console
 from .config.slingshot_cli import SlingshotCLIApp
 from .shared import prompt_for_single_choice
 
 app = SlingshotCLIApp()
 
 
@@ -27,14 +26,7 @@
         url = "https://dev.slingshot.xyz"
     elif url == "prod":
         url = "https://app.slingshot.xyz"
     else:
         url = url.rstrip("/")
     global_config.slingshot_backend_url = url
     console.print(f"Backend URL set to {url}")
-
-
-@app.command(name="rebuild-all-environments", top_level=True, hidden=True, requires_auth=True, requires_project=False)
-async def rebuild_all_environments(sdk: SlingshotSDK) -> None:
-    """Invalidate the environments cache"""
-    resp = await sdk.api.rebuild_all_environments()
-    console.print(resp)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/environment.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,17 +18,22 @@
             "No environments found!"
             "Edit [yellow]slingshot.yaml[/yellow] or use [yellow]slingshot add[/yellow] to add an environment template."
         )
         return
 
     table = Table(title="Environments")
     table.add_column("Environment Name", style="cyan")
-    table.add_column("Status", style="cyan")
-    table.add_column("Build Status", style="cyan")
-    for env in envs:
+    table.add_column("CPU Build Status", style="cyan")
+    table.add_column("GPU Build Status", style="cyan")
+
+    for env_spec in envs:
+        assert env_spec.environment_instances, "Environment spec should have at least one instance"
+        latest_env_instance = env_spec.environment_instances[0]
+        cpu_build = latest_env_instance.execution_environment.cpu_build
+        gpu_build = latest_env_instance.execution_environment.gpu_build
         row = [
-            env.execution_environment_spec_name,
-            env.execution_environment.status,
-            (env.execution_environment.build and env.execution_environment.build.build_status) or "--",
+            env_spec.execution_environment_spec_name,
+            cpu_build.build_status if cpu_build else "-",
+            gpu_build.build_status if gpu_build else "-",
         ]
         table.add_row(*row)
     console.print(table)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,34 +37,24 @@
 
 
 @app.command("start", requires_project=True)
 async def start_deployment(
     name: Optional[str] = typer.Argument(None, help="Deployment name"), *, sdk: SlingshotSDK
 ) -> None:
     """Deploys a model as an inference deployment"""
-    _, await_env_specs = await sdk.apply_project()
+    await sdk.apply_project()
     source_code_id = await prompt_push_code(sdk)
     if not name:
         _, name = await prompt_for_app_spec(sdk, filter_for_deployments, app_display_name="deployment")
 
     assert sdk.project
     deployment_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
     if not deployment_spec:
         raise SlingshotException(f"No run found with the name '{name}'")
 
-    await_env_spec_names = [spec.execution_environment_spec_name for spec in await_env_specs]
-    if deployment_spec.execution_environment_spec.execution_environment_spec_name in await_env_spec_names:
-        console.print(
-            "Waiting for environment "
-            f"'{deployment_spec.execution_environment_spec.execution_environment_spec_name}' to compile"
-        )
-        await sdk._wait_for_env_compile(
-            deployment_spec.execution_environment_spec.execution_environment, should_print=True
-        )
-
     deployment_spec = await sdk.start_deployment(deployment_name=name, source_code_id=source_code_id)
     url = await sdk.web_path_util.deployment(deployment_spec)
     console.print(f"[green]Deployment started successfully[/green]! " f"See details here: {url}")
 
 
 @app.command("stop", requires_project=True)
 async def stop_deployment(
@@ -116,15 +106,15 @@
     table.add_column("Status", style="cyan")
     table.add_column("Environment", style="cyan")
     table.add_column("Source Code", style="cyan")
     table.add_column("Machine Size", style="cyan")
 
     for deployment_spec in deployment_specs:
         source_code = (
-            deployment_spec.deployments[0].source_code.source_code_name if deployment_spec.deployments else '-'
+            deployment_spec.deployments[0].source_code.blob_artifact.name if deployment_spec.deployments else '-'
         )
         row = [
             deployment_spec.app_spec_name,
             deployment_spec.deployment_status,
             deployment_spec.execution_environment_spec.execution_environment_spec_name,
             source_code,
             deployment_spec.machine_size,
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/machine.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/main.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 )
 
 cli = SlingshotCLIApp(no_args_is_help=True, help=f"Slingshot AI CLI 🚀 ({__version__})")
 
 cli.add_command(add.add_component)
 cli.add_command(add.init)
 cli.add_command(apply.apply)
-cli.add_command(apply.plan)
 cli.add_command(apply.pull)
 cli.add_command(logs.logs)
 cli.add_command(machine.list_machines)
 
 cli.add_subcommands(auth.app, name="auth", help="Authenticate with Slingshot 👋", no_args_is_help=True)
 cli.add_subcommands(artifact.app, name="artifact", help="Manage artifacts 💾", no_args_is_help=True)
 cli.add_subcommands(code.app, name="code", help="Manage and push code 👩‍💻", no_args_is_help=True)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/project.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Optional
 
 import typer
 from rich.table import Table
 
 from ..sdk.config import client_settings, project_config
-from ..sdk.errors import SlingshotException
+from ..sdk.errors import SlingshotUnauthenticatedError
 from ..sdk.slingshot_sdk import SlingshotSDK
 from ..sdk.utils import console
 from ..shared.utils import SlingshotFileNotFoundException, load_slingshot_project_config
 from .config.slingshot_cli import SlingshotCLIApp
 from .shared import create_empty_project_manifest, prompt_for_single_choice
 
 app = SlingshotCLIApp()
@@ -48,15 +48,15 @@
         return
     await list_and_set_project_id(sdk)
 
 
 async def list_and_set_project_id(sdk_: SlingshotSDK) -> None:
     me = await sdk_.me()
     if not me:
-        raise SlingshotException("You must be logged in to use this command.")
+        raise SlingshotUnauthenticatedError()
     projects = me.projects
     if not projects:
         console.print("No projects found.")
         return  # Can't set a project ID if user has no projects
     choice = prompt_for_single_choice(
         f"Select the project you want to work on", [i.project_id for i in projects], skip_if_one_value=True
     )
@@ -66,18 +66,21 @@
 
 
 async def _set_project_id(sdk_: SlingshotSDK, project_id: str) -> None:
     old_project_id = project_config.project_id
     project_config.project_id = project_id
     if old_project_id != project_id:
         project_config.last_pushed_manifest = None
-    console.print(f"This directory is now associated with the project: [bold]{project_id}[/bold]")
+
+    directory = project_config.JSONConfig.settings_json_file.parent.parent
+
+    console.print(f"This directory ({directory}) is now associated with the project: [bold]{project_id}[/bold]")
     await sdk_.use_project(project_id)
 
     try:
         load_slingshot_project_config()
     except SlingshotFileNotFoundException:
         console.print("No 'slingshot.yaml' file found -- initializing one from the remote project manifest...")
 
         create_empty_project_manifest(client_settings.slingshot_config_path)
-        await sdk_.apply_to_local(force=True)
+        await sdk_.pull_remote_changes(force=True)
         console.print("Done.")
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/run.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import json
-from datetime import datetime, timezone
+from datetime import datetime
 from pathlib import Path
 from typing import Any, Literal, Optional
 
 import typer
 from rich.table import Table
 
 from .. import schemas
@@ -42,37 +42,29 @@
     config_file: Optional[str] = typer.Option(None, "--config", "-C", help="Path to config file for run."),
     debug: bool = typer.Option(False, "--debug", "-d", help="Run in debug mode.", hidden=True),
 ) -> None:
     """Start a run"""
     if debug:
         console.log("Debug mode enabled.")
 
-    _, await_env_specs = await sdk.apply_project()
+    await sdk.apply_project()
     source_code_id = await prompt_push_code(sdk)
 
     cli_args = parse_extra_args(ctx.args)
     config = await get_hyperparameter_config_from_file(Path(config_file)) if config_file else {}
     config = {**config, **cli_args}
 
     if not name:
         _, name = await prompt_for_app_spec(sdk, filter_for_runs, app_display_name="run")
 
     assert sdk.project
     run_spec = await sdk.api.get_app_spec_by_name(name, sdk.project.project_id)
     if not run_spec:
         raise SlingshotException(f"No run found with the name '{name}'")
 
-    await_env_spec_names = [spec.execution_environment_spec_name for spec in await_env_specs]
-    if run_spec.execution_environment_spec.execution_environment_spec_name in await_env_spec_names:
-        console.print(
-            "Waiting for environment "
-            f"'{run_spec.execution_environment_spec.execution_environment_spec_name}' to compile"
-        )
-        await sdk._wait_for_env_compile(run_spec.execution_environment_spec.execution_environment, should_print=True)
-
     new_run = await sdk.start_run(run_template_name=name, source_code_id=source_code_id, hyperparameters=config)
     link = await sdk.web_path_util.run(new_run)
     console.print(f"Run created with name '{new_run.run_name}', view in browser at {link}")
     console.print(
         f"Following logs. Ctrl-C to stop, and run 'slingshot run logs {new_run.run_name} --follow' to follow again"
     )
     await follow_run_logs_until_done(sdk, run_id=new_run.run_id)
@@ -109,29 +101,27 @@
 
     console.print(
         f"Restoring {len(restored_run_mounts)} mounts from previous run: {list(restored_run_mounts.values())}"
     )
     all_mounts_: dict[Any, MountSpec] = {**reference_mounts, **restored_run_mounts}  # Restored mounts take priority
     all_mounts: list[MountSpec] = list(all_mounts_.values())
     console.print(f"Run will start with {len(all_mounts)} mounts: {all_mounts}")
-    env = run.execution_environment
-    if not env:
-        # TODO: ENG-1062 This means that the run used an outdated env
-        raise SlingshotException(f"Run {run.run_name} cannot be restarted.")
     hyperparameters: dict[str, Any] | None = None
     if run.hyperparameters:
         hyperparameters = json.loads(run.hyperparameters)
+
     new_run = await sdk.start_run(
         run_template_name=reference_run_spec.app_spec_name,
         machine_size=schemas.MachineSize(run.machine_size),
         hyperparameters=hyperparameters,
         cmd=run.cmd,
         mount_specs=all_mounts,
-        exec_env_id=env.execution_environment_id,
+        environment_instance_id=run.environment_instance.environment_instance_id,
     )
+
     assert sdk.project
     link = await sdk.web_path_util.run(new_run)
     console.print(f"Run created with name '{new_run.run_name}', view in browser at {link}")
     console.print(
         f"Following logs. Ctrl-C to stop, and run 'slingshot run logs {new_run.run_name} --follow' to follow again"
     )
     await follow_run_logs_until_done(sdk=sdk, run_id=new_run.run_id)
@@ -196,22 +186,21 @@
     table.add_column("Environment", style="cyan")
     table.add_column("Source Code", style="cyan")
     table.add_column("Machine Size", style="cyan")
     table.add_column("Duration", style="cyan")
     for run in runs:
         duration_seconds = None
         if run.start_time and not run.end_time:
-            duration_seconds = (datetime.now(timezone.utc) - run.start_time).total_seconds()
+            duration_seconds = (datetime.utcnow() - run.start_time).total_seconds()
         elif run.start_time and run.end_time:
             duration_seconds = (run.end_time - run.start_time).total_seconds()
 
         row = [
             run.run_name,
             run.job_status,
-            # TODO: Fix this being nullable with ENG-1062
-            run.execution_environment.execution_environment_id if run.execution_environment else "--",
-            run.source_code.source_code_name,
+            run.environment_instance.execution_environment_spec.execution_environment_spec_name,
+            run.source_code.blob_artifact.name,
             run.machine_size,
             f"{seconds_to_human_readable(duration_seconds)}" if duration_seconds is not None else "N/A",
         ]
         table.add_row(*row)
     console.print(table)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/session.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
   {
    "cell_type": "code",
    "execution_count": null,
    "id": "f3d39bea-de51-48a4-adde-0af77fafb211",
    "metadata": {},
    "outputs": [],
    "source": [
-    "%load_ext autoreload\n",
+    "%load_ext autoreload\\n",
     "%autoreload 2"
    ]
   }
  ],
  "metadata": {
   "kernelspec": {
    "display_name": "Python 3 (ipykernel)",
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/code_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     p = "working directory" if sync_path.cwd().absolute() == sync_path.absolute() else sync_path
     for _ in range(3):  # retry 3 times
         console.print(f"[blue]Syncing {p} to your session...[/blue]")
         try:
             # run unison command in a subprocess
             # assumes ssh key is already added to the server authorized_keys
             with _open_log_file(verbose) as (stdout, stderr):
+                # TODO: support explicit selection of the SSH key
+                #  unison /local/path ssh://remote/path -sshcmd 'ssh -i /path/to/your_specific_key'
                 sh.unison(
                     str(sync_path),
                     f"ssh://slingshot@{hostname}:{ssh_port}//slingshot/session",  # sync to /slingshot/session
                     batch=True,  # batch mode: ask no questions at all
                     repeat="watch",  # synchronize repeatedly (using unison-fsmonitor process to detect changes)
                     prefer="newer",  # choose newer version for conflicting changes
                     copyonconflict=True,  # keep copies of conflicting files
@@ -98,14 +100,17 @@
                     _err=stderr,
                     _out=stdout,
                 )
         except sh.ErrorReturnCode:
             # TODO consider parsing the unison.log to e.g. automatically identify if it's a `Permission denied
             #  (publickey)` error
             console.print("[yellow]An error occurred while syncing your code. Retrying...[/yellow]")
+            console.print(
+                "[yellow]Please make sure the SSH key used for code sync has been added to the SSH agent[/yellow]"
+            )
             await asyncio.sleep(1)  # wait for a second before retrying
     raise SlingshotException(f"Error running unison, please check {Path.home()}/.slingshot/unison.log for more details")
 
 
 def _is_unison_installed() -> bool:
     _unison = shutil.which("unison") is not None
     if not _unison:
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,39 +25,62 @@
     return logline.log
 
 
 def merge_loglines(loglines: list[schemas.LogLine]) -> str:
     return "\n".join(format_logline(logline) for logline in loglines)
 
 
+async def quietly_cancel(task: asyncio.Task[Any]) -> None:
+    """Cancels a task and ignores the CancelledError exception"""
+    task.cancel()
+    try:
+        await task
+    except asyncio.CancelledError:
+        pass
+
+
 async def follow_run_logs_until_done(sdk: SlingshotSDK, run_id: str) -> None:
     task_logs = asyncio.create_task(sdk.print_logs(run_id=run_id, follow=True))
     task_status = asyncio.create_task(_wait_for_run_finished(sdk=sdk, run_id=run_id))
-    done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
-    for task in pending:
-        task.cancel()
+    # Wait for either task to finish
+    await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
+
+    # Case 1: task_status finished first. Either the run finished or task_status exception'd
+    if task_status.done():
+        await quietly_cancel(task_logs)
+        await task_status  # This should raise an exception iff the task_status exception'd
+        return
+
+    # Case 2: task_logs finished first. Something went wrong in task_logs. Let's raise the relevant exception
 
-    await asyncio.gather(*pending)
+    await quietly_cancel(task_status)  # task_status is no longer relevant, let's cancel it quietly
+    await task_logs  # This should raise an exception iff the task_logs exception'd
+
+    # Case 3: This should never happen. If it does, something is wrong
+    raise SlingshotException("Something went wrong while following logs. Please try again.")
 
 
 async def follow_app_logs_until_ready(sdk: SlingshotSDK, app_spec_id: str) -> schemas.AppInstanceStatus:
     task_logs = asyncio.create_task(sdk.print_logs(app_spec_id=app_spec_id, follow=True))
     task_status = asyncio.create_task(_wait_for_app_ready(sdk=sdk, app_spec_id=app_spec_id))
-    done, pending = await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
-    for task in pending:
-        task.cancel()
+    # Wait for either task to finish
+    await asyncio.wait([task_logs, task_status], return_when=asyncio.FIRST_COMPLETED)
 
-    status = None
-    try:
-        await asyncio.gather(*pending)
-        status = await task_status
-    except asyncio.CancelledError:
-        pass
+    # Case 1: task_status finished first. Either the run finished or task_status exception'd
+    if task_status.done():
+        await quietly_cancel(task_logs)
+        return await task_status  # This should raise an exception iff the task_status exception'd
+
+    # Case 2: task_logs finished first. Something went wrong in task_logs. Let's raise the relevant exception
+
+    await quietly_cancel(task_status)  # task_status is no longer relevant, let's cancel it quietly
+    await task_logs  # This should raise an exception iff the task_logs exception'd
 
-    return status or await follow_app_logs_until_ready(sdk=sdk, app_spec_id=app_spec_id)
+    # Case 3: This should never happen. If it does, something is wrong
+    raise SlingshotException("Something went wrong while following logs. Please try again.")
 
 
 def datetime_to_human_readable(dt: datetime) -> str:
     """Assumes UTC datetime and converts to local time in the format of: Mar 2, 2021 1:30AM EST"""
     date_str = dt.strftime('%b %d, %Y %I:%M:%S %p')
     return f'{date_str} UTC'
 
@@ -105,15 +128,15 @@
 
 async def prompt_push_code(sdk: SlingshotSDK) -> str | None:
     """Prompts the user to push code if it has changed since last push."""
     if not await sdk.has_code_changed() or not prompt_confirm(
         "Code has changed since last push. Do you want to push now?", default=True
     ):
         return None
-    source_code = await sdk.push_code(".", and_print=True)
+    source_code = await sdk.push_code(".", and_print=False)
     source_code_id = source_code.source_code_id
     return source_code_id
 
 
 async def get_hyperparameter_config_from_file(config_file: Path) -> JSONType:
     if not config_file.is_file():
         raise SlingshotException(
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.18rc1/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/generated/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # generated by datamodel-codegen:
 #   filename:  openapi-lock.json
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, PositiveInt, constr
 
 
 class AppSpecId(BaseModel):
     app_spec_id: str = Field(..., title='App Spec Id')
 
 
 class AppSubType(str, Enum):
+    REDIS = 'REDIS'
     SESSION = 'SESSION'
     LABEL_STUDIO = 'LABEL_STUDIO'
 
 
 class AppType(str, Enum):
     CUSTOM = 'CUSTOM'
     RUN = 'RUN'
@@ -28,29 +29,19 @@
 class Auth0Metadata(BaseModel):
     auth0_domain: str = Field(..., title='Auth0 Domain')
     auth0_client_id: str = Field(..., title='Auth0 Client Id')
 
 
 class AuthToken(BaseModel):
     token: str = Field(..., title='Token')
-    token_type: Literal['bearer'] = Field(..., title='Token Type')
+    token_type: str = Field('bearer', title='Token Type')
     user_id: str = Field(..., title='User Id')
     is_activated: bool = Field(..., title='Is Activated')
 
 
-class BlobArtifact(BaseModel):
-    blob_artifact_id: str = Field(..., title='Blob Artifact Id')
-    created_at: datetime = Field(..., title='Created At')
-    updated_at: datetime = Field(..., title='Updated At')
-    bytes_hash: str = Field(..., title='Bytes Hash')
-    bytes_size: int = Field(..., title='Bytes Size')
-    tag: Optional[str] = Field(None, title='Tag')
-    name: Optional[str] = Field(None, title='Name')
-
-
 class BlobArtifactFile(BaseModel):
     path: str = Field(..., title='Path')
     is_directory: Optional[bool] = Field(False, title='Is Directory')
     path_prefix: Optional[str] = Field(None, title='Path Prefix')
 
 
 class BlobArtifactId(BaseModel):
@@ -67,14 +58,19 @@
 
 
 class BlobArtifactUploadSignedURL(BaseModel):
     blob_artifact_id: str = Field(..., title='Blob Artifact Id')
     signed_url: str = Field(..., title='Signed Url')
 
 
+class BlobArtifactUploadSignedURLMany(BaseModel):
+    blob_artifact_id: str = Field(..., title='Blob Artifact Id')
+    filename_to_signed_url: Dict[str, str] = Field(..., title='Filename To Signed Url')
+
+
 class BodyAddUserToProject(BaseModel):
     username: str = Field(..., title='Username')
 
 
 class BodyCreateVolume(BaseModel):
     name: str = Field(..., title='Name')
 
@@ -82,50 +78,54 @@
 class BodyLoginToken(BaseModel):
     token: str = Field(..., title='Auth0 ID token')
     cli: Optional[bool] = Field(False, title='Cli')
 
 
 class BodyNewProject(BaseModel):
     project_id: constr(
-        regex=r'^[A-Za-z][A-Za-z0-9_-]*$', min_length=4, max_length=50
+        pattern=r'^[A-Za-z][A-Za-z0-9_-]*$', min_length=4, max_length=50
     ) = Field(
         ...,
         description='This is the unique name to be associated with your new project',
+        examples=['handwritten-digit-recognition'],
         title='Project ID',
     )
     display_name: constr(min_length=4, max_length=50) = Field(
         ...,
         description='An optional name for your project that will be shown in the UI',
+        examples=['Handwritten Digit Recognition'],
         title='Display Name',
     )
 
 
 class BodyPredictByName(BaseModel):
     example: bytes = Field(..., title='Example')
 
 
 class BodyPutSecret(BaseModel):
     secret_value: constr(min_length=1, max_length=4096) = Field(
-        ..., title='Secret Value'
+        ..., examples=['AKIAIOSFODNN7EXAMPLE'], title='Secret Value'
     )
 
 
 class BodySignup(BaseModel):
     signup_token: str = Field(..., title='Sign up token')
 
 
-class BodyUpdateSourceCode(BaseModel):
-    source_code_name: Optional[str] = Field(None, title='Source Code Name')
-    description: Optional[str] = Field(None, title='Source Code Description')
-
-
 class BodyUpdateSshPublicKey(BaseModel):
     ssh_public_key: str = Field(..., title='Ssh Public Key')
 
 
+class CreateEnvironmentSpec(BaseModel):
+    execution_environment_spec_id: str = Field(
+        ..., title='Execution Environment Spec Id'
+    )
+    is_new: bool = Field(..., title='Is New')
+
+
 class CreateServiceAccountResponse(BaseModel):
     service_account_id: str = Field(..., title='Service Account Id')
     key: str = Field(..., title='Key')
 
 
 class DeleteResult(str, Enum):
     NOT_FOUND = 'NOT_FOUND'
@@ -133,33 +133,33 @@
 
 
 class DeploymentInstanceId(BaseModel):
     deployment_id: str = Field(..., title='Deployment Id')
 
 
 class DownloadByNameMountSpecRequest(BaseModel):
-    path: constr(regex=r'/mnt/(?!slingshot).+') = Field(
+    path: constr(pattern=r'/mnt/\w+') = Field(
         ..., description='The path to mount into the environment.', title='Path'
     )
-    mode: Literal['DOWNLOAD'] = Field(
-        ..., description='The mode to use for the mount.', title='Mode'
+    mode: str = Field(
+        'DOWNLOAD', description='The mode to use for the mount.', title='Mode'
     )
     name: str = Field(
         ...,
         description='The name of the asset to mount. Either name or tag should be set, but not both.',
         title='Name',
     )
 
 
 class DownloadByTagMountSpecRequest(BaseModel):
-    path: constr(regex=r'/mnt/(?!slingshot).+') = Field(
+    path: constr(pattern=r'/mnt/\w+') = Field(
         ..., description='The path to mount into the environment.', title='Path'
     )
-    mode: Literal['DOWNLOAD'] = Field(
-        ..., description='The mode to use for the mount.', title='Mode'
+    mode: str = Field(
+        'DOWNLOAD', description='The mode to use for the mount.', title='Mode'
     )
     tag: str = Field(
         ...,
         description='The artifact selector. If multiple matching artifacts contain the tag, the latest one will be used.  Either name or tag should be set, but not both.',
         title='Tag',
     )
 
@@ -168,15 +168,15 @@
     unknown = 'unknown'
     invalid_signup_token = 'invalid_signup_token'
     username_already_taken = 'username_already_taken'
     deployment_not_deployed = 'deployment_not_deployed'
     app_already_started = 'app_already_started'
     app_already_exists = 'app_already_exists'
     app_is_deleted = 'app_is_deleted'
-    exec_env_not_found = 'exec_env_not_found'
+    environment_instance_not_found = 'environment_instance_not_found'
     volume_does_not_exist = 'volume_does_not_exist'
     volume_is_locked = 'volume_is_locked'
     volume_already_exists = 'volume_already_exists'
     volume_name_invalid = 'volume_name_invalid'
     artifact_is_unzipping = 'artifact_is_unzipping'
     entity_does_not_exist = 'entity_does_not_exist'
     multiple_gpus_not_allowed = 'multiple_gpus_not_allowed'
@@ -197,33 +197,27 @@
 
 class EvaluationTestSetResultId(BaseModel):
     evaluation_test_set_result_id: str = Field(
         ..., title='Evaluation Test Set Result Id'
     )
 
 
-class ExecutionEnvironmentSpecId(BaseModel):
-    execution_environment_spec_id: str = Field(
-        ..., title='Execution Environment Spec Id'
-    )
-
-
 class GpuType(str, Enum):
     T4 = 'T4'
     L4 = 'L4'
     A100 = 'A100'
     CPU = 'CPU'
 
 
 class HasAppInstanceId(BaseModel):
     app_instance_id: str = Field(..., title='App Instance Id')
 
 
 class Healthcheck(BaseModel):
-    db: Literal['OK'] = Field(..., title='Db')
+    db: str = Field('OK', title='Db')
 
 
 class HttpErrorBody(BaseModel):
     error: str = Field(..., title='Error')
 
 
 class LatencyQuantiles(BaseModel):
@@ -267,15 +261,15 @@
     CPU_TINY = 'CPU_TINY'
     CPU_SMALL = 'CPU_SMALL'
     CPU_MEDIUM = 'CPU_MEDIUM'
     CPU_LARGE = 'CPU_LARGE'
 
 
 class OpenAIChatRequest(BaseModel):
-    type: Optional[Literal['chat']] = Field('chat', title='Type')
+    type: str = Field('chat', title='Type')
     model: str = Field(..., title='Model')
     messages: List[Dict[str, str]] = Field(..., title='Messages')
     temperature: Optional[float] = Field(None, title='Temperature')
     top_p: Optional[float] = Field(None, title='Top P')
     n: Optional[int] = Field(None, title='N')
     stop: Optional[Union[str, List[str]]] = Field(None, title='Stop')
     max_tokens: Optional[int] = Field(None, title='Max Tokens')
@@ -290,20 +284,20 @@
     message: Dict[str, str] = Field(..., title='Message')
     finish_reason: str = Field(..., title='Finish Reason')
 
 
 class OpenAICompletionChoice(BaseModel):
     text: str = Field(..., title='Text')
     index: int = Field(..., title='Index')
-    logprobs: Optional[Any] = Field(None, title='Logprobs')
+    logprobs: Any = Field(None, title='Logprobs')
     finish_reason: str = Field(..., title='Finish Reason')
 
 
 class OpenAICompletionRequest(BaseModel):
-    type: Optional[Literal['completion']] = Field('completion', title='Type')
+    type: str = Field('completion', title='Type')
     model: str = Field(..., title='Model')
     prompt: Optional[Union[str, List]] = Field(None, title='Prompt')
     suffix: Optional[str] = Field(None, title='Suffix')
     max_tokens: Optional[int] = Field(None, title='Max Tokens')
     temperature: Optional[float] = Field(None, title='Temperature')
     top_p: Optional[float] = Field(None, title='Top P')
     n: Optional[int] = Field(None, title='N')
@@ -320,15 +314,15 @@
 class OpenAIEmbeddingObject(BaseModel):
     object: str = Field(..., title='Object')
     embedding: List[float] = Field(..., title='Embedding')
     index: int = Field(..., title='Index')
 
 
 class OpenAIEmbeddingRequest(BaseModel):
-    type: Optional[Literal['embedding']] = Field('embedding', title='Type')
+    type: str = Field('embedding', title='Type')
     model: str = Field(..., title='Model')
     input: Union[str, List] = Field(..., title='Input')
     user: Optional[str] = Field(None, title='User')
 
 
 class OpenAIUsage(BaseModel):
     prompt_tokens: int = Field(..., title='Prompt Tokens')
@@ -345,15 +339,15 @@
 class ProjectId(BaseModel):
     project_id: str = Field(..., title='Project Id')
 
 
 class PromptOpenAIBody(BaseModel):
     openai_request: Union[
         OpenAIChatRequest, OpenAICompletionRequest, OpenAIEmbeddingRequest
-    ] = Field(..., discriminator='type', title='Openai Request')
+    ] = Field(..., title='Openai Request')
     idempotence_key: Optional[constr(max_length=32)] = Field(
         None,
         description='If specified, the request will be idempotent. If a previous request with the same idempotence key is pending, the previous response will be returned instead of sending a new request to OpenAI. If absent, the request will be sent to OpenAI regardless of whether a previous request with the same parameters is pending.',
         title='Idempotence Key',
     )
     active_throttling: Optional[Union[bool, PositiveInt]] = Field(
         False,
@@ -368,28 +362,28 @@
     NO_CHANGE = 'NO_CHANGE'
 
 
 class RequestedAptPackage(BodyCreateVolume):
     pass
 
 
-class Pin(str, Enum):
+class PinEnum(str, Enum):
     field__ = '=='
     field_ = '@'
     field___1 = '>='
     field___2 = '<='
     field__1 = '>'
     field__2 = '<'
     field___3 = '~='
 
 
 class RequestedRequirement(BaseModel):
     library: str = Field(..., title='Library')
     version: Optional[str] = Field(None, title='Version')
-    pin: Optional[Pin] = Field(None, title='Pin')
+    pin: Optional[PinEnum] = Field(None, title='Pin')
 
 
 class RunCreate(BaseModel):
     run_id: str = Field(..., title='Run Id')
     run_name: str = Field(..., title='Run Name')
     created_at: datetime = Field(..., title='Created At')
 
@@ -397,30 +391,16 @@
 class ServiceAccountToken(BaseModel):
     token: str = Field(..., title='Token')
     service_account_id: str = Field(..., title='Service Account Id')
 
 
 class SlingshotLogicalError(BaseModel):
     message: str = Field(..., title='Message')
-    code: ErrorCode
-    metadata: Dict[str, str] = Field(..., title='Metadata')
-
-
-class SourceCode(BaseModel):
-    source_code_id: str = Field(..., title='Source Code Id')
-    source_code_name: str = Field(..., title='Source Code Name')
-    description: Optional[str] = Field(None, title='Description')
-    project_id: str = Field(..., title='Project Id')
-    created_at: datetime = Field(..., title='Created At')
-    blob_artifact: BlobArtifact
-
-
-class SourceCodeResponse(BaseModel):
-    data: Optional[SourceCode] = None
-    error: Optional[SlingshotLogicalError] = None
+    code: Optional[ErrorCode] = 'unknown'
+    metadata: Optional[Dict[str, str]] = Field(None, title='Metadata')
 
 
 class SshPort(BaseModel):
     ssh_port: int = Field(..., title='Ssh Port')
 
 
 class SshPortResponse(BaseModel):
@@ -435,20 +415,25 @@
 
 class UploadBlobArtifactBody(BaseModel):
     filename: str = Field(..., title='Filename')
     is_zipped_directory: bool = Field(..., title='Is Zipped Directory')
     tag: Optional[str] = Field(None, title='Tag')
 
 
+class UploadBlobArtifactManyBody(BaseModel):
+    filenames: List[str] = Field(..., title='Filenames')
+    tag: Optional[str] = Field(None, title='Tag')
+
+
 class UploadMountSpecRequest(BaseModel):
-    path: constr(regex=r'/mnt/(?!slingshot).+') = Field(
+    path: constr(pattern=r'/mnt/\w+') = Field(
         ..., description='The path to mount into the environment.', title='Path'
     )
-    mode: Literal['UPLOAD'] = Field(
-        ..., description='The mode to use for the mount.', title='Mode'
+    mode: str = Field(
+        'UPLOAD', description='The mode to use for the mount.', title='Mode'
     )
     tag: Optional[str] = Field(
         None, description='Optional tag to attach to the written artifact.', title='Tag'
     )
 
 
 class UploadedSourceCode(BaseModel):
@@ -470,19 +455,19 @@
 class ValidationError(BaseModel):
     loc: List[Union[str, int]] = Field(..., title='Location')
     msg: str = Field(..., title='Message')
     type: str = Field(..., title='Error Type')
 
 
 class VolumeMountSpecRequest(BaseModel):
-    path: constr(regex=r'/mnt/(?!slingshot).+') = Field(
+    path: constr(pattern=r'/mnt/\w+') = Field(
         ..., description='The path to mount into the environment.', title='Path'
     )
-    mode: Literal['VOLUME'] = Field(
-        ..., description='The mode to use for the mount.', title='Mode'
+    mode: str = Field(
+        'VOLUME', description='The mode to use for the mount.', title='Mode'
     )
     name: str = Field(..., description='The name of the volume to mount.', title='Name')
 
 
 class AppSpecIdResponse(BaseModel):
     data: Optional[AppSpecId] = None
     error: Optional[SlingshotLogicalError] = None
@@ -499,21 +484,21 @@
 
 
 class BlobArtifactIdResponse(BaseModel):
     data: Optional[BlobArtifactId] = None
     error: Optional[SlingshotLogicalError] = None
 
 
-class BlobArtifactSignedURLManyResponse(BaseModel):
-    data: Optional[List[BlobArtifactSignedURL]] = Field(None, title='Data')
+class BlobArtifactSignedURLResponse(BaseModel):
+    data: Optional[BlobArtifactSignedURL] = None
     error: Optional[SlingshotLogicalError] = None
 
 
-class BlobArtifactSignedURLResponse(BaseModel):
-    data: Optional[BlobArtifactSignedURL] = None
+class BlobArtifactUploadSignedURLManyResponse(BaseModel):
+    data: Optional[BlobArtifactUploadSignedURLMany] = None
     error: Optional[SlingshotLogicalError] = None
 
 
 class BlobArtifactUploadSignedURLResponse(BaseModel):
     data: Optional[BlobArtifactUploadSignedURL] = None
     error: Optional[SlingshotLogicalError] = None
 
@@ -537,23 +522,21 @@
         ]
     ] = Field(..., title='Mounts')
     config_variables: Optional[Dict[str, Any]] = Field(None, title='Config Variables')
     app_port: Optional[int] = Field(None, title='App Port')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
     soft_concurrency: Optional[PositiveInt] = Field(None, title='Soft Concurrency')
-    name: constr(regex=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(..., title='Name')
+    name: constr(pattern=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(..., title='Name')
     app_type: AppType
     app_sub_type: Optional[AppSubType] = None
 
 
 class CreateEnvironmentSpecResponse(BaseModel):
-    data: Optional[List[Union[ExecutionEnvironmentSpecId, bool]]] = Field(
-        None, max_items=2, min_items=2, title='Data'
-    )
+    data: Optional[CreateEnvironmentSpec] = None
     error: Optional[SlingshotLogicalError] = None
 
 
 class CreateServiceAccountResponseResponse(BaseModel):
     data: Optional[CreateServiceAccountResponse] = None
     error: Optional[SlingshotLogicalError] = None
 
@@ -575,31 +558,31 @@
 
 class EvaluationTestSetResultIdResponse(BaseModel):
     data: Optional[EvaluationTestSetResultId] = None
     error: Optional[SlingshotLogicalError] = None
 
 
 class ExecutionEnvironmentSpecRequestBody(BaseModel):
-    name: constr(regex=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(
+    name: constr(pattern=r'^[A-Za-z][A-Za-z0-9_-]*$') = Field(
         ..., description='Name of the environment.', title='Name'
     )
     python_packages: List[RequestedRequirement] = Field(
         ...,
         description='List of Python packages to install in the environment.',
         title='Python packages',
     )
     apt_packages: List[RequestedAptPackage] = Field(
         ...,
         description='List of APT packages to install in the environment.',
         title='APT packages',
     )
-    gpu_drivers: bool = Field(
-        ...,
-        description='Flag to install GPU drivers in the environment.',
-        title='GPU Drivers',
+    post_install_command: Optional[str] = Field(
+        None,
+        description='Custom command to run after installing packages.',
+        title='Post-install command',
     )
     force_create_environment: Optional[bool] = Field(
         False,
         description='Whether to require that a new environment be created. Otherwise, an existing environment will be used if it is compatible.',
         title='Force Create Environment',
     )
 
@@ -621,20 +604,25 @@
 
 
 class HealthcheckResponse(BaseModel):
     data: Optional[Healthcheck] = None
     error: Optional[SlingshotLogicalError] = None
 
 
-class ListBlobArtifactFilesResponse(BaseModel):
+class ListBlobArtifactFileResponse(BaseModel):
     data: Optional[List[BlobArtifactFile]] = Field(None, title='Data')
     error: Optional[SlingshotLogicalError] = None
 
 
-class LogsResponse(BaseModel):
+class ListBlobArtifactSignedURLResponse(BaseModel):
+    data: Optional[List[BlobArtifactSignedURL]] = Field(None, title='Data')
+    error: Optional[SlingshotLogicalError] = None
+
+
+class ListLogLineResponse(BaseModel):
     data: Optional[List[LogLine]] = Field(None, title='Data')
     error: Optional[SlingshotLogicalError] = None
 
 
 class MachineTypeDetails(BaseModel):
     display_name: str = Field(..., title='Display Name')
     gpu_count_machine_sizes: List[GpuCountMachineSize] = Field(
@@ -693,15 +681,15 @@
 
 class PutResultResponse(BaseModel):
     data: Optional[PutResult] = None
     error: Optional[SlingshotLogicalError] = None
 
 
 class ResponseOK(BaseModel):
-    data: Optional[Literal['OK']] = Field('OK', title='Data')
+    data: str = Field('OK', title='Data')
     error: Optional[SlingshotLogicalError] = None
 
 
 class RunCreateResponse(BaseModel):
     data: Optional[RunCreate] = None
     error: Optional[SlingshotLogicalError] = None
 
@@ -718,15 +706,15 @@
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
-    exec_env_id: str = Field(..., title='Exec Env Id')
+    environment_instance_id: str = Field(..., title='Environment Instance Id')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: Optional[str] = Field(None, title='Source Code Id')
     app_port: Optional[int] = Field(None, title='App Port')
     cmd: Optional[str] = Field(None, title='Cmd')
 
 
 class StartDeploymentBody(BaseModel):
@@ -736,15 +724,15 @@
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
-    exec_env_id: str = Field(..., title='Exec Env Id')
+    environment_instance_id: str = Field(..., title='Environment Instance Id')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
     cmd: str = Field(..., title='Cmd')
     batch_size: Optional[PositiveInt] = Field(None, title='Batch Size')
     batch_interval: Optional[PositiveInt] = Field(None, title='Batch Interval')
 
 
@@ -755,15 +743,15 @@
         Union[
             DownloadByNameMountSpecRequest,
             DownloadByTagMountSpecRequest,
             UploadMountSpecRequest,
             VolumeMountSpecRequest,
         ]
     ] = Field(..., title='Mounts')
-    exec_env_id: str = Field(..., title='Exec Env Id')
+    environment_instance_id: str = Field(..., title='Environment Instance Id')
     attach_project_credentials: bool = Field(..., title='Attach Project Credentials')
     source_code_id: str = Field(..., title='Source Code Id')
     cmd: str = Field(..., title='Cmd')
 
 
 class UpdateAppBody(BaseModel):
     command: Optional[str] = Field(None, title='Command')
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/schema_extensions.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,44 +34,44 @@
 
 import re
 import uuid
 from datetime import datetime
 from enum import Enum
 from typing import Any, Generic, Literal, Optional, Protocol, TypeVar, Union
 
-from pydantic import BaseModel, Field, validator
-from pydantic.generics import GenericModel
+from pydantic import BaseModel, ConfigDict, Field, field_validator
+from pydantic_core.core_schema import FieldValidationInfo
 
 from .generated import schemas
 
 Hyperparameter = dict[str, Any]
 
 DataT = TypeVar("DataT")
 
 
-class Response(GenericModel, Generic[DataT]):
-    data: Optional[DataT]
-    error: Optional[schemas.SlingshotLogicalError]
+class Response(BaseModel, Generic[DataT]):
+    data: Optional[DataT] = None
+    error: Optional[schemas.SlingshotLogicalError] = None
 
 
 class RequirementsParsingError(ValueError):
     pass
 
 
 class RequestedRequirement(BaseModel):
     library: str
-    version: Optional[str]
-    pin: Optional[Literal["==", "@", ">=", "<=", ">", "<", "~="]]
+    version: Optional[str] = None
+    pin: Optional[Literal["==", "@", ">=", "<=", ">", "<", "~="]] = None
 
     # Pin must be present iff version is present
-    @validator("pin")
-    def pin_must_be_present_iff_version_is_present(cls, v: str | None, values: dict[str, Any]) -> object:
-        if v is None and values["version"] is not None:
+    @field_validator("pin")
+    def pin_must_be_present_iff_version_is_present(cls, v: str | None, info: FieldValidationInfo) -> object:
+        if v is None and info.data.get("version") is not None:
             raise ValueError("pin must be present if version is present")
-        if v is not None and values["version"] is None:
+        if v is not None and info.data.get("version") is None:
             raise ValueError("version must be present if pin is present")
         return v
 
     @classmethod
     def from_str(cls, line: str) -> RequestedRequirement:
         if not line:
             raise RequirementsParsingError("empty requirement")
@@ -170,16 +170,16 @@
     schemas.DownloadByNameMountSpecRequest,
     schemas.DownloadByTagMountSpecRequest,
 ]
 
 
 class AuthTokenUnion(BaseModel):
     token: str
-    user_id: Optional[str]
-    service_account_id: Optional[str]
+    user_id: Optional[str] = None
+    service_account_id: Optional[str] = None
 
     @classmethod
     def from_auth_token(cls, auth_token: schemas.AuthToken) -> AuthTokenUnion:
         return cls(token=auth_token.token, user_id=auth_token.user_id, service_account_id=None)
 
     @classmethod
     def from_service_account_token(cls, service_account_token: schemas.ServiceAccountToken) -> AuthTokenUnion:
@@ -191,40 +191,41 @@
     def is_service_account(self) -> bool:
         return self.service_account_id is not None
 
     @property
     def is_user(self) -> bool:
         return self.user_id is not None
 
-    @validator("service_account_id")
-    def validate_xor(cls, v: str | None, values: dict[str, Any]) -> str | None:
-        if v is None and values["user_id"] is None:
+    @field_validator("service_account_id")
+    def validate_xor(cls, v: str | None, info: FieldValidationInfo) -> str | None:
+        if v is None and info.data.get("user_id") is None:
             raise ValueError("Both service_account_id and user_id cannot be None")
-        if v is not None and values["user_id"] is not None:
+        if v is not None and info.data.get("user_id") is not None:
             raise ValueError("Both service_account_id and user_id cannot be set")
         return v
 
 
 # Note: these are copied from the backend schemas, but should ideally be generated from those.
 class Data(BaseModel):
     """
     This can store any data. E.g. if you have a question and a context, you can store them concatenated in text,
     and then split them by key here to get the individual values.
     """
 
-    image_url: Optional[str] = Field(
-        None, alias="imageUrl", description="URL to an image, e.g. a signed URL, if relevant"
-    )
-    image_base64: Optional[str] = Field(None, alias="imageBase64")
-    path: Optional[str] = Field(None, description="Path to the file within the dataset artifact directory, if relevant")
     text: Optional[str] = None
 
-    class Config:
-        extra = "allow"  # This allows fields not specified in the model
-        allow_population_by_field_name = True  # This allows fields to be populated by their alias
+    file_path: Optional[str] = Field(
+        None, alias="filePath", description="Path to the file within the dataset artifact directory, if relevant"
+    )
+    media_url: Optional[str] = Field(
+        None, alias="mediaUrl", description="URL for the data, e.g. a signed URL, if relevant"
+    )
+    media_base64: Optional[str] = Field(None, alias="mediaBase64", description="Base64 encoded data, if relevant")
+
+    model_config = ConfigDict(extra='allow', populate_by_name=True)
 
 
 class Result(BaseModel):
     """
     This is the "Y", i.e. the thing you want to predict.
     """
 
@@ -245,17 +246,15 @@
     #  # For classification, this is {[class:string]:boolean}
     value: dict[str, Any] = Field(
         ...,
         description="The content of the annotation result. For example, for classification, this would be a "
         "dictionary of class names to booleans",
     )
 
-    class Config:
-        allow_population_by_field_name = True  # This allows fields to be populated by their alias
-        extra = "allow"  # E.g. for a model prediction, confidence can go here
+    model_config = ConfigDict(extra='allow', populate_by_name=True)
 
 
 class Annotation(BaseModel):
     annotation_id: str = Field(
         default_factory=lambda: uuid.uuid4().hex[:8], alias="annotationId"
     )  # UUID generated by the end-user
     result: list[Result] = Field(..., description="The annotation result")
@@ -263,47 +262,43 @@
         default_factory=datetime.utcnow, alias="createdAt", description="When the annotation was created"
     )
     updated_at: Optional[datetime] = Field(
         default_factory=datetime.utcnow, alias="updatedAt", description="When the annotation was last updated"
     )
     annotator: Optional[str] = Field(None, alias="annotator", description="The ID or name of the annotator")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Prediction(Annotation):
     model: Optional[str] = Field(None, alias="model", description="The ID or name of the model")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Example(BaseModel):
     example_id: str = Field(
         default_factory=lambda: uuid.uuid4().hex[:8], alias="exampleId"
     )  # UUID generated by the end-user
     created_at: Optional[datetime] = Field(default_factory=datetime.utcnow, alias="createdAt")
     updated_at: Optional[datetime] = Field(default_factory=datetime.utcnow, alias="updatedAt")
     data: Data
     annotations: list[Annotation] = Field(default_factory=list)
     predictions: list[Prediction] = Field(default_factory=list)
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class ExampleModification(BaseModel):
     example_id: str = Field(..., alias="exampleId")
     modified_data: Optional[Data] = Field(None, alias="modifiedData")
     new_annotations: list[Annotation] = Field(default_factory=list, alias="newAnnotations")
     new_predictions: list[Prediction] = Field(default_factory=list, alias="newPredictions")
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Upsert(BaseModel):
     """
     Upserts are used to update the dataset
     """
 
@@ -312,16 +307,15 @@
     modified_examples: list[ExampleModification] = Field(default_factory=list, alias="modifiedExamples")
     updated_at: datetime = Field(
         default_factory=datetime.utcnow,
         alias="updatedAt",
         description="The time at which the upsert was created. Defaults to now.",
     )
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Dataset(BaseModel):
     """
     Dataset is a JSONL of examples
     """
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7055431547619048%*

 * *Differences: {"'$defs'": "OrderedDict([('DeploymentSpec', OrderedDict([('example', OrderedDict([('environment', "*

 * *            "'deployment')])), ('properties', OrderedDict([('name', OrderedDict([('default', "*

 * *            "'deployment'), ('description', 'The name of the deployment.'), ('title', 'Name'), "*

 * *            "('type', 'string')])), ('environment', OrderedDict([('description', 'The name of the "*

 * *            "execution environment.'), ('title', 'Environment'), ('type', 'string')])), "*

 * *            "('machine_type', […]*

```diff
@@ -1,11 +1,9 @@
 {
-    "$id": "https://github.com/slingshot-ai/slingshot/blob/main/slingshot_client/src/slingshot/schemas/slingshot-schema.config.json",
-    "$schema": "http://json-schema.org/draft/2020-12/schema",
-    "definitions": {
+    "$defs": {
         "DeploymentSpec": {
             "example": {
                 "environment": "deployment"
             },
             "properties": {
                 "attach_project_credentials": {
                     "default": true,
@@ -27,36 +25,36 @@
                     "description": "The name of the execution environment.",
                     "title": "Environment",
                     "type": "string"
                 },
                 "machine_type": {
                     "allOf": [
                         {
-                            "$ref": "#/definitions/MachineType"
+                            "$ref": "#/$defs/MachineType"
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
                     "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
-                                "$ref": "#/definitions/DownloadByNameMountSpec"
+                                "$ref": "#/$defs/DownloadByNameMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/DownloadByTagMountSpec"
+                                "$ref": "#/$defs/DownloadByTagMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/UploadMountSpec"
+                                "$ref": "#/$defs/UploadMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/VolumeMountSpec"
+                                "$ref": "#/$defs/VolumeMountSpec"
                             }
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
@@ -78,55 +76,49 @@
             ],
             "title": "Deployment",
             "type": "object"
         },
         "DownloadByNameMountSpec": {
             "properties": {
                 "mode": {
+                    "const": "DOWNLOAD",
                     "default": "DOWNLOAD",
                     "description": "The mode to use for the mount.",
-                    "enum": [
-                        "DOWNLOAD"
-                    ],
-                    "title": "Mode",
-                    "type": "string"
+                    "title": "Mode"
                 },
                 "name": {
                     "description": "The name of the asset to mount. Either name or tag should be set, but not both.",
                     "title": "Name",
                     "type": "string"
                 },
                 "path": {
                     "description": "The path to mount into the environment.",
-                    "pattern": "/mnt/(?!slingshot).+",
+                    "pattern": "/mnt/\\w+",
                     "title": "Path",
                     "type": "string"
                 }
             },
             "required": [
                 "path",
                 "name"
             ],
             "title": "DownloadByNameMountSpec",
             "type": "object"
         },
         "DownloadByTagMountSpec": {
             "properties": {
                 "mode": {
+                    "const": "DOWNLOAD",
                     "default": "DOWNLOAD",
                     "description": "The mode to use for the mount.",
-                    "enum": [
-                        "DOWNLOAD"
-                    ],
-                    "title": "Mode",
-                    "type": "string"
+                    "title": "Mode"
                 },
                 "path": {
                     "description": "The path to mount into the environment.",
-                    "pattern": "/mnt/(?!slingshot).+",
+                    "pattern": "/mnt/\\w+",
                     "title": "Path",
                     "type": "string"
                 },
                 "tag": {
                     "description": "The artifact selector. If multiple matching artifacts contain the tag, the latest one will be used.  Either name or tag should be set, but not both.",
                     "title": "Tag",
                     "type": "string"
@@ -137,45 +129,48 @@
                 "tag"
             ],
             "title": "DownloadByTagMountSpec",
             "type": "object"
         },
         "EnvironmentSpec": {
             "example": {
-                "gpu_drivers": true,
                 "python_packages": [
                     "numpy",
-                    "pandas"
+                    "pandas",
+                    "torch==2.0.1"
                 ],
                 "python_version": "3.10"
             },
             "properties": {
                 "apt_packages": {
                     "description": "List of APT packages to install",
                     "items": {
                         "type": "string"
                     },
                     "title": "APT packages",
                     "type": "array"
                 },
+                "post_install_command": {
+                    "default": "",
+                    "description": "Custom command to run after all packages have been installed. Skipped if not specified.",
+                    "title": "Post-install command",
+                    "type": "string"
+                },
                 "python_packages": {
                     "description": "List of Python packages to install in the environment.",
                     "items": {
                         "type": "string"
                     },
                     "title": "Python packages",
                     "type": "array"
                 },
                 "python_version": {
                     "anyOf": [
                         {
-                            "enum": [
-                                "3.10"
-                            ],
-                            "type": "string"
+                            "const": "3.10"
                         },
                         {
                             "maximum": 3.1,
                             "minimum": 3.1,
                             "type": "number"
                         }
                     ],
@@ -183,27 +178,105 @@
                     "title": "Python version"
                 }
             },
             "title": "Environment",
             "type": "object"
         },
         "MachineType": {
-            "description": "An enumeration.",
             "enum": [
                 "T4",
                 "L4",
                 "A100",
                 "CPU_TINY",
                 "CPU_SMALL",
                 "CPU_MEDIUM",
                 "CPU_LARGE"
             ],
             "title": "MachineType",
             "type": "string"
         },
+        "RedisAppSpec": {
+            "example": {
+                "cmd": "python app.py",
+                "environment": "slackbot"
+            },
+            "properties": {
+                "attach_project_credentials": {
+                    "default": true,
+                    "description": "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environmentvariable so that they can make requests using the Slingshot SDK for this project",
+                    "title": "Attach project credentials",
+                    "type": "boolean"
+                },
+                "config_variables": {
+                    "description": "Optional user defined arguments to pass to the app.",
+                    "title": "Arguments",
+                    "type": "object"
+                },
+                "environment": {
+                    "description": "The name of the execution environment.",
+                    "title": "Environment",
+                    "type": "string"
+                },
+                "machine_type": {
+                    "allOf": [
+                        {
+                            "$ref": "#/$defs/MachineType"
+                        }
+                    ],
+                    "default": "CPU_SMALL",
+                    "description": "The machine size to be used.",
+                    "title": "Machine size"
+                },
+                "mounts": {
+                    "description": "The mounts to be attached.",
+                    "items": {
+                        "anyOf": [
+                            {
+                                "$ref": "#/$defs/DownloadByNameMountSpec"
+                            },
+                            {
+                                "$ref": "#/$defs/DownloadByTagMountSpec"
+                            },
+                            {
+                                "$ref": "#/$defs/UploadMountSpec"
+                            },
+                            {
+                                "$ref": "#/$defs/VolumeMountSpec"
+                            }
+                        ]
+                    },
+                    "title": "Mounts",
+                    "type": "array"
+                },
+                "name": {
+                    "description": "The name of the app.",
+                    "pattern": "^[A-Za-z][A-Za-z0-9_-]*$",
+                    "title": "Name",
+                    "type": "string"
+                },
+                "num_gpu": {
+                    "default": 0,
+                    "description": "The number of GPUs to use.",
+                    "title": "Number of GPUs",
+                    "type": "integer"
+                },
+                "using": {
+                    "const": "redis",
+                    "description": "Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
+                    "title": "Using"
+                }
+            },
+            "required": [
+                "name",
+                "environment",
+                "using"
+            ],
+            "title": "App",
+            "type": "object"
+        },
         "RunSpec": {
             "example": {
                 "cmd": "python train.py",
                 "environment": "training"
             },
             "properties": {
                 "attach_project_credentials": {
@@ -226,36 +299,36 @@
                     "description": "The name of the execution environment.",
                     "title": "Environment",
                     "type": "string"
                 },
                 "machine_type": {
                     "allOf": [
                         {
-                            "$ref": "#/definitions/MachineType"
+                            "$ref": "#/$defs/MachineType"
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
                     "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
-                                "$ref": "#/definitions/DownloadByNameMountSpec"
+                                "$ref": "#/$defs/DownloadByNameMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/DownloadByTagMountSpec"
+                                "$ref": "#/$defs/DownloadByTagMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/UploadMountSpec"
+                                "$ref": "#/$defs/UploadMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/VolumeMountSpec"
+                                "$ref": "#/$defs/VolumeMountSpec"
                             }
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
@@ -299,36 +372,36 @@
                     "description": "The name of the execution environment.",
                     "title": "Environment",
                     "type": "string"
                 },
                 "machine_type": {
                     "allOf": [
                         {
-                            "$ref": "#/definitions/MachineType"
+                            "$ref": "#/$defs/MachineType"
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
                     "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
-                                "$ref": "#/definitions/DownloadByNameMountSpec"
+                                "$ref": "#/$defs/DownloadByNameMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/DownloadByTagMountSpec"
+                                "$ref": "#/$defs/DownloadByTagMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/UploadMountSpec"
+                                "$ref": "#/$defs/UploadMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/VolumeMountSpec"
+                                "$ref": "#/$defs/VolumeMountSpec"
                             }
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
@@ -340,20 +413,17 @@
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
                     "type": "integer"
                 },
                 "using": {
+                    "const": "session",
                     "description": "Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
-                    "enum": [
-                        "session"
-                    ],
-                    "title": "Using",
-                    "type": "string"
+                    "title": "Using"
                 }
             },
             "required": [
                 "name",
                 "environment",
                 "using"
             ],
@@ -386,36 +456,36 @@
                     "description": "The name of the execution environment.",
                     "title": "Environment",
                     "type": "string"
                 },
                 "machine_type": {
                     "allOf": [
                         {
-                            "$ref": "#/definitions/MachineType"
+                            "$ref": "#/$defs/MachineType"
                         }
                     ],
                     "default": "CPU_SMALL",
                     "description": "The machine size to be used.",
                     "title": "Machine size"
                 },
                 "mounts": {
                     "description": "The mounts to be attached.",
                     "items": {
                         "anyOf": [
                             {
-                                "$ref": "#/definitions/DownloadByNameMountSpec"
+                                "$ref": "#/$defs/DownloadByNameMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/DownloadByTagMountSpec"
+                                "$ref": "#/$defs/DownloadByTagMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/UploadMountSpec"
+                                "$ref": "#/$defs/UploadMountSpec"
                             },
                             {
-                                "$ref": "#/definitions/VolumeMountSpec"
+                                "$ref": "#/$defs/VolumeMountSpec"
                             }
                         ]
                     },
                     "title": "Mounts",
                     "type": "array"
                 },
                 "name": {
@@ -427,123 +497,135 @@
                 "num_gpu": {
                     "default": 0,
                     "description": "The number of GPUs to use.",
                     "title": "Number of GPUs",
                     "type": "integer"
                 },
                 "port": {
+                    "anyOf": [
+                        {
+                            "type": "integer"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
                     "description": "The port to expose.",
-                    "title": "Port",
-                    "type": "integer"
+                    "title": "Port"
                 }
             },
             "required": [
                 "name",
                 "environment",
                 "cmd"
             ],
             "title": "App",
             "type": "object"
         },
         "UploadMountSpec": {
             "properties": {
                 "mode": {
+                    "const": "UPLOAD",
                     "default": "UPLOAD",
                     "description": "The mode to use for the mount.",
-                    "enum": [
-                        "UPLOAD"
-                    ],
-                    "title": "Mode",
-                    "type": "string"
+                    "title": "Mode"
                 },
                 "path": {
                     "description": "The path to mount into the environment.",
-                    "pattern": "/mnt/(?!slingshot).+",
+                    "pattern": "/mnt/\\w+",
                     "title": "Path",
                     "type": "string"
                 },
                 "tag": {
+                    "anyOf": [
+                        {
+                            "type": "string"
+                        },
+                        {
+                            "type": "null"
+                        }
+                    ],
+                    "default": null,
                     "description": "Optional tag to attach to the written asset.",
-                    "title": "Tag",
-                    "type": "string"
+                    "title": "Tag"
                 }
             },
             "required": [
                 "path"
             ],
             "title": "UploadMountSpec",
             "type": "object"
         },
         "VolumeMountSpec": {
             "properties": {
                 "mode": {
+                    "const": "VOLUME",
                     "default": "VOLUME",
                     "description": "The mode to use for the mount.",
-                    "enum": [
-                        "VOLUME"
-                    ],
-                    "title": "Mode",
-                    "type": "string"
+                    "title": "Mode"
                 },
                 "name": {
                     "description": "The name of the volume to mount.",
                     "title": "Name",
                     "type": "string"
                 },
                 "path": {
                     "description": "The path to mount into the environment.",
-                    "pattern": "/mnt/(?!slingshot).+",
+                    "pattern": "/mnt/\\w+",
                     "title": "Path",
                     "type": "string"
                 }
             },
             "required": [
                 "path",
                 "name"
             ],
             "title": "VolumeMountSpec",
             "type": "object"
         }
     },
+    "$id": "https://github.com/slingshot-ai/slingshot/blob/main/slingshot_client/src/slingshot/schemas/slingshot-schema.config.json",
+    "$schema": "http://json-schema.org/draft/2020-12/schema",
     "properties": {
         "apps": {
-            "description": "An app script.",
             "items": {
                 "anyOf": [
                     {
-                        "$ref": "#/definitions/SlingshotCustomAppSpec"
+                        "$ref": "#/$defs/SlingshotCustomAppSpec"
+                    },
+                    {
+                        "$ref": "#/$defs/SessionAppSpec"
                     },
                     {
-                        "$ref": "#/definitions/SessionAppSpec"
+                        "$ref": "#/$defs/RedisAppSpec"
                     }
                 ]
             },
             "title": "App",
             "type": "array"
         },
         "deployments": {
-            "description": "Model inference deployment",
             "items": {
-                "$ref": "#/definitions/DeploymentSpec"
+                "$ref": "#/$defs/DeploymentSpec"
             },
             "title": "Deployment",
             "type": "array"
         },
         "environments": {
             "additionalProperties": {
-                "$ref": "#/definitions/EnvironmentSpec"
+                "$ref": "#/$defs/EnvironmentSpec"
             },
             "description": "The environments to use for the job.",
             "title": "Environments",
             "type": "object"
         },
         "runs": {
-            "description": "Model training run",
             "items": {
-                "$ref": "#/definitions/RunSpec"
+                "$ref": "#/$defs/RunSpec"
             },
             "title": "Run",
             "type": "array"
         }
     },
     "title": "Slingshot Config Spec",
     "type": "object"
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 import json
 from abc import ABC
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 import deepdiff
 import pydantic
-from pydantic import BaseModel, Field, confloat, parse_obj_as, validator
+from pydantic import BaseModel, ConfigDict, Field, TypeAdapter, field_validator
+from pydantic_core.core_schema import FieldValidationInfo
+from rich.console import Console
+from typing_extensions import Annotated
 
-from slingshot.schemas import RequestedRequirement
-from slingshot.schemas.generated import schemas
-from slingshot.sdk.errors import SlingshotException
+from slingshot import schemas
+from slingshot.sdk.errors import SlingshotDeprecationException, SlingshotException
 from slingshot.sdk.graphql import fragments
-from slingshot.shared.utils import machine_size_to_machine_type_gpu_count, machine_type_gpu_count_to_machine_size
+from slingshot.shared.utils import (
+    get_default_num_gpu,
+    machine_size_to_machine_type_gpu_count,
+    machine_type_gpu_count_to_machine_size,
+)
 
 REPO = "https://github.com/slingshot-ai/slingshot"
 PATH_TO_FILE = "slingshot_client/src/slingshot/schemas"
 FILENAME = "slingshot-schema.config.json"
 FILE_LOCATION = "/".join([REPO, "blob/main", PATH_TO_FILE, FILENAME])
-PATH_FIELD = Field(
-    ..., title="Path", description="The path to mount into the environment.", regex=r"/mnt/(?!slingshot).+"
-)
+PATH_FIELD = Field(..., title="Path", description="The path to mount into the environment.", pattern=r'/mnt/\w+')
 MODE_FIELD = Field(..., title="Mode", description="The mode to use for the mount.")
 ALPHANUMERIC_UNDERSCORE_HYPHEN_RE = "^[A-Za-z][A-Za-z0-9_-]*$"  # This should match the regex on the backend
 
+console: Console = Console()  # TODO is this okay to use here?
+
 
 class BaseMountSpec(BaseModel):
     mode: str = Field(..., title="Mode", description="The mode to use for the mount.")
-    path: str = Field(
-        ..., title="Path", description="The path to mount into the environment.", regex=r"/mnt/(?!slingshot).+"
-    )
+    path: str = Field(..., title="Path", description="The path to mount into the environment.", pattern=r'/mnt/\w+')
 
     def diff(self, other: BaseMountSpec) -> list[str]:
         what_changed = []
         if self.mode != other.mode:
             what_changed.append(f"mode: {other.mode} → {self.mode}")
         if self.path != other.path:
             what_changed.append(f"path: {other.path} → {self.path}")
@@ -43,17 +47,14 @@
 
 class DownloadByNameMountSpec(BaseMountSpec):
     mode: Literal["DOWNLOAD"] = Field("DOWNLOAD", title="Mode", description="The mode to use for the mount.")
     name: str = Field(
         ..., title="Name", description="The name of the asset to mount. Either name or tag should be set, but not both."
     )
 
-    class Config:
-        exclude_defaults = False
-
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, DownloadByNameMountSpec) and self.name != other.name:
             d.append(f"name: {other.name} → {self.name}")
         elif isinstance(other, DownloadByTagMountSpec):
             d.append(f"replaced tag='{other.tag}' → name='{self.name}'")
         return d
@@ -64,114 +65,119 @@
     tag: str = Field(
         ...,
         title="Tag",
         description="The artifact selector. If multiple matching artifacts contain the tag, the "
         "latest one will be used.  Either name or tag should be set, but not both.",
     )
 
-    class Config:
-        exclude_defaults = False
-
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, DownloadByTagMountSpec) and self.tag != other.tag:
             d.append(f"tag: {other.tag} → {self.tag}")
         elif isinstance(other, DownloadByNameMountSpec):
             d.append(f"replaced name='{other.name}' → tag='{self.tag}'")
         return d
 
 
 class UploadMountSpec(BaseMountSpec):
     mode: Literal["UPLOAD"] = Field("UPLOAD", title="Mode", description="The mode to use for the mount.")
     tag: Optional[str] = Field(None, title="Tag", description="Optional tag to attach to the written asset.")
 
-    class Config:
-        exclude_defaults = False
-
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, UploadMountSpec) and self.tag != other.tag:
             d.append(f"tag: {other.tag} → {self.tag}")
         return d
 
 
 class VolumeMountSpec(BaseMountSpec):
     mode: Literal["VOLUME"] = Field("VOLUME", title="Mode", description="The mode to use for the mount.")
     name: str = Field(..., title="Name", description="The name of the volume to mount.")
 
-    class Config:
-        exclude_defaults = False
-
     def diff(self, other: BaseMountSpec) -> list[str]:
         d = super().diff(other)
         if isinstance(other, VolumeMountSpec) and self.name != other.name:
             d.append(f"name: {other.name} → {self.name}")
         return d
 
 
 MountSpecUnion = Union[DownloadByNameMountSpec, DownloadByTagMountSpec, UploadMountSpec, VolumeMountSpec]
 
 
 def mount_spec_from_remote(mount_spec: fragments.MountSpec) -> MountSpecUnion:
-    return parse_obj_as(MountSpecUnion, mount_spec)
+    return TypeAdapter(MountSpecUnion).validate_python(mount_spec.model_dump())
 
 
 def diff_mount_spec(new: MountSpecUnion, existing: fragments.MountSpec) -> list[str]:
     """Returns a list of differences between a local and a remote mount spec."""
     return new.diff(mount_spec_from_remote(existing))
 
 
 class EnvironmentSpec(BaseModel):
-    python_version: Union[  # type: ignore
+    python_version: Union[
         Literal["3.10"],
-        confloat(
-            # Literal 3.10
-            ge=3.10,
-            le=3.10,
-        ),
+        Annotated[
+            float,
+            Field(
+                # Literal 3.10
+                ge=3.10,
+                le=3.10,
+            ),
+        ],
     ] = Field("3.10", title="Python version")
     python_packages: list[str] = Field(
         default_factory=list,
         title="Python packages",
         description=f"List of Python packages to install in the environment.",
     )
+    post_install_command: str = Field(
+        "",
+        title="Post-install command",
+        description="Custom command to run after all packages have been installed. Skipped if not specified.",
+    )
     apt_packages: list[str] = Field(
         default_factory=list, title="APT packages", description=f"List of APT packages to install"
     )
-
-    class Config:
-        title = "Environment"
-        description = "The environment to use for the job."
-        schema_extra = {
-            "example": {"gpu_drivers": True, "python_version": "3.10", "python_packages": ["numpy", "pandas"]}
-        }
-        exclude_defaults = True
+    model_config = ConfigDict(
+        title="Environment",
+        json_schema_extra={
+            "example": {"python_version": "3.10", "python_packages": ["numpy", "pandas", "torch==2.0.1"]}
+        },
+    )
 
     # All python packages can be converted to RequestedRequirement
-    # noinspection PyMethodParameters
-    @validator("python_packages")
+    @classmethod
+    @field_validator("python_packages")
     def convert_python_packages(cls, v: list[str]) -> list[str]:
         for i in v:
             try:
-                RequestedRequirement.from_str(i)
+                schemas.RequestedRequirement.from_str(i)
             except ValueError as e:
                 raise ValueError(f"Error occurred while trying to parse python packages") from e
-
         return v
 
-    def diff(self, existing: fragments.ExecutionEnvironmentSpec, gpu_drivers: bool) -> list[str]:
+    def diff(self, existing: fragments.ExecutionEnvironmentSpec) -> list[str]:
         """Returns a list of differences between this and another environment spec."""
         diff = []
-        current_python_packages = [RequestedRequirement.from_str(pkg) for pkg in self.python_packages]
+        current_python_packages = [schemas.RequestedRequirement.from_str(pkg) for pkg in self.python_packages]
         current_apt_packages = [schemas.RequestedAptPackage(name=pkg) for pkg in self.apt_packages]
-        existing_python_packages = parse_obj_as(list[RequestedRequirement], existing.requested_python_requirements)
-        existing_apt_packages = parse_obj_as(list[schemas.RequestedAptPackage], existing.requested_apt_packages)
-
-        if gpu_drivers != existing.gpu_drivers:
-            diff.append(f"GPU drivers: {existing.gpu_drivers} → {gpu_drivers}")
+        assert existing.environment_instances, "Environment spec has no instances"
+        existing_env_instance = existing.environment_instances[0]
+        existing_python_packages = TypeAdapter(list[schemas.RequestedRequirement]).validate_python(
+            existing_env_instance.requested_python_requirements
+        )
+        existing_apt_packages = TypeAdapter(list[schemas.RequestedAptPackage]).validate_python(
+            existing_env_instance.requested_apt_packages
+        )
+        existing_post_install_command = existing_env_instance.post_install_command
+
+        if existing_post_install_command != self.post_install_command:
+            existing_post_install_command_repr = existing_post_install_command.replace("\n", "\\n")
+            new_post_install_command_repr = self.post_install_command.replace("\n", "\\n")
+            diff.append(f"Post-install command: {existing_post_install_command_repr} → {new_post_install_command_repr}")
 
         python_package_diffs = self._diff_python_requirements(current_python_packages, existing_python_packages)
         if python_package_diffs:
             diff.append(f"Python packages changed")
             diff.extend(python_package_diffs)
 
         apt_package_diffs = self._diff_apt_packages(current_apt_packages, existing_apt_packages)
@@ -179,15 +185,15 @@
             diff.append(f"APT packages changed")
             diff.extend(apt_package_diffs)
 
         return diff
 
     @staticmethod
     def _diff_python_requirements(
-        current: list[RequestedRequirement], existing: list[RequestedRequirement]
+        current: list[schemas.RequestedRequirement], existing: list[schemas.RequestedRequirement]
     ) -> list[str]:
         diff = []
         for req in current:
             if req not in existing:
                 diff.append(f"  [green]+[/green] {str(req)}")
         for req in existing:
             if req not in current:
@@ -205,15 +211,15 @@
         for req in existing:
             if req not in current:
                 diff.append(f"  [red]-[/red] {req.name}")
         return diff
 
 
 class SlingshotAbstractAppSpec(BaseModel, ABC):
-    name: str = Field(..., title="Name", description="The name of the app.", regex=ALPHANUMERIC_UNDERSCORE_HYPHEN_RE)
+    name: str = Field(..., title="Name", description="The name of the app.", pattern=ALPHANUMERIC_UNDERSCORE_HYPHEN_RE)
     environment: str = Field(..., title="Environment", description="The name of the execution environment.")
     machine_type: schemas.MachineType = Field(
         schemas.MachineType.CPU_SMALL, title="Machine size", description="The machine size to be used."
     )
     num_gpu: int = Field(0, title="Number of GPUs", description="The number of GPUs to use.")
     config_variables: dict[str, Any] = Field(
         default_factory=dict, title="Arguments", description="Optional user defined arguments to pass to the app."
@@ -224,23 +230,20 @@
         True,
         title="Attach project credentials",
         description=(
             "If true, will make an API key available to instances under the `SLINGSHOT_API_KEY` environment"
             "variable so that they can make requests using the Slingshot SDK for this project"
         ),
     )
+    model_config = ConfigDict(
+        title="App", json_schema_extra={"example": {"cmd": "python app.py", "environment": "slackbot"}}
+    )
 
-    class Config:
-        title = "App"
-        description = "An app script."
-        schema_extra = {"example": {"cmd": "python app.py", "environment": "slackbot"}}
-        exclude_defaults = True
-
-    # noinspection PyMethodParameters
-    @validator("mounts")
+    @classmethod
+    @field_validator("mounts")
     def validate_mount_paths_unique(cls, v: list[MountSpecUnion]) -> list[MountSpecUnion]:
         """
         Verify that all download mount paths are unique, and all upload mount paths are unique.
         However, it should be possible for download and upload mounts to share the same mount path.
         """
         download_paths = [str(spec.path) for spec in v if spec.mode == "DOWNLOAD"]
         if len(download_paths) != len(set(download_paths)):
@@ -248,18 +251,20 @@
 
         upload_paths = [str(spec.path) for spec in v if spec.mode == "UPLOAD"]
         if len(upload_paths) != len(set(upload_paths)):
             raise ValueError("All upload mount paths must be unique.")
 
         return v
 
-    @validator("num_gpu")
-    def validate_num_gpu(cls, v: int, values: dict[str, Any]) -> int:
+    @classmethod
+    @field_validator("num_gpu", mode="after")
+    def validate_num_gpu(cls, v: int | None, info: FieldValidationInfo) -> int:
         """Validate that the number of GPUs is valid based on machine_type."""
-        machine_type: schemas.MachineType = values["machine_type"]
+        machine_type: schemas.MachineType = info.data["machine_type"]
+        v = v or get_default_num_gpu(machine_type)
         try:
             machine_type_gpu_count_to_machine_size(gpu_count=v, machine_type=machine_type)
         except ValueError as e:
             raise ValueError(f"Invalid number of GPUs ({v}) for machine type {machine_type}") from e
         return v
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
@@ -307,17 +312,14 @@
         return diff
 
 
 class SlingshotCustomAppSpec(SlingshotAbstractAppSpec):
     port: Optional[int] = Field(None, title="Port", description="The port to expose.")
     cmd: str = Field(..., title="Command", description="The command to run.")
 
-    class Config:
-        exclude_defaults = True
-
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         if existing.app_type != schemas.AppType.CUSTOM:
             raise ValueError(f"Cannot diff an app against a non-app.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
@@ -329,130 +331,177 @@
 class SessionAppSpec(SlingshotAbstractAppSpec):
     using: Literal["session"] = Field(
         ...,
         title="Using",
         description="Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
     )
 
-    class Config:
-        exclude_defaults = True
-
     @property
     def port(self) -> int:
         return 8080
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         if existing.app_sub_type != schemas.AppSubType.SESSION:
             raise ValueError(f"Cannot diff session app against a non-session.")
         diff = super().diff(existing)
-        if self.using and self.using != existing.app_sub_type.lower():
-            diff.append(f"Plugin changed from '{existing.app_sub_type.lower()}' → '{self.using}'")
+        if self.port != existing.app_port:
+            diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
+        return diff
+
+
+class RedisAppSpec(SlingshotAbstractAppSpec):
+    using: Literal["redis"] = Field(
+        ...,
+        title="Using",
+        description="Which package to use. When specified, this feature automatically adjusts the behavior of the app.",
+    )
+
+    @property
+    def port(self) -> int:
+        return 6379
+
+    def diff(self, existing: fragments.AppSpec) -> list[str]:
+        """Returns a list of differences between this and another app spec."""
+        if existing.app_sub_type != schemas.AppSubType.REDIS:
+            raise ValueError(f"Cannot diff redis app against a non-redis one.")
+        diff = super().diff(existing)
         if self.port != existing.app_port:
             diff.append(f"Port changed from '{existing.app_port}' → '{self.port}'")
         return diff
 
 
 class RunSpec(SlingshotAbstractAppSpec):
     name: str = Field("run", title="Name", description="The name of the run.")
     cmd: str = Field(..., title="Command", description="The command to run.")
-
-    class Config:
-        title = "Run"
-        description = "Model training run"
-        schema_extra = {"example": {"cmd": "python train.py", "environment": "training"}}
-        exclude_defaults = True
+    model_config = ConfigDict(
+        title="Run", json_schema_extra={"example": {"cmd": "python train.py", "environment": "training"}}
+    )
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         if existing.app_type != schemas.AppType.RUN:
             raise ValueError(f"Cannot diff a run against a non-run.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
         return diff
 
 
 class DeploymentSpec(SlingshotAbstractAppSpec):
     name: str = Field("deployment", title="Name", description="The name of the deployment.")
     cmd: str = Field(..., title="Command", description="The command to run.")
-
-    class Config:
-        title = "Deployment"
-        description = "Model inference deployment"
-        schema_extra = {"example": {"environment": "deployment"}}
-        exclude_defaults = True
+    model_config = ConfigDict(title="Deployment", json_schema_extra={"example": {"environment": "deployment"}})
 
     def diff(self, existing: fragments.AppSpec) -> list[str]:
         """Returns a list of differences between this and another app spec."""
         if existing.app_type != schemas.AppType.DEPLOYMENT:
             raise ValueError(f"Cannot diff a run against a non-deployment.")
         diff = super().diff(existing)
         if self.cmd != existing.app_spec_command:
             diff.append(f"Command changed from '{existing.app_spec_command}' → '{self.cmd}'")
         return diff
 
 
+class SlingshotValidationResult(BaseModel):
+    warning: Optional[str] = Field(None, title="Warning", description="A warning message.")
+    error: Optional[str] = Field(None, title="Error", description="An error message.")
+
+    @classmethod
+    def of_invalid_machine_type(cls, machine_type: str) -> "SlingshotValidationResult":
+        return cls(
+            error=(
+                f"Machine type '{machine_type}' is not supported in slingshot.yaml (since version '0.0.10'). Hint: Use "
+                "'slingshot machines' for machine options."
+            )
+        )
+
+    def warning_or_raise(self) -> str:
+        if self.error:
+            raise SlingshotDeprecationException(self.error)
+
+        assert self.warning, "No warning or error message found."
+        return self.warning
+
+
 class ProjectManifest(BaseModel):
     environments: dict[str, EnvironmentSpec] = Field(
         default_factory=dict, title="Environments", description="The environments to use for the job."
     )
-    apps: list[Union[SlingshotCustomAppSpec, SessionAppSpec]] = Field(
-        default_factory=list,
-        title=SlingshotAbstractAppSpec.Config.title,
-        description=SlingshotAbstractAppSpec.Config.description,
-    )
-    runs: list[RunSpec] = Field(
-        default_factory=list, title=RunSpec.Config.title, description=RunSpec.Config.description
+    apps: list[Union[SlingshotCustomAppSpec, SessionAppSpec, RedisAppSpec]] = Field(
+        default_factory=list, title=SlingshotAbstractAppSpec.model_config["title"]
     )
-    deployments: list[DeploymentSpec] = Field(
-        default_factory=list, title=DeploymentSpec.Config.title, description=DeploymentSpec.Config.description
+    runs: list[RunSpec] = Field(default_factory=list, title=RunSpec.model_config["title"])
+    deployments: list[DeploymentSpec] = Field(default_factory=list, title=DeploymentSpec.model_config["title"])
+    model_config = ConfigDict(
+        title="Slingshot Config Spec",
+        json_schema_extra={"$schema": "http://json-schema.org/draft/2020-12/schema", "$id": FILE_LOCATION},
     )
 
-    class Config:
-        title = "Slingshot Config Spec"
-        description = "The Slingshot config file."
-        schema_extra = {"$schema": "http://json-schema.org/draft/2020-12/schema", "$id": FILE_LOCATION}
-        exclude_defaults = True
+    @staticmethod
+    def check_deprecations(v: dict[str, Any]) -> list[SlingshotValidationResult]:
+        deprecations = []
+
+        all_apps_runs_deployments = []
+        all_apps_runs_deployments.extend(v.get("apps", []))
+        all_apps_runs_deployments.extend(v.get("runs", []))
+        all_apps_runs_deployments.extend(v.get("deployments", []))
+
+        # Check old GPUs
+        for app_run_deployment in all_apps_runs_deployments:
+            app_run_deployment = (
+                app_run_deployment.model_dump() if isinstance(app_run_deployment, BaseModel) else app_run_deployment
+            )
+            machine_type = ('machine_type' in app_run_deployment and app_run_deployment['machine_type']) or ""
+            if machine_type in {"GPU", "GPU_A100"}:
+                deprecations.append(SlingshotValidationResult.of_invalid_machine_type(machine_type))
+
+        return deprecations
+
+    # TODO: add typing for values and return type, split deprecation checks into a separate validator
+    @classmethod
+    @pydantic.model_validator(mode="before")
+    def validate_environment_names(cls, info: FieldValidationInfo) -> dict[str, Any]:
+        if deprecations := cls.check_deprecations(info.data):
+            warnings = [deprecation.warning_or_raise() for deprecation in deprecations]
+            warnings_fmt = "\n".join(warnings)
+            console.print(f"[yellow]⚠️ Detected deprecated slingshot.yaml fields[/yellow]:\n{warnings_fmt}")
 
-    # noinspection PyMethodParameters
-    @pydantic.root_validator(pre=True)
-    def validate_environment_names(cls, values: dict[str, Any]) -> dict[str, Any]:
         # Validate that jupyter is in all session environments:
-        sessions = [app for app in values.get("apps", []) if isinstance(app, SessionAppSpec)]
-        envs: dict[str, EnvironmentSpec] = values.get("environments", {})
+        sessions = [app for app in info.data.get("apps", []) if isinstance(app, SessionAppSpec)]
+        envs: dict[str, EnvironmentSpec] = info.data.get("environments", {})
 
         if not isinstance(envs, dict):
             raise SlingshotException(f"'environments' must be a YAML mapping (was: {type(envs)})")
 
         session_envs = {
             env_name: env
             for env_name, env in envs.items()
             if any(session.environment == env_name for session in sessions)
         }
         for session_env_name, session_env in session_envs.items():
             requested_python_requirements = session_env.python_packages
             if not any("jupyterlab" in requirement for requirement in requested_python_requirements):
                 raise SlingshotException(
-                    f"'jupyterlab' was not found in {session_env_name}. Please add it and try again."
+                    f"'jupyterlab' was not found in the '{session_env_name}' environment. Please add it and try again."
                 )
 
         # Validate that all referenced environments are in the environments list:
         for app_or_run_or_deployment in [
-            *values.get("apps", []),
-            *values.get("runs", []),
-            *values.get("deployments", []),
+            *info.data.get("apps", []),
+            *info.data.get("runs", []),
+            *info.data.get("deployments", []),
         ]:
             app_ = (
-                app_or_run_or_deployment.dict()
+                app_or_run_or_deployment.model_dump()
                 if not isinstance(app_or_run_or_deployment, dict)
                 else app_or_run_or_deployment
             )
             env = app_.get("environment", '')
             if env not in envs:
                 raise SlingshotException(f"Environment '{env}' not found in 'environments' {list(envs.keys())}")
-        return values
+        return info.data
 
 
 if __name__ == "__main__":
     with open(Path(PATH_TO_FILE) / FILENAME, "w") as f:
-        json.dump(ProjectManifest.schema(), f, indent=2)
+        json.dump(ProjectManifest.model_json_schema(), f, indent=2)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/data_collector.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 from __future__ import annotations
 
 import typing
 
+import sentry_sdk
 from aiohttp.client_exceptions import ClientResponse
 from rich.console import Console
 
+from .config import client_settings
+
 if typing.TYPE_CHECKING:
     from .graphql import GraphQLError
 
 
 class SlingshotException(Exception):
     """Base Slingshot Exception"""
 
+    def __init__(self, msg: str, *, cli: str | None = None):
+        """
+        :param msg: The message to display
+        :param cli: The message to display in the CLI. If not provided, defaults to `msg`
+        """
+        self.cli = cli or msg
+        super().__init__(msg)
+
     def rich_show(self, console: Console, verbose: bool = False) -> None:
         """Return a string representation of the exception"""
-        console.print(f"[bold][red]Error:[/bold][/red] {self}")
+        if self.cli:
+            console.print(f"[bold][red]Error:[/bold][/red] {self.cli}")
+        else:
+            console.print(f"[bold][red]Error:[/bold][/red] {self}")
         if verbose:
             console.print_exception()
 
 
+class SlingshotDeprecationException(SlingshotException):
+    pass
+
+
 class SlingshotClientHttpException(SlingshotException):
     def __init__(self, json: dict[str, typing.Any] | None, text: str, status: int, response: ClientResponse):
         self.json = json
         self.text = text
         self.status = status
         self.response = response
         super().__init__(f"Slingshot Client HTTP {status}: {text}")
 
     @staticmethod
     async def from_response(response: ClientResponse) -> SlingshotClientHttpException:
         try:
-            response_json = await response.json()
+            response_json = await response.model_dump_json()
         except Exception:
             response_json = None
         return SlingshotClientHttpException(
             json=response_json, text=await response.text(), status=response.status, response=response
         )
 
     def rich_show(self, console: Console, verbose: bool = False) -> None:
@@ -107,15 +125,18 @@
 
 class SlingshotUnauthenticatedError(SlingshotException):
     """User is not signed in, but command requires authentication"""
 
     graphql_message = "Missing 'Authorization' or 'Cookie' header in JWT authentication mode"
 
     def __init__(self) -> None:
-        super().__init__(f"You're not signed in.")
+        if client_settings.is_in_app:
+            super().__init__(f"You're not signed in. Did you mean to attach project credentials?")
+        else:
+            super().__init__(f"You're not signed in.")
 
     def rich_show(self, console: Console, verbose: bool = False) -> None:
         console.print("[red]Error:[/red] This command requires you to be signed in. Please run 'slingshot login'.")
 
 
 class SlingshotJWTExpiredError(SlingshotException):
     """JWT token is expired"""
@@ -135,7 +156,23 @@
     graphql_message = "JWSInvalidSignature"
 
     def __init__(self) -> None:
         super().__init__(f"Your login token is invalid.")
 
     def rich_show(self, console: Console, verbose: bool = False) -> None:
         console.print("[red]Error:[/red] Your login token is invalid. Please run 'slingshot login'.")
+
+
+class SlingshotNoProjectSetError(SlingshotException):
+    """No project is set"""
+
+    def __init__(self) -> None:
+        super().__init__(f"No project is set, and no project could be inferred.")
+
+    def rich_show(self, console: Console, verbose: bool = False) -> None:
+        if client_settings.is_in_app:
+            # This should never happen!
+            with sentry_sdk.push_scope() as scope:
+                scope.set_extra("app_type", client_settings.slingshot_app_type)
+                scope.set_extra("app_instance_id", client_settings.slingshot_instance_id)
+                sentry_sdk.capture_exception(self)
+        console.print("[red]Error:[/red] No project is set. Please run 'slingshot project set [project]'.")
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 import abc
-from abc import abstractmethod
-from typing import Any, Generic, Literal, Optional, Type, TypeVar
+from typing import Any, ClassVar, Generic, Literal, Optional, Type, TypeVar
 
 from pydantic import BaseModel
-from pydantic.generics import GenericModel
 
 from slingshot.sdk.errors import SlingshotClientGraphQLException
 
 T = TypeVar("T")
 
 ResponseType = TypeVar("ResponseType", bound=BaseModel)
 
@@ -17,15 +15,15 @@
 class GraphQLError(BaseModel):
     message: str
     locations: Optional[list[dict[str, int]]] = None
     path: Optional[list[str]] = None
     extensions: Optional[dict[str, str]] = None
 
 
-class GraphQLResponse(GenericModel, Generic[T]):
+class GraphQLResponse(BaseModel, Generic[T]):
     data: Optional[T] = None
     errors: Optional[list[GraphQLError]] = None
 
     def as_exception(self) -> SlingshotClientGraphQLException:
         if not self.errors:
             raise ValueError("Cannot create exception from GraphQLResponse with no errors")
         return SlingshotClientGraphQLException.from_graphql_errors(self.errors)
@@ -34,30 +32,23 @@
         if self.errors:
             raise self.as_exception()
         if self.data is None:
             raise ValueError("Cannot get data from GraphQL (unexpected)")
         return self.data
 
 
-class GraphQLSubscriptionResponse(GenericModel, Generic[T]):
+class GraphQLSubscriptionResponse(BaseModel, Generic[T]):
     type: Literal['data']
     id: str
     payload: GraphQLResponse[T]
 
 
 class BaseGraphQLEntity(BaseModel, abc.ABC):
-    @property
-    @abstractmethod
-    def _fragment(self) -> str:
-        ...
-
-    @property
-    @abstractmethod
-    def _depends_on(self) -> list[Type[BaseGraphQLEntity]]:
-        raise NotImplementedError()
+    _fragment: ClassVar[str]  # Abstract
+    _depends_on: ClassVar[list[Type[BaseGraphQLEntity]]]  # Abstract
 
     def _get_dependencies_ext(self, visited: set[Type[BaseGraphQLEntity]]) -> set[Type[BaseGraphQLEntity]]:
         # Recursively get all dependencies
         dependencies = set()
 
         for dependency in self._depends_on:
             dependencies.add(dependency)
@@ -69,31 +60,27 @@
 
     def _get_dependencies(self) -> list[Type[BaseGraphQLEntity]]:
         return list(self._get_dependencies_ext(set()))
 
     def get_fragment_string(self) -> str:
         """Get the GraphQL fragment string for this entity, including all dependencies"""
         dependencies = set(self._get_dependencies())
-        fragments: list[str] = [dependency._fragment for dependency in dependencies]  # type: ignore
+        fragments: list[str] = [dependency._fragment for dependency in dependencies]
         fragments.append(self._fragment)
         return "\n".join(fragments)
 
 
-class BaseGraphQLQuery(BaseGraphQLEntity, GenericModel, Generic[ResponseType], abc.ABC):
+class BaseGraphQLQuery(BaseGraphQLEntity, BaseModel, Generic[ResponseType], abc.ABC):
     query: str
-    variables: Optional[dict[str, Any]]
+    variables: Optional[dict[str, Any]] = None
     response_model: Type[ResponseType]
+    _query: ClassVar[str]  # Abstract
 
     @property
-    @abstractmethod
-    def _query(self) -> str:
-        ...
-
-    @property
-    def _fragment(self) -> str:
+    def _fragment(self) -> str:  # type: ignore[override]
         return self._query
 
     def get_query(self, **kwargs: Any) -> str:
         return self.get_fragment_string()
 
     def __init__(self, variables: Optional[dict[str, Any]], response_model: Type[ResponseType]):
         super().__init__(query=self.get_query(), variables=variables, response_model=response_model)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/fragments.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,27 @@
         fragment BlobArtifactShallow on BlobArtifacts {
           blobArtifactId
           createdAt
           updatedAt
           bytesHash
           bytesSize
           name
+          description
           tag
         } """
 
+    # TODO: get rid of blob_artifact_name and blob_artifact_tag, only keep the name + tag fields
     blob_artifact_id: str = Field(..., alias="blobArtifactId")
-    name: str = Field(..., alias="name")
-    tag: Optional[str] = Field(..., alias="tag")
+    name: Optional[str] = Field(None, alias="name")
+    description: Optional[str] = Field(None, alias="description")
+    tag: Optional[str] = Field(None, alias="tag")
     created_at: datetime = Field(..., alias="createdAt")
     updated_at: datetime = Field(..., alias="updatedAt")
-    bytes_hash: Optional[str] = Field(..., alias="bytesHash")
-    bytes_size: Optional[int] = Field(..., alias="bytesSize")
+    bytes_hash: Optional[str] = Field(None, alias="bytesHash")
+    bytes_size: Optional[int] = Field(None, alias="bytesSize")
     blob_artifact_name: Optional[str] = Field(None, alias="name")
     blob_artifact_tag: Optional[str] = Field(None, alias="tag")
 
 
 class Mount(BaseGraphQLEntity):
     _fragment = """
         fragment Mount on Mount {
@@ -52,17 +55,17 @@
 
     _depends_on = [BlobArtifactShallow]
 
     mount_id: str = Field(..., alias="mountId")
     deployment_id: Optional[str] = Field(None, alias="deploymentId")
     run_id: Optional[str] = Field(None, alias="trainingRunId")
     mount_path: str = Field(..., alias="mountPath")
-    mount_mode: Literal["DOWNLOAD", "UPLOAD", "VOLUME"] = Field(..., alias="mountMode")
-    downloaded_blob_artifact: Optional[BlobArtifactShallow] = Field(..., alias="downloadedBlobArtifact")
-    uploaded_blob_artifact: Optional[BlobArtifactShallow] = Field(..., alias="uploadedBlobArtifact")
+    mount_mode: Literal["DOWNLOAD", "UPLOAD", "VOLUME", "EMPTY"] = Field(..., alias="mountMode")
+    downloaded_blob_artifact: Optional[BlobArtifactShallow] = Field(None, alias="downloadedBlobArtifact")
+    uploaded_blob_artifact: Optional[BlobArtifactShallow] = Field(None, alias="uploadedBlobArtifact")
 
 
 class BlobArtifact(BaseGraphQLEntity):
     _fragment = """
         fragment BlobArtifact on BlobArtifacts {
           blobArtifactId
           createdAt
@@ -76,43 +79,37 @@
             ...Mount
           }
         } """
     _depends_on = [Mount]
 
     blob_artifact_id: str = Field(..., alias="blobArtifactId")
     name: str = Field(..., alias="name")
-    tag: Optional[str] = Field(..., alias="tag")
+    tag: Optional[str] = Field(None, alias="tag")
     created_at: datetime = Field(..., alias="createdAt")
     updated_at: datetime = Field(..., alias="updatedAt")
-    bytes_hash: Optional[str] = Field(..., alias="bytesHash")
-    bytes_size: Optional[int] = Field(..., alias="bytesSize")
+    bytes_hash: Optional[str] = Field(None, alias="bytesHash")
+    bytes_size: Optional[int] = Field(None, alias="bytesSize")
     blob_artifact_name: Optional[str] = Field(None, alias="name")
     blob_artifact_tag: Optional[str] = Field(None, alias="tag")
-    origin_mount: Optional[Mount] = Field(..., alias="originMount")
+    origin_mount: Optional[Mount] = Field(None, alias="originMount")
     is_draft: bool = Field(..., alias="isDraft")
 
 
 class SourceCodeArtifact(BaseGraphQLEntity):
     _depends_on = [BlobArtifactShallow]
     _fragment = """
         fragment SourceCodeArtifact on SourceCodes {
           sourceCodeId
-          sourceCodeName
-          description
-          createdAt
           projectId
           blobArtifact {
             ...BlobArtifactShallow
           }
         } """
 
     source_code_id: str = Field(..., alias="sourceCodeId")
-    source_code_name: str = Field(..., alias="sourceCodeName")
-    description: Optional[str] = Field(..., alias="description")
-    created_at: datetime = Field(..., alias="createdAt")
     project_id: str = Field(..., alias="projectId")
     blob_artifact: BlobArtifactShallow = Field(..., alias="blobArtifact")
 
 
 class Deployment(BaseGraphQLEntity):
     _depends_on = [BlobArtifact, SourceCodeArtifact]
     _fragment = """
@@ -146,40 +143,103 @@
 
 
 class ExecutionEnvironment(BaseGraphQLEntity):
     _depends_on = [Build]
     _fragment = """
         fragment ExecutionEnvironment on ExecutionEnvironments {
           executionEnvironmentId
-          build {
+          cpuBuild {
+            ...Build
+          }
+          gpuBuild {
             ...Build
           }
           createdAt
           requirements
           errorMessage
           status
-          gpuDrivers
           requestedAptPackages
           requestedPythonRequirements
+          postInstallCommand
         } """
     execution_environment_id: str = Field(..., alias="executionEnvironmentId")
     status: schemas.ExecEnvStatus
     created_at: datetime = Field(..., alias="createdAt")
-    build: Optional[Build]
-    requirements: Optional[str]
-    error_message: Optional[str] = Field(..., alias="errorMessage")
-    gpu_drivers: bool = Field(..., alias="gpuDrivers")
+    cpu_build: Optional[Build] = Field(None, alias="cpuBuild")
+    gpu_build: Optional[Build] = Field(None, alias="gpuBuild")
+    requirements: Optional[str] = None
+    error_message: Optional[str] = Field(None, alias="errorMessage")
+    requested_apt_packages: list[dict[str, str]] = Field(..., alias="requestedAptPackages")
+    requested_python_requirements: list[dict[str, Optional[str]]] = Field(
+        ..., alias="requestedPythonRequirements", repr=False
+    )
+    post_install_command: str = Field("", alias="postInstallCommand")
+
+
+class EnvironmentInstanceShallow(BaseGraphQLEntity):
+    _depends_on = [ExecutionEnvironment]
+    _fragment = """
+        fragment EnvironmentInstanceShallow on EnvironmentInstances {
+            environmentInstanceId
+            executionEnvironmentSpecId
+            createdAt
+            requestedAptPackages
+            requestedPythonRequirements
+            postInstallCommand
+            executionEnvironment {
+                ...ExecutionEnvironment
+            }
+        }"""
+
+    environment_instance_id: str = Field(..., alias="environmentInstanceId")
+    execution_environment_spec_id: str = Field(..., alias="executionEnvironmentSpecId")
+    created_at: datetime = Field(..., alias="createdAt")
+    execution_environment: ExecutionEnvironment = Field(..., alias="executionEnvironment")
     requested_apt_packages: list[dict[str, str]] = Field(..., alias="requestedAptPackages")
     requested_python_requirements: list[dict[str, Optional[str]]] = Field(
         ..., alias="requestedPythonRequirements", repr=False
     )
+    post_install_command: str = Field("", alias="postInstallCommand")
+
+
+class ExecutionEnvironmentSpec(BaseGraphQLEntity):
+    _depends_on = [EnvironmentInstanceShallow]
+    _fragment = """
+        fragment ExecutionEnvironmentSpec on ExecutionEnvironmentSpecs {
+            executionEnvironmentSpecId
+            executionEnvironmentSpecName
+            createdAt
+            isArchived
+            environmentInstances(orderBy: { createdAt: DESC }, limit: 1) {
+                ...EnvironmentInstanceShallow
+            }
+        }"""
+
+    execution_environment_spec_id: str = Field(..., alias="executionEnvironmentSpecId")
+    execution_environment_spec_name: str = Field(..., alias="executionEnvironmentSpecName")
+    created_at: datetime = Field(..., alias="createdAt")
+    is_archived: bool = Field(..., alias="isArchived")
+    environment_instances: list[EnvironmentInstanceShallow] = Field(..., alias="environmentInstances")
+
+
+class EnvironmentInstance(EnvironmentInstanceShallow):
+    _depends_on = [EnvironmentInstanceShallow, ExecutionEnvironmentSpec]
+    _fragment = """
+        fragment EnvironmentInstance on EnvironmentInstances {
+            ...EnvironmentInstanceShallow
+            executionEnvironmentSpec {
+                ...ExecutionEnvironmentSpec
+            }
+        }"""
+
+    execution_environment_spec: 'ExecutionEnvironmentSpec' = Field(..., alias="executionEnvironmentSpec")
 
 
 class Run(BaseGraphQLEntity):
-    _depends_on = [ExecutionEnvironment, Mount, SourceCodeArtifact]
+    _depends_on = [EnvironmentInstance, Mount, SourceCodeArtifact]
     _fragment = """
         fragment Run on TrainingRuns {
           trainingRunId
           runSpecId
           trainingRunName
           jobStatus
           createdAt
@@ -187,35 +247,34 @@
           endTime
           machineSize
           hyperparameters
           cmd
           sourceCode {
             ...SourceCodeArtifact
           }
-          executionEnvironment {
-            ...ExecutionEnvironment
+          environmentInstance {
+            ...EnvironmentInstance
           }
           mounts {
             ...Mount
           }
         }
         """
     run_id: str = Field(..., alias="trainingRunId")
-    run_spec_id: Optional[str] = Field(..., alias="runSpecId")
+    run_spec_id: str = Field(..., alias="runSpecId")
     run_name: str = Field(..., alias="trainingRunName")
     job_status: schemas.JobStatus = Field(..., alias="jobStatus")
     created_at: datetime = Field(..., alias="createdAt")
-    start_time: Optional[datetime] = Field(..., alias="startTime")
-    end_time: Optional[datetime] = Field(..., alias="endTime")
+    start_time: Optional[datetime] = Field(None, alias="startTime")
+    end_time: Optional[datetime] = Field(None, alias="endTime")
     machine_size: schemas.MachineSize = Field(..., alias="machineSize")
-    hyperparameters: Optional[str]
-    cmd: Optional[str]
+    hyperparameters: Optional[str] = None
+    cmd: Optional[str] = None
     source_code: SourceCodeArtifact = Field(..., alias="sourceCode")
-    # TODO: ENG-1062 projects don't have permissions for outdated envs so this might be returned as None
-    execution_environment: Optional[ExecutionEnvironment] = Field(..., alias="executionEnvironment")
+    environment_instance: EnvironmentInstance = Field(..., alias="environmentInstance")
     mounts: list[Mount] = Field(..., alias="mounts")
 
 
 class Volume(BaseGraphQLEntity):
     _depends_on = []
     _fragment = """
         fragment Volume on Volumes {
@@ -246,23 +305,23 @@
         fragment BillingLineItem on BillingLineItems {
           appInstanceId
           deploymentId
           runId
           computeCostCredits
           computeCostCreditsInProgress
         } """
-    app_instance_id: Optional[str] = Field(..., alias="appInstanceId")
-    deployment_id: Optional[str] = Field(..., alias="deploymentId")
-    run_id: Optional[str] = Field(..., alias="runId")
-    compute_cost_credits: Optional[int] = Field(..., alias="computeCostCredits")
+    app_instance_id: Optional[str] = Field(None, alias="appInstanceId")
+    deployment_id: Optional[str] = Field(None, alias="deploymentId")
+    run_id: Optional[str] = Field(None, alias="runId")
+    compute_cost_credits: Optional[int] = Field(None, alias="computeCostCredits")
     compute_cost_credits_in_progress: int = Field(..., alias="computeCostCreditsInProgress")
 
 
 class ProjectProjection(BaseModel):
-    project: Optional[ProjectFields]
+    project: Optional[ProjectFields] = None
 
 
 class UserWithProjects(BaseGraphQLEntity):
     _depends_on = [ProjectFields]
     _fragment = """
         fragment UserWithProjects on Users {
           displayName
@@ -274,15 +333,15 @@
             project {
               ...ProjectFields
             }
           }
         } """
     display_name: str = Field(..., alias="displayName")
     username: str = Field(..., alias="username")
-    ssh_public_key: Optional[str] = Field(..., alias="sshPublicKey")
+    ssh_public_key: Optional[str] = Field(None, alias="sshPublicKey")
     user_id: str = Field(..., alias="userId")
     user_project_acls: list[ProjectProjection] = Field(..., alias="userProjectAcls")
     is_activated: bool = Field(..., alias="isActivated")
 
     @property
     def projects(self) -> list[ProjectFields]:
         return [acl.project for acl in self.user_project_acls if acl.project]  # Filter out None values
@@ -295,15 +354,15 @@
               serviceAccountId
               nickname
               lastFour
               apiKeyHash
               createdAt
         } """
     service_account_id: str = Field(..., alias="serviceAccountId")
-    nickname: Optional[str] = Field(..., alias="nickname")
+    nickname: Optional[str] = Field(None, alias="nickname")
     last_four: str = Field(..., alias="lastFour")
     api_key_hash: str = Field(..., alias="apiKeyHash")
     created_at: datetime = Field(..., alias="createdAt")
 
 
 class ServiceAccountWithProjects(ServiceAccount):
     _depends_on = [ProjectFields, ServiceAccount]
@@ -350,47 +409,19 @@
     """
     path: str = Field(..., alias="path")
     mode: Literal["DOWNLOAD", "UPLOAD", "VOLUME_READONLY", "VOLUME"] = Field(..., alias="mode")
     tag: Optional[str] = Field(None, alias="tag")
     name: Optional[str] = Field(None, alias="name")
 
 
-class ExecutionEnvironmentSpec(BaseGraphQLEntity):
-    _depends_on = [ExecutionEnvironment]
-    _fragment = """
-        fragment ExecutionEnvironmentSpec on ExecutionEnvironmentSpecs {
-            executionEnvironmentSpecId
-            executionEnvironmentSpecName
-            createdAt
-            gpuDrivers
-            requestedAptPackages
-            requestedPythonRequirements
-            isArchived
-            executionEnvironment {
-                ...ExecutionEnvironment
-            }
-        }"""
-
-    execution_environment_spec_id: str = Field(..., alias="executionEnvironmentSpecId")
-    execution_environment_spec_name: str = Field(..., alias="executionEnvironmentSpecName")
-    created_at: datetime = Field(..., alias="createdAt")
-    execution_environment: ExecutionEnvironment = Field(..., alias="executionEnvironment")
-    gpu_drivers: bool = Field(..., alias="gpuDrivers")
-    requested_apt_packages: list[dict[str, str]] = Field(..., alias="requestedAptPackages")
-    requested_python_requirements: list[dict[str, Optional[str]]] = Field(
-        ..., alias="requestedPythonRequirements", repr=False
-    )
-    is_archived: bool = Field(..., alias="isArchived")
-
-
 class _AppInstanceProjection(BaseModel):
     app_instance_status: schemas.AppInstanceStatus = Field(..., alias="appInstanceStatus")
-    app_instance_url: Optional[str] = Field(..., alias="appInstanceUrl")
+    app_instance_url: Optional[str] = Field(None, alias="appInstanceUrl")
     created_at: datetime = Field(..., alias="createdAt")
-    ssh_port: Optional[int] = Field(..., alias="sshPort")
+    ssh_port: Optional[int] = Field(None, alias="sshPort")
 
 
 class AppSpec(BaseGraphQLEntity):
     _depends_on = [ExecutionEnvironmentSpec, MountSpec, Deployment]
     _fragment = """
         fragment SlingshotAppSpec on AppSpecs {
             appSpecId
@@ -407,34 +438,34 @@
             batchInterval
             executionEnvironmentSpec {
                 ...ExecutionEnvironmentSpec
             }
             mountSpecs {
                 ...MountSpec
             }
-            appInstances(orderBy:{ createdAt:DESC }, limit:1) {
+            appInstances(orderBy:{ createdAt:DESC }, limit: 1) {
                 appInstanceStatus
                 appInstanceUrl
                 createdAt
                 sshPort
             }
             deployments(orderBy:{ createdAt:DESC }, limit:1) {
                 ...Deployment
             }
         }
     """
     app_spec_id: str = Field(..., alias="appSpecId")
     app_spec_name: str = Field(..., alias="appSpecName")
-    app_spec_command: Optional[str] = Field(..., alias="appSpecCommand")
+    app_spec_command: Optional[str] = Field(None, alias="appSpecCommand")
     app_type: schemas.AppType = Field(..., alias="appType")
-    app_sub_type: Optional[schemas.AppSubType] = Field(..., alias="appSubType")
-    app_port: Optional[int] = Field(..., alias="appPort")
-    config_variables: Optional[str] = Field(..., alias="configVariables")
-    batch_size: Optional[int] = Field(..., alias="batchSize")
-    batch_interval: Optional[int] = Field(..., alias="batchInterval")
+    app_sub_type: Optional[schemas.AppSubType] = Field(None, alias="appSubType")
+    app_port: Optional[int] = Field(None, alias="appPort")
+    config_variables: Optional[str] = Field(None, alias="configVariables")
+    batch_size: Optional[int] = Field(None, alias="batchSize")
+    batch_interval: Optional[int] = Field(None, alias="batchInterval")
     project_id: str = Field(..., alias="projectId")
     machine_size: schemas.MachineSize = Field(..., alias="machineSize")
     service_account: bool = Field(..., alias="serviceAccount")
     execution_environment_spec: ExecutionEnvironmentSpec = Field(..., alias="executionEnvironmentSpec")
     mount_specs: list[MountSpec] = Field(..., alias="mountSpecs")
     app_instances: list[_AppInstanceProjection] = Field(..., alias="appInstances")
     deployments: list[Deployment] = Field(..., alias="deployments")
@@ -477,31 +508,31 @@
             appInstanceId
             appInstanceStatus
             appInstanceUrl
             appType
             appSubType
             appPort
             sshPort
-            executionEnvironmentId
+            environmentInstanceId
             createdAt
             appSpecCommand
             appSpecId
             appSpec {
                 ...SlingshotAppSpec
             }
         }
     """
     app_instance_id: str = Field(..., alias="appInstanceId")
     app_instance_status: schemas.AppInstanceStatus = Field(..., alias="appInstanceStatus")
-    app_instance_url: Optional[str] = Field(..., alias="appInstanceUrl")
+    app_instance_url: Optional[str] = Field(None, alias="appInstanceUrl")
     app_type: schemas.AppType = Field(..., alias="appType")
-    app_sub_type: Optional[schemas.AppSubType] = Field(..., alias="appSubType")
-    app_port: Optional[int] = Field(..., alias="appPort")
-    ssh_port: Optional[int] = Field(..., alias="sshPort")
-    execution_environment_id: str = Field(..., alias="executionEnvironmentId")
+    app_sub_type: Optional[schemas.AppSubType] = Field(None, alias="appSubType")
+    app_port: Optional[int] = Field(None, alias="appPort")
+    ssh_port: Optional[int] = Field(None, alias="sshPort")
+    environment_instance_id: str = Field(..., alias="environmentInstanceId")
     created_at: datetime = Field(..., alias="createdAt")
     app_spec_command: str = Field(..., alias="appSpecCommand")
     app_spec_id: str = Field(..., alias="appSpecId")
     app_spec: AppSpec = Field(..., alias="appSpec")
 
 
 class ProjectSecret(BaseGraphQLEntity):
@@ -519,23 +550,26 @@
     _fragment = """
         fragment DeploymentInstance on Deployments {
           createdAt
           deploymentId
           deploymentStatus
           projectId
           machineSize
+          environmentInstanceId
           appSpecId
           sourceCode {
             ...SourceCodeArtifact
           }
           appSpec {
             ...SlingshotAppSpec
           }
         } """
 
     deployment_id: str = Field(..., alias="deploymentId")
     created_at: datetime = Field(..., alias="createdAt")
     deployment_status: schemas.AppInstanceStatus = Field(..., alias="deploymentStatus")
     project_id: str = Field(..., alias="projectId")
     source_code: SourceCodeArtifact = Field(..., alias="sourceCode")
+    machine_size: schemas.MachineSize = Field(..., alias="machineSize")
+    environment_instance_id: str = Field(..., alias="environmentInstanceId")
     app_spec_id: str = Field(..., alias="appSpecId")
     app_spec: AppSpec = Field(..., alias="appSpec")
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydantic import BaseModel, Field
 
 from ..base_graphql import BaseGraphQLQuery
 from ..fragments import ExecutionEnvironment, ExecutionEnvironmentSpec
 
 
 class ExecutionEnvironmentByIdResponse(BaseModel):
-    execution_environments_by_pk: Optional[ExecutionEnvironment] = Field(..., alias="executionEnvironmentsByPk")
+    execution_environments_by_pk: Optional[ExecutionEnvironment] = Field(None, alias="executionEnvironmentsByPk")
 
 
 class ExecutionEnvironmentByIdQuery(BaseGraphQLQuery[ExecutionEnvironmentByIdResponse]):
     _query = """
         query ExecutionEnvironmentById($execEnvId: String!) {
           executionEnvironmentsByPk(executionEnvironmentId: $execEnvId) {
             ...ExecutionEnvironment
@@ -24,15 +24,15 @@
 
     def __init__(self, exec_env_id: str):
         super().__init__(variables={"execEnvId": exec_env_id}, response_model=ExecutionEnvironmentByIdResponse)
 
 
 class ExecutionEnvironmentSpecByIdResponse(BaseModel):
     execution_environment_specs_by_pk: Optional[ExecutionEnvironmentSpec] = Field(
-        ..., alias="executionEnvironmentSpecsByPk"
+        None, alias="executionEnvironmentSpecsByPk"
     )
 
 
 class ExecutionEnvironmentSpecByIdQuery(BaseGraphQLQuery[ExecutionEnvironmentSpecByIdResponse]):
     _query = """
         query ExecutionEnvironmentSpecById($executionEnvironmentSpecId: String!) {
           executionEnvironmentSpecsByPk(executionEnvironmentSpecId: $executionEnvironmentSpecId) {
@@ -71,15 +71,15 @@
 
 class ExecutionEnvironmentSpecId(BaseModel):
     execution_environment_spec_id: str = Field(..., alias="executionEnvironmentSpecId")
 
 
 class ArchiveExecutionEnvironmentSpecResponse(BaseModel):
     update_execution_environment_specs_by_pk: Optional[ExecutionEnvironmentSpecId] = Field(
-        ..., alias="updateExecutionEnvironmentSpecsByPk"
+        None, alias="updateExecutionEnvironmentSpecsByPk"
     )
 
 
 class ArchiveExecutionEnvironmentSpecMutation(BaseGraphQLQuery[ArchiveExecutionEnvironmentSpecResponse]):
     _query = """
         mutation ArchiveExecutionEnvironmentSpec($executionEnvironmentSpecId: String!, $isArchived: Boolean!) {
           updateExecutionEnvironmentSpecsByPk(pkColumns: {executionEnvironmentSpecId: $executionEnvironmentSpecId},
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from slingshot.sdk.graphql import fragments
 
 from ..base_graphql import BaseGraphQLQuery
 
 
 class UserWithProjectsResponse(BaseModel):
-    users_by_pk: Optional[fragments.UserWithProjects] = Field(..., alias="usersByPk")
+    users_by_pk: Optional[fragments.UserWithProjects] = Field(None, alias="usersByPk")
 
 
 class UserWithProjectsQuery(BaseGraphQLQuery[UserWithProjectsResponse]):
     _query = """
         query UserWithProjects($userId: String!) {
           usersByPk(userId: $userId) {
             ...UserWithProjects
@@ -24,15 +24,15 @@
     _depends_on = [fragments.UserWithProjects]
 
     def __init__(self, user_id: str):
         super().__init__(variables={"userId": user_id}, response_model=UserWithProjectsResponse)
 
 
 class ServiceAccountWithProjectsResponse(BaseModel):
-    service_accounts_by_pk: Optional[fragments.ServiceAccountWithProjects] = Field(..., alias="serviceAccountsByPk")
+    service_accounts_by_pk: Optional[fragments.ServiceAccountWithProjects] = Field(None, alias="serviceAccountsByPk")
 
 
 class ServiceAccountWithProjectsQuery(BaseGraphQLQuery[ServiceAccountWithProjectsResponse]):
     _query = """
         query ServiceAccountWithProjects($serviceAccountId: String!) {
           serviceAccountsByPk(serviceAccountId: $serviceAccountId) {
             ...ServiceAccountWithProjects
@@ -44,15 +44,15 @@
     def __init__(self, service_account_id: str):
         super().__init__(
             variables={"serviceAccountId": service_account_id}, response_model=ServiceAccountWithProjectsResponse
         )
 
 
 class ProjectByIdResponse(BaseModel):
-    projects_by_pk: Optional[fragments.ProjectFields] = Field(..., alias="projectsByPk")
+    projects_by_pk: Optional[fragments.ProjectFields] = Field(None, alias="projectsByPk")
 
 
 class ProjectByIdQuery(BaseGraphQLQuery[ProjectByIdResponse]):
     _query = """
         query ProjectById($projectId: String!) {
           projectsByPk(projectId: $projectId) {
             ...ProjectFields
@@ -112,15 +112,15 @@
 
 
 class ProjectWithSecrets(BaseModel):
     project_secrets: list[fragments.ProjectSecret] = Field(..., alias="projectSecrets")
 
 
 class ProjectSecretsResponse(BaseModel):
-    projects_by_pk: Optional[ProjectWithSecrets] = Field(..., alias="projectsByPk")
+    projects_by_pk: Optional[ProjectWithSecrets] = Field(None, alias="projectsByPk")
 
 
 class ProjectSecretsQuery(BaseGraphQLQuery[ProjectSecretsResponse]):
     _query = """
         query ProjectSecrets($projectId: String!) {
             projectsByPk(projectId: $projectId) {
                 projectSecrets {
@@ -136,22 +136,22 @@
 
 
 class SourceCodesResponse(BaseModel):
     source_codes: list[fragments.SourceCodeArtifact] = Field(..., alias="sourceCodes")
 
 
 class SourceCodesForProjectResponse(BaseModel):
-    projects_by_pk: Optional[SourceCodesResponse] = Field(..., alias="projectsByPk")
+    projects_by_pk: Optional[SourceCodesResponse] = Field(None, alias="projectsByPk")
 
 
 class LatestSourceCodeForProjectQuery(BaseGraphQLQuery[SourceCodesForProjectResponse]):
     _query = """
         query LatestSourceCodeForProject($projectId: String!) {
             projectsByPk(projectId: $projectId) {
-                sourceCodes(orderBy: {createdAt: DESC}, limit: 1) {
+                sourceCodes(orderBy: { blobArtifact: { createdAt: DESC } }, limit: 1) {
                     ...SourceCodeArtifact
                 }
             }
         } """
 
     _depends_on = [fragments.SourceCodeArtifact]
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def __init__(self, project_id: str, run_name: str):
         super().__init__(
             variables={"projectId": project_id, "runName": run_name}, response_model=RunsForProjectResponse
         )
 
 
 class RunByIdResponse(BaseModel):
-    run: Optional[Run] = Field(..., alias="trainingRunsByPk")
+    run: Optional[Run] = Field(None, alias="trainingRunsByPk")
 
 
 class RunByIdQuery(BaseGraphQLQuery[RunByIdResponse]):
     _query = """
         query RunById($runId: String!) {
           trainingRunsByPk(trainingRunId: $runId) {
             ...Run
@@ -63,15 +63,15 @@
 
 
 class RunWithStatus(BaseModel):
     job_status: schemas.JobStatus = Field(..., alias="jobStatus")
 
 
 class RunsWithStatusResponse(BaseModel):
-    run: Optional[RunWithStatus] = Field(..., alias="trainingRunsByPk")
+    run: Optional[RunWithStatus] = Field(None, alias="trainingRunsByPk")
 
 
 class RunStatusSubscription(BaseGraphQLQuery[RunsWithStatusResponse]):
     _query = """
         subscription RunStatusSubscription($runId: String!) {
           trainingRunsByPk(trainingRunId: $runId) {
             jobStatus
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class BlobArtifactsResponse(BaseModel):
     blob_artifacts: list[BlobArtifact] = Field(..., alias="blobArtifacts")
 
 
 class BlobArtifactsForProjectResponse(BaseModel):
-    projects_by_pk: Optional[BlobArtifactsResponse] = Field(..., alias="projectsByPk")
+    projects_by_pk: Optional[BlobArtifactsResponse] = Field(None, alias="projectsByPk")
 
 
 class LatestBlobArtifactsForProjectQuery(BaseGraphQLQuery[BlobArtifactsForProjectResponse]):
     _query = """
         query LatestBlobArtifactsForProjectQuery($projectId: String!) {
             projectsByPk(projectId: $projectId) {
                 blobArtifacts(orderBy: {createdAt: DESC}) {
@@ -47,15 +47,15 @@
     def __init__(self, project_id: str, tag: str):
         super().__init__(
             variables={"projectId": project_id, "tag": tag}, response_model=BlobArtifactsForProjectResponse
         )
 
 
 class BlobArtifactByIdResponse(BaseModel):
-    blob_artifacts_by_pk: Optional[BlobArtifact] = Field(..., alias="blobArtifactsByPk")
+    blob_artifacts_by_pk: Optional[BlobArtifact] = Field(None, alias="blobArtifactsByPk")
 
 
 class BlobArtifactByIdQuery(BaseGraphQLQuery[BlobArtifactByIdResponse]):
     _query = """
         query BlobArtifactById($blobArtifactId: String!) {
           blobArtifactsByPk(blobArtifactId: $blobArtifactId) {
             ...BlobArtifact
@@ -68,14 +68,18 @@
         super().__init__(variables={"blobArtifactId": blob_artifact_id}, response_model=BlobArtifactByIdResponse)
 
 
 class BlobArtifactByNameResponse(BaseModel):
     blob_artifacts: list[BlobArtifact] = Field(..., alias="blobArtifacts")
 
 
+class BlobArtifactByTagResponse(BaseModel):
+    blob_artifacts: list[BlobArtifact] = Field(..., alias="blobArtifacts")
+
+
 class BlobArtifactByNameQuery(BaseGraphQLQuery[BlobArtifactByNameResponse]):
     _query = """
         query BlobArtifactByName($blobArtifactName: String!, $projectId: String!) {
           blobArtifacts(where: {_and: {name: {_eq: $blobArtifactName}, projectId: {_eq: $projectId}}}) {
             ...BlobArtifact
           }
         }
@@ -86,14 +90,34 @@
     def __init__(self, blob_artifact_name: str, project_id: str):
         super().__init__(
             variables={"blobArtifactName": blob_artifact_name, "projectId": project_id},
             response_model=BlobArtifactByNameResponse,
         )
 
 
+class BlobArtifactByTagQuery(BaseGraphQLQuery[BlobArtifactByTagResponse]):
+    _query = """
+        query BlobArtifactByTag($blobArtifactTag: String!, $projectId: String!) {
+          blobArtifacts(
+            where: {_and: {tag: {_eq: $blobArtifactTag}, projectId: {_eq: $projectId}, isDraft: {_neq: true}}}
+          ) {
+            ...BlobArtifact
+          }
+        }
+    """
+
+    _depends_on = [BlobArtifact]
+
+    def __init__(self, blob_artifact_tag: str, project_id: str):
+        super().__init__(
+            variables={"blobArtifactTag": blob_artifact_tag, "projectId": project_id},
+            response_model=BlobArtifactByTagResponse,
+        )
+
+
 class VolumesForProjectResponse(BaseModel):
     volumes: list[Volume] = Field(..., alias="volumes")
 
 
 class VolumesForProjectQuery(BaseGraphQLQuery[VolumesForProjectResponse]):
     _query = """
         query VolumesForProject($projectId: String!) {
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import contextlib
 import datetime
 import json
 import logging
 import shutil
+import uuid
 from pathlib import Path
 from typing import (
     Any,
     AsyncGenerator,
     AsyncIterator,
     Awaitable,
     BinaryIO,
@@ -20,15 +21,15 @@
     overload,
 )
 
 import aiohttp
 import backoff
 import sentry_sdk
 from aiohttp import FormData, WSMessage
-from pydantic import BaseModel, ValidationError, parse_obj_as
+from pydantic import BaseModel, TypeAdapter, ValidationError
 
 from .. import schemas
 from ..schemas import AuthTokenUnion, Hyperparameter, MachineSize
 from ..shared.utils import get_data_or_raise
 from . import config
 from .errors import (
     SlingshotBackoffError,
@@ -42,15 +43,15 @@
 from .graphql import BaseGraphQLQuery, base_graphql, fragments, queries
 from .graphql.queries import (
     ProjectSecretsQuery,
     ProjectSecretsResponse,
     RunByIdResponse,
     ServiceAccountWithProjectsResponse,
 )
-from .utils import gql_mount_spec_to_read_mount_spec
+from .utils import console, gql_mount_spec_to_read_mount_spec
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=Union[BaseModel, str, bytes, tuple[Any, ...], list[Any], dict[str, Any]])
 JSONType = dict[str, Any]
 ParamsType = dict[str, Union[str, float, int]]
 
@@ -106,15 +107,15 @@
     async def make_request(
         self,
         url: str,
         *,
         method: str,
         response_model: Type[T] | None,
         params: ParamsType | None = None,
-        json_data: JSONType | None = None,
+        json_data: JSONType | str | None = None,
         data: dict[str, Any] | FormData | BinaryIO | bytes | None = None,
         headers: dict[str, str] | None = None,
         timeout: datetime.timedelta | None = None,
         _setup: bool = True,
     ) -> T:
         # If the url is relative, we need to prepend the base url
         if not url.startswith("http"):
@@ -157,15 +158,15 @@
                         return await resp.json()
                     resp_data: dict[str, Any] | FormData | None = await resp.json()
         except aiohttp.ClientConnectorError as e:
             if self._slingshot_url != config.global_config.slingshot_local_url:
                 sentry_sdk.capture_exception(e, api_url=self._api_url)
             raise SlingshotConnectionError(self._api_url) from e
         try:
-            return parse_obj_as(response_model, resp_data)
+            return TypeAdapter(response_model).validate_python(resp_data)
         except ValidationError as e:
             if self._slingshot_url != config.global_config.slingshot_local_url:
                 with sentry_sdk.push_scope() as scope:
                     scope.set_extra("response", resp_data)
                     scope.set_extra("response_model", response_model)
                     sentry_sdk.capture_exception(e, api_url=self._api_url)
             raise SlingshotException(f"Unexpected response format. {e}: {resp_data}") from e
@@ -217,15 +218,15 @@
                         if msg.type == aiohttp.WSMsgType.TEXT:
                             data = json.loads(msg.data)
                             if data["type"] == "connection_error":
                                 raise SlingshotException(f"WebSocket connection error: {data['payload']}")
                             elif "errors" in data:
                                 raise SlingshotException(f"GraphQL error: {data['errors']}")
                             elif data["type"] == "data":
-                                yield parse_obj_as(type_, data).payload
+                                yield TypeAdapter(type_).validate_python(data).payload
                             else:
                                 logger.debug(f"Received unexpected message: {data}")
                         elif msg.type == aiohttp.WSMsgType.ERROR:
                             raise SlingshotException(f"WebSocket error: {msg.data}")
 
             logger.info("Websocket connection closed -- retrying")
 
@@ -261,14 +262,21 @@
 
     async def list_machine_types(self) -> list[schemas.MachineTypeListItem]:
         """Get a list of available machine types."""
         return await self._client.make_request(
             "machine_types", method="get", response_model=list[schemas.MachineTypeListItem]
         )
 
+    async def project_id_available(self, project_id: str) -> bool:
+        """Check if a project ID is available."""
+        resp = await self._client.make_request(
+            "/project/project_id_available", method="post", json_data=project_id, response_model=schemas.BoolResponse
+        )
+        return get_data_or_raise(resp)
+
     """
     Auth API methods
     """
 
     async def user_login(self, auth0_token: str) -> schemas.AuthToken:
         """Sign in with an Auth0 CLI token."""
         auth_token_resp: schemas.AuthTokenResponse = await self._client.make_request(
@@ -470,21 +478,18 @@
     ) -> schemas.UsageBinsLatencyQuantiles:
         """Get the latencies for a deployment."""
         resp = await self._client.make_request(
             url=f"project/{project_id}/deploy/{deployment_id}/latencies",
             method="get",
             response_model=schemas.UsageBinsLatencyQuantilesResponse,
         )
-        if resp.error:
-            raise SlingshotException(resp.error)
-
         return get_data_or_raise(resp)
 
     async def get_environment_spec(
-        self, execution_environment_spec_id: str, *, project_id: str
+        self, execution_environment_spec_id: str
     ) -> fragments.ExecutionEnvironmentSpec | None:
         """Get an execution environment spec by id."""
         query = queries.ExecutionEnvironmentSpecByIdQuery(execution_environment_spec_id=execution_environment_spec_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         return data and data.execution_environment_specs_by_pk
 
@@ -500,14 +505,22 @@
     ) -> fragments.BlobArtifact | None:
         """Get a blob artifact by id."""
         query = queries.BlobArtifactByNameQuery(blob_artifact_name=blob_artifact_name, project_id=project_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         return data.blob_artifacts[0] if data.blob_artifacts else None
 
+    async def get_blob_artifacts_by_tag(
+        self, blob_artifact_tag: str, *, project_id: str
+    ) -> list[fragments.BlobArtifact]:
+        query = queries.BlobArtifactByTagQuery(blob_artifact_tag=blob_artifact_tag, project_id=project_id)
+        resp = await self._client.make_graphql_request(query)
+        data = resp.get_data_or_raise()
+        return data.blob_artifacts
+
     async def get_exec_env(self, exec_env_id: str) -> fragments.ExecutionEnvironment | None:
         """Get an execution environment by id."""
         query = queries.ExecutionEnvironmentByIdQuery(exec_env_id=exec_env_id)
         resp = await self._client.make_graphql_request(query)
         data = resp.get_data_or_raise()
         if not data.execution_environments_by_pk:
             return None
@@ -626,15 +639,15 @@
         self, project_id: str, project_display_name: Optional[str] = None
     ) -> schemas.Response[schemas.ProjectId]:
         """Create a new project."""
         return await self._client.make_request(
             url=f"project",
             method="post",
             response_model=schemas.Response[schemas.ProjectId],
-            json_data=schemas.BodyNewProject(project_id=project_id, display_name=project_display_name).dict(),
+            json_data=schemas.BodyNewProject(project_id=project_id, display_name=project_display_name).model_dump(),
         )
 
     async def create_app(
         self,
         name: str,
         command: str | None,
         app_type: schemas.AppType,
@@ -645,56 +658,59 @@
         attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         *,
         project_id: str,
     ) -> schemas.AppSpecIdResponse:
         """Create an app spec."""
-        mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mounts]
         body = schemas.CreateAppBody(
             name=name,
             command=command,
             app_type=app_type,
             app_sub_type=app_sub_type,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
-            mounts=mount_requests,
+            mounts=[mount.model_dump() for mount in mounts],  # Must be dict or Pydantic fails to process the union
             attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
-        ).dict()
+        ).model_dump()
         body["machine_size"] = machine_size.value
 
         return await self._client.make_request(
             url=f"project/{project_id}/apps", method="post", response_model=schemas.AppSpecIdResponse, json_data=body
         )
 
     async def create_or_update_environment_spec(
         self,
         name: str,
         requested_python_requirements: list[schemas.RequestedRequirement] | None = None,
         requested_apt_requirements: list[schemas.RequestedAptPackage] | None = None,
-        gpu_drivers: bool = False,
+        post_install_command: str | None = None,
         force_create_environment: bool = False,
         *,
         project_id: str,
     ) -> schemas.CreateEnvironmentSpecResponse:
         """Create or update an environment spec."""
+        python_packages = [req.model_dump() for req in requested_python_requirements or []]
+        apt_packages = [req.model_dump() for req in requested_apt_requirements or []]
         body = schemas.ExecutionEnvironmentSpecRequestBody(
             name=name,
-            python_packages=requested_python_requirements or [],
-            apt_packages=requested_apt_requirements or [],
-            gpu_drivers=gpu_drivers,
+            # The following two fields must be dicts, otherwise we get a parsing error since we override the generated
+            # API models with custom validators
+            python_packages=python_packages,
+            apt_packages=apt_packages,
+            post_install_command=post_install_command or "",
             force_create_environment=force_create_environment,
         )
         return await self._client.make_request(
             url=f"project/{project_id}/environment",
             method="post",
             response_model=schemas.CreateEnvironmentSpecResponse,
-            json_data=body.dict(),
+            json_data=body.model_dump(),
         )
 
     async def create_volume(self, volume_name: str, *, project_id: str) -> schemas.Response[str]:
         """Create a volume."""
         return await self._client.make_request(
             url=f"project/{project_id}/volume",
             method="post",
@@ -715,37 +731,34 @@
         mounts: list[schemas.MountSpecUnion],
         attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         batch_size: int | None = None,
         batch_interval: int | None = None,
         *,
-        name: str | None = None,
         project_id: str,
-    ) -> schemas.Response[bool]:
+    ) -> schemas.BoolResponse:
         """Update an app spec."""
-        mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mounts]
         body = schemas.UpdateAppBody(
             command=command,
-            name=name,
             exec_env_spec_id=exec_env_spec_id,
             machine_size=machine_size,
-            mounts=mount_requests,
+            mounts=[mount.model_dump() for mount in mounts],  # Must be dict or Pydantic fails to process the union
             config_variables=config_variables,
             attach_project_credentials=attach_project_credentials,
             app_port=app_port,
             batch_size=batch_size,
             batch_interval=batch_interval,
-        ).dict()
+        ).model_dump()
         # TODO: Find a way for pydantic not to convert machine_size to an enum
         body["machine_size"] = machine_size.value
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec_id}",
             method="post",
-            response_model=schemas.Response[bool],
+            response_model=schemas.BoolResponse,
             json_data=body,
         )
 
     async def put_secret(self, secret_name: str, secret_value: str, *, project_id: str) -> schemas.PutResultResponse:
         """Update a secret by name."""
         return await self._client.make_request(
             url=f"project/{project_id}/secret/{secret_name}",
@@ -760,29 +773,27 @@
 
     async def delete_app(self, app_spec_id: str, project_id: str) -> schemas.ResponseOK:
         """Delete an app spec."""
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec_id}", method="delete", response_model=schemas.ResponseOK
         )
 
-    async def delete_environment_spec(
-        self, execution_environment_spec_id: str, *, project_id: str | None = None
-    ) -> None:
+    async def delete_environment_spec(self, execution_environment_spec_id: str) -> None:
         """Delete an environment spec."""
         mutation = queries.ArchiveExecutionEnvironmentSpecMutation(
             execution_environment_spec_id=execution_environment_spec_id, is_archived=True
         )
         resp = await self._client.make_graphql_request(mutation)
         resp.get_data_or_raise()
         return None
 
-    async def delete_volume(self, volume_name: str, *, project_id: str) -> schemas.Response[bool]:
+    async def delete_volume(self, volume_name: str, *, project_id: str) -> schemas.BoolResponse:
         """Delete a volume."""
         return await self._client.make_request(
-            url=f"project/{project_id}/volume/{volume_name}", method="delete", response_model=schemas.Response[bool]
+            url=f"project/{project_id}/volume/{volume_name}", method="delete", response_model=schemas.BoolResponse
         )
 
     async def delete_secret(self, secret_name: str, *, project_id: str) -> schemas.DeleteResultResponse:
         """Delete a secret by name."""
         return await self._client.make_request(
             url=f"project/{project_id}/secret/{secret_name}",
             method="delete",
@@ -798,15 +809,15 @@
         *,
         app_spec: fragments.AppSpec,
         machine_size: schemas.MachineSize | None = None,
         source_code_id: str | None = None,
         cmd: str | None = None,
         mount_specs: list[schemas.MountSpecUnion] | None = None,
         config_variables: JSONType | None = None,
-        exec_env_id: str | None = None,
+        env_instance_id: str | None = None,
         attach_project_credentials: bool | None = None,
         app_port: int | None = None,
         project_id: str,
     ) -> schemas.HasAppInstanceIdResponse:
         """Start an app."""
         # TODO: Separate the SDK logic (using existing spec) from the API logic
 
@@ -815,125 +826,139 @@
 
         machine_size = machine_size or app_spec.machine_size
         command = cmd or app_spec.app_spec_command
         if mount_specs is None:
             mount_specs = [schemas.mount_spec_from_remote(mount_spec) for mount_spec in app_spec.mount_specs]
         if config_variables is None and app_spec.config_variables is not None:
             config_variables = json.loads(app_spec.config_variables)
-        exec_env_id = exec_env_id or app_spec.execution_environment_spec.execution_environment.execution_environment_id
+        env_instance_id = (
+            env_instance_id or app_spec.execution_environment_spec.environment_instances[0].environment_instance_id
+        )
         attach_project_credentials = (
             attach_project_credentials if attach_project_credentials is not None else app_spec.service_account
         )
         app_port = app_port or app_spec.app_port
-        mount_requests = [parse_obj_as(schemas.MountRequestUnion, i) for i in mount_specs]
         body = schemas.StartAppBody(
             machine_size=machine_size,
             source_code_id=source_code_id,
             cmd=command,
-            mounts=mount_requests,
+            mounts=[mount.model_dump() for mount in mount_specs],  # Must be dict or Pydantic fails to process the union
             config_variables=config_variables,
-            exec_env_id=exec_env_id,
+            environment_instance_id=env_instance_id,
             attach_project_credentials=attach_project_credentials,
             app_port=app_port,
         )
 
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec.app_spec_id}/start",
             method="post",
             response_model=schemas.HasAppInstanceIdResponse,
-            json_data=body.dict(),
+            json_data=body.model_dump(),
         )
 
     async def start_run(
         self,
         run_spec: fragments.AppSpec,
         source_code_id: str | None = None,
         machine_size: Optional[schemas.MachineSize] = None,
         hyperparameters: Hyperparameter | None = None,
         cmd: str | None = None,
         mount_specs: list[schemas.MountSpecUnion] | None = None,
-        exec_env_id: str | None = None,
+        environment_instance_id: str | None = None,
         attach_project_credentials: bool | None = None,
         debug_mode: bool = False,  # TODO: maybe don't expose this to the user
         *,
         project_id: str,
     ) -> schemas.RunCreateResponse:
         """Start a run."""
         machine_size = machine_size or run_spec.machine_size
         if not hyperparameters and run_spec.config_variables:
             hyperparameters = json.loads(run_spec.config_variables)
         command = cmd or run_spec.app_spec_command
         mount_specs = mount_specs or [
             gql_mount_spec_to_read_mount_spec(mount_spec) for mount_spec in run_spec.mount_specs
         ]
-        exec_env_id = exec_env_id or run_spec.execution_environment_spec.execution_environment.execution_environment_id
+        environment_instance_id = (
+            environment_instance_id
+            or run_spec.execution_environment_spec.environment_instances[0].environment_instance_id
+        )
         should_attach_project_credentials = (
             attach_project_credentials if attach_project_credentials is not None else run_spec.service_account
         )
 
+        download_tag_mount_specs = [spec for spec in mount_specs if isinstance(spec, schemas.DownloadByTagMountSpec)]
+        for mount in download_tag_mount_specs:
+            artifacts = await self.get_blob_artifacts_by_tag(mount.tag, project_id=project_id)
+            if not artifacts:
+                console.print(
+                    f"[yellow]Warning[/yellow]: No artifacts found for tag '{mount.tag}' -- this will cause "
+                    f"'{mount.path}' to be mounted as an empty directory."
+                )
+
         body = schemas.StartAppBody(
             source_code_id=source_code_id,
             machine_size=machine_size,
             config_variables=hyperparameters,
             cmd=command,
-            mounts=mount_specs,  # TODO: Fix this
-            exec_env_id=exec_env_id,
+            mounts=[mount.model_dump() for mount in mount_specs],  # Must be dict or Pydantic fails to process the union
+            environment_instance_id=environment_instance_id,
             attach_project_credentials=should_attach_project_credentials,
         )
 
         return await self._client.make_request(
             url=f"project/{project_id}/run/{run_spec.app_spec_id}/start",
             method="post",
             response_model=schemas.RunCreateResponse,
             params={"debug_mode": json.dumps(debug_mode)},
-            json_data=body.dict(),
+            json_data=body.model_dump(),
         )
 
     async def deploy_model(
         self,
         source_code_id: str,
         deployment_spec_id: str,
         machine_size: schemas.MachineSize | None = None,
         config_variables: JSONType | None = None,
         mount_specs: list[schemas.MountSpecUnion] | None = None,
-        exec_env_id: str | None = None,
+        environment_instance_id: str | None = None,
         cmd: str | None = None,
         *,
         project_id: str,
     ) -> schemas.DeploymentInstanceIdResponse:
         """Start a deployment."""
         deployment_spec = await self.get_app_spec_by_id(deployment_spec_id, project_id=project_id)
         if not deployment_spec:
             raise SlingshotException(f"Deployment not found: {deployment_spec_id}")
         machine_size = machine_size or deployment_spec.machine_size
         if not config_variables and deployment_spec.config_variables:
             config_variables = json.loads(deployment_spec.config_variables)
         mount_specs = mount_specs or [
             gql_mount_spec_to_read_mount_spec(mount_spec) for mount_spec in deployment_spec.mount_specs
         ]
-        exec_env_id = (
-            exec_env_id or deployment_spec.execution_environment_spec.execution_environment.execution_environment_id
+        environment_instance_id = (
+            environment_instance_id
+            or deployment_spec.execution_environment_spec.environment_instances[0].environment_instance_id
         )
         cmd = cmd or deployment_spec.app_spec_command
         should_attach_project_credentials = deployment_spec.service_account
 
         body = schemas.StartAppBody(
             source_code_id=source_code_id,
             machine_size=machine_size,
             config_variables=config_variables,
-            mounts=mount_specs,  # TODO: Fix this
-            exec_env_id=exec_env_id,
+            mounts=[mount.model_dump() for mount in mount_specs],  # Must be dict or Pydantic fails to process the union
+            environment_instance_id=environment_instance_id,
             cmd=cmd,
             attach_project_credentials=should_attach_project_credentials,
         )
         return await self._client.make_request(
             url=f"project/{project_id}/deploy/{deployment_spec_id}/start",
             method="post",
             response_model=schemas.DeploymentInstanceIdResponse,
-            json_data=body.dict(),
+            json_data=body.model_dump(),
         )
 
     async def start_app_code_sync(self, app_spec_id: str, *, project_id: str) -> schemas.Response[schemas.SshPort]:
         """Start code sync for an app."""
         return await self._client.make_request(
             url=f"project/{project_id}/apps/{app_spec_id}/sync/start",
             method="post",
@@ -964,24 +989,26 @@
             response_model=schemas.ResponseOK,
         )
 
     """
     Logs API methods
     """
 
-    async def get_app_logs(self, app_spec_id: str, project_id: str) -> schemas.LogsResponse:
+    async def get_app_logs(self, app_spec_id: str, project_id: str) -> schemas.ListLogLineResponse:
         """Get logs for an app spec."""
         return await self._client.make_request(
-            url=f"project/{project_id}/apps/{app_spec_id}/logs", method="get", response_model=schemas.LogsResponse
+            url=f"project/{project_id}/apps/{app_spec_id}/logs",
+            method="get",
+            response_model=schemas.ListLogLineResponse,
         )
 
-    async def get_run_logs(self, run_id: str, *, project_id: str) -> schemas.LogsResponse:
+    async def get_run_logs(self, run_id: str, *, project_id: str) -> schemas.ListLogLineResponse:
         """Get logs for a run."""
         return await self._client.make_request(
-            url=f"project/{project_id}/run/{run_id}/logs", method="get", response_model=schemas.LogsResponse
+            url=f"project/{project_id}/run/{run_id}/logs", method="get", response_model=schemas.ListLogLineResponse
         )
 
     """
     Predict API methods
     """
 
     async def predict(
@@ -1007,36 +1034,36 @@
         """Make a prediction to an OpenAI model."""
         # TODO: Add idempotence key. If the client wants to cache, they can set idempotence_key to hash of prompt.
         try:
             return await self._client.make_request(
                 url=f"project/{project_id}/prompt/openai",
                 method="post",
                 response_model=schemas.OpenAIResponse,
-                json_data=request.dict(),
+                json_data=request.model_dump(),
                 timeout=timeout,
             )
         except SlingshotClientHttpException as e:
             if e.status == 429 or e.status == 503:
                 raise Retry(e)
             raise e
 
     """
     Artifact API methods
     """
 
     async def signed_url_blob_artifact_many(
         self, blob_artifact_id: str, expiration: datetime.timedelta = datetime.timedelta(hours=1), *, project_id: str
-    ) -> schemas.BlobArtifactSignedURLManyResponse:
-        """Get a signed URL for an artifact."""
+    ) -> schemas.ListBlobArtifactSignedURLResponse:
+        """Get signed URLs for an artifact's contents."""
         params: dict[str, float | str] = {"expiration": expiration.total_seconds()}
         return await self._client.make_request(
             url=f"project/{project_id}/artifact/{blob_artifact_id}/signed_url_many",
             params=params,
             method="get",
-            response_model=schemas.BlobArtifactSignedURLManyResponse,
+            response_model=schemas.ListBlobArtifactSignedURLResponse,
         )
 
     async def signed_url_blob_artifact(
         self,
         blob_artifact_id: str,
         file_path: str | None = None,
         expiration: datetime.timedelta = datetime.timedelta(hours=1),
@@ -1060,29 +1087,40 @@
         """Apply an upsert to the latest dataset matching the given tag using an existing upsert artifact."""
         return await self._client.make_request(
             url=f"project/{project_id}/artifact/{upsert_artifact_id}/upsert/{dataset_artifact_tag}",
             method="post",
             response_model=schemas.BlobArtifactIdResponse,
         )
 
+    async def upload_signed_url_blob_artifact_many(
+        self, filenames: list[str], *, project_id: str, blob_artifact_tag: str | None = None
+    ) -> schemas.BlobArtifactUploadSignedURLManyResponse:
+        """Get signed URLs for an artifact's contents."""
+        return await self._client.make_request(
+            url=f"project/{project_id}/artifact/upload_signed_url_many",
+            method="get",
+            json_data=schemas.UploadBlobArtifactManyBody(filenames=filenames, tag=blob_artifact_tag).model_dump(),
+            response_model=schemas.BlobArtifactUploadSignedURLManyResponse,
+        )
+
     async def upload_signed_url_blob_artifact(
         self,
         filename: str,
         as_zip: bool,  # Defaults to True if artifact_path is a directory
         blob_artifact_tag: str | None = None,
         *,
         project_id: str,
     ) -> schemas.BlobArtifactUploadSignedURLResponse:
         """Get a signed URL for uploading an artifact."""
         return await self._client.make_request(
             url=f"project/{project_id}/artifact/upload_signed_url",
             method="get",
             json_data=schemas.UploadBlobArtifactBody(
                 filename=filename, tag=blob_artifact_tag, is_zipped_directory=as_zip
-            ).dict(),
+            ).model_dump(),
             response_model=schemas.BlobArtifactUploadSignedURLResponse,
         )
 
     """
     Source code API methods
     """
 
@@ -1096,26 +1134,23 @@
         return await self._client.make_request(
             url=f"project/{project_id}/source_code",
             method="post",
             response_model=schemas.Response[schemas.UploadedSourceCode],
             params=params,
         )
 
-    """
-    Environment API methods
-    """
-
-    async def rebuild_all_environments(self) -> str:
-        """Trigger a rebuild of all environments."""
-        return await self._client.make_request(url=f"admin/rebuild_all_environments", method="post", response_model=str)
-
 
 async def _zip_dir(dir_path: Path) -> str:
     # TODO: Use a temporary directory instead of the current directory, Then delete the temporary directory.
-    return shutil.make_archive("data", "zip", dir_path)
+    # Choose a filename that doesn't exist in the local folder to avoid overwriting files.
+    while True:
+        filename = f"data_{uuid.uuid4().hex[:8]}"
+        if not Path(filename).exists():
+            break
+    return shutil.make_archive(filename, "zip", dir_path)
 
 
 @contextlib.asynccontextmanager
 async def _maybe_make_http_session(session: aiohttp.ClientSession | None) -> AsyncIterator[aiohttp.ClientSession]:
     if session is None or session.closed:
         async with aiohttp.ClientSession() as session:
             yield session
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import datetime
 import functools
+import glob
 import json
 import os
 import tempfile
 import time
 import typing
 import uuid
 from asyncio import wait_for
@@ -18,35 +19,41 @@
 
 import openai.error
 import typer
 from tqdm.auto import tqdm
 
 from slingshot import schemas
 from slingshot.sdk import config
-from slingshot.sdk.errors import SlingshotCodeNotFound, SlingshotException, SlingshotUnauthenticatedError
+from slingshot.sdk.errors import (
+    SlingshotCodeNotFound,
+    SlingshotException,
+    SlingshotNoProjectSetError,
+    SlingshotUnauthenticatedError,
+)
 from slingshot.sdk.upload_download_utils import download_file_in_parts, upload_file_in_parts_to_gcs
 from slingshot.slingshot_version import __version__
 
 from ..cli.shared import format_logline
 from ..schemas import Hyperparameter, LogLine, Response, SshPort
 from ..shared.utils import get_data_or_raise
 from .apply import ApplyService
 from .auth import login_auth0
 from .config import global_config, project_config
 from .graphql import fragments
-from .graphql.fragments import ExecutionEnvironmentSpec
 from .slingshot_api import JSONType, SlingshotAPI, SlingshotClient, _zip_dir
 from .sync import sync_code, zip_code_artifact
 from .utils import console, md5_hash
 from .web_path_util import WebPathUtil
 
 logger = getLogger(__name__)
 
 Function = typing.TypeVar("Function", bound=typing.Callable[..., typing.Awaitable[typing.Any]])
 
+BYTES_PER_MB = 1024 * 1024
+
 
 def experimental(f: Function) -> Function:
     """Decorator for experimental functions"""
 
     @wraps(f)
     def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
         # TODO: Implement some kind of warning
@@ -219,50 +226,40 @@
         """Set the current project"""
         project_fields = await self._api.get_project_by_id(project_id)
         if not project_fields:
             raise SlingshotException(f"Project '{project_id}' not found.")
         self.project = project_fields
         project_config.project_id = project_id
 
-    async def apply_project(
-        self, and_wait: bool = False, force: bool = False
-    ) -> tuple[bool, list[ExecutionEnvironmentSpec]]:
+    async def apply_project(self, force: bool = False) -> bool:
         """
         Apply the YAML configuration in the current directory to the current project.
 
         Returns True if any changes were applied, False otherwise.
         """
-        return await ApplyService(self).plan_prompt_apply(and_wait=and_wait, force=force)
+        return await ApplyService(self).apply(force=force)
 
-    async def apply_to_local(self, force: bool = False, print_logs: bool = False) -> bool:
+    async def pull_remote_changes(self, force: bool = False) -> bool:
         """
-        Apply the YAML configuration from the remote project to the current project.
+        Pull the YAML configuration from the remote project to the current project.
 
-        Returns True if any changes were applied.
+        Returns True if any changes were pulled.
         """
-        any_changes_applied = await ApplyService(self).apply_to_local(None, force=force)
-
-        if print_logs:
-            if not any_changes_applied:
-                console.print("No changes pulled")
-            else:
-                console.print("Changes pulled to your local 'slingshot.yaml'.")
-
-        return any_changes_applied
+        return await ApplyService(self).check_conflicts_pull_remote_changes(force=force)
 
     """
     Source code SDK methods
     """
 
     async def push_code(
         self, code_dir: str | None = None, description: Optional[str] = None, and_print: bool = False
     ) -> schemas.UploadedSourceCode:
         """Push code from current (or specified) directory to Slingshot"""
         path = Path(code_dir or ".")
-        created_source_code, is_new = await sync_code(self, path, description)
+        created_source_code, is_new = await sync_code(self, path, description, quiet=not and_print)
         source_code_name = created_source_code.source_code_name
         link = await self.web_path_util.code(created_source_code)
         if not and_print:
             return created_source_code
         if is_new:
             console.print(f"Pushed new source code '{source_code_name}', view in browser at {link}")
         else:
@@ -308,19 +305,19 @@
             download_filepath = typer.prompt("Please enter a new filename")
 
         Path(download_filepath).parent.mkdir(parents=True, exist_ok=True)
         await download_file_in_parts(download_filepath, signed_url=signed_url, client=self._client)
         return download_filepath
 
     async def download_artifact(
-        self, blob_artifact_id: str, save_path: str | None = None, prompt_overwrite: bool = False, unzip: bool = False
+        self, blob_artifact_id: str, save_path: str | None = None, prompt_overwrite: bool = False, no_zip: bool = False
     ) -> str:
         """Download an artifact from the current project."""
         project_id = await self._get_current_project_id_or_raise()
-        if unzip:
+        if no_zip:
             blob_artifacts_response = await self._api.signed_url_blob_artifact_many(
                 blob_artifact_id, project_id=project_id
             )
 
             list_response = get_data_or_raise(blob_artifacts_response)
             # TODO: batch these requests -- currently we are downloading all at once which is not scalable and will
             #  probably cause timeouts.
@@ -334,66 +331,162 @@
                     for url_response in list_response
                 ]
             ):
                 res = await path
                 console.print(f"Completed processing {res}")
             return save_path or (list_response and list_response[0].blob_artifact_name) or ""
 
-        blob_artifact_response = await self._api.signed_url_blob_artifact(blob_artifact_id, project_id=project_id)
+        # Check the blob artifact size before proceeding in zipped mode.
+        blob_artifact_response = await self._api.get_blob_artifact_by_id(blob_artifact_id)
+
+        if not blob_artifact_response:
+            raise SlingshotException(f"Blob artifact {blob_artifact_id} not found")
+
+        if not blob_artifact_response.bytes_size:
+            raise SlingshotException(
+                f"Blob artifact {blob_artifact_id} may be corrupt -- contact slingshot support for help."
+            )
+
+        if blob_artifact_response.bytes_size > 100 * BYTES_PER_MB:
+            console.print("Artifact too large to zip -- downloading in non-zip mode.")
+            return await self.download_artifact(blob_artifact_id, save_path, prompt_overwrite, no_zip=True)
+
+        blob_artifact_url_response = await self._api.signed_url_blob_artifact(blob_artifact_id, project_id=project_id)
 
-        url_response = get_data_or_raise(blob_artifact_response)
+        url_response = get_data_or_raise(blob_artifact_url_response)
 
         return await self._process_signed_url_download(
             url_response, save_path=save_path, prompt_overwrite=prompt_overwrite
         )
 
+    async def _process_signed_url_upload(
+        self,
+        *,
+        filename: str,
+        blob_artifact_tag: str | None,
+        as_zip: bool,
+        project_id: str,
+        artifact_path: Path,
+        quiet: bool = False,
+    ) -> fragments.BlobArtifact:
+        resp: schemas.BlobArtifactUploadSignedURLManyResponse = await self._api.upload_signed_url_blob_artifact(
+            filename, blob_artifact_tag=blob_artifact_tag, as_zip=as_zip, project_id=project_id
+        )
+
+        upload_signed_url_response = get_data_or_raise(resp)
+        upload_signed_url = upload_signed_url_response.signed_url
+        blob_artifact_id = upload_signed_url_response.blob_artifact_id
+
+        await upload_file_in_parts_to_gcs(
+            str(artifact_path), upload_signed_url=upload_signed_url, client=self._client, quiet=quiet
+        )
+
+        # Finalize the upload once all parts have been uploaded
+        finalize = await self._client.make_request(
+            url=f"project/{project_id}/artifact/{blob_artifact_id}/finalize",
+            method="post",
+            response_model=schemas.ResponseOK,
+        )
+        get_data_or_raise(finalize)
+        blob_artifact = await self._api.get_blob_artifact_by_id(blob_artifact_id=blob_artifact_id)
+
+        assert blob_artifact, "Blob artifact not found"
+        return blob_artifact
+
     async def upload_artifact(
         self,
         artifact_path: Path,
         blob_artifact_tag: str | None = None,
         as_zip: bool | None = None,  # Defaults to True if artifact_path is a directory
+        quiet: bool = False,
     ) -> fragments.BlobArtifact:
         """Upload an artifact to the current project."""
         project_id = await self._get_current_project_id_or_raise()
-        is_directory = os.path.isdir(artifact_path)
-        if is_directory:
-            logger.info(f"Zipping directory {artifact_path}")
-            artifact_path = Path(await _zip_dir(artifact_path))
-            as_zip = True if as_zip is None else as_zip
-
-        if not os.path.isfile(artifact_path):
+        if not artifact_path.exists():
             raise SlingshotException(f"File path {artifact_path} does not exist")
 
-        if is_directory and not as_zip:
-            raise SlingshotException("Uploading unzipped directories is not supported yet")
+        if artifact_path.is_dir():
+            as_zip = True if as_zip is None else as_zip
 
         filename = os.path.basename(artifact_path)
         if as_zip is None:
             # If filename ends with .zip, and we haven't set as_zip yet, then assume it's a zip file, otherwise must be
             #  a file.
             as_zip = filename.endswith(".zip")
 
-        resp: schemas.BlobArtifactUploadSignedURLResponse = await self._api.upload_signed_url_blob_artifact(
-            filename, blob_artifact_tag=blob_artifact_tag, as_zip=as_zip, project_id=project_id
+        # Case 1: we are uploading a zip file from a local path
+        if as_zip:
+            logger.info(f"Zipping directory {artifact_path}")
+            artifact_path = Path(await _zip_dir(artifact_path)) if not filename.endswith(".zip") else artifact_path
+            blob_artifact = await self._process_signed_url_upload(
+                filename=filename,
+                blob_artifact_tag=blob_artifact_tag,
+                as_zip=as_zip,
+                project_id=project_id,
+                artifact_path=artifact_path,
+                quiet=quiet,
+            )
+
+            # If we created a new zip file, then clean it up
+            # TODO: we should probably do this in a `finally` block or use a context manager
+            os.remove(artifact_path)
+
+            return blob_artifact
+
+        # Case 2: we are uploading a non-zip of a single file.
+        if not artifact_path.is_dir():
+            return await self._process_signed_url_upload(
+                filename=filename,
+                blob_artifact_tag=blob_artifact_tag,
+                as_zip=as_zip,
+                project_id=project_id,
+                artifact_path=artifact_path,
+                quiet=quiet,
+            )
+
+        # Case 3: we are uploading a directory in non-zipped form but producing just one artifact.
+        filename_candidates = glob.glob(f"{filename}/**", recursive=True)
+        filenames = [
+            os.path.relpath(glob_result, Path(filename))
+            for glob_result in filename_candidates
+            if Path(glob_result).is_file()
+        ]
+
+        resp: schemas.BlobArtifactUploadSignedURLManyResponse = await self._api.upload_signed_url_blob_artifact_many(
+            filenames, blob_artifact_tag=blob_artifact_tag, project_id=project_id
         )
-        upload_signed_url_response = get_data_or_raise(resp)
-        upload_signed_url = upload_signed_url_response.signed_url
-        blob_artifact_id = upload_signed_url_response.blob_artifact_id
 
-        await upload_file_in_parts_to_gcs(str(artifact_path), upload_signed_url=upload_signed_url, client=self._client)
+        upload_url_many_data = get_data_or_raise(resp)
+        blob_artifact_id = upload_url_many_data.blob_artifact_id
+        filename_to_signed_url = upload_url_many_data.filename_to_signed_url
+
+        # TODO: batch these requests -- currently we are uploading all at once which is not scalable and will probably
+        #  cause timeouts.
+        for task in asyncio.as_completed(
+            [
+                upload_file_in_parts_to_gcs(
+                    f"{filename}/{rel_path}", upload_signed_url=upload_signed_url, client=self._client, quiet=quiet
+                )
+                for rel_path, upload_signed_url in filename_to_signed_url.items()
+            ]
+        ):
+            await task
 
         # Finalize the upload once all parts have been uploaded
-        await self._client.make_request(
+        res = await self._client.make_request(
             url=f"project/{project_id}/artifact/{blob_artifact_id}/finalize",
             method="post",
             response_model=schemas.ResponseOK,
         )
-        blob_artifact = await self._api.get_blob_artifact_by_id(blob_artifact_id=blob_artifact_id)
-        assert blob_artifact, "Blob artifact not found"
-        return blob_artifact
+
+        get_data_or_raise(res)
+
+        blob_artifact_ = await self._api.get_blob_artifact_by_id(blob_artifact_id=blob_artifact_id)
+        assert blob_artifact_, "Blob artifact not found"
+        return blob_artifact_
 
     @experimental
     async def upsert_dataset_artifact(self, upsert: schemas.Upsert | Path, dataset_tag: str) -> fragments.BlobArtifact:
         """
         Apply an upsert to the latest dataset matching the given tag.
 
         All upsert datasets need to contain a file called `dataset.jsonl` in the root of the artifact.
@@ -402,15 +495,15 @@
         Otherwise, a new dataset will be created with the given tag that only contains the upsert data.
         """
         project_id = await self._get_current_project_id_or_raise()
         if isinstance(upsert, schemas.Upsert):
             with tempfile.TemporaryDirectory() as tmpdir:
                 upsert_filename = Path(tmpdir) / f"upsert-{uuid.uuid4().hex[:8]}.json"
                 with open(upsert_filename, "w") as f:
-                    json.dump(json.loads(upsert.json()), f)
+                    json.dump(json.loads(upsert.model_dump_json()), f)
                 console.print(f"Sending upsert to Slingshot...")
                 upsert_artifact = await self.upload_artifact(
                     upsert_filename, blob_artifact_tag="dataset_upsert", as_zip=False
                 )
         else:  # Path
             upsert_artifact = await self.upload_artifact(upsert, blob_artifact_tag="dataset_upsert", as_zip=False)
         if not upsert_artifact:
@@ -500,15 +593,15 @@
             example_bytes=example_bytes,
             timeout_seconds=timeout_seconds,
         )
         return get_data_or_raise(resp)
 
     @staticmethod
     def _maybe_raise_concrete_openai_error(error: schemas.SlingshotLogicalError) -> None:
-        if err_type := error.metadata.get("concrete_error_type"):
+        if error.metadata and (err_type := error.metadata.get("concrete_error_type")):
             openai_concrete_error_types = {
                 openai.error.ServiceUnavailableError,
                 openai.error.RateLimitError,
                 openai.error.AuthenticationError,
                 openai.error.APIConnectionError,
                 openai.error.APIError,
                 openai.error.APIConnectionError,
@@ -537,15 +630,15 @@
         *,
         force_redo: bool = False,
         timeout: datetime.timedelta = datetime.timedelta(seconds=600),
         active_throttling: bool | int = False,
     ) -> schemas.OpenAIChatResponse:
         """Make a prediction to a chat model on OpenAI."""
         project_id = await self._get_current_project_id_or_raise()
-        idempotence_key = md5_hash(openai_request.json().encode()) if not force_redo else uuid.uuid4().hex
+        idempotence_key = md5_hash(openai_request.model_dump_json().encode()) if not force_redo else uuid.uuid4().hex
 
         request = schemas.PromptOpenAIBody(
             openai_request=openai_request, idempotence_key=idempotence_key, active_throttling=active_throttling
         )
         resp = await self._api.prompt_openai(request, timeout=timeout, project_id=project_id)
         if resp.error:
             self._maybe_raise_concrete_openai_error(resp.error)
@@ -563,15 +656,15 @@
         *,
         force_redo: bool = False,
         timeout: datetime.timedelta = datetime.timedelta(seconds=600),
         active_throttling: bool | int = False,
     ) -> schemas.OpenAICompletionResponse:
         """Make a prediction to a text completion model on OpenAI."""
         project_id = await self._get_current_project_id_or_raise()
-        idempotence_key = md5_hash(openai_request.json().encode()) if not force_redo else uuid.uuid4().hex
+        idempotence_key = md5_hash(openai_request.model_dump_json().encode()) if not force_redo else uuid.uuid4().hex
         request = schemas.PromptOpenAIBody(
             openai_request=openai_request, idempotence_key=idempotence_key, active_throttling=active_throttling
         )
         result = await self._api.prompt_openai(request, timeout=timeout, project_id=project_id)
         if result.error:
             self._maybe_raise_concrete_openai_error(result.error)
             raise SlingshotException(result.error.message)
@@ -633,15 +726,15 @@
                     completion_tokens=None,
                     total_tokens=sum(result.usage.total_tokens for result in results),
                 ),
             )
 
         project_id = await self._get_current_project_id_or_raise()
         openai_request = schemas.OpenAIEmbeddingRequest(model=model, input=_input)
-        idempotence_key = md5_hash(openai_request.json().encode()) if not force_redo else uuid.uuid4().hex
+        idempotence_key = md5_hash(openai_request.model_dump_json().encode()) if not force_redo else uuid.uuid4().hex
         request = schemas.PromptOpenAIBody(
             openai_request=openai_request, idempotence_key=idempotence_key, active_throttling=active_throttling
         )
         result = await self._api.prompt_openai(request, timeout=timeout, project_id=project_id)
         if result.error:
             self._maybe_raise_concrete_openai_error(result.error)
             raise SlingshotException(result.error.message)
@@ -681,15 +774,15 @@
         self,
         run_template_name: str,
         source_code_id: str | None = None,
         machine_size: schemas.MachineSize | None = None,
         hyperparameters: Hyperparameter | None = None,
         cmd: str | None = None,
         mount_specs: list[fragments.MountSpec] | None = None,
-        exec_env_id: str | None = None,
+        environment_instance_id: str | None = None,
         debug_mode: bool = False,
     ) -> fragments.Run:
         """
         Start a run in the current project.
         """
         project_id = await self._get_current_project_id_or_raise()
         run_spec = await self._api.get_app_spec_by_name(app_spec_name=run_template_name, project_id=project_id)
@@ -705,15 +798,15 @@
         resp = await self._api.start_run(
             run_spec=run_spec,
             source_code_id=source_code_id,
             machine_size=machine_size,
             hyperparameters=hyperparameters,
             cmd=cmd,
             mount_specs=mount_specs,
-            exec_env_id=exec_env_id,
+            environment_instance_id=environment_instance_id,
             project_id=project_id,
             debug_mode=debug_mode,
         )
         data = get_data_or_raise(resp)
         run = await self._api.get_run(run_id=data.run_id, project_id=project_id)
         if not run:
             raise SlingshotException(f"Could not find run with id {data.run_id}")
@@ -867,16 +960,16 @@
     async def get_deployment_latencies(self, deployment_id: str) -> schemas.UsageBinsLatencyQuantiles:
         """Get a deployment's latencies by deployment id."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.get_deployment_latencies(deployment_id, project_id=project_id)
 
     async def get_environment(self, environment_id: str) -> fragments.ExecutionEnvironmentSpec | None:
         """Get an environment by id."""
-        project_id = await self._get_current_project_id_or_raise()
-        return await self._api.get_environment_spec(environment_id, project_id=project_id)
+        await self._get_current_project_id_or_raise()
+        return await self._api.get_environment_spec(environment_id)
 
     async def get_artifact(self, blob_artifact_name: str) -> fragments.BlobArtifact | None:
         """Get an artifact by name."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.get_blob_artifact_by_name(blob_artifact_name, project_id=project_id)
 
     """
@@ -962,24 +1055,24 @@
         )
 
     async def create_environment(
         self,
         name: str,
         requested_python_requirements: list[schemas.RequestedRequirement] | None = None,
         requested_apt_requirements: list[schemas.RequestedAptPackage] | None = None,
-        gpu_drivers: bool = False,
+        post_install_command: str | None = None,
         force_create_environment: bool = False,
     ) -> schemas.CreateEnvironmentSpecResponse:
         """Create a new environment with the given name and requirements."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.create_or_update_environment_spec(
             name=name,
             requested_python_requirements=requested_python_requirements,
             requested_apt_requirements=requested_apt_requirements,
-            gpu_drivers=gpu_drivers,
+            post_install_command=post_install_command or "",
             force_create_environment=force_create_environment,
             project_id=project_id,
         )
 
     async def create_volume(self, volume_name: str) -> None:
         """
         Create a volume in the current project.
@@ -1007,22 +1100,19 @@
         machine_size: schemas.MachineSize,
         mounts: list[schemas.MountSpecUnion],
         attach_project_credentials: bool,
         config_variables: JSONType | None = None,
         app_port: int | None = None,
         batch_size: int | None = None,
         batch_interval: int | None = None,
-        *,
-        name: str | None = None,
-    ) -> schemas.Response[bool]:
+    ) -> schemas.BoolResponse:
         """Updates app with the given id and configuration."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.update_app(
             app_spec_id=app_spec_id,
-            name=name,
             command=command,
             exec_env_spec_id=env_spec_id,
             machine_size=machine_size,
             mounts=mounts,
             attach_project_credentials=attach_project_credentials,
             config_variables=config_variables,
             app_port=app_port,
@@ -1032,24 +1122,24 @@
         )
 
     async def update_environment(
         self,
         name: str,
         requested_python_requirements: list[schemas.RequestedRequirement] | None = None,
         requested_apt_requirements: list[schemas.RequestedAptPackage] | None = None,
-        gpu_drivers: bool = False,
+        post_install_command: str | None = None,
         force_create_environment: bool = False,
     ) -> schemas.CreateEnvironmentSpecResponse:
         """Updates environment with the given name and configuration."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.create_or_update_environment_spec(
             name=name,
             requested_python_requirements=requested_python_requirements,
             requested_apt_requirements=requested_apt_requirements,
-            gpu_drivers=gpu_drivers,
+            post_install_command=post_install_command or "",
             force_create_environment=force_create_environment,
             project_id=project_id,
         )
 
     """
     Delete SDK methods
     """
@@ -1057,16 +1147,16 @@
     async def delete_app(self, app_spec_id: str) -> schemas.ResponseOK:
         """Delete an app with the given id."""
         project_id = await self._get_current_project_id_or_raise()
         return await self._api.delete_app(app_spec_id=app_spec_id, project_id=project_id)
 
     async def delete_environment(self, environment_id: str) -> None:
         """Delete an environment with the given id."""
-        project_id = await self._get_current_project_id_or_raise()
-        await self._api.delete_environment_spec(execution_environment_spec_id=environment_id, project_id=project_id)
+        await self._get_current_project_id_or_raise()
+        await self._api.delete_environment_spec(execution_environment_spec_id=environment_id)
 
     async def delete_volume(self, volume_name: str) -> None:
         """
         Delete a volume in the current project.
         """
         project_id = await self._get_current_project_id_or_raise()
         resp = await self._api.delete_volume(volume_name=volume_name, project_id=project_id)
@@ -1087,17 +1177,17 @@
         if self.project:
             return self.project
         await self.setup()
         if self.project:
             return self.project
 
         if not await self.is_signed_in():
-            raise SlingshotException("Not signed in. Please sign in with `slingshot login`.")
+            raise SlingshotUnauthenticatedError()
 
-        raise SlingshotException("No project set. Please set a project with `slingshot use`.")
+        raise SlingshotNoProjectSetError()
 
     async def _get_current_project_id_or_raise(self) -> str:
         project = await self._get_current_project_or_raise()
         return project.project_id
 
     def _get_apply_service(self) -> ApplyService:
         return ApplyService(self)
@@ -1140,44 +1230,14 @@
                     raise SlingshotException(f"Run status is error : {current_status}")
 
         try:
             await wait_for(_wait_for_status(), max_wait)
         except asyncio.TimeoutError:
             raise SlingshotException(f"Run status timed out waiting for {status} after {max_wait} seconds")
 
-    async def _wait_for_env_compile(
-        self: SlingshotSDK,
-        env: schemas.HasExecutionEnvironmentId,
-        *,
-        max_wait: float | None = None,
-        poll_interval: int = 3,
-        should_print: bool = False,
-    ) -> schemas.ExecEnvStatus:
-        """
-        Wait for an environment to not be in the COMPILING status.
-        If it doesn't reach the status within max_wait seconds, raises a SlingshotException.
-        Returns the final status.
-        """
-
-        async def _wait_for_status() -> schemas.ExecEnvStatus:
-            while True:
-                env_response = await self._api.get_exec_env(env.execution_environment_id)
-                if not env_response:
-                    raise SlingshotException(f"Could not find environment {env.execution_environment_id}")
-                if env_response.status != schemas.ExecEnvStatus.COMPILING:
-                    return env_response.status
-                if should_print:
-                    console.print(".", end="")
-                await asyncio.sleep(poll_interval)
-
-        try:
-            return await wait_for(_wait_for_status(), max_wait)
-        except asyncio.TimeoutError:
-            raise SlingshotException(f"Environment still compiling after {max_wait} seconds")
-
     async def _wait_for_app_status(
         self: SlingshotSDK,
         app: schemas.HasAppSpecId,
         status: schemas.AppInstanceStatus,
         *,
         max_wait: float | None = None,
     ) -> None:
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,41 +112,42 @@
                             style="yellow",
                         )
                     continue
                 zf.write(file_path)
 
 
 async def sync_code(
-    sdk: SlingshotSDK, path: Path, description: Optional[str]
+    sdk: SlingshotSDK, path: Path, description: Optional[str], quiet: bool = False
 ) -> tuple[schemas.UploadedSourceCode, bool]:
     logger.debug(f"Zipping up {path}...")
     zip_bytes = zip_code_artifact(path)
 
     # Check if the code is already uploaded
     local_code_hash = md5_hash(zip_bytes)
     project_id = await sdk._get_current_project_id_or_raise()
     latest_source_code = await sdk.api.get_latest_source_codes_for_project(project_id)
     if latest_source_code is not None and latest_source_code.blob_artifact.bytes_hash == local_code_hash:
         console.print(f"Code hasn't changed. Skipping upload.")
         return (
             schemas.UploadedSourceCode(
-                source_code_id=latest_source_code.source_code_id, source_code_name=latest_source_code.source_code_name
+                source_code_id=latest_source_code.source_code_id, source_code_name=latest_source_code.blob_artifact.name
             ),
             False,
         )
 
     num_bytes = len(zip_bytes)
     console.print(f"Pushing code to Slingshot ({bytes_to_str(num_bytes)})...")
     # Save zip_bytes to a temporary file
     with TemporaryDirectory() as tmpdir:
         artifact_path = Path(tmpdir) / "code.zip"
         with open(artifact_path, "wb") as f:
             f.write(zip_bytes)
-        artifact = await sdk.upload_artifact(artifact_path=artifact_path, blob_artifact_tag="code", as_zip=True)
-        artifact_path.unlink()  # Remove the temporary file
+        artifact = await sdk.upload_artifact(
+            artifact_path=artifact_path, blob_artifact_tag="code", as_zip=True, quiet=quiet
+        )
     if not artifact:
         raise SlingshotException("Failed to upload code to Slingshot")
     resp = await sdk.api.upload_source_code(artifact.blob_artifact_id, description, project_id=project_id)
     uploaded_source_code_resp = get_data_or_raise(resp)
     return uploaded_source_code_resp, True
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/upload_download_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 logger = getLogger(__name__)
 
 UPLOAD_TIMEOUT_MIN = 120
 MAX_RETRIES = 3
 CHUNK_SIZE_BYTES = 1024 * 1024  # 1 MB
 
 
-async def upload_file_in_parts_to_gcs(artifact_path: str, upload_signed_url: str, *, client: SlingshotClient) -> None:
+async def upload_file_in_parts_to_gcs(
+    artifact_path: str, upload_signed_url: str, *, client: SlingshotClient, quiet: bool = False
+) -> None:
     logger.debug(f"Uploading {artifact_path} to {upload_signed_url}")
     with open(artifact_path, 'rb') as file:
         # Get the size of the file to be uploaded and create a progress bar for it
         file_size = os.path.getsize(artifact_path)
-        with tqdm(total=file_size, unit='B', unit_scale=True, desc="Uploading") as pbar:
+        with tqdm(total=file_size, unit='B', unit_scale=True, desc="Uploading", disable=quiet) as pbar:
             position = 0  # Current position in the file
             while position < file_size:
                 chunk = file.read(CHUNK_SIZE_BYTES)
                 retries = 0
                 while retries < MAX_RETRIES:
                     try:
                         # Upload the chunk with a PUT request to the session URI
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from __future__ import annotations
 
 import base64
 import contextlib
 import copy
 import hashlib
+import json
 import os
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Any, Iterator
+from typing import Any, Iterator, Type, TypeVar
 
-from pydantic.tools import parse_obj_as
+from pydantic import TypeAdapter
+from pydantic.main import BaseModel
 from rich.console import Console
 from ruamel import yaml as r_yaml
 from ruamel.yaml.representer import RepresenterError
 
 from slingshot import schemas
 from slingshot.sdk.config import client_settings
 from slingshot.sdk.errors import SlingshotException
 from slingshot.sdk.graphql.fragments import MountSpec
 
 console = Console()
 yaml = r_yaml.YAML()
 
+T = TypeVar("T", bound=BaseModel)
+
 
 def time_since_string(then: datetime) -> str:
     """Compute the time since a given datetime as a pretty string"""
     now = datetime.utcnow()
     diff = now - then
     if diff.total_seconds() < 0:
         # Lol this should never happen, but it was helpful for debugging! We should remove in prod.
@@ -56,17 +60,16 @@
     m.update(input_bytes)
     hash_digest = m.digest()
     return base64.b64encode(hash_digest).decode("utf-8")
 
 
 def gql_mount_spec_to_read_mount_spec(mount_spec: MountSpec) -> schemas.MountSpecUnion:
     """Converts the MountSpec schema received from GQL type to the ReadMountSpec type."""
-    return parse_obj_as(
-        schemas.MountSpecUnion,
-        {"path": mount_spec.path, "mode": mount_spec.mode, "tag": mount_spec.tag, "name": mount_spec.name},
+    return TypeAdapter(schemas.MountSpecUnion).validate_python(
+        {"path": mount_spec.path, "mode": mount_spec.mode, "tag": mount_spec.tag, "name": mount_spec.name}
     )
 
 
 @contextlib.contextmanager
 def edit_slingshot_yaml(raise_if_absent: bool = True, filename: str | None = None) -> Iterator[dict[str, Any]]:
     file = (Path(os.getcwd()) / filename) if filename else client_settings.slingshot_config_path
 
@@ -116,7 +119,15 @@
     elif isinstance(value, list):
         value = [recursive_enum_to_str(x) for x in value]
     elif isinstance(value, Enum):
         value = value.value
     else:
         value = value
     return value
+
+
+def get_config(config_class: Type[T] | None = None) -> dict[str, Any] | T:
+    """Get the config from the environment, or return the default config if none is set"""
+    config_dict = json.loads(os.environ.get("CONFIG", "{}"))
+    if config_class is None:
+        return config_dict
+    return config_class.model_validate(config_dict)
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/web_path_util.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/shared/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import typing
+from pathlib import Path
 from typing import Any
 
 from pydantic import BaseModel, ValidationError
 from ruamel import yaml as r_yaml
 
 from slingshot import schemas
 from slingshot.sdk.config import client_settings
@@ -14,44 +15,47 @@
 yaml = r_yaml.YAML()
 
 
 class SlingshotFileNotFoundException(SlingshotException):
     pass
 
 
-def load_slingshot_project_config() -> schemas.ProjectManifest:
+def load_slingshot_project_config(config_path: Path = client_settings.slingshot_config_path) -> schemas.ProjectManifest:
+    """
+    Loads the slingshot.yaml file from the given path and parses it into a ProjectManifest object.
+
+    :param config_path: The path to the slingshot.yaml file. This should only be used for testing.
+    :return ProjectManifest:
+    """
     try:
-        text = client_settings.slingshot_config_path.read_text()
+        text = config_path.read_text()
     except FileNotFoundError as e:
         raise SlingshotFileNotFoundException(
-            f"Could not find slingshot.yaml at {client_settings.slingshot_config_path}.\n"
-            f"You can add one by running 'slingshot init'"
+            f"Could not find slingshot.yaml at {config_path}.\n" f"You can add one by running 'slingshot init'"
         ) from e
     try:
         d = r_yaml.safe_load(text)
     except r_yaml.YAMLError as e:
-        raise SlingshotException(f"Could not parse slingshot.yaml in {client_settings.slingshot_config_path}") from e
+        raise SlingshotException(f"Could not parse slingshot.yaml in {config_path}") from e
     if not d:
-        raise SlingshotException(
-            f"Empty slingshot.yaml in {client_settings.slingshot_config_path}. Please run 'slingshot init'"
-        )
+        raise SlingshotException(f"Empty slingshot.yaml in {config_path}. Please run 'slingshot init'")
     try:
-        return schemas.ProjectManifest.parse_obj(d)
+        return schemas.ProjectManifest.model_validate(d)
     except Exception as e:
         raise _beautify_project_manifest_parsing_exception(d, e) from e
 
 
 # noinspection PyBroadException
 def _beautify_project_manifest_parsing_exception(d: dict[typing.Any, typing.Any], e: Exception) -> SlingshotException:
     if (isinstance(e, ValidationError) or isinstance(e, KeyError)) and "environments" in str(e):
         for env in d["environments"].values():
             try:
                 # Try to parse each environment individually to get a more helpful error message,
                 #  if it's one of them that's failing.
-                schemas.EnvironmentSpec.parse_obj(env)
+                schemas.EnvironmentSpec.model_validate(env)
             except ValidationError as e2:
                 model = e2.model.__name__
                 errs = e2.errors()
                 if len(errs) > 0:
                     message = None
                     try:
                         given = errs[0]["ctx"]["given"]
@@ -66,39 +70,39 @@
                     if message:
                         return SlingshotException(message)
 
     if (isinstance(e, ValidationError) or isinstance(e, KeyError)) and "mounts" in str(e):
         for app in d.get("apps", []):
             for mount in app.get("mounts", []):
                 try:
-                    schemas.BaseMountSpec.parse_obj(mount)
+                    schemas.BaseMountSpec.model_validate(mount)
                 except ValidationError as e2:
                     try:
                         message = f"Mount for {app['name']} with {mount['path']} was invalid -- {e2.errors()[0]['msg']}"
                         return SlingshotException(message)
                     except Exception:
                         pass
                 except Exception:
                     pass
         for run in d.get("runs", []):
             for mount in run.get("mounts", []):
                 try:
-                    schemas.BaseMountSpec.parse_obj(mount)
+                    schemas.BaseMountSpec.model_validate(mount)
                 except ValidationError as e2:
                     try:
                         message = f"Mount for {run['name']} with {mount['path']} was invalid -- {e2.errors()[0]['msg']}"
                         return SlingshotException(message)
                     except Exception:
                         pass
                 except Exception:
                     pass
         for deployment in d.get("deployments", []):
             for mount in deployment.get("mounts", []):
                 try:
-                    schemas.BaseMountSpec.parse_obj(mount)
+                    schemas.BaseMountSpec.model_validate(mount)
                 except ValidationError as e2:
                     try:
                         message = (
                             f"Mount for {deployment['name']} with {mount['path']} was invalid -- "
                             f"{e2.errors()[0]['msg']}"
                         )
                         return SlingshotException(message)
@@ -109,15 +113,15 @@
 
     if isinstance(e, SlingshotException):
         return e
 
     return SlingshotException(f"Invalid slingshot.yaml: {e=}")
 
 
-T = typing.TypeVar("T")
+T = typing.TypeVar("T", bound=BaseModel)
 
 
 class ResponseProtocol(typing.Protocol[T]):
     data: typing.Optional[T]
     error: typing.Optional[schemas.SlingshotLogicalError]
 
 
@@ -147,16 +151,33 @@
 
 def machine_size_to_machine_type_gpu_count(machine_size: schemas.MachineSize) -> tuple[schemas.MachineType, int]:
     if machine_size not in _machine_size_to_machine_type_gpu_count:
         raise ValueError(f"Unknown machine size {machine_size}")
     return _machine_size_to_machine_type_gpu_count[machine_size]
 
 
-def machine_type_gpu_count_to_machine_size(machine_type: schemas.MachineType, gpu_count: int) -> schemas.MachineSize:
+def machine_type_gpu_count_to_machine_size(
+    machine_type: schemas.MachineType, gpu_count: int | None
+) -> schemas.MachineSize:
+    if gpu_count is None:
+        gpu_count = 0
     if (machine_type, gpu_count) not in _machine_type_gpu_count_to_machine_size:
         raise ValueError(f"Unknown machine type {machine_type} with {gpu_count} GPUs")
     return _machine_type_gpu_count_to_machine_size[(machine_type, gpu_count)]
 
 
+def get_default_num_gpu(machine_type: schemas.MachineType) -> int:
+    cpu_machine_types = {
+        schemas.MachineType.CPU_TINY,
+        schemas.MachineType.CPU_SMALL,
+        schemas.MachineType.CPU_MEDIUM,
+        schemas.MachineType.CPU_LARGE,
+    }
+    # CPU machines have no GPUs
+    if machine_type in cpu_machine_types:
+        return 0
+    return 1
+
+
 def pydantic_to_dict(pydantic: BaseModel, *, exclude_unset: bool = True) -> dict[str, Any]:
     # Convert enums to strings
-    return json.loads(pydantic.json(exclude_none=True, exclude_unset=exclude_unset))
+    return json.loads(pydantic.model_dump_json(exclude_none=True, exclude_unset=exclude_unset))
```

### Comparing `slingshot_ai-0.0.17/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.18rc1/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.17/PKG-INFO` & `slingshot_ai-0.0.18rc1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.17
+Version: 0.0.18rc1
 Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp (>=3.8.1,<3.9.0)
-Requires-Dist: backoff (>=2.0.0,<2.1.0)
-Requires-Dist: deepdiff (>=6.3.0,<6.4.0)
-Requires-Dist: fastapi (>=0.88.0,<0.89.0)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (<=1.10.11)
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28.1,<2.29.0)
-Requires-Dist: ruamel.yaml (>=0.17.0,<0.18.0)
-Requires-Dist: sentry-sdk (>=1.16.0,<1.17.0)
-Requires-Dist: sh (>=1.14.3,<1.15.0)
-Requires-Dist: simple-term-menu (>=1.6.0,<1.7.0)
-Requires-Dist: tqdm (>=4.63.0,<4.64.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Requires-Dist: urllib3 (>=1.26.11,<1.27.0)
-Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
+Requires-Dist: aiohttp (>=3.8.1)
+Requires-Dist: backoff (>=2.0.0)
+Requires-Dist: deepdiff (>=6.3.0)
+Requires-Dist: openai (>=0.27.8)
+Requires-Dist: pydantic (>=2.0.0,<3)
+Requires-Dist: pydantic-settings (>=2.0.0,<3)
+Requires-Dist: pyyaml (>=6.0)
+Requires-Dist: requests (>=2.28.1)
+Requires-Dist: ruamel.yaml (>=0.17.0)
+Requires-Dist: sentry-sdk (>=1.16.0)
+Requires-Dist: sh (>=1.14.3)
+Requires-Dist: simple-term-menu (>=1.6.0)
+Requires-Dist: tqdm (>=4.63.0)
+Requires-Dist: typer[all] (>=0.7.0)
+Requires-Dist: urllib3 (>=1.26.11)
```

