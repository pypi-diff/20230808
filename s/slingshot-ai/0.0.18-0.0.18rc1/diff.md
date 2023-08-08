# Comparing `tmp/slingshot_ai-0.0.18.tar.gz` & `tmp/slingshot_ai-0.0.18rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slingshot_ai-0.0.18.tar", max compression
+gzip compressed data, was "slingshot_ai-0.0.18rc1.tar", max compression
```

## Comparing `slingshot_ai-0.0.18.tar` & `slingshot_ai-0.0.18rc1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0      809 2023-08-08 18:52:34.695559 slingshot_ai-0.0.18/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-14 01:36:51.753575 slingshot_ai-0.0.18/src/slingshot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.733834 slingshot_ai-0.0.18/src/slingshot/cli/__init__.py
--rw-r--r--   0        0        0    17826 2023-08-01 14:47:02.806869 slingshot_ai-0.0.18/src/slingshot/cli/add.py
--rw-r--r--   0        0        0     1328 2023-08-08 14:59:18.891294 slingshot_ai-0.0.18/src/slingshot/cli/apply.py
--rw-r--r--   0        0        0     5931 2023-07-28 21:27:30.614734 slingshot_ai-0.0.18/src/slingshot/cli/apps.py
--rw-r--r--   0        0        0     8225 2023-08-02 14:52:04.657063 slingshot_ai-0.0.18/src/slingshot/cli/artifact.py
--rw-r--r--   0        0        0     5388 2023-07-21 18:05:09.101272 slingshot_ai-0.0.18/src/slingshot/cli/auth.py
--rw-r--r--   0        0        0      970 2023-06-08 13:51:24.734880 slingshot_ai-0.0.18/src/slingshot/cli/code.py
--rw-r--r--   0        0        0        0 2023-06-12 16:23:44.406584 slingshot_ai-0.0.18/src/slingshot/cli/config/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.734966 slingshot_ai-0.0.18/src/slingshot/cli/config/py.typed
--rw-r--r--   0        0        0      850 2023-06-14 16:35:36.287763 slingshot_ai-0.0.18/src/slingshot/cli/config/sentry_setup.py
--rw-r--r--   0        0        0    13774 2023-06-27 15:26:50.739279 slingshot_ai-0.0.18/src/slingshot/cli/config/slingshot_cli.py
--rw-r--r--   0        0        0      899 2023-08-08 14:59:18.892346 slingshot_ai-0.0.18/src/slingshot/cli/dev.py
--rw-r--r--   0        0        0     1422 2023-07-28 21:27:30.615238 slingshot_ai-0.0.18/src/slingshot/cli/environment.py
--rw-r--r--   0        0        0     4778 2023-07-28 21:27:30.615824 slingshot_ai-0.0.18/src/slingshot/cli/inference.py
--rw-r--r--   0        0        0     3059 2023-06-08 13:51:24.735634 slingshot_ai-0.0.18/src/slingshot/cli/logs.py
--rw-r--r--   0        0        0     1951 2023-07-03 17:32:15.325020 slingshot_ai-0.0.18/src/slingshot/cli/machine.py
--rw-r--r--   0        0        0     2731 2023-08-08 14:59:18.893351 slingshot_ai-0.0.18/src/slingshot/cli/main.py
--rw-r--r--   0        0        0     3087 2023-08-08 18:30:38.222638 slingshot_ai-0.0.18/src/slingshot/cli/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.735998 slingshot_ai-0.0.18/src/slingshot/cli/py.typed
--rw-r--r--   0        0        0     8170 2023-07-28 21:27:30.616461 slingshot_ai-0.0.18/src/slingshot/cli/run.py
--rw-r--r--   0        0        0     3648 2023-06-08 14:01:51.180092 slingshot_ai-0.0.18/src/slingshot/cli/secret.py
--rw-r--r--   0        0        0     3846 2023-07-21 18:05:09.101837 slingshot_ai-0.0.18/src/slingshot/cli/session.py
--rw-r--r--   0        0        0       67 2023-06-08 13:51:24.737453 slingshot_ai-0.0.18/src/slingshot/cli/shared/__init__.py
--rw-r--r--   0        0        0     6582 2023-07-21 18:05:09.102433 slingshot_ai-0.0.18/src/slingshot/cli/shared/code_sync.py
--rw-r--r--   0        0        0     7036 2023-07-12 21:00:50.134070 slingshot_ai-0.0.18/src/slingshot/cli/shared/prompt.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738086 slingshot_ai-0.0.18/src/slingshot/cli/shared/py.typed
--rw-r--r--   0        0        0      200 2023-08-08 14:59:18.893874 slingshot_ai-0.0.18/src/slingshot/cli/shared/settings.py
--rw-r--r--   0        0        0     7527 2023-08-01 14:47:02.809069 slingshot_ai-0.0.18/src/slingshot/cli/shared/utils.py
--rw-r--r--   0        0        0     1388 2023-06-08 13:51:24.738677 slingshot_ai-0.0.18/src/slingshot/cli/volume.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.738829 slingshot_ai-0.0.18/src/slingshot/code/__init__.py
--rw-r--r--   0        0        0        1 2023-06-08 13:51:24.739138 slingshot_ai-0.0.18/src/slingshot/code/annotation.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.739256 slingshot_ai-0.0.18/src/slingshot/code/py.typed
--rw-r--r--   0        0        0       56 2023-06-14 01:36:51.755302 slingshot_ai-0.0.18/src/slingshot/inference_model/__init__.py
--rw-r--r--   0        0        0     3941 2023-06-14 14:56:40.736423 slingshot_ai-0.0.18/src/slingshot/inference_model/inference_model.py
--rw-r--r--   0        0        0      205 2023-06-08 13:51:24.739905 slingshot_ai-0.0.18/src/slingshot/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740119 slingshot_ai-0.0.18/src/slingshot/schemas/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740282 slingshot_ai-0.0.18/src/slingshot/schemas/generated/py.typed
--rw-r--r--   0        0        0    26165 2023-08-08 18:53:03.000000 slingshot_ai-0.0.18/src/slingshot/schemas/generated/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.740843 slingshot_ai-0.0.18/src/slingshot/schemas/py.typed
--rw-r--r--   0        0        0    10081 2023-08-08 14:59:18.895096 slingshot_ai-0.0.18/src/slingshot/schemas/schema_extensions.py
--rw-r--r--   0        0        0    17610 2023-08-08 16:31:24.438357 slingshot_ai-0.0.18/src/slingshot/schemas/slingshot-schema.config.json
--rw-r--r--   0        0        0    22973 2023-08-08 18:30:38.223631 slingshot_ai-0.0.18/src/slingshot/schemas/slingshot_schema.py
--rw-r--r--   0        0        0      155 2023-07-28 16:35:47.947662 slingshot_ai-0.0.18/src/slingshot/sdk/__init__.py
--rw-r--r--   0        0        0    33808 2023-08-08 18:30:38.224911 slingshot_ai-0.0.18/src/slingshot/sdk/apply.py
--rw-r--r--   0        0        0     4193 2023-08-08 14:59:18.897723 slingshot_ai-0.0.18/src/slingshot/sdk/apply_diff.py
--rw-r--r--   0        0        0     2217 2023-06-08 13:51:24.742861 slingshot_ai-0.0.18/src/slingshot/sdk/auth.py
--rw-r--r--   0        0        0     3070 2023-08-08 14:59:18.898395 slingshot_ai-0.0.18/src/slingshot/sdk/config.py
--rw-r--r--   0        0        0     3052 2023-08-08 18:30:38.225822 slingshot_ai-0.0.18/src/slingshot/sdk/config_utils.py
--rw-r--r--   0        0        0     2372 2023-07-06 15:25:20.145323 slingshot_ai-0.0.18/src/slingshot/sdk/data_collector.py
--rw-r--r--   0        0        0     6805 2023-08-08 14:59:18.899695 slingshot_ai-0.0.18/src/slingshot/sdk/errors.py
--rw-r--r--   0        0        0      126 2023-06-08 13:51:24.743741 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/__init__.py
--rw-r--r--   0        0        0     3100 2023-08-08 14:59:18.899991 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/base_graphql.py
--rw-r--r--   0        0        0    19980 2023-08-08 14:59:18.900787 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/fragments.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.744284 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/py.typed
--rw-r--r--   0        0        0      138 2023-06-08 13:51:24.744487 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/__init__.py
--rw-r--r--   0        0        0     5265 2023-07-06 15:15:48.339951 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/apps.py
--rw-r--r--   0        0        0      986 2023-06-08 13:51:24.744887 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/deployment.py
--rw-r--r--   0        0        0     3674 2023-08-08 14:59:18.901522 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/environment.py
--rw-r--r--   0        0        0     5272 2023-08-08 14:59:18.901882 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/project.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745499 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/py.typed
--rw-r--r--   0        0        0     2418 2023-08-08 14:59:18.902150 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/run.py
--rw-r--r--   0        0        0     4362 2023-08-08 14:59:18.902390 slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/storage.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.745963 slingshot_ai-0.0.18/src/slingshot/sdk/py.typed
--rw-r--r--   0        0        0    51025 2023-08-08 18:30:38.226689 slingshot_ai-0.0.18/src/slingshot/sdk/slingshot_api.py
--rw-r--r--   0        0        0    54502 2023-08-08 14:59:18.903690 slingshot_ai-0.0.18/src/slingshot/sdk/slingshot_sdk.py
--rw-r--r--   0        0        0     7008 2023-08-01 14:47:02.813054 slingshot_ai-0.0.18/src/slingshot/sdk/sync.py
--rw-r--r--   0        0        0     2904 2023-08-01 14:47:02.814359 slingshot_ai-0.0.18/src/slingshot/sdk/upload_download_utils.py
--rw-r--r--   0        0        0     4583 2023-08-08 14:59:18.904148 slingshot_ai-0.0.18/src/slingshot/sdk/utils.py
--rw-r--r--   0        0        0     4361 2023-07-05 13:59:49.269504 slingshot_ai-0.0.18/src/slingshot/sdk/web_path_util.py
--rw-r--r--   0        0        0     6786 2023-08-08 18:30:38.227474 slingshot_ai-0.0.18/src/slingshot/sdk/wrapped_diff.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747738 slingshot_ai-0.0.18/src/slingshot/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.747833 slingshot_ai-0.0.18/src/slingshot/shared/py.typed
--rw-r--r--   0        0        0     7416 2023-08-08 16:23:35.204415 slingshot_ai-0.0.18/src/slingshot/shared/utils.py
--rw-r--r--   0        0        0       23 2023-08-08 18:53:06.769448 slingshot_ai-0.0.18/src/slingshot/slingshot_version.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748427 slingshot_ai-0.0.18/src/slingshot/templates/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-28 22:37:34.391674 slingshot_ai-0.0.18/src/slingshot/templates/inference_template.py
--rw-r--r--   0        0        0     3582 2023-08-08 14:59:18.906095 slingshot_ai-0.0.18/src/slingshot/templates/label_studio_data_export_template.py
--rw-r--r--   0        0        0        0 2023-06-08 13:51:24.748968 slingshot_ai-0.0.18/src/slingshot/templates/py.typed
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 slingshot_ai-0.0.18/PKG-INFO
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

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/add.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/add.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/apply.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/apply.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/apps.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/artifact.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/artifact.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/auth.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/code.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/code.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/config/sentry_setup.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/config/sentry_setup.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/config/slingshot_cli.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/config/slingshot_cli.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/dev.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/dev.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/environment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/inference.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/inference.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/logs.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/logs.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/machine.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/machine.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/main.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/main.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/project.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 async def _set_project_id(sdk_: SlingshotSDK, project_id: str) -> None:
     old_project_id = project_config.project_id
     project_config.project_id = project_id
     if old_project_id != project_id:
         project_config.last_pushed_manifest = None
 
-    directory = project_config.model_config.get('config_file').parent.parent
+    directory = project_config.JSONConfig.settings_json_file.parent.parent
 
     console.print(f"This directory ({directory}) is now associated with the project: [bold]{project_id}[/bold]")
     await sdk_.use_project(project_id)
 
     try:
         load_slingshot_project_config()
     except SlingshotFileNotFoundException:
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/run.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/secret.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/secret.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/session.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/session.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/shared/code_sync.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/code_sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/shared/prompt.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/prompt.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/shared/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/cli/volume.py` & `slingshot_ai-0.0.18rc1/src/slingshot/cli/volume.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/inference_model/inference_model.py` & `slingshot_ai-0.0.18rc1/src/slingshot/inference_model/inference_model.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/schemas/generated/schemas.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/generated/schemas.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/schemas/schema_extensions.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/schema_extensions.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/schemas/slingshot-schema.config.json` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot-schema.config.json`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/schemas/slingshot_schema.py` & `slingshot_ai-0.0.18rc1/src/slingshot/schemas/slingshot_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,14 @@
     apps: list[Union[SlingshotCustomAppSpec, SessionAppSpec, RedisAppSpec]] = Field(
         default_factory=list, title=SlingshotAbstractAppSpec.model_config["title"]
     )
     runs: list[RunSpec] = Field(default_factory=list, title=RunSpec.model_config["title"])
     deployments: list[DeploymentSpec] = Field(default_factory=list, title=DeploymentSpec.model_config["title"])
     model_config = ConfigDict(
         title="Slingshot Config Spec",
-        from_attributes=True,
         json_schema_extra={"$schema": "http://json-schema.org/draft/2020-12/schema", "$id": FILE_LOCATION},
     )
 
     @staticmethod
     def check_deprecations(v: dict[str, Any]) -> list[SlingshotValidationResult]:
         deprecations = []
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/apply.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/apply.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,19 +569,17 @@
     existing_env_specs = await sdk.list_environments()
     env_specs_by_name = {}
     for env_spec in existing_env_specs:
         assert env_spec.environment_instances, "Environment spec has no instances"
         env_instance = env_spec.environment_instances[0]
         parsed_env_spec = schemas.EnvironmentSpec(
             python_packages=[
-                str(schemas.RequestedRequirement.model_validate(i)) for i in env_instance.requested_python_requirements
-            ],
-            apt_packages=[
-                schemas.RequestedAptPackage.model_validate(i).name for i in env_instance.requested_apt_packages
+                schemas.RequestedRequirement.parse_obj(i).as_str() for i in env_instance.requested_python_requirements
             ],
+            apt_packages=[schemas.RequestedAptPackage.parse_obj(i).name for i in env_instance.requested_apt_packages],
             post_install_command=env_instance.post_install_command,
         )
         env_specs_by_name[env_spec.execution_environment_spec_name] = parsed_env_spec
 
     app_specs: list[schemas.SlingshotAbstractAppSpec] = []
     existing_app_specs = await sdk.list_apps()
     for spec in existing_app_specs:
@@ -707,13 +705,13 @@
 def _load_last_pushed_manifest() -> tuple[schemas.ProjectManifest, bool]:
     """Load the last pushed manifest, and return if the last pushed manifest is empty."""
     last_pushed_manifest_dict = config.project_config.last_pushed_manifest
     is_last_pushed_manifest_empty = last_pushed_manifest_dict is None
 
     # First make sure this is a valid project manifest
     if last_pushed_manifest_dict:
-        last_pushed_manifest = ProjectManifest.model_validate(last_pushed_manifest_dict)
+        last_pushed_manifest = ProjectManifest.parse_obj(last_pushed_manifest_dict)
     else:
         # If there is no last pushed manifest, we use an empty manifest as the base of the diff to ensure that
         #  all remote changes are computed in the plan and can be applied correctly.
         last_pushed_manifest = ProjectManifest()
     return last_pushed_manifest, is_last_pushed_manifest_empty
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/apply_diff.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/apply_diff.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/auth.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/config.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/config.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/config_utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/config_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,9 +69,8 @@
         super().__setattr__(key, value)
         self._save()
 
     def _save(self) -> None:
         settings_json_file = self.model_config.get('config_file')
         os.makedirs(settings_json_file.parent, exist_ok=True)
         with open(settings_json_file, "w") as f:
-            model_dict = self.model_dump(warnings=False)  # Ignore warnings about dict vs ProjectManifest
-            json.dump(model_dict, f, indent=4)
+            json.dump(self.model_dump(), f, indent=4)
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/data_collector.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/errors.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/base_graphql.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/base_graphql.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/fragments.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/fragments.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/apps.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/apps.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/deployment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/deployment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/environment.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/environment.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/project.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/project.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/run.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/run.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/graphql/queries/storage.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/graphql/queries/storage.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/slingshot_api.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
                         if msg.type == aiohttp.WSMsgType.TEXT:
                             data = json.loads(msg.data)
                             if data["type"] == "connection_error":
                                 raise SlingshotException(f"WebSocket connection error: {data['payload']}")
                             elif "errors" in data:
                                 raise SlingshotException(f"GraphQL error: {data['errors']}")
                             elif data["type"] == "data":
-                                yield type_.model_validate(data).payload
+                                yield TypeAdapter(type_).validate_python(data).payload
                             else:
                                 logger.debug(f"Received unexpected message: {data}")
                         elif msg.type == aiohttp.WSMsgType.ERROR:
                             raise SlingshotException(f"WebSocket error: {msg.data}")
 
             logger.info("Websocket connection closed -- retrying")
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/slingshot_sdk.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/slingshot_sdk.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/sync.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/sync.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/upload_download_utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/upload_download_utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/web_path_util.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/web_path_util.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/sdk/wrapped_diff.py` & `slingshot_ai-0.0.18rc1/src/slingshot/sdk/wrapped_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,44 +78,39 @@
 
 class PathNodeKey(BaseModel):
     key: str
 
     def __str__(self) -> str:
         return self.key
 
-    @property
-    def access_key(self) -> str:
-        return self.key
-
 
 class PathNodeIndex(BaseModel):
     index: int
     name: str
 
     def __str__(self) -> str:
         return self.name
 
-    @property
-    def access_key(self) -> str | int:
-        return self.index
-
 
 PathNode = PathNodeKey | PathNodeIndex
 
 
 class DiffItem(abc.ABC):
     def __init__(self, value: Any, path: list[PathNode]):
         self.value = value
         self.path = path
 
     @property
     def identifier(self) -> str:
         id_parts = []
         for path_part in self.path:
-            id_parts.append(str(path_part))
+            if isinstance(path_part, PathNodeKey):
+                id_parts.append(path_part.key)
+            elif isinstance(path_part, PathNodeIndex):
+                id_parts.append(path_part.name)
         return ".".join(id_parts)
 
     def has_conflict(self, other: DiffItem) -> bool:
         # If the identifiers are the same, there is a conflict if the values are different
         if self.identifier == other.identifier:
             return type(self) != type(other) or self.value != other.value
 
@@ -128,53 +123,56 @@
     @abc.abstractmethod
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         ...
 
     def _walk_to_last_path_node(self, root: dict[str, Any] | list[Any]) -> Any:
         current_walked_obj: Any = root
         for path_part in self.path[:-1]:
-            current_walked_obj = current_walked_obj[path_part.access_key]
+            if isinstance(path_part, PathNodeKey):
+                current_walked_obj = current_walked_obj[path_part.key]
+            elif isinstance(path_part, PathNodeIndex):
+                current_walked_obj = current_walked_obj[path_part.index]
         return current_walked_obj
 
 
 class DictionaryItemAdded(DiffItem):
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
-        current_walked_obj[self.path[-1].access_key] = self.value
+        current_walked_obj[self.path[-1].key] = self.value
 
 
 class DictionaryItemRemoved(DiffItem):
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
-        del current_walked_obj[self.path[-1].access_key]
+        del current_walked_obj[self.path[-1].key]
 
 
 class IterableItemAdded(DiffItem):
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
         current_walked_obj.append(self.value)
 
 
 class IterableItemRemoved(DiffItem):
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
-        del current_walked_obj[self.path[-1].access_key]
+        del current_walked_obj[self.path[-1].index]
 
 
 class ValueChanged(DiffItem):
     def __init__(self, old_value: Any, new_value: Any, path: list[PathNode]):
         super().__init__(new_value, path)
         self.old_value = old_value
 
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
-        current_walked_obj[self.path[-1].access_key] = self.value
+        current_walked_obj[self.path[-1].key] = self.value
 
 
 class TypeChanges(DiffItem):
     def __init__(self, old_value: Any, new_value: Any, path: list[PathNode]):
         super().__init__(new_value, path)
         self.old_value = old_value
 
     def apply_in_place(self, root: dict[str, Any] | list[Any]) -> None:
         current_walked_obj = self._walk_to_last_path_node(root)
-        current_walked_obj[self.path[-1].access_key] = self.value
+        current_walked_obj[self.path[-1].key] = self.value
```

### Comparing `slingshot_ai-0.0.18/src/slingshot/shared/utils.py` & `slingshot_ai-0.0.18rc1/src/slingshot/shared/utils.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/templates/inference_template.py` & `slingshot_ai-0.0.18rc1/src/slingshot/templates/inference_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/src/slingshot/templates/label_studio_data_export_template.py` & `slingshot_ai-0.0.18rc1/src/slingshot/templates/label_studio_data_export_template.py`

 * *Files identical despite different names*

### Comparing `slingshot_ai-0.0.18/PKG-INFO` & `slingshot_ai-0.0.18rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: slingshot-ai
-Version: 0.0.18
-Summary: Slingshot Python SDK
+Version: 0.0.18rc1
+Summary: 
 Author: Slingshot AI
 Author-email: service-account@slingshot.xyz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1)
```

