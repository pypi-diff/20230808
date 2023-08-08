# Comparing `tmp/tecton-0.8.0b4.tar.gz` & `tmp/tecton-0.8.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.8.0b4.tar", last modified: Wed Aug  2 22:51:03 2023, max compression
+gzip compressed data, was "tecton-0.8.0b5.tar", last modified: Tue Aug  8 21:38:00 2023, max compression
```

## Comparing `tecton-0.8.0b4.tar` & `tecton-0.8.0b5.tar`

### file list

```diff
@@ -1,558 +1,578 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.608910 tecton-0.8.0b4/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-08-02 22:50:59.000000 tecton-0.8.0b4/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3889 2023-08-02 22:51:03.608910 tecton-0.8.0b4/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-08-02 22:50:59.000000 tecton-0.8.0b4/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.552906 tecton-0.8.0b4/protoc_gen_swagger/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/protoc_gen_swagger/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.552906 tecton-0.8.0b4/protoc_gen_swagger/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/protoc_gen_swagger/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-08-02 22:50:59.000000 tecton-0.8.0b4/protoc_gen_swagger/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-08-02 22:50:59.000000 tecton-0.8.0b4/protoc_gen_swagger/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-08-02 22:51:03.608910 tecton-0.8.0b4/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2093 2023-08-02 22:50:59.000000 tecton-0.8.0b4/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.556907 tecton-0.8.0b4/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5291 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.556907 tecton-0.8.0b4/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2259 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6181 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      944 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26794 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.560907 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3115 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2628 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/query_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.560907 tecton-0.8.0b4/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11417 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15439 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12522 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9017 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20686 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15669 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_internals/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.560907 tecton-0.8.0b4/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34143 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4315 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2738 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14945 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3281 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5832 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      810 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    89724 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19825 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31279 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13789 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34112 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   166758 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21844 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22506 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3009 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.564907 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.568907 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.568907 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.572908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.572908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.572908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.572908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.572908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.576908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.576908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.576908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.576908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.576908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.556907 tecton-0.8.0b4/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3889 2023-08-02 22:51:01.000000 tecton-0.8.0b4/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19107 2023-08-02 22:51:02.000000 tecton-0.8.0b4/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-08-02 22:51:01.000000 tecton-0.8.0b4/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-08-02 22:51:02.000000 tecton-0.8.0b4/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      833 2023-08-02 22:51:02.000000 tecton-0.8.0b4/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       95 2023-08-02 22:51:02.000000 tecton-0.8.0b4/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14624 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8498 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/odfv_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2291 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17780 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.580908 tecton-0.8.0b4/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.584909 tecton-0.8.0b4/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13329 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19699 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7206 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5409 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4818 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19497 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2309 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      623 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7393 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/materialization_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6916 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1395 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6304 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/pipeline_common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4393 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/pipeline_sql_builder.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.584909 tecton-0.8.0b4/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10765 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28576 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8446 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69568 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.584909 tecton-0.8.0b4/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2677 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8356 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      283 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      610 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9133 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5813 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/schema_derivation_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.584909 tecton-0.8.0b4/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    38770 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33509 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4912 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.584909 tecton-0.8.0b4/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    84302 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3520 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4122 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34925 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/auditlog/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auditlog/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auditlog/metadata_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.588909 tecton-0.8.0b4/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21878 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2970 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.592909 tecton-0.8.0b4/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.592909 tecton-0.8.0b4/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.592909 tecton-0.8.0b4/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/common/spark_schema_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.592909 tecton-0.8.0b4/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/data_source_access_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15875 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16873 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13426 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13389 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.596910 tecton-0.8.0b4/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   114010 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/online_store_writer/config_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/snowflake/location_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7722 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.600910 tecton-0.8.0b4/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29236 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33593 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.604910 tecton-0.8.0b4/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.604910 tecton-0.8.0b4/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25814 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2090 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35900 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      890 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.604910 tecton-0.8.0b4/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1600615 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4039 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22947 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11059 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34132 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:51:03.608910 tecton-0.8.0b4/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28800 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1229 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4248 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7985 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5424 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17320 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5404 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2135 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1677 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4842 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-08-02 22:50:59.000000 tecton-0.8.0b4/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.209794 tecton-0.8.0b5/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      159 2023-08-08 21:37:56.000000 tecton-0.8.0b5/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3912 2023-08-08 21:38:00.205794 tecton-0.8.0b5/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2023-08-08 21:37:56.000000 tecton-0.8.0b5/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.149794 tecton-0.8.0b5/protoc_gen_swagger/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/protoc_gen_swagger/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.149794 tecton-0.8.0b5/protoc_gen_swagger/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/protoc_gen_swagger/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2657 2023-08-08 21:37:56.000000 tecton-0.8.0b5/protoc_gen_swagger/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16494 2023-08-08 21:37:56.000000 tecton-0.8.0b5/protoc_gen_swagger/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-08-08 21:38:00.209794 tecton-0.8.0b5/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2138 2023-08-08 21:37:56.000000 tecton-0.8.0b5/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.149794 tecton-0.8.0b5/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5291 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.153794 tecton-0.8.0b5/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11143 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1169 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6175 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7925 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26971 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2901 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13125 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      666 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.153794 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      421 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3078 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3111 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1782 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2624 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      198 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4147 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16135 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/query_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12564 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/querytree_api.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.153794 tecton-0.8.0b5/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11415 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10844 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15546 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12512 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9421 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9161 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2823 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6101 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15679 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4991 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       36 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_internals/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      276 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2238 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.157794 tecton-0.8.0b5/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15083 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1574 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34116 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4310 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6569 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2738 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14931 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25411 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3281 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7680 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1664 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1312 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6859 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      670 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1850 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/duckdb_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.157794 tecton-0.8.0b5/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7294 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      914 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    89724 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28500 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31504 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13799 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7485 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   166925 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22255 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      673 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22506 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3888 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10498 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3113 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2730 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3422 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.161794 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.165794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.165794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.169794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.169794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.169794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.169794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.169794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.173794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.177794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21163 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.177794 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1185 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.149794 tecton-0.8.0b5/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3912 2023-08-08 21:37:58.000000 tecton-0.8.0b5/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19699 2023-08-08 21:37:59.000000 tecton-0.8.0b5/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-08-08 21:37:58.000000 tecton-0.8.0b5/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2023-08-08 21:37:58.000000 tecton-0.8.0b5/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      870 2023-08-08 21:37:58.000000 tecton-0.8.0b5/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      109 2023-08-08 21:37:59.000000 tecton-0.8.0b5/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.177794 tecton-0.8.0b5/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14624 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8498 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5747 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/odfv_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6356 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.177794 tecton-0.8.0b5/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2294 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17720 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.177794 tecton-0.8.0b5/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3863 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.181794 tecton-0.8.0b5/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13235 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20506 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7222 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5643 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4883 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19524 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9765 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2464 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      628 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/materialization_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8257 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6449 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/pipeline_common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4416 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/pipeline_sql_builder.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.181794 tecton-0.8.0b5/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10840 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31236 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      630 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/executor_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9307 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    76676 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.181794 tecton-0.8.0b5/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3380 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9006 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      283 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1837 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/pandas/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8188 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/query_tree_compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12815 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/query_tree_executor.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      849 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11421 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      756 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1961 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5813 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/schema_derivation_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      660 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    38760 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1258 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5274 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33479 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6872 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_duckdb/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_duckdb/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_duckdb/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_duckdb/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1384 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_duckdb/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      993 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_duckdb/query/rewrite.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4278 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    84302 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9207 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.185794 tecton-0.8.0b5/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17760 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3587 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2481 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4335 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34925 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6463 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4071 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7076 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/auditlog/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auditlog/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auditlog/metadata_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21878 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2935 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1922 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3027 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2970 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1339 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2070 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/common/spark_schema_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.189794 tecton-0.8.0b5/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3289 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.193794 tecton-0.8.0b5/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6382 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1589 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/data_source_access_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1921 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2758 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4497 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15875 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2124 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1971 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5638 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2316 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2696 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16873 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4541 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9668 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3945 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2142 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2358 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9697 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2979 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.193794 tecton-0.8.0b5/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1937 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1708 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3569 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13651 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7654 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2598 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13389 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5790 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2691 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14321 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   114132 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4353 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/online_store_writer/config_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8041 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/snowflake/location_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7263 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7722 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.197794 tecton-0.8.0b5/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.201794 tecton-0.8.0b5/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29246 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.201794 tecton-0.8.0b5/tecton_snowflake/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      768 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/dataframe_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7613 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/queries.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2278 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7376 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33561 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.201794 tecton-0.8.0b5/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.205794 tecton-0.8.0b5/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      465 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26266 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2138 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    36066 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      898 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.205794 tecton-0.8.0b5/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1600615 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4064 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23229 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11198 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34441 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:38:00.205794 tecton-0.8.0b5/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3054 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8463 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29062 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1393 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4856 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8617 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5668 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17320 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5496 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2310 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4858 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2023-08-08 21:37:56.000000 tecton-0.8.0b5/tecton_spark/udfs.py
```

### Comparing `tecton-0.8.0b4/PKG-INFO` & `tecton-0.8.0b5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.8.0b4
+Version: 0.8.0b5
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Provides-Extra: databricks-connect10
 Provides-Extra: databricks-connect11
 Provides-Extra: pyspark
 Provides-Extra: pyspark3
 Provides-Extra: pyspark3.1
 Provides-Extra: pyspark3.2
 Provides-Extra: pyspark3.3
+Provides-Extra: duckdb
 Provides-Extra: snowflake
 Provides-Extra: snowpark
 Provides-Extra: athena
 
 ![logo](https://s3.us-west-2.amazonaws.com/tecton.ai.public/documentation/pypi/tecton-logo.svg)
 
 Tecton is the fastest way to build operational machine learning applications. It helps automate real-time decision making like fraud detection, product recommendations, and search result ranking in production applications.
```

### Comparing `tecton-0.8.0b4/README.md` & `tecton-0.8.0b5/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/protoc_gen_swagger/options/annotations_pb2.py` & `tecton-0.8.0b5/protoc_gen_swagger/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/protoc_gen_swagger/options/openapiv2_pb2.py` & `tecton-0.8.0b5/protoc_gen_swagger/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/setup.py` & `tecton-0.8.0b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.8.0b4',
+    version='0.8.0b5',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version'],
-    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'snowflake': ['snowflake-connector-python[pandas]~=2.8'], 'snowpark': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=2.15']},
+    install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos~=1.52', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas~=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow~=8.0'],
+    extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'duckdb': ['duckdb~=0.8.1'], 'snowflake': ['snowflake-connector-python[pandas]~=2.8'], 'snowpark': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=2.15']},
     packages=packages,
 )
```

### Comparing `tecton-0.8.0b4/tecton/__init__.py` & `tecton-0.8.0b5/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/analytics.py` & `tecton-0.8.0b5/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/athena_api.py` & `tecton-0.8.0b5/tecton/_internals/athena_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     feature_set_config: FeatureSetConfig,
     spine: Optional[Union[pandas.DataFrame, str]] = None,
     timestamp_key: Optional[str] = None,
     include_feature_view_timestamp_columns: bool = False,
     from_source: bool = False,
     save: bool = False,
     save_as: Optional[str] = None,
-    start_time: datetime = None,
-    end_time: datetime = None,
+    start_time: Optional[datetime] = None,
+    end_time: Optional[datetime] = None,
     entities: Optional[Union[pandas.DataFrame]] = None,
 ) -> TectonDataFrame:
     if from_source:
         msg = "Retrieving features directly from data sources (i.e. using from_source=True) is not supported with Athena retrieval. Use from_source=False and feature views that have offline materialization enabled."
         raise TectonAthenaNotImplementedError(msg)
     if save or save_as is not None:
         msg = "save is not supported for Athena"
```

### Comparing `tecton-0.8.0b4/tecton/_internals/data_frame_helper.py` & `tecton-0.8.0b5/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/delete_keys_api.py` & `tecton-0.8.0b5/tecton/_internals/delete_keys_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     keys: Union[pyspark_sql.DataFrame, pd.DataFrame],
     feature_definition: feature_definition_wrapper.FeatureDefinitionWrapper,
 ):
     if not offline and not online:
         raise errors.NO_STORE_SELECTED
 
     materialization_state_transitions = feature_definition.fv_spec.materialization_state_transitions
-    if offline and any([transition.offline_enabled for transition in materialization_state_transitions]):
+    if offline and any(transition.offline_enabled for transition in materialization_state_transitions):
         if not feature_definition.offline_store_config.HasField("delta"):
             raise errors.OFFLINE_STORE_NOT_SUPPORTED
 
-    if online and all([not transition.online_enabled for transition in materialization_state_transitions]):
+    if online and all(not transition.online_enabled for transition in materialization_state_transitions):
         print("Online materialization was never enabled. No data to be deleted in online store.")
         online = False
 
-    if offline and all([not transition.offline_enabled for transition in materialization_state_transitions]):
+    if offline and all(not transition.offline_enabled for transition in materialization_state_transitions):
         print("Offline materialization was never enabled. No data to be deleted in offline store.")
         offline = False
 
     if not (offline or online):
         return None
 
     spark_df = _get_keys_spark_df(keys, feature_definition.view_schema)
```

### Comparing `tecton-0.8.0b4/tecton/_internals/display.py` & `tecton-0.8.0b5/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/env_utils.py` & `tecton-0.8.0b5/tecton/_internals/env_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,8 @@
 
 
 def _get_current_username_uncached() -> str:
     for f in (_get_databricks_user, _get_system_user):
         user = f()
         if user:
             return user
-    else:
-        return ""
+    return ""
```

### Comparing `tecton-0.8.0b4/tecton/_internals/errors.py` & `tecton-0.8.0b5/tecton/_internals/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 
 def INVALID_SPINE_TIME_KEY_TYPE_SPARK(t):
     return TectonValidationError(
         f"Invalid type of timestamp_key column in the given spine. Expected TimestampType, got {t}"
     )
 
 
+INVALID_NULL_SPINE_TIME_KEY = TectonValidationError(
+    "Unable to infer the time range of the spine. This typically occurs when all the timestamps in the spine are null."
+)
+
+
 def INVALID_SPINE_TIME_KEY_TYPE_PANDAS(t):
     return TectonValidationError(f"Invalid type of timestamp_key column in the given spine. Expected datetime, got {t}")
 
 
 def MISSING_SPINE_COLUMN(param, col, existing_cols):
     return TectonValidationError(
         f"{param} column is missing from the spine. Expected to find '{col}' among available spine columns: '{', '.join(existing_cols)}'."
```

### Comparing `tecton-0.8.0b4/tecton/_internals/find_spark.py` & `tecton-0.8.0b5/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/ingest_utils.py` & `tecton-0.8.0b5/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/materialization_api.py` & `tecton-0.8.0b5/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service_impl/error_lib.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service_impl/http_client.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service_impl/http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """
         :param grpc_call: gRPC call object representation
         :param request: Request proto.
         :param timeout_sec: timeout for request in seconds
 
         :return: Response proto.
         """
-        json_request = dict()
+        json_request = {}
         json_request["method"] = grpc_call.method
         json_request["metadata"] = request_lib.request_headers()
         json_request["request"] = base64.encodebytes(grpc_call.request_serializer(request)).decode("utf-8")
 
         request_url = request_lib.request_url()
         response = requests_session.post(request_url, json=json_request, timeout=timeout_sec)
         response.raise_for_status()
```

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service_impl/response.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/metadata_service_impl/service_calls.py` & `tecton-0.8.0b5/tecton/_internals/metadata_service_impl/service_calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 def get_method_name_to_grpc_call() -> Dict[str, GrpcCall]:
     """
     dictionary of mds methods to grpc call repr obj
     later used by the grpc stub and the http stub for MDS py client
     """
-    method_name_to_call = dict()
+    method_name_to_call = {}
     for module in grpc_service_modules:
         for service_name, descriptor in module.DESCRIPTOR.services_by_name.items():
             for method in descriptor.methods:
                 if method.input_type.name == "Empty":
                     request_serializer = Empty.SerializeToString
                 else:
                     request_serializer = getattr(module, method.input_type.name).SerializeToString
```

### Comparing `tecton-0.8.0b4/tecton/_internals/mock_source_utils.py` & `tecton-0.8.0b5/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/query_helper.py` & `tecton-0.8.0b5/tecton/_internals/query_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         data = {key: [value] * response_count for key, value in join_keys.items()}
         for result in response.results:
             features = self._feature_dict(result, response.metadata)
             # note that int(1) = np.int_(1) so dict lookup works here
             for k, v in features.items():
                 if k not in data.keys():
                     data[k] = []
-                data[k] = list(data[k]) + [v]  # type: ignore
+                data[k] = [*list(data[k]), v]  # type: ignore
         return pd.DataFrame(data=data)
 
     def _pb_to_python_value(self, v: Value, data_type: FeatureServerComplexDataType):
         """Converts a "Value" wrapped value into the type indicated by "type"."""
         which = v.WhichOneof("kind")
         if which is None or which == TYPE_NULL_VALUE:
             return None
```

### Comparing `tecton-0.8.0b4/tecton/_internals/repo/function_serialization.py` & `tecton-0.8.0b5/tecton/_internals/repo/function_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 # shouldn't cause any wrong behavior.
 # IMPORTANT: Include backslash paths for windows.
 TECTON_TRANSFORMATION_WHITELIST = ["tecton/compat", "tecton\compat", "integration_tests/"]
 
 
 # returns true if the module is defined by tecton, rather than by the user
 def is_tecton_defined(module):
-    return any([whitelist_str in module for whitelist_str in TECTON_TRANSFORMATION_WHITELIST])
+    return any(whitelist_str in module for whitelist_str in TECTON_TRANSFORMATION_WHITELIST)
 
 
 def should_serialize_function(func):
     """Determines if the function should be serialized or not.
 
     During notebook development, not all functions need to be serialized since they never need to be sent over the wire.
```

### Comparing `tecton-0.8.0b4/tecton/_internals/rewrite.py` & `tecton-0.8.0b5/tecton/_internals/rewrite.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from typing import Optional
 from typing import Type
 
 import attrs
 import pendulum
 
+from tecton._internals import errors
 from tecton._internals import time_utils
 from tecton_core import conf
 from tecton_core.pipeline_common import get_time_window_from_data_source_node
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.node_interface import QueryNode
 from tecton_core.query.nodes import AddAnchorTimeNode
 from tecton_core.query.nodes import AddDurationNode
@@ -22,17 +23,17 @@
 from tecton_core.query.nodes import FeatureViewPipelineNode
 from tecton_core.query.nodes import MockDataSourceScanNode
 from tecton_core.query.nodes import OfflineStoreScanNode
 from tecton_core.query.nodes import PartialAggNode
 from tecton_core.query.nodes import RenameColsNode
 from tecton_core.query.nodes import RespectFeatureStartTimeNode
 from tecton_core.query.nodes import SelectDistinctNode
+from tecton_core.query.nodes import StagingNode
 from tecton_core.query.nodes import UserSpecifiedDataNode
 from tecton_core.query.rewrite import Rewrite
-from tecton_core.query.rewrite import tree_contains
 
 
 def _find_all_nodes_of_type(tree: NodeRef, node_type: Type[QueryNode]) -> List[NodeRef]:
     """Returns a list of all NodeRefs of the given type."""
     nodes = []
 
     if isinstance(tree.node, node_type):
@@ -93,30 +94,40 @@
         # In our current usage of AsofJoinNode, we always pass in the spine on the left.
         spine_df = NodeRef.shallow_copy(node.left_container.node)
         self.pushdown_entities(node.right_container.node, spine_df, node.join_cols)
 
     def rewrite_asof_full_agg(self, tree: NodeRef):
         node = tree.node
 
-        # We only want to rewrite for a user specified spine.
-        if not tree_contains(node.spine, UserSpecifiedDataNode):
+        if not node.enable_spine_entity_pushdown_rewrite:
             return
-        spine = NodeRef.shallow_copy(node.spine)
-        self.pushdown_entities(node.partial_agg_node, spine, node.fdw.join_keys)
+
+        user_provided_spine_node = _get_spine_user_specified_data_node(NodeRef.shallow_copy(node.spine)).as_ref()
+
+        # Note: we can't simply using join keys to pushdown entity because wildcard FV can have a spine missing wildcard
+        # key, so we need to check what exact entities are used in spine if wildcard key is present, and only push those
+        # entities down.
+        entities_to_push_down = node.fdw.join_keys
+        if node.fdw.wildcard_join_key and node.fdw.wildcard_join_key not in user_provided_spine_node.columns:
+            entities_to_push_down = set(entities_to_push_down) - {node.fdw.wildcard_join_key}
+
+        # entity_rewritable ensures there is a UserSpecifiedDataNode in the spine.
+        self.pushdown_entities(node.partial_agg_node, user_provided_spine_node, list(entities_to_push_down))
 
     def pushdown_entities(self, tree: NodeRef, spine: NodeRef, join_cols: List[str]):
         node = tree.node
         can_be_pushed_down = (
             RespectFeatureStartTimeNode,
             RenameColsNode,
             FeatureTimeFilterNode,
             AddAnchorTimeNode,
             AddDurationNode,
             AddEffectiveTimestampNode,
             PartialAggNode,
+            StagingNode,
         )
         if isinstance(node, can_be_pushed_down):
             self.pushdown_entities(node.input_node, spine, join_cols)
         else:
             entities_node = SelectDistinctNode(spine, join_cols).as_ref()
             tree.node = EntityFilterNode(node.as_ref(), entities_node, join_cols)
 
@@ -155,22 +166,15 @@
 
         self.pushdown_time_range(node.right_container.node, self.spine_time_limits)
 
     def rewrite_asof_full_agg(self, tree: NodeRef):
         """Computes the spine time limits and pushes them down to all relevant nodes in the partial aggregates."""
         node = tree.node
 
-        # For an AsofFullAggJoinNode, the spine is the left side of the join and the partial aggregates are the right.
-        # The rewrite should only be applied when (a) the correct time range can be determined from the spine and (b)
-        # specific time filters have not yet been applied to the partial aggregates.
-        # Condition (a) means that the spine must contain a UserSpecifiedDataNode.
-        # Condition (b) means that the fv.run and fv.ghf(time range) cases should be avoided, since the time ranges will
-        # already have been applied to the partial aggregates. Both of these cases use a PartialAggNode as a fake spine,
-        # so they can be avoided by skipping the rewrite if the spine contains a PartialAggNode.
-        if tree_contains(node.spine, PartialAggNode) or not tree_contains(node.spine, UserSpecifiedDataNode):
+        if not node.enable_spine_time_pushdown_rewrite:
             return
 
         if self.spine_time_limits is None:
             self.spine_time_limits = _get_spine_time_limits(node)
         self.pushdown_time_range(node.partial_agg_node, self.spine_time_limits)
 
     # Push down and convert spine time filter to either raw data or feature time filter at the DataSourceScanNode or OfflineStoreScanNode.
@@ -181,14 +185,15 @@
             RespectFeatureStartTimeNode,
             RenameColsNode,
             PartialAggNode,
             FeatureTimeFilterNode,
             AddAnchorTimeNode,
             AddDurationNode,
             AddEffectiveTimestampNode,
+            StagingNode,
         )
         if isinstance(node, can_be_pushed_down):
             self.pushdown_time_range(node.input_node, spine_time_limits)
         elif isinstance(node, (OfflineStoreScanNode, FeatureViewPipelineNode)):
             feature_time_limits = time_utils.get_feature_data_time_limits(
                 fd=node.feature_definition_wrapper, spine_time_limits=spine_time_limits
             )
@@ -231,13 +236,18 @@
     for child in cur_node.inputs:
         node = _get_spine_user_specified_data_node(child.node)
         if node:
             return node
     return None
 
 
-def _get_spine_time_limits(cur_node: QueryNode) -> Optional[pendulum.Period]:
+def _get_spine_time_limits(cur_node: QueryNode) -> pendulum.Period:
     user_specified_data_node = _get_spine_user_specified_data_node(cur_node)
     if not user_specified_data_node:
-        return None
+        # We don't expect this to occur
+        msg = "Expected spine to contain a UserSpecifiedDataNode, but it did not."
+        raise ValueError(msg)
     timestamp_key = user_specified_data_node.metadata["timestamp_key"]
-    return user_specified_data_node.data.get_time_range(timestamp_key)
+    limits = user_specified_data_node.data.get_time_range(timestamp_key)
+    if limits is None:
+        raise errors.INVALID_NULL_SPINE_TIME_KEY
+    return limits
```

### Comparing `tecton-0.8.0b4/tecton/_internals/run_api.py` & `tecton-0.8.0b5/tecton/_internals/run_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from tecton_core.query.builder import build_get_full_agg_features
 from tecton_core.query.builder import build_materialization_querytree
 from tecton_core.query.builder import build_pipeline_querytree
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.nodes import AddAnchorTimeNode
 from tecton_core.query.nodes import ConvertEpochToTimestampNode
 from tecton_core.query.nodes import RenameColsNode
-from tecton_core.query.sql_compat import default_case
+from tecton_core.query.nodes import StagingNode
 from tecton_proto.args import pipeline_pb2
 from tecton_proto.data import feature_view_pb2
 from tecton_spark import materialization_plan
 from tecton_spark.partial_aggregations import partial_aggregate_column_renames
 from tecton_spark.pipeline_helper import get_all_input_keys
 from tecton_spark.pipeline_helper import get_fco_ids_to_input_keys
 from tecton_spark.pipeline_helper import run_mock_odfv_pipeline
@@ -115,16 +115,18 @@
     Any extra querytree nodes in this function should simply be a display-level
     modification (like field rename, type change, etc).
     """
     if fd.is_temporal:
         qt = build_materialization_querytree(fd, for_stream=False, feature_data_time_limits=feature_time_limits_aligned)
         # For a BFV, the materialization querytree is an `AddAnchorTimeNode` wrapped around exactly what we want, so we
         # just extract the input node.
-        assert isinstance(qt.node, AddAnchorTimeNode)
-        return qt.node.inputs[0]
+        assert isinstance(qt.node, StagingNode)
+        staging_node_input = qt.node.inputs[0]
+        assert isinstance(staging_node_input.node, AddAnchorTimeNode)
+        return staging_node_input.node.inputs[0]
     elif fd.is_temporal_aggregate:
         if aggregation_level == AGGREGATION_LEVEL_PARTIAL:
             qt = build_materialization_querytree(
                 fd,
                 for_stream=False,
                 feature_data_time_limits=feature_time_limits_aligned,
                 include_window_end_time=True,
@@ -133,15 +135,15 @@
             if fd.is_continuous:
                 renames = {
                     **partial_aggregate_column_renames(
                         slide_interval_string=fd.get_aggregate_slide_interval_string,
                         trailing_time_window_aggregation=fd.trailing_time_window_aggregation,
                     ),
                 }
-                drop = [default_case(ANCHOR_TIME)]
+                drop = [ANCHOR_TIME]
             else:
                 # The `PartialAggNode` returned by `build_materialization_querytree` converts timestamps to epochs. We convert back
                 # from epochs to timestamps since timestamps are more readable.
                 qt = ConvertEpochToTimestampNode(
                     qt, {col: fd.get_feature_store_format_version for col in (ANCHOR_TIME, WINDOW_END_COLUMN_NAME)}
                 ).as_ref()
                 renames = {
```

### Comparing `tecton-0.8.0b4/tecton/_internals/sdk_decorators.py` & `tecton-0.8.0b5/tecton/_internals/sdk_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,26 +199,26 @@
 
 
 @overload
 def sdk_public_method(
     *,
     requires_validation: bool = False,
     validation_error_message: Callable[[str, str, str], Exception] = errors.TECTON_OBJECT_REQUIRES_VALIDATION,
-    supports_skip_validation: Tuple[compute_mode.ComputeMode, ...] = tuple(),
+    supports_skip_validation: Tuple[compute_mode.ComputeMode, ...] = (),
 ) -> Callable[[Callable[_PT, _RT]], Callable[_PT, _RT]]:
     ...
 
 
 @typeguard.typeguard_ignore
 def sdk_public_method(
     original_function: Optional[Callable[_PT, _RT]] = None,
     *,
     requires_validation: bool = False,
     validation_error_message: Callable[[str, str, str], Exception] = errors.TECTON_OBJECT_REQUIRES_VALIDATION,
-    supports_skip_validation: Tuple[compute_mode.ComputeMode, ...] = tuple(),
+    supports_skip_validation: Tuple[compute_mode.ComputeMode, ...] = (),
 ) -> Union[Callable[_PT, _RT], Callable[[Callable[_PT, _RT]], Callable[_PT, _RT]]]:
     """Decorator for public SDK methods that should have analytics logging.
 
     :param original_function: The function to be wrapped.
     :param requires_validation: If True, will run Tecton object validation (if needed) before entering running original
         function. Automatically triggered validation will be logged separately. Should only be set to True when used
         to wrap a "Tecton object" (e.g. a DataSource or FeatureView) method.
```

### Comparing `tecton-0.8.0b4/tecton/_internals/snowflake_api.py` & `tecton-0.8.0b5/tecton/_internals/snowflake_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -153,16 +153,16 @@
         cur = connection.cursor()
         cur.execute(sql_str, _statement_params={"SF_PARTNER": "tecton-ai"})
         return TectonDataFrame._create(cur.fetch_pandas_all())
 
 
 def get_dataframe_for_data_source(
     data_source: specs.DataSourceSpec,
-    start_time: datetime = None,
-    end_time: datetime = None,
+    start_time: Optional[datetime] = None,
+    end_time: Optional[datetime] = None,
 ) -> TectonDataFrame:
     if not conf.get_bool("ALPHA_SNOWFLAKE_SNOWPARK_ENABLED"):
         msg = "get_dataframe is only supported with Snowpark enabled"
         raise TectonSnowflakeNotImplementedError(msg)
 
     start_time = get_timezone_aware_datetime(start_time)
     end_time = get_timezone_aware_datetime(end_time)
@@ -204,15 +204,19 @@
     view_schema: schema_pb2.Schema,
     feature_view_args: feature_view__args_pb2.FeatureViewArgs,
 ) -> schema_pb2.Schema:
     is_aggregate = len(feature_view_args.materialized_feature_view_args.aggregations) > 0
     if not is_aggregate:
         return view_schema
 
+    # Tecton on Snowflake doesn't include the anchor time in the materialization schema
+    # But if Snowflake is used only to execute the FV pipeline to pass to DuckDB, DuckDB expects an anchor time
+    # TODO(danny): remove this when Tecton on Python relies on explicit schemas
+    include_anchor_time_in_schema = conf.get_or_none("SQL_DIALECT") == "duckdb"
     materialization_schema = core_schema_derivation_utils.compute_aggregate_materialization_schema_from_view_schema(
-        view_schema, feature_view_args, is_spark=False
+        view_schema, feature_view_args, is_spark=include_anchor_time_in_schema
     )
 
     # Make column name uppercase.
     for column in materialization_schema.columns:
         column.name = column.name.upper()
     return materialization_schema
```

### Comparing `tecton-0.8.0b4/tecton/_internals/spark_api.py` & `tecton-0.8.0b5/tecton_spark/offline_store.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,502 +1,517 @@
+import functools
+import itertools
 import logging
-import tempfile
+import os
+import random
+import time
+from abc import ABC
+from abc import abstractmethod
+from dataclasses import dataclass
 from datetime import datetime
-from typing import Callable
-from typing import Dict
+from datetime import timedelta
 from typing import List
 from typing import Optional
-from typing import Sequence
-from typing import Union
 
-import pandas as pd
 import pendulum
-from pyspark import sql as pyspark_sql
-from pyspark.sql import streaming as pyspark_streaming
+from py4j.protocol import Py4JJavaError
+from pyspark.sql import Column
+from pyspark.sql import DataFrame
+from pyspark.sql import SparkSession
+from pyspark.sql import functions
+from pyspark.sql.types import IntegerType
+from pyspark.sql.types import LongType
+from pyspark.sql.types import StructType
+from pyspark.sql.types import TimestampType
+
+from tecton_core import time_utils as core_time_utils
+from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper as FeatureDefinition
+from tecton_core.offline_store import TIME_PARTITION
+from tecton_core.offline_store import _check_supported_offline_store_version
+from tecton_core.offline_store import _timestamp_formats
+from tecton_core.offline_store import partition_col_for_parquet
+from tecton_core.offline_store import partition_size_for_delta
+from tecton_core.offline_store import partition_size_for_parquet
+from tecton_core.offline_store import window_size_seconds
+from tecton_core.query_consts import ANCHOR_TIME
+from tecton_spark import time_utils as spark_time_utils
+
+
+DBRICKS_MULTI_CLUSTER_WRITES_ENABLED = "spark.databricks.delta.multiClusterWrites.enabled"
+DBRICKS_RUNTIME_VERSION = "DATABRICKS_RUNTIME_VERSION"
 
-from tecton import tecton_context
-from tecton import types as sdk_types
-from tecton._internals import errors
-from tecton._internals import ingest_utils
-from tecton._internals import rewrite
-from tecton._internals import time_utils
-from tecton._internals import type_utils
-from tecton._internals import utils
-from tecton.framework.data_frame import TectonDataFrame
-from tecton.framework.dataset import Dataset
-from tecton.tecton_context import TectonContext
-from tecton_core import data_types
-from tecton_core import errors as core_errors
-from tecton_core import feature_set_config
-from tecton_core import materialization_context
-from tecton_core import query_consts
-from tecton_core import schema
-from tecton_core import schema_derivation_utils as core_schema_derivation_utils
-from tecton_core import specs
-from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
-from tecton_core.feature_set_config import FeatureDefinitionAndJoinConfig
-from tecton_core.query import builder
-from tecton_core.query import node_interface
-from tecton_core.query import nodes
-from tecton_core.query import sql_compat
-from tecton_core.time_utils import align_time_downwards
-from tecton_proto.args import feature_view_pb2
-from tecton_proto.args import virtual_data_source_pb2 as virtual_data_source__args_pb2
-from tecton_proto.common import schema_pb2
-from tecton_proto.common import spark_schema_pb2
-from tecton_proto.data import feature_view_pb2 as feature_view__data_pb2
-from tecton_spark import data_source_helper
-from tecton_spark import schema_derivation_utils
-from tecton_spark import schema_spark_utils
-from tecton_spark import spark_schema_wrapper
-from tecton_spark.spark_helper import check_spark_version
-from tecton_spark.time_utils import convert_epoch_to_datetime
-from tecton_spark.time_utils import convert_timestamp_to_epoch
+SPARK_GCS_DELTA_LOGSTORE_CLASS = "io.delta.storage.GCSLogStore"
 
+SPARK31_DELTA_LOGSTORE_CLASS = "spark.delta.logStore.class"
+SPARK31_DYNAMODB_LOGSTORE_CLASS = "io.delta.storage.DynamoDBLogStore"
 
-logger = logging.getLogger(__name__)
-
-_CHECKPOINT_DIRECTORIES: List[tempfile.TemporaryDirectory] = []
+SPARK32_OR_HIGHER_DELTA_LOGSTORE_CLASS = "spark.delta.logStore.s3.impl"
+SPARK32_OR_HIGHER_DYNAMODB_LOGSTORE_CLASS = "io.delta.storage.S3DynamoDBLogStore"
 
+logger = logging.getLogger(__name__)
 
-def get_historical_features_for_feature_service(
-    feature_service_spec: specs.FeatureServiceSpec,
-    feature_set_config: feature_set_config.FeatureSetConfig,
-    spine: Union[pyspark_sql.DataFrame, pd.DataFrame, TectonDataFrame],
-    timestamp_key: Optional[str],
-    from_source: bool,
-    save: bool,
-    save_as: Optional[str],
-) -> TectonDataFrame:
-    timestamp_required = spine is not None and any(
-        [_should_infer_timestamp_of_spine(fd, timestamp_key) for fd in feature_set_config.feature_definitions]
-    )
-
-    if timestamp_required:
-        timestamp_key = timestamp_key or utils.infer_timestamp(spine)
-
-    if isinstance(spine, pd.DataFrame):
-        spine_schema = feature_set_config.spine_schema
-        if timestamp_key is not None:
-            spine_schema += schema.Schema.from_dict({timestamp_key: data_types.TimestampType()})
-        spine = TectonDataFrame._create_from_pandas_with_schema(spine, spine_schema)
-    elif not isinstance(spine, TectonDataFrame):
-        spine = TectonDataFrame._create(spine)
-
-    if spine:
-        utils.validate_spine_dataframe(spine, timestamp_key, feature_set_config.request_context_keys)
-
-    user_data_node_metadata = {}
-    # TODO: Create a SpineNode with a param of timestamp_key instead of using UserSpecifiedNode.
-    if timestamp_key:
-        user_data_node_metadata["timestamp_key"] = timestamp_key
-    tree = builder.build_feature_set_config_querytree(
-        feature_set_config,
-        nodes.UserSpecifiedDataNode(spine, user_data_node_metadata).as_ref(),
-        timestamp_key,
-        from_source,
-    )
-
-    df = TectonDataFrame._create(tree)
-    if save or save_as is not None:
-        return Dataset._create(
-            df=df,
-            save_as=save_as,
-            workspace=feature_service_spec.workspace,
-            feature_service_id=feature_service_spec.id,
-            spine=spine,
-            timestamp_key=timestamp_key,
-        )
-    else:
-        return df
 
+@dataclass
+class OfflineStoreWriterParams:
+    s3_path: str
+
+    always_store_anchor_column: bool
+    """Whether the anchor column should be stored in the Offline Feature Store regardless of whether it is
+    required by the storage layer.
 
-def get_historical_features_for_feature_definition(
-    feature_definition: FeatureDefinitionWrapper,
-    spine: Optional[Union[pyspark_sql.DataFrame, pd.DataFrame, TectonDataFrame]],
-    timestamp_key: Optional[str],
-    start_time: Optional[Union[pendulum.DateTime, datetime]],
-    end_time: Optional[Union[pendulum.DateTime, datetime]],
-    entities: Optional[Union[pyspark_sql.DataFrame, pd.DataFrame, TectonDataFrame]],
-    from_source: bool,
-    save: bool,
-    save_as: Optional[str],
-    mock_data_sources: Dict[str, pyspark_sql.DataFrame],
-) -> TectonDataFrame:
-    if not feature_definition.is_on_demand:
-        check_spark_version(feature_definition.fv_spec.batch_cluster_config)
-
-    if spine is not None:
-        if _should_infer_timestamp_of_spine(feature_definition, timestamp_key):
-            timestamp_key = utils.infer_timestamp(spine)
-        if isinstance(spine, pd.DataFrame):
-            fd_schema = feature_definition.spine_schema
-            if timestamp_key is not None:
-                fd_schema += schema.Schema.from_dict({timestamp_key: data_types.TimestampType()})
-            spine = TectonDataFrame._create_from_pandas_with_schema(spine, schema=fd_schema)
-        elif not isinstance(spine, TectonDataFrame):
-            spine = TectonDataFrame._create(spine)
-        qt = _point_in_time_get_historical_features_for_feature_definition(
-            feature_definition, spine, timestamp_key, from_source
-        )
-    else:
-        if entities is not None:
-            if not isinstance(entities, TectonDataFrame):
-                entities = TectonDataFrame._create(entities)
-            assert set(entities._dataframe.columns).issubset(
-                set(feature_definition.join_keys)
-            ), f"Entities should only contain columns that can be used as Join Keys: {feature_definition.join_keys}"
-
-        qt = _time_range_get_historical_features_for_feature_definition(
-            feature_definition,
-            start_time=start_time,
-            end_time=end_time,
-            entities=entities,
-            from_source=from_source,
-        )
-
-    rewrite.MockDataRewrite(mock_data_sources).rewrite(qt)
+    If this is false the anchor column will be dropped from the stored data if it's not needed by the
+    OfflineStoreWriter implementation.
+    """
 
-    df = TectonDataFrame._create(qt)
+    time_column: str
+    """The column containing the timestamp value used for time-based partitioning"""
 
-    if save or save_as is not None:
-        return Dataset._create(
-            df=df,
-            save_as=save_as,
-            workspace=feature_definition.workspace,
-            feature_definition_id=feature_definition.id,
-            spine=spine,
-            timestamp_key=timestamp_key,
-        )
-    return df
+    join_key_columns: List[str]
 
-
-def _should_infer_timestamp_of_spine(
-    feature_definition: FeatureDefinitionWrapper,
-    timestamp_key: Optional[str],
-):
-    if feature_definition.is_on_demand:
-        # If the ODFV does not depend on any materialized feature definitions, then there is no need to infer a
-        # timestamp key.
-        return (
-            timestamp_key is None
-            and utils.get_num_dependent_fv(feature_definition.pipeline.root, visited_inputs={}) > 0
-        )
-    else:
-        return timestamp_key is None
+    is_continuous: bool
 
 
-def _point_in_time_get_historical_features_for_feature_definition(
-    feature_definition: FeatureDefinitionWrapper,
-    spine: TectonDataFrame,
-    timestamp_key: Optional[str],
-    from_source: bool,
-) -> node_interface.NodeRef:
-    if feature_definition.is_on_demand:
-        utils.validate_spine_dataframe(spine, timestamp_key, feature_definition.request_context_keys)
-    else:
-        utils.validate_spine_dataframe(spine, timestamp_key)
-
-    dac = FeatureDefinitionAndJoinConfig.from_feature_definition(feature_definition)
-    user_data_node_metadata = {}
-    if timestamp_key:
-        user_data_node_metadata["timestamp_key"] = timestamp_key
-
-    qt = builder.build_spine_join_querytree(
-        dac,
-        nodes.UserSpecifiedDataNode(spine, user_data_node_metadata).as_ref(),
-        timestamp_key,
-        from_source,
-    )
+def get_offline_store_writer(
+    params: OfflineStoreWriterParams, fd: FeatureDefinition, version: int, spark: SparkSession
+) -> "OfflineStoreWriter":
+    """Creates a concrete implementation of OfflineStoreWriter based on fv_config."""
+    fv_config = fd.offline_store_config
+    case = fv_config.WhichOneof("store_type")
+    if case == "delta":
+        return DeltaWriter(fd, params, spark, version)
+    elif case == "parquet":
+        return ParquetWriter(fd, params, spark, version)
+    # Remove default after database migration is complete.
+    # raise KeyError(case)
+    return ParquetWriter(fd, params, spark, version)
+
+
+def get_offline_store_reader(
+    spark: SparkSession, fd: FeatureDefinition, path: Optional[str] = None
+) -> "OfflineStoreReader":
+    case = fd.offline_store_config.WhichOneof("store_type")
+    if case == "delta":
+        return DeltaReader(spark, fd, path=path)
+    elif case == "parquet":
+        return ParquetReader(spark, fd, path=path)
+    # Remove default after database migration is complete.
+    # raise KeyError(case)
+    return ParquetReader(spark, fd, path=path)
+
+
+class OfflineStoreWriter(ABC):
+    """Interface for Offline Feature Store writers."""
+
+    @abstractmethod
+    def append_dataframe(self, data_frame: DataFrame) -> None:
+        """Append the rows from data_frame to the Store table. Nothing is overwritten."""
+        raise NotImplementedError
+
+    @abstractmethod
+    def upsert_dataframe(self, data_frame: DataFrame) -> None:
+        """Upsert the rows from data_frame to the Store table.
+
+        Rows with matching join keys and time column are overwritten. Other rows are inserted.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def delete_keys(self, data_frame: DataFrame) -> int:
+        """Delete rows from the Store table that match the keys inside the data_frame.
+
+        Return number of successfully deleted keys."""
+        raise NotImplementedError
+
+
+class OfflineStoreReader(ABC):
+    @abstractmethod
+    def read(self, partition_time_limits: pendulum.Period) -> DataFrame:
+        """Note that partition_time_limits only applies partition filtering, so you can have records outside it"""
+        raise NotImplementedError
+
+
+class ParquetWriter(OfflineStoreWriter):
+    """Parquet implementation of OfflineStoreWriter"""
+
+    def __init__(
+        self, fd: FeatureDefinition, params: OfflineStoreWriterParams, spark: SparkSession, version: int
+    ) -> None:
+        _check_supported_offline_store_version(fd)
+        self._fd = fd
+        self._params = params
+        self._spark = spark
+        self._version = version
+        self._partition_size = partition_size_for_parquet(fd).as_timedelta()
+        self._partition_col = partition_col_for_parquet(fd)
+
+    def append_dataframe(self, data_frame: DataFrame) -> None:
+        if self._partition_col == TIME_PARTITION:
+            align_duration = core_time_utils.convert_timedelta_for_version(self._partition_size, self._version)
+            aligned_time = _align_timestamp(functions.col(ANCHOR_TIME), functions.lit(align_duration))
+            data_frame = data_frame.withColumn(TIME_PARTITION, aligned_time)
+
+        data_frame.write.option("partitionOverwriteMode", "dynamic").partitionBy(self._partition_col).parquet(
+            self._params.s3_path, mode="overwrite"
+        )
+
+    def upsert_dataframe(self, data_frame: DataFrame) -> None:
+        raise NotImplementedError()
+
+    def delete_keys(self, data_frame: DataFrame) -> int:
+        raise NotImplementedError()
+
+
+class ParquetReader(OfflineStoreReader):
+    def __init__(self, spark: SparkSession, fd: FeatureDefinition, path: Optional[str]) -> None:
+        _check_supported_offline_store_version(fd)
+        self._spark = spark
+        assert fd.materialization_enabled and fd.writes_to_offline_store
+        self._path = path or fd.materialized_data_path
+        self._partition_col = partition_col_for_parquet(fd)
+        self._partition_size = partition_size_for_parquet(fd).as_timedelta()
+        self.version = fd.get_feature_store_format_version
+
+    def read(self, partition_time_limits: Optional[pendulum.Period]) -> DataFrame:
+        spark_df = self._spark.read.parquet(self._path)
+
+        # Parquet is partitioned by TIME_PARTITION when is_continuous and ANCHOR_TIME when not.
+        # We want to explicitly cast the partition type in case:
+        #   `spark.sql.sources.partitionColumnTypeInference.enabled` = "false"
+
+        spark_df = spark_df.withColumn(self._partition_col, functions.col(self._partition_col).cast("long"))
+
+        if partition_time_limits and self._partition_size:
+            aligned_start_time = core_time_utils.align_time_downwards(partition_time_limits.start, self._partition_size)
+            aligned_end_time = core_time_utils.align_time_downwards(partition_time_limits.end, self._partition_size)
+            start_time_epoch = core_time_utils.convert_timestamp_for_version(aligned_start_time, self.version)
+            end_time_epoch = core_time_utils.convert_timestamp_for_version(aligned_end_time, self.version)
+            partition_col = functions.col(self._partition_col)
+            spark_df = spark_df.where((start_time_epoch <= partition_col) & (partition_col <= end_time_epoch))
+
+        return spark_df.drop(TIME_PARTITION)
+
+
+_EXCEPTION_PACKAGES = {
+    "com.databricks.sql.transaction.tahoe",  # Used by Databricks
+    "org.apache.spark.sql.delta",  # Used by open source
+}
+
+_EXCEPTION_CLASSES = {
+    "ConcurrentAppendException",
+    "ConcurrentDeleteReadException",
+    "ConcurrentDeleteDeleteException",
+    "ProtocolChangedException",  # This can occur when two txns create the same table concurrently
+}
+
+_RETRYABLE_DELTA_EXCEPTIONS = {
+    f"{pkg}.{cls}" for pkg, cls in itertools.product(_EXCEPTION_PACKAGES, _EXCEPTION_CLASSES)
+}
+
+
+def _with_delta_retries(f, max_retries=5):
+    """Retries the wrapped function upon Deltalake conflict errors."""
+
+    @functools.wraps(f)
+    def wrapper(*args, **kwargs):
+        from delta.exceptions import ConcurrentAppendException
+        from delta.exceptions import ConcurrentDeleteDeleteException
+        from delta.exceptions import ConcurrentDeleteReadException
+        from delta.exceptions import ConcurrentTransactionException
+        from delta.exceptions import DeltaConcurrentModificationException
+        from delta.exceptions import MetadataChangedException
+        from delta.exceptions import ProtocolChangedException
+
+        final_exception = None
+        for i in range(max_retries):
+            try:
+                if i > 0:
+                    # Add a random delay (with exponential backoff) before the retries to decrease
+                    # the chance of recurrent conflicts between the parallel offline store writers.
+                    # Possible 10s of seconds of delay is insignificant to the overall job's latency.
+                    exponential_coef = 2 ** (i - 1)
+                    retry_delay = exponential_coef * random.uniform(0, 1)
+                    time.sleep(retry_delay)
+                f(*args, **kwargs)
+                return
+            except Py4JJavaError as e:
+                exception_class = e.java_exception.getClass().getCanonicalName()
+                if exception_class not in _RETRYABLE_DELTA_EXCEPTIONS:
+                    raise e
+                final_exception = e
+                logger.info(
+                    f"Delta transaction failed (attempt {i + 1}/5); retrying",
+                    exc_info=True,  # Include information about the exception currently being handled
+                )
+            except (
+                ConcurrentAppendException,
+                ConcurrentDeleteDeleteException,
+                ConcurrentDeleteReadException,
+                ConcurrentTransactionException,
+                DeltaConcurrentModificationException,
+                MetadataChangedException,
+                ProtocolChangedException,
+            ) as e:
+                final_exception = e
+                logger.info(
+                    f"Delta transaction failed (attempt {i + 1}/5); retrying",
+                    exc_info=True,  # Include information about the exception currently being handled
+                )
+            except Exception:
+                logger.warning("Uncaught exception raised during Delta write", exc_info=True)
+                raise
+        msg = f"Exceeded maximum Delta transaction retries ({max_retries})"
+        raise Exception(msg) from final_exception
+
+    return wrapper
 
-    return qt
 
+def _assert_safe_delta_write_configuration(spark: SparkSession) -> bool:
+    """Asserts that the Spark configuration is such that it is safe to write to Delta concurrently.
 
-def _most_recent_tile_end_time(fd: FeatureDefinitionWrapper, timestamp: datetime) -> int:
-    """Computes the most recent tile end time which is ready to be computed.
+    With the Open Source Delta JAR installed (as it is on EMR), writing to a Delta table concurrently with another
+    Spark cluster could corrupt the table unless the Delta Logstore class is overridden.
 
-    :param timestamp: The timestamp in python datetime format
-    :return: The timestamp in seconds of the greatest ready tile end time <= timestamp.
+    On Databricks everything is fine as multi-cluster writes are enabled (the default).
     """
-    # Account for data delay
-    timestamp = timestamp - fd.max_source_data_delay
-    if fd.min_scheduling_interval:
-        timestamp = align_time_downwards(timestamp, fd.min_scheduling_interval)
-    return convert_timestamp_to_epoch(timestamp, fd.get_feature_store_format_version)
-
-
-def _time_range_get_historical_features_for_feature_definition(
-    fd: FeatureDefinitionWrapper,
-    entities: TectonDataFrame,
-    start_time: Optional[Union[pendulum.DateTime, datetime]],
-    end_time: Optional[Union[pendulum.DateTime, datetime]],
-    from_source: bool,
-) -> node_interface.NodeRef:
-    if start_time is not None and isinstance(start_time, datetime):
-        start_time = pendulum.instance(start_time)
-    if end_time is not None and isinstance(end_time, datetime):
-        end_time = pendulum.instance(end_time)
-
-    if start_time is not None and fd.feature_start_timestamp is not None and start_time < fd.feature_start_timestamp:
-        logger.warning(
-            f'The provided start_time ({start_time}) is before "{fd.name}"\'s feature_start_time ({fd.feature_start_timestamp}). No feature values will be returned before the feature_start_time.'
-        )
-        start_time = fd.feature_start_timestamp
 
-    # TODO(brian): construct the timestamps a bit more directly. This code in
-    # general reuses utilities not really meant for the semantics of this API.
-    if fd.is_temporal_aggregate or fd.is_temporal:
-        # Feature views where materialization is not enabled may not have a feature_start_time.
-        _start = start_time or fd.feature_start_timestamp or pendulum.datetime(1970, 1, 1)
-        # we need to add 1 to most_recent_anchor since we filter end_time exclusively
-        if end_time:
-            _end = end_time
-        else:
-            anchor_time = _most_recent_tile_end_time(fd, pendulum.now("UTC") - fd.min_scheduling_interval)
-            _end = convert_epoch_to_datetime(anchor_time, fd.get_feature_store_format_version) + pendulum.duration(
-                microseconds=1
+    configs = {
+        DBRICKS_RUNTIME_VERSION: os.environ.get(DBRICKS_RUNTIME_VERSION, None),
+        DBRICKS_MULTI_CLUSTER_WRITES_ENABLED: spark.conf.get(DBRICKS_MULTI_CLUSTER_WRITES_ENABLED, None),
+        SPARK31_DELTA_LOGSTORE_CLASS: spark.conf.get(SPARK31_DELTA_LOGSTORE_CLASS, None),
+        SPARK32_OR_HIGHER_DELTA_LOGSTORE_CLASS: spark.conf.get(SPARK32_OR_HIGHER_DELTA_LOGSTORE_CLASS, None),
+    }
+    if configs[DBRICKS_RUNTIME_VERSION] and configs[DBRICKS_MULTI_CLUSTER_WRITES_ENABLED] == "true":
+        return True
+
+    # either the spark 3.1 or spark 3.2+ DELTA_LOGSTORE_CLASS name can be set
+    if configs[SPARK31_DELTA_LOGSTORE_CLASS] in [SPARK31_DYNAMODB_LOGSTORE_CLASS, SPARK_GCS_DELTA_LOGSTORE_CLASS]:
+        return True
+    if configs[SPARK32_OR_HIGHER_DELTA_LOGSTORE_CLASS] in [
+        SPARK32_OR_HIGHER_DYNAMODB_LOGSTORE_CLASS,
+        SPARK_GCS_DELTA_LOGSTORE_CLASS,
+    ]:
+        return True
+    msg = f"Configuration is not safe for concurrent writes: {configs}"
+    raise AssertionError(msg)
+
+
+class DeltaWriter(OfflineStoreWriter):
+    """DeltaLake implementation of OfflineStoreWriter"""
+
+    def __init__(
+        self, fd: FeatureDefinition, params: OfflineStoreWriterParams, spark: SparkSession, version: int
+    ) -> None:
+        _check_supported_offline_store_version(fd)
+        self._params = params
+        self._version = version
+        self._spark = spark
+        self._partition_size = partition_size_for_delta(fd).as_timedelta()
+        self._metadata_writer = DeltaMetadataWriter(spark)
+        if not spark.conf.get("spark.databricks.delta.commitInfo.userMetadata"):
+            msg = "Expected spark.databricks.delta.commitInfo.userMetadata to be set for delta writes"
+            raise AssertionError(msg)
+
+    def append_dataframe(self, data_frame: DataFrame) -> None:
+        data_frame = self._add_partition(data_frame)
+        self._ensure_table_exists(self._spark, data_frame.schema)
+        self._append_dataframe(data_frame)
+
+    def upsert_dataframe(self, data_frame):
+        # See https://github.com/delta-io/delta/issues/282 for why this isn't at the top of the file
+        from delta.tables import DeltaTable
+
+        _assert_safe_delta_write_configuration(self._spark)
+
+        data_frame = self._add_partition(data_frame)
+        self._ensure_table_exists(self._spark, data_frame.schema)
+
+        table = DeltaTable.forPath(self._spark, self._params.s3_path)
+
+        base = table.toDF().alias("base")
+        updates = data_frame.alias("updates")
+
+        # Build a condition which matches on all join keys, the timestamp, and the time partition column. The time
+        # partition column is not needed for correctness, but it allows some files to be skipped by Delta.
+        all_match_keys = [self._params.time_column, TIME_PARTITION, *self._params.join_key_columns]
+        key_matches = [base[k] == updates[k] for k in all_match_keys]
+        match_condition = functools.reduce(lambda l, r: l & r, key_matches)
+
+        @_with_delta_retries
+        def _execute():
+            table.merge(updates, match_condition).whenMatchedUpdateAll().whenNotMatchedInsertAll().execute()
+
+        _execute()
+
+    def delete_keys(self, data_frame: DataFrame) -> int:
+        # See https://github.com/delta-io/delta/issues/282 for why this isn't at the top of the file
+        from delta.tables import DeltaTable
+
+        _assert_safe_delta_write_configuration(self._spark)
+
+        deltaTable = DeltaTable.forPath(self._spark, self._params.s3_path)
+        query = ""
+        columns = data_frame.columns
+        for column in columns:
+            if query:
+                query = query + " AND "
+            query = query + "t." + column + " = k." + column
+
+        @_with_delta_retries
+        def _execute():
+            deltaTable.alias("t").merge(data_frame.alias("k"), query).whenMatchedDelete().execute()
+
+        @_with_delta_retries
+        def _vacuum():
+            deltaTable.vacuum()
+
+        _execute()
+        _vacuum()
+
+        last_operation = deltaTable.history(1).collect()
+        if not last_operation:
+            return 0
+
+        return int(last_operation[0].operationMetrics.get("numTargetRowsDeleted", 0))
+
+    def delete_time_range(
+        self,
+        feature_start_time: datetime,
+        feature_end_time: datetime,
+        feature_store_format_version: int,
+    ) -> None:
+        from delta.tables import DeltaTable
+
+        aligned_start_time = core_time_utils.align_time_downwards(feature_start_time, self._partition_size)
+        aligned_end_time = core_time_utils.align_time_downwards(feature_end_time, self._partition_size)
+        start_partition = _datetime_to_partition_str(aligned_start_time, self._partition_size)
+        end_partition = _datetime_to_partition_str(aligned_end_time, self._partition_size)
+        start_time = core_time_utils.convert_timestamp_for_version(feature_start_time, feature_store_format_version)
+        end_time = core_time_utils.convert_timestamp_for_version(feature_end_time, feature_store_format_version)
+
+        assert self._params.always_store_anchor_column
+
+        table = DeltaTable.forPath(self._spark, self._params.s3_path)
+
+        @_with_delta_retries
+        def _execute():
+            table.delete(
+                f'{ANCHOR_TIME} >= {start_time} and {ANCHOR_TIME} < {end_time} and {TIME_PARTITION} >= to_timestamp("{start_partition}") and {TIME_PARTITION} <= to_timestamp("{end_partition}")'
             )
-    else:
-        _start = start_time or pendulum.datetime(1970, 1, 1)
-        _end = end_time or pendulum.now("UTC")
-
-    if _start >= _end:
-        # TODO(felix): Move this and other instances of validating user inputs to top-level get_historical_features() methods.
-        raise core_errors.START_TIME_NOT_BEFORE_END_TIME(_start, _end)
-    time_range = pendulum.Period(_start, _end)
-
-    effective_timestamp_field = sql_compat.default_case(query_consts.EFFECTIVE_TIMESTAMP)
-
-    # TODO(felix): Move this logic to `builder.py` once it does not rely on Spark-specific time util functions.
-    if fd.is_temporal or fd.is_feature_table:
-        qt = builder.build_get_features(fd, from_source=from_source, feature_data_time_limits=time_range)
-        qt = nodes.RenameColsNode(qt, drop=[sql_compat.default_case(query_consts.ANCHOR_TIME)]).as_ref()
-        batch_schedule_seconds = 0 if fd.is_feature_table else fd.batch_materialization_schedule.in_seconds()
-
-        qt = nodes.AddEffectiveTimestampNode(
-            qt,
-            timestamp_field=fd.timestamp_key,
-            effective_timestamp_name=effective_timestamp_field,
-            batch_schedule_seconds=batch_schedule_seconds,
-            data_delay_seconds=fd.online_store_data_delay_seconds,
-            is_stream=fd.is_stream,
-            is_temporal_aggregate=False,
-        ).as_ref()
-    else:
-        feature_data_time_limits = time_utils.get_feature_data_time_limits(
-            fd=fd,
-            spine_time_limits=time_range,
-        )
-        # TODO(brian): refactor to share more with run api full aggregation
-        qt = builder.build_get_full_agg_features(
-            fd,
-            from_source=from_source,
-            feature_data_time_limits=feature_data_time_limits,
-            show_effective_time=True,
-        )
-
-    # Validate that entities only contains Join Key Columns.
-    if entities is not None:
-        columns = list(entities.columns)
-        entities_df = nodes.SelectDistinctNode(nodes.UserSpecifiedDataNode(entities).as_ref(), columns).as_ref()
-        qt = nodes.JoinNode(qt, entities_df, columns, how="right").as_ref()
-
-    qt = nodes.FeatureTimeFilterNode(
-        qt,
-        feature_data_time_limits=time_range,
-        policy=feature_view__data_pb2.MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE,
-        timestamp_field=fd.timestamp_key,
-    ).as_ref()
-
-    return qt
-
-
-def get_dataframe_for_data_source(
-    data_source: specs.DataSourceSpec,
-    start_time: datetime,
-    end_time: datetime,
-    apply_translator: bool,
-) -> TectonDataFrame:
-    spark = TectonContext.get_instance()._spark
-    if isinstance(data_source.batch_source, specs.SparkBatchSourceSpec):
-        if not data_source.batch_source.supports_time_filtering and (start_time or end_time):
-            raise errors.DS_INCORRECT_SUPPORTS_TIME_FILTERING
-
-        node = builder.build_datasource_scan_node(
-            data_source, for_stream=False, start_time=start_time, end_time=end_time
-        )
-        return TectonDataFrame._create(node)
 
-    elif apply_translator:
-        timestamp_key = data_source.batch_source.timestamp_field
-        if not timestamp_key and (start_time or end_time):
-            raise errors.DS_DATAFRAME_NO_TIMESTAMP
+        _execute()
 
-        node = builder.build_datasource_scan_node(
-            data_source, for_stream=False, start_time=start_time, end_time=end_time
-        )
-        return TectonDataFrame._create(node)
-    else:
-        if start_time is not None or end_time is not None:
-            raise errors.DS_RAW_DATAFRAME_NO_TIMESTAMP_FILTER
-
-        node = nodes.RawDataSourceScanNode(data_source).as_ref()
-        return TectonDataFrame._create(node)
-
-
-def start_stream_preview(
-    data_source: specs.DataSourceSpec,
-    table_name: str,
-    apply_translator: bool,
-    option_overrides: Optional[Dict[str, str]],
-) -> pyspark_streaming.StreamingQuery:
-    df = get_stream_preview_dataframe(data_source, apply_translator, option_overrides)
-
-    # Set a tempdir checkpointLocation. This is needed for the stream preview to work in EMR notebooks. The
-    # TemporaryDirectory object handles cleaning up the temporary directory when it is destroyed, so add the object to
-    # a global list that will be cleaned up with the program exits. (This isn't guaranteed - but it's not the end of
-    # the world if we leak some temporary directories.)
-    d = tempfile.TemporaryDirectory()
-    _CHECKPOINT_DIRECTORIES.append(d)
-
-    return (
-        df.writeStream.format("memory")
-        .queryName(table_name)
-        .option("checkpointLocation", d.name)
-        .outputMode("append")
-        .start()
-    )
-
-
-def get_stream_preview_dataframe(
-    data_source: specs.DataSourceSpec, apply_translator: bool, option_overrides: Optional[Dict[str, str]]
-) -> pyspark_sql.DataFrame:
-    """
-    Helper function that allows start_stream_preview() to be unit tested, since we can't easily unit test writing
-    to temporary tables.
-    """
-    spark = tecton_context.TectonContext.get_instance()._spark
+    def _add_partition(self, data_frame: DataFrame) -> DataFrame:
+        """Adds the time_partition column and drops the _anchor_time column if needed."""
+        partition = _timestamp_to_partition_column(
+            data_frame, self._params.time_column, self._partition_size, self._version
+        )
+        data_frame = data_frame.withColumn(TIME_PARTITION, partition)
+        if not self._params.always_store_anchor_column:
+            data_frame = data_frame.drop(ANCHOR_TIME)
+        return data_frame
+
+    def _ensure_table_exists(self, spark: SparkSession, schema: StructType) -> None:
+        """Ensures that the table exists with the given schema.
+
+        Some operations (including merge) fail when the table doesn't already exist. Others (append) can have conflicts
+        where they wouldn't normally when they also create a new table. This function ensures neither will happen.
+        """
+        df = spark.createDataFrame([], schema)  # DF with 0 rows
+        self._append_dataframe(df)
+
+        # Manifest files are not supported on GCS
+        if not self._params.s3_path.startswith("gs://"):
+            # we set auto manifest so each job generates its own manifest (necessary for athena retrieval)
+            self._metadata_writer.set_table_property(
+                self._params.s3_path, "delta.compatibility.symlinkFormatManifest.enabled", "true"
+            )
 
-    if apply_translator or isinstance(data_source.stream_source, specs.SparkStreamSourceSpec):
-        return data_source_helper.get_ds_dataframe(
-            spark, data_source, consume_streaming_data_source=True, stream_option_overrides=option_overrides
-        )
-    else:
-        return data_source_helper.get_non_dsf_raw_stream_dataframe(spark, data_source.stream_source, option_overrides)
+    @_with_delta_retries
+    def _append_dataframe(self, df: DataFrame) -> None:
+        _assert_safe_delta_write_configuration(self._spark)
+        df.write.partitionBy(TIME_PARTITION).format("delta").mode("append").save(self._params.s3_path)
+
+
+class DeltaMetadataWriter:
+    def __init__(self, spark: SparkSession) -> None:
+        self._spark = spark
+
+    @_with_delta_retries
+    def generate_symlink_manifest(self, path: str) -> None:
+        _assert_safe_delta_write_configuration(self._spark)
+        # we need spark_catalog in cases where the data source switches catalogs
+        self._spark.sql(f"GENERATE symlink_format_manifest FOR TABLE spark_catalog.delta.`{path}`")
+
+    @_with_delta_retries
+    def set_table_property(self, path, key, val):
+        _assert_safe_delta_write_configuration(self._spark)
+        # we need spark_catalog in cases where the data source switches catalogs
+        existing_tbl_properties = self._spark.sql(f"show tblproperties spark_catalog.delta.`{path}`").collect()
+        # tblproperties are case sensitive
+        has_tbl_property = any(key == r.key and val == r.value for r in existing_tbl_properties)
+        # we only set it if not already set to avoid delta conflicts
+        if not has_tbl_property:
+            self._spark.sql(f"ALTER TABLE spark_catalog.delta.`{path}` SET TBLPROPERTIES({key}={val})")
+
+    @_with_delta_retries
+    def optimize_execute_compaction(self, path):
+        _assert_safe_delta_write_configuration(self._spark)
+        self._spark.sql(f"OPTIMIZE '{path}'")
+
+
+class DeltaReader(OfflineStoreReader):
+    def __init__(self, spark: SparkSession, fd: FeatureDefinition, path: Optional[str]) -> None:
+        _check_supported_offline_store_version(fd)
+        self._spark = spark
+        assert fd.materialization_enabled and fd.writes_to_offline_store
+        self._path = path or fd.materialized_data_path
+        self._partition_size = partition_size_for_delta(fd).as_timedelta()
+
+    def read(self, partition_time_limits: Optional[pendulum.Period]) -> DataFrame:
+        spark_df = self._spark.read.format("delta").load(self._path)
+
+        # Whenever the partition filtering logic is changed, also make sure the changes are applied to the sql based
+        # version in query/nodes.py
+
+        # Delta is always partitioned by TIME_PARTITION. We want to explicitly cast to a timestamp in case:
+        #   `spark.sql.sources.partitionColumnTypeInference.enabled` = "false"
+        spark_df = spark_df.withColumn(TIME_PARTITION, functions.col(TIME_PARTITION).cast("timestamp"))
+
+        if partition_time_limits is not None and self._partition_size:
+            aligned_start_time = core_time_utils.align_time_downwards(partition_time_limits.start, self._partition_size)
+            aligned_end_time = core_time_utils.align_time_downwards(partition_time_limits.end, self._partition_size)
+            start_partition = _datetime_to_partition_str(aligned_start_time, self._partition_size)
+            end_partition = _datetime_to_partition_str(aligned_end_time, self._partition_size)
+            partition_col = functions.col(TIME_PARTITION)
+            spark_df = spark_df.where((start_partition <= partition_col) & (partition_col <= end_partition))
+
+        return spark_df.drop(TIME_PARTITION)
+
+
+def _timestamp_to_partition_column(df: DataFrame, time_col: str, partition_size: timedelta, version: int) -> Column:
+    # For some insane reason from_unixtime returns a timestamp in the session timezone, so it's pretty annoying to
+    # convert a unix time to a formatted UTC timestamp unless the session is set to UTC. This only runs in
+    # materialization so we can just assert that that's the case.
+    tz = df.sql_ctx.sparkSession.conf.get("spark.sql.session.timeZone")
+    if tz not in {"UTC", "Etc/UTC", "GMT"}:
+        msg = f"spark.sql.session.timeZone must be UTC, not {tz}"
+        raise AssertionError(msg)
+    time_column_type = df.schema[time_col].dataType
+    allowed_types = {IntegerType(), TimestampType(), LongType()}
+    if time_column_type not in allowed_types:
+        msg = f"timestamp column must be one of {allowed_types}, not {time_column_type}"
+        raise AssertionError(msg)
+    time_val = functions.col(time_col).cast(LongType())
+    if time_col == ANCHOR_TIME:
+        time_val = spark_time_utils.convert_epoch_to_datetime(functions.col(time_col), version).cast(LongType())
+    aligned = functions.from_unixtime(_align_timestamp(time_val, window_size_seconds(partition_size)))
+    partition_format = _timestamp_formats(partition_size).spark_format
+    return functions.date_format(aligned.cast(TimestampType()), partition_format)
+
+
+def _datetime_to_partition_str(dt: datetime, partition_size: timedelta) -> str:
+    partition_format = _timestamp_formats(partition_size).python_format
+    return dt.strftime(partition_format)
 
 
-def derive_view_schema_for_feature_view(
-    fv_args: feature_view_pb2.FeatureViewArgs,
-    transformations: Sequence[specs.TransformationSpec],
-    data_sources: Sequence[specs.DataSourceSpec],
-) -> schema_pb2.Schema:
-    spark = TectonContext.get_instance()._spark
-    return schema_derivation_utils.get_feature_view_view_schema(spark, fv_args, transformations, data_sources)
-
-
-def spark_schema_to_tecton_schema(spark_schema: spark_schema_pb2.SparkSchema) -> schema_pb2.Schema:
-    wrapper = spark_schema_wrapper.SparkSchemaWrapper.from_proto(spark_schema)
-    return schema_spark_utils.schema_from_spark(wrapper.unwrap()).proto
-
-
-def derive_materialization_schema_for_feature_view(
-    view_schema: schema_pb2.Schema,
-    feature_view_args: feature_view_pb2.FeatureViewArgs,
-) -> schema_pb2.Schema:
-    is_aggregate = len(feature_view_args.materialized_feature_view_args.aggregations) > 0
-    if not is_aggregate:
-        return view_schema
-
-    return core_schema_derivation_utils.compute_aggregate_materialization_schema_from_view_schema(
-        view_schema, feature_view_args, is_spark=True
-    )
-
-
-def derive_view_schema_for_feature_table(
-    fv_args: feature_view_pb2.FeatureViewArgs,
-) -> schema_pb2.Schema:
-    output_schema = fv_args.feature_table_args.schema
-    wrapper = spark_schema_wrapper.SparkSchemaWrapper.from_proto(output_schema)
-
-
-def derive_batch_schema(
-    ds_args: virtual_data_source__args_pb2.VirtualDataSourceArgs,
-    batch_post_processor: Optional[Callable],
-    batch_data_source_function: Optional[Callable],
-) -> spark_schema_pb2.SparkSchema:
-    spark = TectonContext.get_instance()._spark
-    return schema_derivation_utils.derive_batch_schema(spark, ds_args, batch_post_processor, batch_data_source_function)
-
-
-def derive_stream_schema(
-    ds_args: virtual_data_source__args_pb2.VirtualDataSourceArgs,
-    stream_post_processor: Optional[Callable],
-    stream_data_source_function: Optional[Callable],
-) -> spark_schema_pb2.SparkSchema:
-    spark = TectonContext.get_instance()._spark
-    return schema_derivation_utils.derive_stream_schema(
-        spark, ds_args, stream_post_processor, stream_data_source_function
-    )
-
-
-_TRANSFORMATION_RUN_TEMP_VIEW_PREFIX = "_tecton_transformation_run_"
-CONST_TYPE = Union[str, int, float, bool]
-
-
-def run_transformation_mode_spark_sql(
-    *inputs: Union[pd.DataFrame, pd.Series, TectonDataFrame, pyspark_sql.DataFrame, CONST_TYPE],
-    transformer: Callable,
-    context: materialization_context.BaseMaterializationContext = None,
-    transformation_name: str,
-) -> TectonDataFrame:
-    def create_temp_view(df, dataframe_index) -> str:
-        df = TectonDataFrame._create(df).to_spark()
-        temp_view = f"{_TRANSFORMATION_RUN_TEMP_VIEW_PREFIX}{transformation_name}_input_{dataframe_index}"
-        df.createOrReplaceTempView(temp_view)
-        return temp_view
-
-    args = [create_temp_view(v, i) if not isinstance(v, CONST_TYPE.__args__) else v for i, v in enumerate(inputs)]
-    if context is not None:
-        args.append(context)
-
-    spark = TectonContext.get_instance()._get_spark()
-    return TectonDataFrame._create(spark.sql(transformer(*args)))
-
-
-def run_transformation_mode_pyspark(
-    *inputs: Union[pd.DataFrame, pd.Series, TectonDataFrame, pyspark_sql.DataFrame, CONST_TYPE],
-    transformer: Callable,
-    context: materialization_context.BaseMaterializationContext,
-) -> TectonDataFrame:
-    args = [TectonDataFrame._create(v).to_spark() if not isinstance(v, CONST_TYPE.__args__) else v for v in inputs]
-    if context is not None:
-        args.append(context)
-
-    return TectonDataFrame._create(transformer(*args))
-
-
-def write_dataframe_to_path_or_url(
-    df: Union[pyspark_sql.DataFrame, pd.DataFrame], df_path: str, upload_url: str, view_schema: schema.Schema
-):
-    """Used for Feature Table ingest and deleting keys."""
-    # We write in the native format and avoid converting Pandas <-> Spark due to partially incompatible
-    # type system, in specifically missing Int in Pandas
-    if isinstance(df, pyspark_sql.DataFrame):
-        df.write.parquet(df_path)
-        return
-
-    if upload_url:
-        ingest_utils.upload_df_pandas(upload_url, df)
-    elif df_path:
-        spark_df = ingest_utils.convert_pandas_to_spark_df(df, view_schema)
-        spark_df.write.parquet(df_path)
-
-
-def get_request_schema_from_tecton_schema(tecton_schema: schema_pb2.Schema) -> List[sdk_types.Field]:
-    """Convert TectonSchema into a list of Tecton Fields."""
-    columns_and_types = schema.Schema(tecton_schema).column_name_and_data_types()
-    request_schema = []
-    for c_and_t in columns_and_types:
-        name = c_and_t[0]
-        data_type = type_utils.sdk_type_from_tecton_type(c_and_t[1])
-        request_schema.append(sdk_types.Field(name, data_type))
-    return request_schema
+def _align_timestamp(int_timestamp_col, window_size):
+    return int_timestamp_col - (int_timestamp_col % window_size)
```

### Comparing `tecton-0.8.0b4/tecton/_internals/spark_utils.py` & `tecton-0.8.0b5/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/time_utils.py` & `tecton-0.8.0b5/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/type_utils.py` & `tecton-0.8.0b5/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/_internals/utils.py` & `tecton-0.8.0b5/tecton/_internals/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     if len(join_keys) > len(set(join_keys)):
         msg = "join_keys"
         raise errors.DUPLICATED_ELEMENTS_IN_ARGUMENT(msg)
 
 
 def validate_spine_dataframe(
-    spine: DataframeWrapper, timestamp_key: Optional[str], request_context_keys: List[str] = None
+    spine: DataframeWrapper, timestamp_key: Optional[str], request_context_keys: Optional[List[str]] = None
 ):
     spine_df = spine._dataframe
     if timestamp_key:
         if timestamp_key not in spine_df.columns:
             msg = "timestamp_key"
             raise errors.MISSING_SPINE_COLUMN(msg, timestamp_key, spine_df.columns)
         if isinstance(spine_df, pysparkDF):
```

### Comparing `tecton-0.8.0b4/tecton/_internals/validations_api.py` & `tecton-0.8.0b5/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/aggregation_functions.py` & `tecton-0.8.0b5/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/access_control.py` & `tecton-0.8.0b5/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/api_key.py` & `tecton-0.8.0b5/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/cli.py` & `tecton-0.8.0b5/tecton/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,29 +504,29 @@
     VIRTUAL_ENV = os.getenv("VIRTUAL_ENV")
     if VIRTUAL_ENV:
         return list(filter(lambda f: not f.startswith(VIRTUAL_ENV), candidate_test_files))
 
     return list(candidate_test_files)
 
 
-def run_tests(debug: bool, pytest_extra_args: Tuple[str, ...] = tuple()):
+def run_tests(debug: bool, pytest_extra_args: Tuple[str, ...] = ()):
     repo_root = repo_file_handler._maybe_get_repo_root()
     if repo_root is None:
         printer.safe_print("Tecton tests must be run from a feature repo initialized using 'tecton init'!")
         sys.exit(1)
 
     prepare_args(debug)
 
     tests = get_test_paths(repo_root)
     if len(tests) == 0:
         printer.safe_print("⚠️  Running Tests: No tests found.")
         return
 
     os.chdir(repo_root)
-    args = ["--disable-pytest-warnings", "-s"] + tests
+    args = ["--disable-pytest-warnings", "-s", *tests]
 
     if pytest_extra_args:
         args.extend(pytest_extra_args)
 
     printer.safe_print("🏃 Running Tests")
     exitcode = pytest.main(args)
 
@@ -627,15 +627,15 @@
     repo_root = repo_file_handler._maybe_get_repo_root()
     if repo_root not in [Path().resolve(), None]:
         printer.safe_print(".tecton already exists in a parent directory:", repo_root)
         sys.exit(1)
 
     child_dir_matches = list(Path().rglob("*/.tecton"))
     if len(child_dir_matches) > 0:
-        dirs_str = "\n\t".join(map(lambda c: str(c.parent.resolve()), child_dir_matches))
+        dirs_str = "\n\t".join((str(c.parent.resolve()) for c in child_dir_matches))
         printer.safe_print(f".tecton already exists in child directories:\n\t{dirs_str}")
         sys.exit(1)
 
     dot_tecton = Path(".tecton")
     if not dot_tecton.exists():
         dot_tecton.touch()
         printer.safe_print("Local feature repository root set to", Path().resolve(), "\n", file=sys.stderr)
@@ -750,15 +750,15 @@
         host = tecton_url
     try:
         urlparse(host)
     except Exception:
         printer.safe_print("Tecton Cluster URL must be a valid URL")
         sys.exit(1)
     # add this check for now since it can be hard to debug if you don't specify https and API_SERVICE fails
-    if host is None or not (host.startswith("https://") or host.startswith("http://localhost:")):
+    if host is None or not (host.startswith(("https://", "http://localhost:"))):
         if host is not None and "//" not in host:
             host = f"https://{host}"
         else:
             printer.safe_print("Tecton Cluster URL must start with https://")
             sys.exit(1)
 
     # get login configs
```

### Comparing `tecton-0.8.0b4/tecton/cli/cli_utils.py` & `tecton-0.8.0b5/tecton/cli/cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def color_diff(lines):
     return map(color_line, lines)
 
 
 def indent_line(lines, indent):
-    return map(lambda x: " " * indent + x, lines)
+    return (" " * indent + x for x in lines)
 
 
 # TODO: Reuse this in other places that does the same (engine.py)
 def pprint_dict(kv, colwidth, indent=0):
     for k, v in kv.items():
         printer.safe_print(indent * " " + f"{k.ljust(colwidth)} {v}")
```

### Comparing `tecton-0.8.0b4/tecton/cli/command.py` & `tecton-0.8.0b5/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/common.py` & `tecton-0.8.0b5/tecton/cli/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # Python 3.7.
     if not (hasattr(site, "getsitepackages") and hasattr(site, "getusersitepackages")):
         logger.warn(
             "Python 'site' pakcage doesn't contain 'getsitepackages' or 'getusersitepackages' methods. SourceInfo is not going to be populated."
         )
         return source_info
 
-    excluded_site_pkgs = site.getsitepackages() + [site.getusersitepackages()]
+    excluded_site_pkgs = [*site.getsitepackages(), site.getusersitepackages()]
 
     frames = inspect.stack()
     repo_root_path = Path(repo_root)
     for frame in frames:
         if SKIP_FRAME_REGEX.match(frame.frame.f_code.co_filename) is not None:
             continue
         frame_path = Path(frame.frame.f_code.co_filename).resolve()
```

### Comparing `tecton-0.8.0b4/tecton/cli/engine.py` & `tecton-0.8.0b5/tecton/cli/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,15 @@
                     )
                 else:
                     printer.safe_print(f"\nUploading feature repo failed with reason: {r.reason}")
                 sys.exit(1)
             return
         except requests.RequestException as e:
             last_error = e
-    else:
-        raise SystemExit(last_error)
+    raise SystemExit(last_error)
 
 
 def _construct_new_plan_request_v1(
     workspace_name: str,
     upgrade_all: bool,
     fco_args: List[FcoArgs],
     repo_source_info: FeatureRepoSourceInfo,
```

### Comparing `tecton-0.8.0b4/tecton/cli/engine_renderer.py` & `tecton-0.8.0b5/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/environment.py` & `tecton-0.8.0b5/tecton/cli/environment.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/error_utils.py` & `tecton-0.8.0b5/tecton/cli/error_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
     pretty_frames: List[PrettyFrameInfo] = []
 
     # Otherwise, get error info from the call stack by finding the frame that contains
     # user-provided Python code.
     # TODO: handle the case when there is more than one frame of user code in the stack trace.
     fail_frame = None
-    user_files_set = set(path.resolve() for path in user_file_paths)
+    user_files_set = {path.resolve() for path in user_file_paths}
 
     for frame in traceback.extract_tb(exception.__traceback__):
         frame_file_path = Path(frame.filename).resolve()
         if frame_file_path in user_files_set:
             # Extract code block around the error location
             code, start_line = extract_code_block(frame_file_path, frame.lineno)
             if code is not None and start_line is not None:
```

### Comparing `tecton-0.8.0b4/tecton/cli/printer.py` & `tecton-0.8.0b5/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/service_account.py` & `tecton-0.8.0b5/tecton/cli/service_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     try:
         request = CreateServiceAccountRequest(name=name, description=description)
         response = metadata_service.instance().CreateServiceAccount(request)
     except TectonAPIValidationError as e:
         printer.safe_print(f"Failed to create service account: {e}", file=sys.stderr)
         sys.exit(1)
     if json_out:
-        service_account = dict()
+        service_account = {}
         service_account["api_key"] = response.api_key
         service_account["id"] = response.id
         printer.safe_print(json.dumps(service_account, indent=4))
     else:
         printer.safe_print("Save this API Key - you will not be able to get it again.")
         printer.safe_print(f"API Key:            {response.api_key}")
         printer.safe_print(f"Service Account ID: {response.id}")
@@ -125,15 +125,15 @@
 
     if len(response.service_accounts) == 0:
         printer.safe_print("No Service Accounts Found")
         return
 
     for k in response.service_accounts:
         if json_out:
-            account = dict()
+            account = {}
             account["name"] = k.name
             account["id"] = k.id
             account["description"] = k.description
             account["active"] = k.is_active
             service_accounts.append(account)
         else:
             printer.safe_print(f"{'Name: ': <15}{k.name}")
```

### Comparing `tecton-0.8.0b4/tecton/cli/user.py` & `tecton-0.8.0b5/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/workspace.py` & `tecton-0.8.0b5/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/cli/workspace_utils.py` & `tecton-0.8.0b5/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/fco_listers.py` & `tecton-0.8.0b5/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/base_tecton_object.py` & `tecton-0.8.0b5/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/compute_mode.py` & `tecton-0.8.0b5/tecton/framework/compute_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from tecton_core import conf
 
 
 class ComputeMode(str, Enum):
     SPARK = "spark"
     SNOWFLAKE = "snowflake"
     ATHENA = "athena"
+    DUCK_DB = "duckdb"
 
 
 def get_compute_mode() -> ComputeMode:
     """Returns the compute mode that Tecton is running in."""
 
     compute_mode = conf.get_or_raise("TECTON_COMPUTE_MODE")
-    if conf.get_bool("ALPHA_SNOWFLAKE_COMPUTE_ENABLED") or compute_mode == ComputeMode.SNOWFLAKE:
+    if compute_mode == ComputeMode.DUCK_DB:
+        return ComputeMode.DUCK_DB
+    elif conf.get_bool("ALPHA_SNOWFLAKE_COMPUTE_ENABLED") or compute_mode == ComputeMode.SNOWFLAKE:
         return ComputeMode.SNOWFLAKE
     elif conf.get_bool("ALPHA_ATHENA_COMPUTE_ENABLED") or compute_mode == ComputeMode.ATHENA:
         return ComputeMode.ATHENA
     elif compute_mode == ComputeMode.SPARK:
         return ComputeMode.SPARK
     else:
         msg = f"Invalid Tecton compute mode: {compute_mode}. Must be one of {[[e.value for e in ComputeMode]]}"
```

### Comparing `tecton-0.8.0b4/tecton/framework/configs.py` & `tecton-0.8.0b5/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/data_source.py` & `tecton-0.8.0b5/tecton/framework/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from tecton._internals import validations_api
 from tecton.framework import base_tecton_object
 from tecton.framework import compute_mode
 from tecton.framework import configs
 from tecton.framework import data_frame
 from tecton_core import id_helper
 from tecton_core import specs
+from tecton_core.query import sql_compat
 from tecton_proto.args import basic_info_pb2
 from tecton_proto.args import fco_args_pb2
 from tecton_proto.args import virtual_data_source_pb2 as virtual_data_source__args_pb2
 from tecton_proto.common import data_source_type_pb2
 from tecton_proto.common import fco_locator_pb2
 from tecton_proto.common import framework_version_pb2
 from tecton_proto.common import schema_container_pb2
@@ -298,15 +299,18 @@
             source_info=None,
             args_supplement=None,
         )
         return obj
 
     def _derive_schemas(self, indentation_level: int) -> None:
         validations_api.print_deriving_schemas(self, indentation_level)
-        if compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE:
+        if (
+            compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE
+            or sql_compat.dialect() == sql_compat.Dialect.SNOWFLAKE
+        ):
             self._args_supplement.batch_schema = snowflake_api.derive_batch_schema(self._args)
         else:
             self._args_supplement.batch_schema = spark_api.derive_batch_schema(
                 self._args, self._args_supplement.batch_post_processor, self._args_supplement.batch_data_source_function
             )
 
     @sdk_decorators.sdk_public_method(requires_validation=True)
@@ -598,15 +602,18 @@
 
     def _derive_schemas(self, indentation_level: int) -> None:
         assert self._args is not None
         if self._args.type == data_source_type_pb2.DataSourceType.PUSH_NO_BATCH:
             return
 
         validations_api.print_deriving_schemas(self, indentation_level)
-        if compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE:
+        if (
+            compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE
+            or sql_compat.dialect() == sql_compat.Dialect.SNOWFLAKE
+        ):
             self._args_supplement.batch_schema = snowflake_api.derive_batch_schema(self._args)
         else:
             self._args_supplement.batch_schema = spark_api.derive_batch_schema(
                 self._args, self._args_supplement.batch_post_processor, self._args_supplement.batch_data_source_function
             )
 
     @sdk_decorators.sdk_public_method(requires_validation=True)
```

### Comparing `tecton-0.8.0b4/tecton/framework/dataset.py` & `tecton-0.8.0b5/tecton/framework/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if self._pandas_df is not None:
             return self._pandas_df
 
         self._try_fetch_spark_df()
         return super().to_pandas()
 
     @sdk_public_method
-    def fetch_as_pandas(self, n_samples: int = None, **kwargs) -> pd.DataFrame:
+    def fetch_as_pandas(self, n_samples: Optional[int] = None, **kwargs) -> pd.DataFrame:
         """
         Fetches a saved dataset from S3 as a pandas DataFrame.
 
         :param n_samples: Number of samples to read from parquet files. If None, read all.
         :param kwargs: Additional arguments to pass to pd.read_parquet function.
         :return: pandas DataFrame containing the saved dataset
         """
```

### Comparing `tecton-0.8.0b4/tecton/framework/entity.py` & `tecton-0.8.0b5/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/feature_service.py` & `tecton-0.8.0b5/tecton/framework/feature_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from typeguard import typechecked
 
 from tecton._internals import athena_api
 from tecton._internals import display
 from tecton._internals import errors
 from tecton._internals import metadata_service
 from tecton._internals import query_helper
+from tecton._internals import querytree_api
 from tecton._internals import sdk_decorators
 from tecton._internals import snowflake_api
-from tecton._internals import spark_api
 from tecton._internals import utils as internal_utils
 from tecton._internals import validations_api
 from tecton.framework import base_tecton_object
 from tecton.framework import compute_mode
 from tecton.framework import configs
 from tecton.framework import data_frame as tecton_dataframe
 from tecton.framework import feature_view as framework_feature_view
@@ -120,15 +120,17 @@
         *,
         name: str,
         description: Optional[str] = None,
         tags: Optional[Dict[str, str]] = None,
         owner: Optional[str] = None,
         prevent_destroy: bool = False,
         online_serving_enabled: bool = True,
-        features: List[Union[framework_feature_view.FeatureReference, framework_feature_view.FeatureView]] = None,
+        features: Optional[
+            List[Union[framework_feature_view.FeatureReference, framework_feature_view.FeatureView]]
+        ] = None,
         logging: Optional[configs.LoggingConfig] = None,
         on_demand_environment: Optional[str] = None,
     ):
         """
         Instantiates a new FeatureService.
 
         :param name: A unique name for the Feature Service.
@@ -234,15 +236,15 @@
         else:
             return self._spec.validation_args
 
     def _get_dependent_objects(self, include_indirect_dependencies: bool) -> List[base_tecton_object.BaseTectonObject]:
         dependent_objects = []
         for fv in self._feature_definitions:
             if include_indirect_dependencies:
-                dependent_objects.extend(fv._get_dependent_objects(include_indirect_dependencies=True) + [fv])
+                dependent_objects.extend([*fv._get_dependent_objects(include_indirect_dependencies=True), fv])
             else:
                 dependent_objects.append(fv)
 
         # Dedupe by ID.
         return list({fco_obj.id: fco_obj for fco_obj in dependent_objects}.values())
 
     @property
@@ -253,15 +255,15 @@
         if self._is_valid:
             return
 
         validations_api.print_validating_dependencies(self, self._feature_definitions, indentation_level)
         dependent_specs = []
         for feature_definition in self._feature_definitions:
             feature_definition._validate(indentation_level + 1)
-            dependent_specs.extend(feature_definition._get_dependent_specs() + [feature_definition._spec])
+            dependent_specs.extend([*feature_definition._get_dependent_specs(), feature_definition._spec])
 
         validations_api.run_backend_validation_and_assert_valid(
             self,
             validator_pb2.ValidationRequest(
                 validation_args=[
                     dependent_obj._build_fco_validation_args()
                     for dependent_obj in self._get_dependent_objects(include_indirect_dependencies=True)
@@ -272,15 +274,15 @@
         )
 
         supplement = specs.FeatureServiceSpecArgsSupplement(
             ids_to_feature_views={spec.id: spec for spec in dependent_specs if isinstance(spec, specs.FeatureViewSpec)}
         )
         fs_spec = specs.FeatureServiceSpec.from_args_proto(self._args, supplement)
 
-        fco_container_specs = [fs_spec] + dependent_specs
+        fco_container_specs = [fs_spec, *dependent_specs]
         fco_container_ = fco_container.FcoContainer.from_specs(specs=fco_container_specs, root_ids=[fs_spec.id])
         self._feature_set_config = feature_set_config.FeatureSetConfig.from_feature_service_spec(
             fs_spec, fco_container_
         )
         self._spec = fs_spec
 
     @sdk_decorators.sdk_public_method
@@ -347,15 +349,15 @@
     @property
     def _feature_definitions(self) -> Set[framework_feature_view.FeatureView]:
         """Returns the set of unique Feature Definitions directly depended on by this Feature Service.
 
         A single Feature Definition may be included multiple times in a Feature Service under different namespaces.
         This method dedupes those.
         """
-        return set(ref.feature_definition for ref in self._feature_references)
+        return {ref.feature_definition for ref in self._feature_references}
 
     @sdk_decorators.assert_valid
     def _check_can_query_from_source(self, from_source: Optional[bool]) -> framework_feature_view.QuerySources:
         all_query_sources = framework_feature_view.QuerySources()
 
         for fv in self._feature_definitions:
             sources = fv._check_can_query_from_source(from_source)
@@ -463,15 +465,15 @@
                 feature_set_config=self._feature_set_config,
             )
 
         if isinstance(spine, str):
             msg = "When using spark compute, `spine` must be one of (pyspark.sql.dataframe.DataFrame, pandas.core.frame.DataFrame, tecton.framework.data_frame.TectonDataFrame); got str instead."
             raise TypeError(msg)
 
-        return spark_api.get_historical_features_for_feature_service(
+        return querytree_api.get_historical_features_for_feature_service(
             feature_service_spec=self._spec,
             feature_set_config=self._feature_set_config,
             spine=spine,
             timestamp_key=timestamp_key,
             from_source=from_source,
             save=save,
             save_as=save_as,
```

### Comparing `tecton-0.8.0b4/tecton/framework/feature_view.py` & `tecton-0.8.0b5/tecton/framework/feature_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from tecton._internals import delete_keys_api
 from tecton._internals import display
 from tecton._internals import errors
 from tecton._internals import materialization_api
 from tecton._internals import metadata_service
 from tecton._internals import mock_source_utils
 from tecton._internals import query_helper
+from tecton._internals import querytree_api
 from tecton._internals import run_api
 from tecton._internals import sdk_decorators
 from tecton._internals import snowflake_api
 from tecton._internals import spark_api
 from tecton._internals import type_utils
 from tecton._internals import utils as internal_utils
 from tecton._internals import validations_api
@@ -59,14 +60,15 @@
 from tecton_core import materialization_context
 from tecton_core import pipeline_common
 from tecton_core import request_context
 from tecton_core import schema_derivation_utils
 from tecton_core import specs
 from tecton_core import time_utils
 from tecton_core.errors import TectonValidationError
+from tecton_core.query import sql_compat
 from tecton_core.time_utils import to_human_readable_str
 from tecton_proto.args import basic_info_pb2
 from tecton_proto.args import fco_args_pb2
 from tecton_proto.args import feature_service_pb2
 from tecton_proto.args import feature_view_pb2 as feature_view__args_pb2
 from tecton_proto.args import pipeline_pb2
 from tecton_proto.common import data_source_type_pb2
@@ -210,15 +212,14 @@
         """Returns all of the specs dependend on by this Feature View."""
         dependent_objects = self._get_dependent_objects(include_indirect_dependencies=True)
         assert all(
             obj._is_valid for obj in dependent_objects
         ), "_get_dependent_specs expects that dependent objects have been validated."
         return [obj._spec for obj in dependent_objects]
 
-    @property
     @sdk_decorators.assert_valid
     def _check_can_query_from_source(self, from_source: Optional[bool]) -> QuerySources:
         raise NotImplementedError
 
     @property
     @sdk_decorators.sdk_public_method
     def join_keys(self) -> List[str]:
@@ -290,15 +291,15 @@
                 ]
                 + [self._build_fco_validation_args()],
             ),
             indentation_level,
         )
 
         fv_spec = specs.create_feature_view_spec_from_args_proto(self._args, self._args_supplement)
-        fco_container_specs = self._get_dependent_specs() + [fv_spec]
+        fco_container_specs = [*self._get_dependent_specs(), fv_spec]
         fco_container_ = fco_container.FcoContainer.from_specs(specs=fco_container_specs, root_ids=[fv_spec.id])
         self._feature_definition = feature_definition_wrapper.FeatureDefinitionWrapper(fv_spec, fco_container_)
 
     @sdk_decorators.sdk_public_method
     @sdk_decorators.assert_remote_object
     def summary(self) -> display.Displayable:
         """Displays a human readable summary of this data source."""
@@ -492,20 +493,23 @@
         return obj
 
     def _get_dependent_objects(self, include_indirect_dependencies: bool) -> List[base_tecton_object.BaseTectonObject]:
         return list(self.sources) + list(self.entities) + list(self.transformations)
 
     def _derive_schemas(self) -> None:
         assert all(
-            [obj._is_valid for obj in self.transformations + self.sources]
+            obj._is_valid for obj in self.transformations + self.sources
         ), "_derive_schemas expects that dependent objects have been validated."
         transformation_specs = [transformation._spec for transformation in self.transformations]
         data_source_specs = [source._spec for source in self.sources]
 
-        if compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE:
+        if (
+            compute_mode.get_compute_mode() == compute_mode.ComputeMode.SNOWFLAKE
+            or sql_compat.dialect() == sql_compat.Dialect.SNOWFLAKE
+        ):
             view_schema = snowflake_api.derive_view_schema_for_feature_view(
                 self._args, transformation_specs, data_source_specs
             )
             materialization_schema = snowflake_api.derive_materialization_schema_for_feature_view(
                 view_schema, self._args
             )
         else:
@@ -750,15 +754,15 @@
             else:
                 feature_definition = self._feature_definition
 
             mock_data_sources = mock_source_utils.convert_mock_inputs_to_mock_sources(feature_definition, mock_inputs)
         else:
             feature_definition = self._feature_definition
 
-        return spark_api.get_historical_features_for_feature_definition(
+        return querytree_api.get_historical_features_for_feature_definition(
             feature_definition=feature_definition,
             spine=spine,
             timestamp_key=timestamp_key,
             start_time=start_time,
             end_time=end_time,
             entities=entities,
             from_source=from_source,
@@ -2285,15 +2289,15 @@
                 entities=entities,
                 from_source=False,
                 save=save,
                 save_as=save_as,
                 feature_set_config=self._construct_feature_set_config(),
             )
 
-        return spark_api.get_historical_features_for_feature_definition(
+        return querytree_api.get_historical_features_for_feature_definition(
             feature_definition=self._feature_definition,
             spine=spine,
             timestamp_key=timestamp_key,
             start_time=start_time,
             end_time=end_time,
             entities=entities,
             from_source=False,
@@ -2534,15 +2538,15 @@
 
         return obj
 
     def _get_dependent_objects(self, include_indirect_dependencies: bool) -> List[base_tecton_object.BaseTectonObject]:
         dependent_objects = list(self.transformations)
         for fv in self._get_dependent_feature_views():
             if include_indirect_dependencies:
-                dependent_objects.extend(fv._get_dependent_objects(include_indirect_dependencies=True) + [fv])
+                dependent_objects.extend([*fv._get_dependent_objects(include_indirect_dependencies=True), fv])
             else:
                 dependent_objects.append(fv)
 
         # Dedupe by ID.
         return list({fco_obj.id: fco_obj for fco_obj in dependent_objects}.values())
 
     def _get_dependent_feature_views(self) -> List[FeatureView]:
@@ -2726,15 +2730,15 @@
                 timestamp_key=timestamp_key,
                 from_source=from_source,
                 save=save,
                 save_as=save_as,
                 feature_set_config=feature_set_config,
             )
 
-        return spark_api.get_historical_features_for_feature_definition(
+        return querytree_api.get_historical_features_for_feature_definition(
             feature_definition=self._feature_definition,
             spine=spine,
             timestamp_key=timestamp_key,
             start_time=None,
             end_time=None,
             entities=None,
             from_source=from_source,
@@ -2967,15 +2971,15 @@
         *,
         feature_definition: FeatureView,
         namespace: Optional[str] = None,
         features: Optional[List[str]] = None,
         override_join_keys: Optional[Dict[str, str]] = None,
     ):
         namespace = namespace if namespace is not None else feature_definition.name
-        return self.__attrs_init__(
+        self.__attrs_init__(
             feature_definition=feature_definition,
             namespace=namespace,
             features=features,
             override_join_keys=override_join_keys,
         )
 
     @property
@@ -3081,15 +3085,15 @@
 
 def _build_odfv_sources_from_spec(
     spec: specs.OnDemandFeatureViewSpec, fco_container_: fco_container.FcoContainer
 ) -> Tuple[Union[FeatureReference, configs.RequestSource], ...]:
     sources = []
     request_context = pipeline_common.find_request_context(spec.pipeline.root)
     if request_context is not None:
-        request_schema = spark_api.get_request_schema_from_tecton_schema(request_context.tecton_schema)
+        request_schema = querytree_api.get_request_schema_from_tecton_schema(request_context.tecton_schema)
         sources.append(configs.RequestSource(schema=request_schema))
 
     feature_view_nodes = pipeline_common.get_all_feature_view_nodes(spec.pipeline)
     for node in feature_view_nodes:
         fv_spec = fco_container_.get_by_id_proto(node.feature_view_node.feature_view_id)
         fv = feature_view_from_spec(fv_spec, fco_container_)
         override_join_keys = {
@@ -3331,15 +3335,15 @@
         if aggregation_interval is None:
             aggregation_interval = datetime.timedelta(seconds=0)
 
         aggregation_protos = [agg._to_proto(aggregation_interval, is_continuous) for agg in aggregations]
 
     secondary_key_output_columns = None
     if aggregation_secondary_key:
-        secondary_key_time_windows = sorted(set(agg.time_window for agg in aggregations))
+        secondary_key_time_windows = sorted({agg.time_window for agg in aggregations})
         secondary_key_output_columns = [
             feature_view__args_pb2.SecondaryKeyOutputColumn(
                 time_window=time_utils.timedelta_to_proto(window),
                 name=_construct_secondary_key_output_list_name(aggregation_secondary_key, window),
             )
             for window in secondary_key_time_windows
         ]
```

### Comparing `tecton-0.8.0b4/tecton/framework/filtered_source.py` & `tecton-0.8.0b5/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/transformation.py` & `tecton-0.8.0b5/tecton/framework/transformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from inspect import signature
+from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import attrs
@@ -230,15 +231,15 @@
         """Override the user defined transformation function.
 
         Returns a PipelineNode for this transformation which is used to construct the pipelines for feature views."""
         node_wrapper = PipelineNodeWrapper(
             node_proto=pipeline_pb2.PipelineNode(
                 transformation_node=pipeline_pb2.TransformationNode(transformation_id=self.info._id_proto)
             ),
-            transformations=set([self]),
+            transformations={self},
         )
         user_function = self._spec.user_function if self._spec is not None else self._user_function
 
         try:
             bound_user_function = signature(user_function).bind(*args, **kwargs)
         except TypeError as e:
             msg = f"while binding inputs to function {self.info.name}, TypeError: {e}"
@@ -292,31 +293,40 @@
         validations_api.run_backend_validation_and_assert_valid(
             self,
             validator_pb2.ValidationRequest(validation_args=[self._build_fco_validation_args()]),
             indentation_level,
         )
         self._spec = specs.TransformationSpec.from_args_proto(self._args, self._user_function)
 
-    def _on_demand_run(self, *inputs: pd.DataFrame) -> data_frame.TectonDataFrame:
-        for df in inputs:
-            if not isinstance(df, pd.DataFrame):
-                msg = f"Input must be of type pandas.DataFrame, but was {type(df)}."
+    def _on_demand_run(self, *inputs: Union[pd.DataFrame, Dict[str, Any]]) -> Union[data_frame.TectonDataFrame, Dict]:
+        for _input in inputs:
+            if not isinstance(_input, pd.DataFrame) and not isinstance(_input, dict):
+                msg = f"Input must be of type pandas.DataFrame or Dict, but was {type(_input)}."
                 raise TypeError(msg)
 
-        return data_frame.TectonDataFrame._create(self.transformer(*inputs))
+        output = self.transformer(*inputs)
+        if isinstance(output, pd.DataFrame):
+            return data_frame.TectonDataFrame._create(output)
+        else:
+            return output
 
     @sdk_decorators.sdk_public_method
     @typechecked
     def run(
         self,
         *inputs: Union[
-            "pd.DataFrame", "pd.Series", "data_frame.TectonDataFrame", "pyspark.sql.DataFrame", spark_api.CONST_TYPE
+            "pd.DataFrame",
+            "pd.Series",
+            "data_frame.TectonDataFrame",
+            "pyspark.sql.DataFrame",
+            Dict,
+            spark_api.CONST_TYPE,
         ],
         context: materialization_context.BaseMaterializationContext = None,
-    ) -> data_frame.TectonDataFrame:
+    ) -> Union[data_frame.TectonDataFrame, Dict]:
         """Run the transformation against inputs.
 
         Currently, this method only supports spark_sql, pyspark, and pandas modes.
 
         :param inputs: positional arguments to the transformation function. For PySpark and SQL transformations,
                        these are either ``pandas.DataFrame`` or ``pyspark.sql.DataFrame`` objects.
                        For on-demand transformations, these are ``pandas.Dataframe`` objects.
@@ -328,15 +338,18 @@
         )
         if transformation_mode == transformation__args_proto.TransformationMode.TRANSFORMATION_MODE_SPARK_SQL:
             return spark_api.run_transformation_mode_spark_sql(
                 *inputs, transformer=self.transformer, context=context, transformation_name=self.info.name
             )
         elif transformation_mode == transformation__args_proto.TransformationMode.TRANSFORMATION_MODE_PYSPARK:
             return spark_api.run_transformation_mode_pyspark(*inputs, transformer=self.transformer, context=context)
-        elif transformation_mode == transformation__args_proto.TransformationMode.TRANSFORMATION_MODE_PANDAS:
+        elif transformation_mode in {
+            transformation__args_proto.TransformationMode.TRANSFORMATION_MODE_PANDAS,
+            transformation__args_proto.TransformationMode.TRANSFORMATION_MODE_PYTHON,
+        }:
             return self._on_demand_run(*inputs)
         msg = f"{transformation_mode} does not support `run(...)`"
         raise RuntimeError(msg)
 
     @sdk_decorators.sdk_public_method
     @sdk_decorators.assert_remote_object
     def summary(self):
```

### Comparing `tecton-0.8.0b4/tecton/framework/utils.py` & `tecton-0.8.0b5/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/validation_mode.py` & `tecton-0.8.0b5/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/framework/workspace.py` & `tecton-0.8.0b5/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/identities/api_keys.py` & `tecton-0.8.0b5/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/identities/credentials.py` & `tecton-0.8.0b5/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/identities/okta.py` & `tecton-0.8.0b5/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/pytest_tecton.py` & `tecton-0.8.0b5/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/snowflake_context.py` & `tecton-0.8.0b5/tecton/snowflake_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 
     def get_connection(self):
         if self._connection is None:
             raise errors.SNOWFLAKE_CONNECTION_NOT_SET
         return self._connection
 
     @classmethod
+    def is_initialized(cls):
+        return cls._current_context_instance is not None
+
+    @classmethod
     @sdk_public_method
     def get_instance(cls) -> "SnowflakeContext":
         """
         Get the singleton instance of SnowflakeContext.
         """
         # If the instance doesn't exist, raise the error to instruct user to set connection first. Otherwise
         # return the current snowflake context.
```

### Comparing `tecton-0.8.0b4/tecton/tecton_context.py` & `tecton-0.8.0b5/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/types.py` & `tecton-0.8.0b5/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/__diff.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/__init__.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/_dill.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/_objects.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/detect.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/info.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/pointers.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/settings.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/source.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/dill/dill/temp.py` & `tecton-0.8.0b5/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.8.0b5/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/vendor_dill.py` & `tecton-0.8.0b5/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/vendor/vendor_pyspark.py` & `tecton-0.8.0b5/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton/version.py` & `tecton-0.8.0b5/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton.egg-info/PKG-INFO` & `tecton-0.8.0b5/tecton.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.8.0b4
+Version: 0.8.0b5
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Provides-Extra: databricks-connect10
 Provides-Extra: databricks-connect11
 Provides-Extra: pyspark
 Provides-Extra: pyspark3
 Provides-Extra: pyspark3.1
 Provides-Extra: pyspark3.2
 Provides-Extra: pyspark3.3
+Provides-Extra: duckdb
 Provides-Extra: snowflake
 Provides-Extra: snowpark
 Provides-Extra: athena
 
 ![logo](https://s3.us-west-2.amazonaws.com/tecton.ai.public/documentation/pypi/tecton-logo.svg)
 
 Tecton is the fastest way to build operational machine learning applications. It helps automate real-time decision making like fraud detection, product recommendations, and search result ranking in production applications.
```

### Comparing `tecton-0.8.0b4/tecton.egg-info/SOURCES.txt` & `tecton-0.8.0b5/tecton.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 protoc_gen_swagger/__init__.py
 protoc_gen_swagger/options/__init__.py
 protoc_gen_swagger/options/annotations_pb2.py
 protoc_gen_swagger/options/openapiv2_pb2.py
 tecton/__init__.py
 tecton/_stamp.py
 tecton/aggregation_functions.py
+tecton/duckdb_context.py
 tecton/fco_listers.py
 tecton/pytest_tecton.py
 tecton/run_api_consts.py
 tecton/snowflake_context.py
 tecton/tecton_context.py
 tecton/types.py
 tecton/version.py
@@ -31,14 +32,15 @@
 tecton/_internals/errors.py
 tecton/_internals/find_spark.py
 tecton/_internals/ingest_utils.py
 tecton/_internals/materialization_api.py
 tecton/_internals/metadata_service.py
 tecton/_internals/mock_source_utils.py
 tecton/_internals/query_helper.py
+tecton/_internals/querytree_api.py
 tecton/_internals/rewrite.py
 tecton/_internals/run_api.py
 tecton/_internals/sdk_decorators.py
 tecton/_internals/snowflake_api.py
 tecton/_internals/spark_api.py
 tecton/_internals/spark_utils.py
 tecton/_internals/time_utils.py
@@ -268,22 +270,26 @@
 tecton_core/request_context.py
 tecton_core/schema.py
 tecton_core/schema_derivation_utils.py
 tecton_core/time_utils.py
 tecton_core/query/__init__.py
 tecton_core/query/aggregation_plans.py
 tecton_core/query/builder.py
+tecton_core/query/executor_params.py
 tecton_core/query/node_interface.py
 tecton_core/query/nodes.py
+tecton_core/query/query_tree_compute.py
+tecton_core/query/query_tree_executor.py
 tecton_core/query/rewrite.py
 tecton_core/query/sql_compat.py
 tecton_core/query/pandas/__init__.py
 tecton_core/query/pandas/node.py
 tecton_core/query/pandas/nodes.py
 tecton_core/query/pandas/sql.py
+tecton_core/query/pandas/translate.py
 tecton_core/specs/__init__.py
 tecton_core/specs/data_source_spec.py
 tecton_core/specs/entity_spec.py
 tecton_core/specs/feature_service_spec.py
 tecton_core/specs/feature_view_spec.py
 tecton_core/specs/tecton_object_spec.py
 tecton_core/specs/transformation_spec.py
@@ -292,14 +298,18 @@
 tecton_core/vendor/vendor_treelib.py
 tecton_core/vendor/treelib/__init__.py
 tecton_core/vendor/treelib/exceptions.py
 tecton_core/vendor/treelib/misc.py
 tecton_core/vendor/treelib/node.py
 tecton_core/vendor/treelib/plugins.py
 tecton_core/vendor/treelib/tree.py
+tecton_duckdb/__init__.py
+tecton_duckdb/query/__init__.py
+tecton_duckdb/query/nodes.py
+tecton_duckdb/query/rewrite.py
 tecton_proto/__init__.py
 tecton_proto/amplitude/__init__.py
 tecton_proto/amplitude/amplitude_pb2.py
 tecton_proto/amplitude/client_logging_pb2.py
 tecton_proto/api/__init__.py
 tecton_proto/api/featureservice/__init__.py
 tecton_proto/api/featureservice/feature_service_pb2.py
@@ -434,14 +444,21 @@
 tecton_snowflake/__init__.py
 tecton_snowflake/pipeline_helper.py
 tecton_snowflake/schema_derivation_utils.py
 tecton_snowflake/snowflake_type_utils.py
 tecton_snowflake/sql_helper.py
 tecton_snowflake/templates_utils.py
 tecton_snowflake/utils.py
+tecton_snowflake/query/__init__.py
+tecton_snowflake/query/aggregation_plans.py
+tecton_snowflake/query/dataframe_helper.py
+tecton_snowflake/query/nodes.py
+tecton_snowflake/query/queries.py
+tecton_snowflake/query/rewrite.py
+tecton_snowflake/query/translate.py
 tecton_snowflake/templates/__init__.py
 tecton_snowflake/templates/copier_macro.sql
 tecton_snowflake/templates/create_temp_table_for_bfv.sql
 tecton_snowflake/templates/create_temp_table_for_bwafv.sql
 tecton_snowflake/templates/data_source.sql
 tecton_snowflake/templates/delete_orphaned_schemas.sql
 tecton_snowflake/templates/delete_staged_files.sql
```

### Comparing `tecton-0.8.0b4/tecton.egg-info/requires.txt` & `tecton-0.8.0b5/tecton.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 typing-extensions~=4.1
 pygments>=2.7.4
 pytest
 click~=8.0
 typeguard~=2.0
 sqlparse
 semantic_version
+pyarrow~=8.0
 
 [athena]
 awswrangler~=2.15
 
 [databricks-connect]
 databricks-connect[sql]~=10.4.12
 
@@ -33,14 +34,17 @@
 
 [databricks-connect11]
 databricks-connect[sql]~=11.3.12
 
 [databricks-connect9]
 databricks-connect[sql]~=9.1.23
 
+[duckdb]
+duckdb~=0.8.1
+
 [pyspark]
 pyspark[sql]~=3.2.1
 
 [pyspark3]
 pyspark[sql]~=3.2.1
 
 [pyspark3.1]
```

### Comparing `tecton-0.8.0b4/tecton_athena/athena_session.py` & `tecton-0.8.0b5/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/data_catalog_helper.py` & `tecton-0.8.0b5/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/odfv_helper.py` & `tecton-0.8.0b5/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/pipeline_helper.py` & `tecton-0.8.0b5/tecton_athena/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/query/translate.py` & `tecton-0.8.0b5/tecton_athena/query/translate.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 
 # Converts a logical querytree to a physical Athena querytree by converting the RenameColsNodes and
 # MultiOdfvPipelineNode at the top of the tree to PandasExecNodes and the input node directly below these nodes to an
 # Athena SqlExecNode that will execute the SQL in an Athena session. The requirement here is that ODFVPipelineNodes will
 # not appear in a middle of a querytree and will only ever appear at the top of the querytree.
 def athena_convert(node_ref: NodeRef, sql_executor: AthenaSqlExecutor) -> PandasExecNode:
     if tree_contains(node_ref, MultiOdfvPipelineNode):
-        return convert_to_pandas_nodes(node_ref, sql_executor)
+        return _convert_to_pandas_nodes(node_ref, sql_executor)
     else:
         return SqlExecNode.from_sql_inputs(node_ref.node, sql_executor)
 
 
-def convert_to_pandas_nodes(tree: NodeRef, sql_executor):
+def _convert_to_pandas_nodes(tree: NodeRef, sql_executor):
     # Recurses over RenameColsNodes and MultiOdfvPipelineNode at the top of the tree and converts them to
     # PandasExecNodes and converts only the node immediately below these nodes to a SqlExecNode
     logical_tree_node = tree.node
     node_mapping = {
         MultiOdfvPipelineNode: PandasMultiOdfvPipelineNode,
         RenameColsNode: PandasRenameColsNode,
     }
     if logical_tree_node.__class__ in node_mapping:
-        input_node = convert_to_pandas_nodes(logical_tree_node.input_node, sql_executor)
+        input_node = _convert_to_pandas_nodes(logical_tree_node.input_node, sql_executor)
         return node_mapping[logical_tree_node.__class__].from_node_inputs(logical_tree_node, input_node)
     else:
         return SqlExecNode.from_sql_inputs(logical_tree_node, sql_executor)
```

### Comparing `tecton-0.8.0b4/tecton_athena/sql_helper.py` & `tecton-0.8.0b5/tecton_athena/sql_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     # Get a list of all the join keys in the spine.
     spine_keys = {}
     for item in feature_set_items:
         fd = item.feature_definition
 
         if not fd.is_on_demand:
-            join_keys = {key: value for key, value in item.join_keys}
+            join_keys = dict(item.join_keys)
             spine_keys.update(join_keys)
 
     spine_info = upload_spine(spine=spine, expected_spine_keys=list(spine_keys), expected_timestamp_key=timestamp_key)
 
     for item in feature_set_items:
         fd = item.feature_definition
 
@@ -152,19 +152,19 @@
 
         # Change the feature view name if it's for internal udf use.
         if item.namespace.startswith("_udf_internal"):
             name = item.namespace.upper()
         else:
             name = fd.name
 
-        join_keys = {key: value for key, value in item.join_keys}
+        join_keys = dict(item.join_keys)
         features = [
             col_name
             for col_name in fd.view_schema.column_names()
-            if col_name not in (list(join_keys.keys()) + [fd.timestamp_key])
+            if col_name not in ([*list(join_keys.keys()), fd.timestamp_key])
         ]
         if len(fd.online_serving_index.join_keys) != len(fd.join_keys):
             msg = "Wildcard is not supported for Athena"
             raise TectonAthenaNotImplementedError(msg)
 
         if spine_info is not None:
             feature_start_time, feature_end_time = _get_feature_selection_time_bounds_from_spine_time_range(
@@ -357,16 +357,16 @@
 def upload_spine(
     spine: Optional[Union[pandas.DataFrame]], expected_spine_keys: List[str], expected_timestamp_key: str
 ) -> Optional[_SpineInfo]:
     if spine is None:
         return None
 
     if isinstance(spine, pandas.DataFrame):
-        spine_columns = set([c.lower() for c in list(spine.columns)])
-        expected_spine_columns = set([c.lower() for c in expected_spine_keys])
+        spine_columns = {c.lower() for c in list(spine.columns)}
+        expected_spine_columns = {c.lower() for c in expected_spine_keys}
         expected_spine_columns.add(expected_timestamp_key.lower())
 
         non_key_columns_in_spine = spine_columns - expected_spine_columns
         missing_columns_in_spine = expected_spine_columns - spine_columns
 
         if len(missing_columns_in_spine) > 0:
             msg = f"Expected to find the following columns in the spine: {missing_columns_in_spine}"
```

### Comparing `tecton-0.8.0b4/tecton_athena/templates/create_table.sql` & `tecton-0.8.0b5/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/templates/historical_features.sql` & `tecton-0.8.0b5/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/templates/materialization_tile.sql` & `tecton-0.8.0b5/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.8.0b5/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/templates/time_limit.sql` & `tecton-0.8.0b5/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_athena/templates_utils.py` & `tecton-0.8.0b5/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/aggregation_utils.py` & `tecton-0.8.0b5/tecton_core/aggregation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     return AGGREGATION_FUNCTIONS_TO_COLUMN_NAME[aggregation_function_enum]
 
 
 # Column prefixes that can't be derived from aggregation function name.
 sum_of_squares_column_prefix = get_aggregation_function_name(afpb.AGGREGATION_FUNCTION_SUM) + "_of_squares"
 
 
-def get_pretty_column_prefix(materialized_column_prefix: str):
+def get_pretty_column_prefix(materialized_column_prefix: str) -> str:
     """Formats a materialized column prefix to be more human readable.
 
     For example, maps 'lastn10' to 'last_distinct_10' and 'last_non_distinct_n10' to 'last_10'.
 
     Only used for cosmetic purposes, to prettify the materialized column prefixes in the run API.
     """
     if materialized_column_prefix.startswith("lastn"):
@@ -194,20 +194,15 @@
 @typechecked
 def aggregation_prefix_to_tecton_type(prefix: str) -> Optional[tecton_types.DataType]:
     prefix = prefix.lower()
     if prefix == "count":
         return tecton_types.Int64Type()
     elif prefix == "mean" or prefix == "sum_of_squares":
         return tecton_types.Float64Type()
-    elif (
-        prefix.startswith("lastn")
-        or prefix.startswith("last_non_distinct_n")
-        or prefix.startswith("first_non_distinct_n")
-        or prefix.startswith("first_distinct_n")
-    ):
+    elif prefix.startswith(("lastn", "last_non_distinct_n", "first_non_distinct_n", "first_distinct_n")):
         return tecton_types.ArrayType(tecton_types.StringType())
     else:
         return None
 
 
 @typechecked
 def get_materialization_column_name(prefix: str, input_column_name: str) -> str:
```

### Comparing `tecton-0.8.0b4/tecton_core/conf.py` & `tecton-0.8.0b5/tecton_core/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import Iterable
+from typing import Iterator
 from typing import List
 from typing import Optional
 
 from tecton_core import errors
 
 
 logging.getLogger("boto3").setLevel(logging.ERROR)
@@ -57,66 +58,66 @@
 class _Debugger(object):
     @classmethod
     def _debug_enabled(cls) -> bool:
         debug_value = _get_runtime_only("TECTON_DEBUG")
         return debug_value is not None and debug_value.lower() in ("1", "true", "yes")
 
     @classmethod
-    def preamble(cls, key: str):
+    def preamble(cls, key: str) -> None:
         if cls._debug_enabled():
             print(f"Looking up {key}", file=sys.stderr)
 
     @classmethod
-    def print(cls, src: ConfSource, key: str, val: Optional[str] = None, details: Optional[str] = None):
+    def print(cls, src: ConfSource, key: str, val: Optional[str] = None, details: Optional[str] = None) -> None:
         if not cls._debug_enabled():
             return
 
         if src == ConfSource.NOT_FOUND:
             print(f"Unable to find {key}\n", file=sys.stderr)
             return
 
         details_str = f"({details})" if details else ""
         val_str = val if val is not None else "not found"
         symbol_str = "[x]" if val is not None else "[ ]"
         print(symbol_str, f"{key} in {src.name} -> {val_str}", details_str, file=sys.stderr)
 
 
-def set(key, value):
+def set(key: str, value: str) -> None:
     _set(key, value)
 
 
-def unset(key):
+def unset(key: str) -> None:
     del _CONFIG_OVERRIDES[key]
 
 
-def _set(key, value):
+def _set(key: str, value: str) -> None:
     _CONFIG_OVERRIDES[key] = value
 
 
 @contextlib.contextmanager
-def _temporary_set(key, value):
+def _temporary_set(key: str, value: str) -> Iterator[None]:
     curr_val = _CONFIG_OVERRIDES.get(key)
     _CONFIG_OVERRIDES[key] = value
     try:
         yield
     finally:
         if curr_val:
             _CONFIG_OVERRIDES[key] = curr_val
         else:
             del _CONFIG_OVERRIDES[key]
 
 
-def _does_key_have_valid_prefix(key) -> bool:
+def _does_key_have_valid_prefix(key: str) -> bool:
     for prefix in _VALID_KEY_PREFIXES:
         if key.startswith(prefix):
             return True
     return False
 
 
-def _get(key) -> Optional[str]:
+def _get(key: str) -> Optional[str]:
     """Get the config value for the given key, or return None if not found."""
     _Debugger.preamble(key)
 
     if key in _VALID_KEYS_TO_ALLOWED_SOURCES:
         allowed_sources = _VALID_KEYS_TO_ALLOWED_SOURCES[key]
     elif _does_key_have_valid_prefix(key):
         allowed_sources = DEFAULT_ALLOWED_SOURCES
@@ -190,15 +191,15 @@
         _Debugger.print(ConfSource.DEFAULT, key, value)
         return value
 
     _Debugger.print(ConfSource.NOT_FOUND, key)
     return None
 
 
-def _get_runtime_only(key) -> Optional[str]:
+def _get_runtime_only(key: str) -> Optional[str]:
     """An alternate _get() that will look up only from runtime sources. Used to avoid infinite loops."""
     if key not in _VALID_KEYS_TO_ALLOWED_SOURCES:
         msg = f"_get_runtime_only should only used with valid keys. {key}"
         raise errors.TectonInternalError(msg)
 
     allowed_sources = _VALID_KEYS_TO_ALLOWED_SOURCES[key]
     # Use `builtins.set` since we shadowed the `set` built-in in this module.
@@ -219,27 +220,27 @@
     if key in _DEFAULTS:
         value = _DEFAULTS[key]()
         return value
 
     return None
 
 
-def get_or_none(key) -> Optional[str]:
+def get_or_none(key: str) -> Optional[str]:
     return _get(key)
 
 
-def get_or_raise(key) -> str:
+def get_or_raise(key: str) -> str:
     val = _get(key)
     if val is None:
         msg = f"{key} not set"
         raise errors.TectonInternalError(msg)
     return val
 
 
-def get_bool(key) -> bool:
+def get_bool(key: str) -> bool:
     val = _get(key)
     if val is None:
         return False
     # bit of a hack for if people set a boolean value in a local override
     if isinstance(val, bool):
         return val
     if not isinstance(val, str):
@@ -255,27 +256,27 @@
 
 # Internal
 
 _LOCAL_TECTON_CONFIG_FILE = Path(os.environ.get("TECTON_CONFIG_PATH", Path.home() / ".tecton/config"))
 _LOCAL_TECTON_TOKENS_FILE = _LOCAL_TECTON_CONFIG_FILE.with_suffix(".tokens")
 
 _VALID_KEYS_TO_ALLOWED_SOURCES = {
-    "API_SERVICE": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_CONFIG,),
-    "FEATURE_SERVICE": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_CONFIG,),
-    "CLI_CLIENT_ID": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_CONFIG,),
-    "TECTON_WORKSPACE": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_CONFIG,),
-    "ALPHA_SNOWFLAKE_COMPUTE_ENABLED": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_CONFIG,),
+    "API_SERVICE": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_CONFIG),
+    "FEATURE_SERVICE": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_CONFIG),
+    "CLI_CLIENT_ID": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_CONFIG),
+    "TECTON_WORKSPACE": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_CONFIG),
+    "ALPHA_SNOWFLAKE_COMPUTE_ENABLED": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_CONFIG),
     "TECTON_COMPUTE_MODE": (
         ConfSource.SESSION_OVERRIDE,
         ConfSource.OS_ENV,
         ConfSource.REMOTE_MDS_CONFIG,
     ),
-    "OAUTH_ACCESS_TOKEN": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_TOKENS,),
-    "OAUTH_ACCESS_TOKEN_EXPIRATION": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_TOKENS,),
-    "OAUTH_REFRESH_TOKEN": DEFAULT_ALLOWED_SOURCES + (ConfSource.LOCAL_TECTON_TOKENS,),
+    "OAUTH_ACCESS_TOKEN": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_TOKENS),
+    "OAUTH_ACCESS_TOKEN_EXPIRATION": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_TOKENS),
+    "OAUTH_REFRESH_TOKEN": (*DEFAULT_ALLOWED_SOURCES, ConfSource.LOCAL_TECTON_TOKENS),
     # TECTON_CLUSTER_NAME is needed for looking up AWS and Databricks secrets. CLUSTER_REGION is used for looking up AWS
     # secrets. To avoid an infinite loop, these keys cannot be looked up from those sources.
     "TECTON_CLUSTER_NAME": (
         ConfSource.SESSION_OVERRIDE,
         ConfSource.OS_ENV,
         ConfSource.REMOTE_MDS_CONFIG,
     ),
@@ -296,15 +297,22 @@
     "TECTON_RUNTIME_MODE": RUNTIME_ALLOWED_SOURCES,
     "TECTON_VALIDATION_MODE": RUNTIME_ALLOWED_SOURCES,
     "TECTON_FORCE_FUNCTION_SERIALIZATION": RUNTIME_ALLOWED_SOURCES,
     "TECTON_REPO_IGNORE_ALL_HIDDEN_DIRS": RUNTIME_ALLOWED_SOURCES,
     "SKIP_OBJECT_VERSION_CHECK": RUNTIME_ALLOWED_SOURCES,
     "ATHENA_TEST_ENABLED": RUNTIME_ALLOWED_SOURCES,
     "ALPHA_ATHENA_COMPUTE_ENABLED": DEFAULT_ALLOWED_SOURCES,
-    "SQL_DIALECT": DEFAULT_ALLOWED_SOURCES,
+    "SQL_DIALECT": RUNTIME_ALLOWED_SOURCES,
+    "AGG_SQL_DIALECT": RUNTIME_ALLOWED_SOURCES,
+    "STAGING_S3_PREFIX": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_DEBUG": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_BENCHMARK": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_PERSIST_DB": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_MEMORY_LIMIT": DEFAULT_ALLOWED_SOURCES,
+    "DUCKDB_NTHREADS": DEFAULT_ALLOWED_SOURCES,
     "ATHENA_S3_PATH": DEFAULT_ALLOWED_SOURCES,
     "ATHENA_DATABASE": DEFAULT_ALLOWED_SOURCES,
     "ENABLE_TEMPO": DEFAULT_ALLOWED_SOURCES,
     "QUERY_REWRITE_ENABLED": DEFAULT_ALLOWED_SOURCES,
     "ALPHA_SNOWFLAKE_SNOWPARK_ENABLED": DEFAULT_ALLOWED_SOURCES,
     "AWS_ACCESS_KEY_ID": DEFAULT_ALLOWED_SOURCES,
     "AWS_SECRET_ACCESS_KEY": DEFAULT_ALLOWED_SOURCES,
@@ -313,25 +321,27 @@
     "HIVE_METASTORE_USERNAME": DEFAULT_ALLOWED_SOURCES,
     "HIVE_METASTORE_DATABASE": DEFAULT_ALLOWED_SOURCES,
     "HIVE_METASTORE_PASSWORD": DEFAULT_ALLOWED_SOURCES,
     "SPARK_DRIVER_LOCAL_IP": DEFAULT_ALLOWED_SOURCES,
     "METADATA_SERVICE": DEFAULT_ALLOWED_SOURCES,
     "TECTON_API_KEY": DEFAULT_ALLOWED_SOURCES,
     "QUERYTREE_SHORT_SQL_ENABLED": RUNTIME_ALLOWED_SOURCES,
+    "QUERYTREE_SHORT_SQL_TYPE": RUNTIME_ALLOWED_SOURCES,
     "REDSHIFT_USER": DEFAULT_ALLOWED_SOURCES,
     "REDSHIFT_PASSWORD": DEFAULT_ALLOWED_SOURCES,
     "SKIP_FEATURE_TIMESTAMP_VALIDATION": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_ACCOUNT_IDENTIFIER": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_DEBUG": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_SHORT_SQL_ENABLED": DEFAULT_ALLOWED_SOURCES,  # Whether to break up long SQL statements into temporary views for Snowflake
     "SNOWFLAKE_TEMP_TABLE_ENABLED": DEFAULT_ALLOWED_SOURCES,  # Whether to break up long SQL statements with temporary tables for Snowflake, takes precedence over SNOWFLAKE_SHORT_SQL_ENABLED
     "SNOWFLAKE_USER": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_PASSWORD": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_WAREHOUSE": DEFAULT_ALLOWED_SOURCES,
     "SNOWFLAKE_DATABASE": DEFAULT_ALLOWED_SOURCES,
+    "SNOWFLAKE_PANDAS_ODFV_ENABLED": RUNTIME_ALLOWED_SOURCES,
     "REDIS_AUTH_TOKEN": DEFAULT_ALLOWED_SOURCES,
 }
 
 _VALID_KEY_PREFIXES = ["SECRET_"]
 
 
 def _snowpark_enabled():
@@ -350,36 +360,38 @@
     "FEATURE_SERVICE": (lambda: _get("API_SERVICE")),
     "ALPHA_SNOWFLAKE_SNOWPARK_ENABLED": (_snowpark_enabled),
     "ENABLE_TEMPO": (lambda: "false"),
     "QUERY_REWRITE_ENABLED": (lambda: "true"),
     "SQL_DIALECT": (lambda: "spark"),
     "TECTON_VALIDATION_MODE": (lambda: "explicit"),
     "TECTON_REPO_IGNORE_ALL_HIDDEN_DIRS": (lambda: "true"),
+    "QUERYTREE_SHORT_SQL_TYPE": (lambda: "table"),
+    "DUCKDB_MEMORY_LIMIT": (lambda: "1GB"),
 }
 
 _REMOTE_MDS_CONFIGS: _ConfigSettings = {}
 
 _is_running_on_databricks_cache = None
 _is_running_on_emr_cache = None
 TectonEnv = Enum("TectonEnv", "DATABRICKS EMR UNKNOWN")
 
 
-def _is_running_on_databricks():
+def _is_running_on_databricks() -> bool:
     """Whether we're running in Databricks notebook or not."""
     global _is_running_on_databricks_cache
     if _is_running_on_databricks_cache is None:
         main = __import__("__main__")
         filename = os.path.basename(getattr(main, "__file__", ""))
         is_python_shell = filename == "PythonShell.py"
         is_databricks_env = "DBUtils" in main.__dict__
         _is_running_on_databricks_cache = is_python_shell and is_databricks_env
     return _is_running_on_databricks_cache
 
 
-def _is_running_on_emr():
+def _is_running_on_emr() -> bool:
     """Whether we're running in EMR notebook or not."""
     global _is_running_on_emr_cache
     if _is_running_on_emr_cache is None:
         _is_running_on_emr_cache = "EMR_CLUSTER_ID" in os.environ
     return _is_running_on_emr_cache
 
 
@@ -389,20 +401,20 @@
         set(key, "DATABRICKS")
     elif _is_running_on_emr():
         set(key, "EMR")
     else:
         set(key, "UNKNOWN")
 
 
-def _is_mode_materialization():
+def _is_mode_materialization() -> bool:
     runtime_mode = get_or_none("TECTON_RUNTIME_MODE")
     return runtime_mode == "MATERIALIZATION"
 
 
-def _get_runtime_env():
+def _get_runtime_env() -> TectonEnv:
     # Use _get_runtime_only() and not _get() to avoid an infinite loop.
     runtime_env = _get_runtime_only("TECTON_RUNTIME_ENV")
     if runtime_env == "DATABRICKS":
         return TectonEnv.DATABRICKS
     elif runtime_env == "EMR":
         return TectonEnv.EMR
     else:
@@ -417,39 +429,39 @@
 
 
 def _get_keys_with_allowed_source(source: ConfSource) -> List[str]:
     """Returns all the keys that have the allowed ConfSource."""
     return [key for key, allowed_sources in _VALID_KEYS_TO_ALLOWED_SOURCES.items() if source in allowed_sources]
 
 
-def save_tecton_configs():
+def save_tecton_configs() -> None:
     _save_tecton_config(_LOCAL_TECTON_CONFIG_FILE, _get_keys_with_allowed_source(ConfSource.LOCAL_TECTON_CONFIG))
     _save_tecton_config(_LOCAL_TECTON_TOKENS_FILE, _get_keys_with_allowed_source(ConfSource.LOCAL_TECTON_TOKENS))
 
 
-def _save_tecton_config(path: Path, keys: Iterable[str]):
+def _save_tecton_config(path: Path, keys: Iterable[str]) -> None:
     tecton_config = {key: get_or_none(key) for key in keys if get_or_none(key) is not None}
     path.parent.mkdir(parents=True, exist_ok=True)
     with open(path, "w") as f:
         json.dump(tecton_config, f, sort_keys=True, indent=2)
         f.write("\n")
 
 
 # Get key by looking in TECTON_CLUSTER_NAME'd scope and falling back to "tecton"
-def _get_secret_scopes():
+def _get_secret_scopes() -> List[str]:
     cluster_name = get_or_none("TECTON_CLUSTER_NAME")
     secret_scopes = []
     if cluster_name:
         secret_prefix = cluster_name if cluster_name.startswith("tecton-") else f"tecton-{cluster_name}"
         secret_scopes.append(secret_prefix)
     secret_scopes.append("tecton")
     return secret_scopes
 
 
-def _get_from_secretsmanager(key: str, scope: str):
+def _get_from_secretsmanager(key: str, scope: str) -> Optional[str]:
     try:
         # Try to Grab secret from AWS secrets manager
         from boto3 import client
 
         if _is_mode_materialization():
             aws_secret_client = client("secretsmanager")
         else:
@@ -457,15 +469,15 @@
         secret = aws_secret_client.get_secret_value(SecretId=f"{scope}/{key}")
         return secret["SecretString"]
     except Exception:
         # Do not fail if secret is not found
         return None
 
 
-def _get_from_db_secrets(key: str, scope: str):
+def _get_from_db_secrets(key: str, scope: str) -> Optional[str]:
     try:
         dbutils = _get_dbutils()
         return dbutils.secrets.get(scope, key)
     except Exception:
         return None
 
 
@@ -489,15 +501,15 @@
     except json.decoder.JSONDecodeError as e:
         raise ValueError(
             f"Unable to decode JSON configuration file {file_path} ({str(e)}). "
             + "To regenerate configuration, delete this file and run `tecton login`."
         )
 
 
-def validate_api_service_url(url: str):
+def validate_api_service_url(url: str) -> None:
     """Validate Tecton API URL.
     Returns nothing for valid URLs or raises an error."""
     if "localhost" in url or "ingress" in url:
         return
     if not url.endswith("/api"):
         msg = f'Tecton API URL ("{url}") should be formatted "https://<deployment>.tecton.ai/api"'
         raise errors.TectonAPIValidationError(msg)
```

### Comparing `tecton-0.8.0b4/tecton_core/data_types.py` & `tecton-0.8.0b5/tecton_core/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     @abc.abstractmethod
     def proto(self) -> data_type_pb2.DataType:
         pass
 
     def __hash__(self) -> int:
         return hash(self.proto.SerializeToString(deterministic=True))
 
-    def __eq__(self, other: object):
+    def __eq__(self, other: object) -> bool:
         if not isinstance(other, DataType):
             return False
         return self.proto == other.proto
 
     def __str__(self):
         # Require __str__ implementation. Used in error messages.
         raise NotImplementedError
@@ -192,15 +192,15 @@
     @property
     def sql_type(self) -> SqlTypes:
         # Used for safe typecasting in sql-based compute platforms
         raise NotImplementedError
 
 
 class MapType(DataType):
-    def __init__(self, key_type: DataType, value_type: DataType):
+    def __init__(self, key_type: DataType, value_type: DataType) -> None:
         self._key_type = key_type
         self._value_type = value_type
 
     @property
     def proto(self) -> data_type_pb2.DataType:
         return data_type_pb2.DataType(
             type=data_type_pb2.DATA_TYPE_MAP, map_key_type=self._key_type.proto, map_value_type=self._value_type.proto
```

### Comparing `tecton-0.8.0b4/tecton_core/errors.py` & `tecton-0.8.0b5/tecton_core/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,49 +57,49 @@
 
 class FailedPreconditionError(Exception):
     """
     Exception that indicates some prequisite has not been met (e.g the CLI/SDK needs to be updated).
     """
 
 
-def INGEST_DF_MISSING_COLUMNS(columns: List[str]):
+def INGEST_DF_MISSING_COLUMNS(columns: List[str]) -> TectonValidationError:
     return TectonValidationError(f"Missing columns in the DataFrame: {', '.join(columns)}")
 
 
-def INGEST_COLUMN_TYPE_MISMATCH(column_name: str, expected_type: str, actual_type: str):
+def INGEST_COLUMN_TYPE_MISMATCH(column_name: str, expected_type: str, actual_type: str) -> TectonValidationError:
     return TectonValidationError(
         f"Column type mismatch for column '{column_name}', expected {expected_type}, got {actual_type}"
     )
 
 
-def UDF_ERROR(error: Exception):
+def UDF_ERROR(error: Exception) -> TectonValidationError:
     return TectonValidationError(
         "UDF Error: please review and ensure the correctness of your feature definition and the input data passed in. Otherwise please contact Tecton Support for assistance."
         + f" Running the transformation resulted in the following error: {type(error).__name__}: {str(error)} "
     )
 
 
-def UDF_TYPE_ERROR(error: Exception):
+def UDF_TYPE_ERROR(error: Exception) -> TectonValidationError:
     return TectonValidationError(
         "UDF Type Error: please ensure that your UDF correctly handles the typing of row values. Make sure to cast dataframe values to the correct type and ensure that you are handling"
         + f" null column values correctly in your UDF. Running the transformation resulted in the following error: {type(error).__name__}: {str(error)} "
     )
 
 
-def INVALID_SPINE_SQL(error: Exception):
+def INVALID_SPINE_SQL(error: Exception) -> TectonValidationError:
     return TectonValidationError(
         f"Invalid SQL: please review your SQL for the spine passed in. Received error: {type(error).__name__}: {str(error)} "
     )
 
 
-def START_TIME_NOT_BEFORE_END_TIME(start_time: datetime, end_time: datetime):
+def START_TIME_NOT_BEFORE_END_TIME(start_time: datetime, end_time: datetime) -> TectonValidationError:
     return TectonValidationError(f"start_time ({start_time}) must be less than end_time ({end_time}).")
 
 
-def DS_ARGS_MISSING_FIELD(ds_type: str, field: str):
+def DS_ARGS_MISSING_FIELD(ds_type: str, field: str) -> TectonValidationError:
     return TectonValidationError(f"{ds_type} data source args must contain field {field}.")
 
 
 REDSHIFT_DS_EITHER_TABLE_OR_QUERY = TectonValidationError(
     "Redshift data source must contain either table or query, but not both."
 )
 
@@ -123,27 +123,27 @@
 
 FV_BFC_SINGLE_FROM_SOURCE = TectonValidationError(
     "Computing features from source is not supported for Batch Feature Views with incremental_backfills set to True. "
     + "Enable offline materialization for this feature view in a live workspace to use `get_historical_features()`. Alternatively, use `run()` to test this feature view without materializing data."
 )
 
 
-def FV_NEEDS_TO_BE_MATERIALIZED(fv_name):
+def FV_NEEDS_TO_BE_MATERIALIZED(fv_name: str) -> TectonValidationError:
     return TectonValidationError(
         f"Feature View '{fv_name}' has not been configured for materialization. "
         + "Please use from_source=True when getting features or "
         + "configure offline materialization for this Feature View in a live workspace."
     )
 
 
 FT_DF_TOO_LARGE = TectonValidationError(
     "Dataframe too large for a single ingestion, consider splitting into smaller ones"
 )
 
 
-def FT_UPLOAD_FAILED(reason):
+def FT_UPLOAD_FAILED(reason: str) -> TectonValidationError:
     return TectonValidationError(f"Failed to upload dataframe: {reason}")
 
 
 SNOWFLAKE_CONNECTION_NOT_SET = TectonValidationError(
-    "Snowflake connection not configuered. Please set Snowflake connection using tecton.snowflake_context.set_connection(connection). https://docs.tecton.ai/docs/setting-up-tecton/connecting-to-a-data-platform/tecton-on-snowflake/connecting-notebooks-to-snowflake"
+    "Snowflake connection not configured. Please set Snowflake connection using tecton.snowflake_context.set_connection(connection). https://docs.tecton.ai/docs/setting-up-tecton/connecting-to-a-data-platform/tecton-on-snowflake/connecting-notebooks-to-snowflake"
 )
```

### Comparing `tecton-0.8.0b4/tecton_core/fco_container.py` & `tecton-0.8.0b5/tecton_core/fco_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
+from typing import Union
 
 import attrs
 from typeguard import typechecked
 
 from tecton_core import specs
 from tecton_core.id_helper import IdHelper
 from tecton_proto.common import id_pb2
 from tecton_proto.data import fco_pb2
 from tecton_proto.data.feature_view_pb2 import FeatureView as FeatureViewProto
-from tecton_proto.data.transformation_pb2 import Transformation as Transformation
+from tecton_proto.data.transformation_pb2 import Transformation
 from tecton_proto.data.virtual_data_source_pb2 import VirtualDataSource as DataSourceProto
 
 
 @attrs.frozen
 class FcoContainer:
     """A wrapper class for FcoContainer proto, contains convenience accessors."""
 
@@ -101,15 +102,15 @@
     elif fco.HasField("feature_service"):
         return specs.FeatureServiceSpec.from_data_proto(fco.feature_service)
     else:
         msg = f"Unexpected fco type: {fco}"
         raise ValueError(msg)
 
 
-def _wrap_data_fco(inner_proto) -> fco_pb2.Fco:
+def _wrap_data_fco(inner_proto: Union[DataSourceProto, Transformation, FeatureViewProto]) -> fco_pb2.Fco:
     fco = fco_pb2.Fco()
     if isinstance(inner_proto, DataSourceProto):
         fco.virtual_data_source.CopyFrom(inner_proto)
     elif isinstance(inner_proto, Transformation):
         fco.transformation.CopyFrom(inner_proto)
     elif isinstance(inner_proto, FeatureViewProto):
         fco.feature_view.CopyFrom(inner_proto)
```

### Comparing `tecton-0.8.0b4/tecton_core/feature_definition_wrapper.py` & `tecton-0.8.0b5/tecton_core/feature_definition_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 class FeatureDefinitionWrapper:
     """A container for a Feature View spec and its dependent specs, i.e. data sources, transformations, and entities."""
 
     fv_spec: specs.FeatureViewSpec
     fco_container: FcoContainer
 
     @typechecked
-    def __init__(self, feature_view_spec: specs.FeatureViewSpec, fco_container: FcoContainer):
-        return self.__attrs_init__(  # type: ignore
+    def __init__(self, feature_view_spec: specs.FeatureViewSpec, fco_container: FcoContainer) -> None:
+        self.__attrs_init__(  # type: ignore
             fv_spec=feature_view_spec,
             fco_container=fco_container,
         )
 
     @property
     def id(self) -> str:
         return self.fv_spec.id
@@ -184,15 +184,15 @@
         The columns to group by for partial aggregations. This includes the join keys of the feature view, and the
         aggregation secondary key if configured.
         """
         if not self.is_temporal_aggregate:
             msg = f"Feature View '{self.name}' does not have partial_agg_group_keys"
             raise ValueError(msg)
         return (
-            self.join_keys + [self.fv_spec.aggregation_secondary_key]
+            [*self.join_keys, self.fv_spec.aggregation_secondary_key]
             if self.fv_spec.aggregation_secondary_key
             else self.join_keys
         )
 
     @property
     def offline_store_config(self) -> OfflineFeatureStoreConfig:
         if isinstance(self.fv_spec, specs.OnDemandFeatureViewSpec) or self.fv_spec.offline_store is None:
@@ -294,15 +294,15 @@
         return [IdHelper.to_string(node.virtual_data_source_id) for node in nodes]
 
     @property
     def data_sources(self) -> List[specs.DataSourceSpec]:
         ds_ids = self.data_source_ids
         return self.fco_container.get_by_ids(ds_ids)
 
-    def get_data_source_with_input_name(self, input_name) -> specs.DataSourceSpec:
+    def get_data_source_with_input_name(self, input_name: str) -> specs.DataSourceSpec:
         """Get the data source spec that uses `input_name` for the feature view transformation."""
         input_name_to_ds_id = pipeline_common.get_input_name_to_ds_id_map(self.pipeline)
 
         if input_name not in input_name_to_ds_id:
             msg = (
                 f"Feature view '{self.name}' does not have an input data source with the parameter name '{input_name}'"
             )
@@ -472,15 +472,15 @@
             tile_interval = self.get_tile_interval_for_version
         return -convert_timedelta_for_version(window, version=self.get_feature_store_format_version) + tile_interval
 
 
 def pipeline_to_ds_inputs(pipeline: Pipeline) -> Dict[str, DataSourceNode]:
     ds_nodes: Dict[str, DataSourceNode] = {}
 
-    def _recurse_pipeline_to_ds_nodes(pipeline_node: PipelineNode, ds_nodes_: Dict[str, DataSourceNode]):
+    def _recurse_pipeline_to_ds_nodes(pipeline_node: PipelineNode, ds_nodes_: Dict[str, DataSourceNode]) -> None:
         if pipeline_node.HasField("data_source_node"):
             ds_nodes_[pipeline_node.data_source_node.input_name] = pipeline_node.data_source_node
         elif pipeline_node.HasField("transformation_node"):
             inputs = pipeline_node.transformation_node.inputs
             for input_ in inputs:
                 _recurse_pipeline_to_ds_nodes(input_.node, ds_nodes_)
 
@@ -488,15 +488,15 @@
 
     return ds_nodes
 
 
 def pipeline_to_transformation_ids(pipeline: Pipeline) -> List[str]:
     id_list: List[str] = []
 
-    def _recurse_pipeline_to_transformation_ids(node: PipelineNode, id_list: List[str]):
+    def _recurse_pipeline_to_transformation_ids(node: PipelineNode, id_list: List[str]) -> List[str]:
         if node.HasField("transformation_node"):
             id_list.append(IdHelper.to_string(node.transformation_node.transformation_id))
             for input in node.transformation_node.inputs:
                 _recurse_pipeline_to_transformation_ids(input.node, id_list)
         return id_list
 
     _recurse_pipeline_to_transformation_ids(pipeline.root, id_list)
```

### Comparing `tecton-0.8.0b4/tecton_core/feature_set_config.py` & `tecton-0.8.0b5/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/feature_view_utils.py` & `tecton-0.8.0b5/tecton_core/feature_view_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 
 def get_input_feature_columns(view_schema: SchemaProto, join_keys: List[str], timestamp_key: str) -> List[str]:
     column_names = (c.name for c in view_schema.columns)
     return [c for c in column_names if c not in join_keys and c != timestamp_key]
 
 
-def construct_aggregation_interval_name(aggregation_interval: duration_pb2.Duration, is_continuous: bool):
+def construct_aggregation_interval_name(aggregation_interval: duration_pb2.Duration, is_continuous: bool) -> str:
     if is_continuous:
         return "continuous"
     else:
         return to_human_readable_str(aggregation_interval)
 
 
 @typechecked
 def construct_aggregation_output_feature_name(
     column: str,
     aggregation_function_str: str,
     params: Mapping[str, feature_view_pb2.ParamValue],
     window: duration_pb2.Duration,
     aggregation_interval: duration_pb2.Duration,
     is_continuous: bool,
-):
+) -> str:
     """Constructs the name for the output feature column of an aggregation.
 
     For example, "VALUE_sum_7d_1d" or "VALUE_sum_7d_continuous".
     """
     aggregation_function_resolved_str = _resolve_function_name(aggregation_function_str, params)
     window_name = to_human_readable_str(window)
     aggregation_interval_name = construct_aggregation_interval_name(aggregation_interval, is_continuous)
```

### Comparing `tecton-0.8.0b4/tecton_core/function_deserialization.py` & `tecton-0.8.0b5/tecton_core/function_deserialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import sys
+from typing import Any
+from typing import Callable
+from typing import Dict
+from typing import Optional
 
 from tecton_core import materialization_context
 from tecton_core.errors import TectonValidationError
 from tecton_proto.args.user_defined_function_pb2 import UserDefinedFunction
 
 
 # TODO(deprecated_after=0.5): handle backward-compatibility for builtin transformations that did not use tecton.materialization_context
 # but instead directly accessed tecton_spark.materialization_context
 sys.modules["tecton_spark.materialization_context"] = materialization_context
 
 
-def from_proto(serialized_transform: UserDefinedFunction, globals_=None, locals_=None):
+def from_proto(
+    serialized_transform: UserDefinedFunction,
+    globals_: Optional[Dict[str, Any]] = None,
+    locals_: Optional[Dict[str, Any]] = None,
+) -> Callable:
     """
     deserialize into the provided scope, by default we deserialize the functions into their own scopes
     """
 
     if globals_ is None:
         globals_ = {}
 
@@ -43,14 +51,14 @@
 
 # This version of function deserialization uses the "main scope".
 # This has historically been the behavior of function deserialization.
 # Generally this should be avoided since it can cause hard to debug issues,
 # e.g. two helper functions of the same name can shadow each other. This global
 # scope can also cause issues since it allows for users to access imported
 # libraries that they did not import themselves.
-def from_proto_to_main(serialized_transform: UserDefinedFunction):
+def from_proto_to_main(serialized_transform: UserDefinedFunction) -> Callable:
     """
     deserialize into global scope by default
     """
 
     main_scope = __import__("__main__").__dict__
     return from_proto(serialized_transform, globals_=main_scope)
```

### Comparing `tecton-0.8.0b4/tecton_core/id_helper.py` & `tecton-0.8.0b5/tecton_core/id_helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,13 +13,13 @@
         return "%032x" % random.randrange(16**32)
 
     @staticmethod
     def generate_id() -> Id:
         return IdHelper.from_string(IdHelper.generate_string_id())
 
     @staticmethod
-    def from_string(s) -> Id:
+    def from_string(s: str) -> Id:
         res = Id()
 
         res.most_significant_bits = int(s[:16], 16)
         res.least_significant_bits = int(s[16:], 16)
         return res
```

### Comparing `tecton-0.8.0b4/tecton_core/materialization_context.py` & `tecton-0.8.0b5/tecton_core/materialization_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
         return BoundMaterializationContext(
             _feature_start_time_DONT_ACCESS_DIRECTLY=feature_start_time,
             _feature_end_time_DONT_ACCESS_DIRECTLY=feature_end_time,
             _batch_schedule_DONT_ACCESS_DIRECTLY=batch_schedule,
         )
 
     @classmethod
-    def _create_from_period(cls, feature_time_limits: Optional[pendulum.Period], batch_schedule: pendulum.Duration):
+    def _create_from_period(
+        cls, feature_time_limits: Optional[pendulum.Period], batch_schedule: pendulum.Duration
+    ) -> "BoundMaterializationContext":
         feature_start_time = (
             feature_time_limits.start
             if feature_time_limits is not None
             else pendulum.from_timestamp(0, pendulum.tz.UTC)
         )
         feature_end_time = feature_time_limits.end if feature_time_limits is not None else pendulum.datetime(2100, 1, 1)
         return BoundMaterializationContext(
```

### Comparing `tecton-0.8.0b4/tecton_core/offline_store.py` & `tecton-0.8.0b5/tecton_core/offline_store.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,27 +5,37 @@
 
 import attrs
 import pendulum
 
 from tecton_core import time_utils
 from tecton_core.errors import TectonInternalError
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper as FeatureDefinition
+from tecton_core.query import sql_compat
 from tecton_core.query_consts import ANCHOR_TIME
+from tecton_proto.args.feature_view_pb2 import OfflineFeatureStoreConfig
 from tecton_proto.data.feature_view_pb2 import DeltaOfflineStoreVersion
 from tecton_proto.data.feature_view_pb2 import ParquetOfflineStoreVersion
 
 
 TIME_PARTITION = "time_partition"
 SECONDS_TO_NANOSECONDS = 1000 * 1000 * 1000
 CONTINUOUS_PARTITION_SIZE_SECONDS = 86400
 
 
 class PartitionType(str, enum.Enum):
     DATE_STR = "DateString"
     EPOCH = "Epoch"
+    # RAW_TIMESTAMP is only used for Snowflake
+    RAW_TIMESTAMP = "RawTimestamp"
+
+
+class OfflineStoreType(str, enum.Enum):
+    PARQUET = "parquet"
+    DELTA = "delta"
+    SNOWFLAKE = "snowflake"
 
 
 @attrs.frozen
 class TimestampFormats:
     spark_format: str
     python_format: str
 
@@ -78,15 +88,15 @@
 
 PARQUET_SUPPORTED_VERSIONS = [
     ParquetOfflineStoreVersion.PARQUET_OFFLINE_STORE_VERSION_1,
     ParquetOfflineStoreVersion.PARQUET_OFFLINE_STORE_VERSION_2,
 ]
 
 
-def _check_supported_offline_store_version(fd: FeatureDefinition):
+def _check_supported_offline_store_version(fd: FeatureDefinition) -> None:
     if fd.offline_store_params is None:
         return
     if (
         fd.offline_store_params.HasField("delta")
         and fd.offline_store_params.delta.version not in DELTA_SUPPORTED_VERSIONS
     ):
         msg = (
@@ -97,14 +107,29 @@
         fd.offline_store_params.HasField("parquet")
         and fd.offline_store_params.parquet.version not in PARQUET_SUPPORTED_VERSIONS
     ):
         msg = f"Unsupported offline store version {fd.offline_store_params.parquet.version}. Try upgrading your Tecton SDK."
         raise TectonInternalError(msg)
 
 
+def get_offline_store_type(offline_store_config: OfflineFeatureStoreConfig) -> OfflineStoreType:
+    # TODO(TEC-15800): Update Snowflake FV protos to have snowflake as their store type
+    if sql_compat.dialect() == sql_compat.Dialect.SNOWFLAKE:
+        return OfflineStoreType.SNOWFLAKE
+
+    store_type = offline_store_config.WhichOneof("store_type")
+    if store_type == OfflineStoreType.PARQUET:
+        return OfflineStoreType.PARQUET
+    elif store_type == OfflineStoreType.DELTA:
+        return OfflineStoreType.DELTA
+    else:
+        msg = f"Unknown offline store type {store_type}"
+        raise TectonInternalError(msg)
+
+
 def get_offline_store_partition_params(feature_definition: FeatureDefinition) -> OfflineStorePartitionParams:
     # Examples of how our offline store is partitioned
     ### BWAFV on Delta
     # Partition Column: time_partition
     # Materialized Columns: _anchor_time, [join_keys], [feature_columns]
 
     ### Continuous SWAFV on Parquet
@@ -117,22 +142,31 @@
     # Materialized Columns: _anchor_time, [join_keys], [feature_columns]
     # !! In this case we need to drop the partition column from the top level columns
 
     ### BFV on Parquet
     # Partition Column: _anchor_time
     # Materialized Columns: ts, [join_keys], [feature_columns]
 
+    ### Any FV on Snowflake
+    # Partition Column: none
+    # Materialized Columns: ts, [join_keys], [feature_columns]
+
     _check_supported_offline_store_version(feature_definition)
     offline_store_config = feature_definition.offline_store_config
-    store_type = offline_store_config.WhichOneof("store_type")
-    if store_type == "delta":
+    store_type = get_offline_store_type(offline_store_config)
+
+    if store_type == OfflineStoreType.SNOWFLAKE:
+        partition_by = feature_definition.time_key
+        partition_type = PartitionType.RAW_TIMESTAMP
+        partition_interval = pendulum.Duration(seconds=0)
+    elif store_type == OfflineStoreType.DELTA:
         partition_by = TIME_PARTITION
         partition_type = PartitionType.DATE_STR
         partition_interval = partition_size_for_delta(feature_definition)
-    elif store_type == "parquet":
+    elif store_type == OfflineStoreType.PARQUET:
         partition_by = partition_col_for_parquet(feature_definition)
         partition_type = PartitionType.EPOCH
         partition_interval = partition_size_for_parquet(feature_definition)
     else:
         msg = "Unexpected offline store config"
         raise Exception(msg)
     return OfflineStorePartitionParams(partition_by, partition_type, partition_interval)
@@ -153,21 +187,21 @@
     aligned_time = time_utils.align_time_downwards(timestamp, partition_params.partition_interval.as_timedelta())
     # align_time_downwards returns the time without tzinfo. convert_timestamp_for_version calls timestamp() which
     # treats naive datetime instances as local time. This can cause an issue if local time is not in UTC.
     aligned_time = aligned_time.replace(tzinfo=datetime.timezone.utc)
     return time_utils.convert_timestamp_for_version(aligned_time, feature_store_format_version)
 
 
-def window_size_seconds(window: Union[timedelta, pendulum.Duration]):
+def window_size_seconds(window: Union[timedelta, pendulum.Duration]) -> int:
     if isinstance(window, pendulum.Duration):
         window = window.as_timedelta()
     if window % timedelta(seconds=1) != timedelta(0):
         msg = f"partition_size is not a round number of seconds: {window}"
         raise AssertionError(msg)
     return int(window.total_seconds())
 
 
-def _timestamp_formats(partition_size: timedelta):
+def _timestamp_formats(partition_size: timedelta) -> TimestampFormats:
     if partition_size % timedelta(days=1) == timedelta(0):
         return TimestampFormats(spark_format="yyyy-MM-dd", python_format="%Y-%m-%d")
     else:
         return TimestampFormats(spark_format="yyyy-MM-dd-HH:mm:ss", python_format="%Y-%m-%d-%H:%M:%S")
```

### Comparing `tecton-0.8.0b4/tecton_core/online_serving_index.py` & `tecton-0.8.0b5/tecton_core/online_serving_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,24 @@
     and queryable in FeatureServices that include this feature definition.
     For example, for a feature definition that has join keys ["user", "page"],
     if we pass OnlineServingIndex(["user"]), we will be able to invoke
     feature_service.query_features({"user": "user_1"})
     and get back feature vectors for all user-page pairs where user="user_1".
     """
 
-    def __init__(self, join_keys: List[str]):
+    def __init__(self, join_keys: List[str]) -> None:
         """
         Create a new OnlineServingIndex.
 
         :param join_keys: The partial join keys that will be indexed in the online feature store
         """
         self.join_keys = join_keys
 
     @classmethod
-    def from_proto(cls, proto: OnlineServingIndexProto):
+    def from_proto(cls, proto: OnlineServingIndexProto) -> "OnlineServingIndex":
         """Instantiates object from the provided proto object."""
         return cls(list(proto.join_keys))
 
     def to_proto(self):
         """Returns proto object created from the existing object."""
         proto = OnlineServingIndexProto()
         proto.join_keys.extend(self.join_keys)
```

### Comparing `tecton-0.8.0b4/tecton_core/pipeline_common.py` & `tecton-0.8.0b5/tecton_core/pipeline_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from tecton_core.id_helper import IdHelper
 from tecton_proto.args.pipeline_pb2 import ConstantNode
 from tecton_proto.args.pipeline_pb2 import DataSourceNode
 from tecton_proto.args.pipeline_pb2 import Input as InputProto
 from tecton_proto.args.pipeline_pb2 import Pipeline
 from tecton_proto.args.pipeline_pb2 import PipelineNode
 from tecton_proto.args.pipeline_pb2 import RequestContext as RequestContextProto
+from tecton_proto.args.pipeline_pb2 import TransformationNode
 
 
 CONSTANT_TYPE = Optional[Union[str, int, float, bool]]
 CONSTANT_TYPE_OBJECTS = (str, int, float, bool)
 
 
 def _make_mode_to_type() -> Dict[str, Any]:
@@ -58,27 +59,29 @@
         return constant_node.bool_const
     elif constant_node.HasField("null_const"):
         return None
     msg = f"Unknown ConstantNode type: {constant_node}"
     raise KeyError(msg)
 
 
-def get_keyword_inputs(transformation_node) -> Dict[str, InputProto]:
+def get_keyword_inputs(transformation_node: TransformationNode) -> Dict[str, InputProto]:
     """Returns the keyword inputs of transformation_node in a dict."""
     return {
         node_input.arg_name: node_input for node_input in transformation_node.inputs if node_input.HasField("arg_name")
     }
 
 
-def positional_inputs(transformation_node) -> List[InputProto]:
+def positional_inputs(transformation_node: TransformationNode) -> List[InputProto]:
     """Returns the positional inputs of transformation_node in order."""
     return [node_input for node_input in transformation_node.inputs if node_input.HasField("arg_index")]
 
 
-def transformation_type_checker(object_name, result, mode: str, supported_modes) -> None:
+def transformation_type_checker(
+    object_name: str, result: Any, mode: str, supported_modes: List[str]  # noqa: ANN401
+) -> None:
     possible_mode = None
     for candidate_mode, candidate_type in MODE_TO_TYPE_LOOKUP.items():
         if isinstance(result, candidate_type):
             possible_mode = candidate_mode
             break
     expected_type = MODE_TO_TYPE_LOOKUP[mode]
     actual_type = type(result)
```

### Comparing `tecton-0.8.0b4/tecton_core/pipeline_sql_builder.py` & `tecton-0.8.0b5/tecton_core/pipeline_sql_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ret: List[Tuple[str, str]] = []
         for i in subtree.transformation_node.inputs:
             if i.node.HasField("transformation_node"):
                 ret.extend(self._get_queries_helper(i.node))
         ret.append(self._get_query(subtree))
         return ret
 
-    def _node_to_value(self, pipeline_node: PipelineNode):
+    def _node_to_value(self, pipeline_node: PipelineNode) -> Any:  # noqa: ANN401
         """
         This returns the value of the node to be used as the input to the transformation_node that is its parent.
         The transformation defined by the user can look like:
         return f"SELECT {context.end_time} timestamp, d.* from {data_source} d join {transformation_output} t on d.x = t.y + {constant}"
         """
         if pipeline_node.HasField("transformation_node"):
             return unique_node_alias(pipeline_node)
```

### Comparing `tecton-0.8.0b4/tecton_core/query/aggregation_plans.py` & `tecton-0.8.0b5/tecton_core/query/aggregation_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,37 +52,37 @@
 
     def materialized_column_names(self, input_column_name: str) -> List[str]:
         return [f"{prefix}_{input_column_name}" for prefix in self.materialized_column_prefixes]
 
 
 def _get_simple_window_query(
     col: str, query_window_spec: QueryWindowSpec, analytic_function: WindowFrameAnalyticFunction
-):
+) -> Term:
     return (
         analytic_function(Field(col))
         .over(*[Field(x) for x in query_window_spec.partition_cols])
         .orderby(*[Field(query_window_spec.order_by_col)])
         .range(query_window_spec.range_start, query_window_spec.range_end)
     )
 
 
 def _simple_aggregation_plan(
     aggregation_function: afpb.AggregationFunction, analytic_function: WindowFrameAnalyticFunction
-):
+) -> Term:
     return AggregationPlan(
         partial_aggregation_query_terms=lambda col: [analytic_function(Field(col))],
         full_aggregation_query_term=lambda cols, query_window_spec: _get_simple_window_query(
             cols[0], query_window_spec, analytic_function
         ),
         materialized_column_prefixes=get_materialization_aggregation_column_prefixes(aggregation_function),
         continuous_aggregation_query_terms=lambda col: [Field(col)],
     )
 
 
-def _mean_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec):
+def _mean_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec) -> Term:
     mean_col, count_col = cols
     sum_query_term = (
         Sum(Field(mean_col) * Field(count_col))
         .over(*[Field(x) for x in query_window_spec.partition_cols])
         .orderby(*[Field(query_window_spec.order_by_col)])
         .range(query_window_spec.range_start, query_window_spec.range_end)
     )
@@ -92,15 +92,15 @@
         .orderby(*[Field(query_window_spec.order_by_col)])
         .range(query_window_spec.range_start, query_window_spec.range_end)
     )
     return sum_query_term / count_query_term
 
 
 # sample variation equation: (Σ(x^2) - (Σ(x)^2)/N)/N-1
-def _var_samp_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec):
+def _var_samp_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec) -> Term:
     sum_of_squares_col, count_col, sum_col = cols
     count_query_term = Cast(
         (
             Sum(Field(count_col))
             .over(*[Field(x) for x in query_window_spec.partition_cols])
             .orderby(*[Field(query_window_spec.order_by_col)])
             .range(query_window_spec.range_start, query_window_spec.range_end)
@@ -128,15 +128,15 @@
     # check if count is equal to 0 for divide by 0 errors
     var_samp_col = (sum_of_squares_query_term - (sum_query_term**2) / count_query_term) / NullIf(
         count_query_term - 1, 0
     )
     return var_samp_col
 
 
-def _var_pop_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec):
+def _var_pop_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec) -> Term:
     sum_of_squares_col, count_col, sum_col = cols
     count_query_term = Cast(
         (
             Sum(Field(count_col))
             .over(*[Field(x) for x in query_window_spec.partition_cols])
             .orderby(*[Field(query_window_spec.order_by_col)])
             .range(query_window_spec.range_start, query_window_spec.range_end)
@@ -160,23 +160,23 @@
             .range(query_window_spec.range_start, query_window_spec.range_end)
         ),
         "double",
     )
     return (sum_of_squares_query_term / count_query_term) - (sum_query_term / count_query_term) ** 2
 
 
-def _stddev_samp_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec):
+def _stddev_samp_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec) -> Term:
     return Sqrt(_var_samp_full_aggregation(cols, query_window_spec))
 
 
-def _stddev_pop_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec):
+def _stddev_pop_full_aggregation(cols: List[str], query_window_spec: QueryWindowSpec) -> Term:
     return Sqrt(_var_pop_full_aggregation(cols, query_window_spec))
 
 
-def _mean_aggregation_plan():
+def _mean_aggregation_plan() -> AggregationPlan:
     return AggregationPlan(
         partial_aggregation_query_terms=lambda col: [Avg(Field(col)), Count(Field(col))],
         full_aggregation_query_term=lambda cols, query_window_spec: _mean_full_aggregation(cols, query_window_spec),
         materialized_column_prefixes=get_materialization_aggregation_column_prefixes(afpb.AGGREGATION_FUNCTION_MEAN),
         continuous_aggregation_query_terms=lambda col: [Cast(Field(col), "double"), Cast(LiteralValue("1"), "bigint")],
     )
```

### Comparing `tecton-0.8.0b4/tecton_core/query/builder.py` & `tecton-0.8.0b5/tecton_core/query/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from tecton_core import specs
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
 from tecton_core.feature_definition_wrapper import pipeline_to_ds_inputs
 from tecton_core.feature_set_config import FeatureDefinitionAndJoinConfig
 from tecton_core.feature_set_config import FeatureSetConfig
 from tecton_core.feature_set_config import find_dependent_feature_set_items
 from tecton_core.pipeline_common import get_time_window_from_data_source_node
+from tecton_core.query.executor_params import QueryTreeComputeType
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.nodes import AddAnchorTimeNode
 from tecton_core.query.nodes import AddDurationNode
 from tecton_core.query.nodes import AddEffectiveTimestampNode
 from tecton_core.query.nodes import AddRetrievalAnchorTimeNode
+from tecton_core.query.nodes import AddUniqueIdNode
 from tecton_core.query.nodes import AggregationSecondaryKeyExplodeNode
 from tecton_core.query.nodes import AggregationSecondaryKeyRollupNode
 from tecton_core.query.nodes import AsofJoinFullAggNode
 from tecton_core.query.nodes import AsofJoinInputContainer
 from tecton_core.query.nodes import AsofJoinNode
 from tecton_core.query.nodes import AsofSecondaryKeyExplodeNode
 from tecton_core.query.nodes import ConvertEpochToTimestampNode
@@ -36,25 +38,28 @@
 from tecton_core.query.nodes import MultiOdfvPipelineNode
 from tecton_core.query.nodes import OfflineStoreScanNode
 from tecton_core.query.nodes import PartialAggNode
 from tecton_core.query.nodes import RenameColsNode
 from tecton_core.query.nodes import RespectFeatureStartTimeNode
 from tecton_core.query.nodes import RespectTTLNode
 from tecton_core.query.nodes import SelectDistinctNode
+from tecton_core.query.nodes import StagingNode
 from tecton_core.query.nodes import StreamWatermarkNode
 from tecton_core.query.nodes import WildcardJoinNode
 from tecton_core.query.sql_compat import default_case
 from tecton_core.query_consts import ANCHOR_TIME
 from tecton_core.query_consts import EFFECTIVE_TIMESTAMP
 from tecton_core.query_consts import EXPIRATION_TIMESTAMP
+from tecton_core.query_consts import ODFV_INTERNAL_STAGING_TABLE
+from tecton_core.query_consts import TECTON_UNIQUE_ID_COL
 from tecton_core.query_consts import UDF_INTERNAL
 from tecton_proto.args.pipeline_pb2 import DataSourceNode as ProtoDataSourceNode
 
 
-WINDOW_END_COLUMN_NAME = "tile_end_time"
+WINDOW_END_COLUMN_NAME = default_case("tile_end_time")
 
 
 def build_datasource_scan_node(
     ds: specs.DataSourceSpec,
     for_stream: bool,
     start_time: Optional[datetime] = None,
     end_time: Optional[datetime] = None,
@@ -164,27 +169,33 @@
     tree = build_pipeline_querytree(fdw, for_stream, feature_data_time_limits)
     if for_stream:
         watermark = get_stream_watermark(fdw)
         if watermark:
             tree = StreamWatermarkNode(tree, fdw.time_key, watermark).as_ref()
     if enable_feature_metrics:
         tree = MetricsCollectorNode(tree).as_ref()
-    anchor_time_field = default_case(ANCHOR_TIME)
+    anchor_time_field = ANCHOR_TIME
     if fdw.is_temporal:
         # BFVs require an anchor time column, but SFVs do not.
         if not for_stream:
             assert not include_window_end_time, "Not supported window end time for temporal"
             tree = AddAnchorTimeNode(
                 tree,
                 feature_store_format_version=fdw.get_feature_store_format_version,
                 batch_schedule=fdw.get_batch_schedule_for_version,
                 timestamp_field=fdw.timestamp_key,
             ).as_ref()
+        tree = StagingNode(
+            input_node=tree, staging_table_name=f"{fdw.name}", query_tree_stage=QueryTreeComputeType.STAGING
+        ).as_ref()
     elif fdw.is_temporal_aggregate:
-        window_end_column_name = default_case(WINDOW_END_COLUMN_NAME) if include_window_end_time else None
+        window_end_column_name = WINDOW_END_COLUMN_NAME if include_window_end_time else None
+        tree = StagingNode(
+            input_node=tree, staging_table_name=f"{fdw.name}", query_tree_stage=QueryTreeComputeType.STAGING
+        ).as_ref()
         tree = PartialAggNode(
             tree,
             fdw=fdw,
             window_start_column_name=anchor_time_field,
             window_end_column_name=window_end_column_name,
             aggregation_anchor_time=aggregation_anchor_time,
         ).as_ref()
@@ -195,15 +206,15 @@
 
 
 def build_get_features(
     fdw: FeatureDefinitionWrapper,
     from_source: Optional[bool],
     feature_data_time_limits: Optional[pendulum.Period] = None,
     aggregation_anchor_time: Optional[datetime] = None,
-):
+) -> NodeRef:
     # NOTE: this is ideally the *only* place where we validate
     # from_source arguments. However, until Snowflake and Athena are migrated
     # to QueryTree, we also need validations to live in the interactive/unified
     # SDK.
     #
     # Behavior:
     #   from_source is True: force compute from source
@@ -240,44 +251,49 @@
 def build_get_full_agg_features(
     fdw: FeatureDefinitionWrapper,
     from_source: Optional[bool],
     feature_data_time_limits: Optional[pendulum.Period] = None,
     respect_feature_start_time: bool = True,
     aggregation_anchor_time: Optional[datetime] = None,
     show_effective_time: bool = False,
-):
+) -> NodeRef:
     partial_aggs = build_get_features(
         fdw,
         from_source,
         feature_data_time_limits=feature_data_time_limits,
         aggregation_anchor_time=aggregation_anchor_time,
     )
 
     if fdw.aggregation_secondary_key:
         cols_to_drop = list(
-            set(partial_aggs.columns) - set(list(fdw.join_keys) + [ANCHOR_TIME, fdw.aggregation_secondary_key])
+            set(partial_aggs.columns) - {*list(fdw.join_keys), ANCHOR_TIME, fdw.aggregation_secondary_key}
         )
         spine = AggregationSecondaryKeyExplodeNode(
             input_node=RenameColsNode(partial_aggs, drop=cols_to_drop).as_ref(),
             fdw=fdw,
         ).as_ref()
     else:
-        cols_to_drop = list(set(partial_aggs.columns) - set(list(fdw.join_keys) + [ANCHOR_TIME]))
+        cols_to_drop = list(set(partial_aggs.columns) - {*list(fdw.join_keys), ANCHOR_TIME})
         spine = RenameColsNode(partial_aggs, drop=cols_to_drop).as_ref()
 
     full_aggregation_node = AsofJoinFullAggNode(
         spine=spine,
         partial_agg_node=partial_aggs,
         fdw=fdw,
+        # Do not push down the timestamp if the spine is completely from partial agg, such as `ghf` and `run` with time
+        # range.
+        enable_spine_time_pushdown_rewrite=False,
+        enable_spine_entity_pushdown_rewrite=False,
     ).as_ref()
 
     if fdw.aggregation_secondary_key:
         full_aggregation_node = AggregationSecondaryKeyRollupNode(
             full_aggregation_node=full_aggregation_node,
             fdw=fdw,
+            group_by_columns=[*list(fdw.join_keys), ANCHOR_TIME],
         ).as_ref()
 
     if respect_feature_start_time and fdw.feature_start_timestamp:
         full_aggregation_node = RespectFeatureStartTimeNode.for_anchor_time_column(
             full_aggregation_node, ANCHOR_TIME, fdw
         ).as_ref()
 
@@ -308,30 +324,35 @@
             is_temporal_aggregate=True,
         ).as_ref()
 
     return qt
 
 
 def build_spine_join_querytree(
-    dac: FeatureDefinitionAndJoinConfig, spine_node: NodeRef, spine_time_field: str, from_source: Optional[bool]
+    dac: FeatureDefinitionAndJoinConfig,
+    spine_node: NodeRef,
+    spine_time_field: str,
+    from_source: Optional[bool],
+    use_namespace_feature_prefix: bool = True,
 ) -> NodeRef:
     fdw = dac.feature_definition
     if fdw.timestamp_key is not None and spine_time_field != fdw.timestamp_key:
         spine_node = RenameColsNode(spine_node, mapping={spine_time_field: fdw.timestamp_key}).as_ref()
-    if any([jk[0] != jk[1] for jk in dac.join_keys]):
+    if any(jk[0] != jk[1] for jk in dac.join_keys):
         spine_node = RenameColsNode(
             spine_node, mapping={jk[0]: jk[1] for jk in dac.join_keys if jk[0] != jk[1]}
         ).as_ref()
 
     if fdw.is_temporal or fdw.is_feature_table:
         ret = _build_spine_query_tree_temporal_or_feature_table(
             spine_node=spine_node,
             dac=dac,
             data_delay_seconds=fdw.online_store_data_delay_seconds,
             from_source=from_source,
+            use_namespace_feature_prefix=use_namespace_feature_prefix,
         )
     elif fdw.is_temporal_aggregate:
         partial_agg_node = build_get_features(
             fdw,
             from_source=from_source,
             # NOTE: feature_data_time_limits is set to None since time pushdown
             # should happen as part of a optimization rewrite.
@@ -341,110 +362,136 @@
 
         augmented_spine = _augment_spine_for_window_aggregation(fdw, spine_node, partial_agg_node)
 
         full_agg_node = AsofJoinFullAggNode(
             spine=augmented_spine,
             partial_agg_node=partial_agg_node,
             fdw=fdw,
+            # Allow timestamp push down if the spine is provided by users.
+            enable_spine_time_pushdown_rewrite=True,
+            enable_spine_entity_pushdown_rewrite=True,
         ).as_ref()
 
         if fdw.aggregation_secondary_key:
             full_agg_node = AggregationSecondaryKeyRollupNode(
                 full_aggregation_node=full_agg_node,
                 fdw=fdw,
+                # Beside join keys and anchor time, we need to group by timestamp_key and TECTON_UNIQUE_ID_COL because:
+                #   1. Grouping by timestamp_key is required to keep the timestamp column in the result.
+                #   2. Grouping by TECTON_UNIQUE_ID_COL can distinguish duplicated rows in the spine.
+                group_by_columns=[*list(fdw.join_keys), ANCHOR_TIME, fdw.timestamp_key, TECTON_UNIQUE_ID_COL],
             ).as_ref()
+            full_agg_node = RenameColsNode(full_agg_node, drop=[TECTON_UNIQUE_ID_COL]).as_ref()
 
         if fdw.feature_start_timestamp:
-            full_agg_node = RespectFeatureStartTimeNode.for_anchor_time_column(
-                full_agg_node, default_case(ANCHOR_TIME), fdw
-            ).as_ref()
-        ret = _rename_feature_columns_and_drop_non_feature_columns(dac, full_agg_node)
+            full_agg_node = RespectFeatureStartTimeNode.for_anchor_time_column(full_agg_node, ANCHOR_TIME, fdw).as_ref()
+        ret = _rename_feature_columns_and_drop_non_feature_columns(dac, full_agg_node, use_namespace_feature_prefix)
     elif fdw.is_on_demand:
         inputs = find_dependent_feature_set_items(
             fdw.fco_container,
             fdw.pipeline.root,
             visited_inputs={},
             fv_id=fdw.id,
         )
         dac = FeatureDefinitionAndJoinConfig.from_feature_definition(fdw)
-        fsc = FeatureSetConfig(inputs + [dac])
-        ret = build_feature_set_config_querytree(fsc, spine_node, spine_time_field, from_source)
+        fsc = FeatureSetConfig([*inputs, dac])
+        ret = build_feature_set_config_querytree(
+            fsc, spine_node, spine_time_field, from_source, use_namespace_feature_prefix
+        )
     else:
         raise NotImplementedError
     if fdw.timestamp_key is not None and spine_time_field != fdw.timestamp_key:
         ret = RenameColsNode(ret, {fdw.timestamp_key: spine_time_field}).as_ref()
-    if any([jk[0] != jk[1] for jk in dac.join_keys]):
+    if any(jk[0] != jk[1] for jk in dac.join_keys):
         ret = RenameColsNode(ret, {jk[1]: jk[0] for jk in dac.join_keys if jk[0] != jk[1]}).as_ref()
     return ret
 
 
-def _update_internal_cols(fdw: FeatureDefinitionWrapper, dac: FeatureDefinitionAndJoinConfig, internal_cols: Set[str]):
+def _update_internal_cols(
+    fdw: FeatureDefinitionWrapper, dac: FeatureDefinitionAndJoinConfig, internal_cols: Set[str]
+) -> None:
     if dac.namespace.startswith(UDF_INTERNAL):
         for feature in fdw.features:
             internal_cols.add(dac.namespace + fdw.namespace_separator + feature)
     for feature in dac.features:
         if UDF_INTERNAL in feature:
             internal_cols.add(feature)
 
 
 # Construct each wildcard materialized fvtree by joining against distinct set of join keys.
 # Then, outer join these using WildcardJoinNode which performs an outer join while handling null-valued features properly.
-def _build_wild_fv_subtree(spine_node, fv_dacs, spine_time_field, from_source) -> NodeRef:
+def _build_wild_fv_subtree(
+    spine_node: NodeRef,
+    fv_dacs: List[FeatureDefinitionAndJoinConfig],
+    spine_time_field: str,
+    from_source: Optional[bool],
+) -> NodeRef:
     newtree = None
     for dac in fv_dacs:
         fdw = dac.feature_definition
 
         subspine_join_keys = [jk[0] for jk in dac.join_keys if jk[0] != fdw.wildcard_join_key]
         # SelectDistinctNode is needed for correctness in order to filter out rows with duplicate join keys before
         # retrieving feature values. This avoids exploding wildcard rows when there are duplicates in both the spine and the
         # feature view tree.
-        subspine = SelectDistinctNode(spine_node, subspine_join_keys + [spine_time_field]).as_ref()
+        subspine = SelectDistinctNode(spine_node, [*subspine_join_keys, spine_time_field]).as_ref()
         fvtree = build_spine_join_querytree(dac, subspine, spine_time_field, from_source)
         if len(dac.features) < len(fdw.features):
             fvtree = RenameColsNode(
                 fvtree,
                 drop=[f"{fdw.name}{fdw.namespace_separator}{f}" for f in fdw.features if f not in dac.features],
             ).as_ref()
         if newtree is None:
             newtree = fvtree
         else:
-            join_cols = subspine_join_keys + [spine_time_field, fdw.wildcard_join_key]
+            join_cols = [*subspine_join_keys, spine_time_field, fdw.wildcard_join_key]
             newtree = WildcardJoinNode(newtree, fvtree, join_cols=join_cols).as_ref()
     return newtree
 
 
 # Construct each non-wildcard materialized fvtree by joining against distinct set of join keys.
 # Then, outer join these fvtrees together.
-def _build_standard_fv_subtree(spine_node, fv_dacs, spine_time_field, from_source):
+def _build_standard_fv_subtree(
+    spine_node: NodeRef,
+    fv_dacs: List[FeatureDefinitionAndJoinConfig],
+    spine_time_field: str,
+    from_source: Optional[bool],
+) -> Tuple[NodeRef, Set[str]]:
     newtree = spine_node
-    internal_cols = set()
+    internal_cols: Set[str] = set()
     for dac in fv_dacs:
         fdw = dac.feature_definition
         _update_internal_cols(fdw, dac, internal_cols)
 
         subspine_join_keys = [jk[0] for jk in dac.join_keys]
         # SelectDistinctNode is needed for correctness in the case that there are duplicate rows in the spine. The
         # alternative considered was to add a row_id as a hash of the row or a monotonically increasing id, however the
         # row_id as a hash is not unique for duplicate rows and a monotonically increasing id is non-deterministic.
-        subspine = SelectDistinctNode(spine_node, subspine_join_keys + [spine_time_field]).as_ref()
+        subspine = SelectDistinctNode(spine_node, [*subspine_join_keys, spine_time_field]).as_ref()
         fvtree = build_spine_join_querytree(dac, subspine, spine_time_field, from_source)
         if len(dac.features) < len(fdw.features):
             fvtree = RenameColsNode(
                 fvtree,
                 drop=[f"{fdw.name}{fdw.namespace_separator}{f}" for f in fdw.features if f not in dac.features],
             ).as_ref()
-        newtree = JoinNode(newtree, fvtree, how="inner", join_cols=subspine_join_keys + [spine_time_field]).as_ref()
+        newtree = JoinNode(newtree, fvtree, how="inner", join_cols=[*subspine_join_keys, spine_time_field]).as_ref()
     return newtree, internal_cols
 
 
 # Compute odfvs via udf on the parent (not using joins)
-def _build_odfv_subtree(parent_tree: NodeRef, odfv_dacs: List[FeatureDefinitionAndJoinConfig]):
-    newtree = parent_tree
+def _build_odfv_subtree(
+    parent_tree: NodeRef, odfv_dacs: List[FeatureDefinitionAndJoinConfig], use_namespace_feature_prefix: bool = True
+) -> NodeRef:
+    newtree = StagingNode(
+        input_node=parent_tree,
+        staging_table_name=ODFV_INTERNAL_STAGING_TABLE,
+        query_tree_stage=QueryTreeComputeType.AGGREGATION,
+    ).as_ref()
     feature_definitions_namespaces = [(dac.feature_definition, dac.namespace) for dac in odfv_dacs]
-    newtree = MultiOdfvPipelineNode(newtree, feature_definitions_namespaces).as_ref()
+    newtree = MultiOdfvPipelineNode(newtree, feature_definitions_namespaces, use_namespace_feature_prefix).as_ref()
 
     # Compute the union of the features to be computed
     dac_features = set()
     fdw_features = set()
     for dac in odfv_dacs:
         feature_prefix = f"{dac.namespace}{dac.feature_definition.namespace_separator}"
         dac_features.update({f"{feature_prefix}{f}" for f in dac.features})
@@ -459,15 +506,19 @@
     return newtree
 
 
 # Construct each materialized fvtree by joining against distinct set of join keys.
 # Then, join the full spine against each of those.
 # Finally, compute odfvs via udf on top of the result (not using joins)
 def build_feature_set_config_querytree(
-    fsc: FeatureSetConfig, spine_node: NodeRef, spine_time_field: str, from_source: Optional[bool]
+    fsc: FeatureSetConfig,
+    spine_node: NodeRef,
+    spine_time_field: str,
+    from_source: Optional[bool],
+    use_namespace_feature_prefix: bool = True,
 ) -> NodeRef:
     odfv_dacs: List[FeatureDefinitionAndJoinConfig] = []
     wildcard_dacs: List[FeatureDefinitionAndJoinConfig] = []
     normal_fv_dacs: List[FeatureDefinitionAndJoinConfig] = []
 
     for dac in fsc.definitions_and_configs:
         if dac.feature_definition.is_on_demand:
@@ -483,81 +534,82 @@
             normal_fv_dacs.append(dac)
 
     if wildcard_dacs:
         newtree = _build_wild_fv_subtree(spine_node, wildcard_dacs, spine_time_field, from_source)
     else:
         newtree = spine_node
 
-    internal_cols = set()
+    internal_cols: Set[str] = set()
     if normal_fv_dacs:
         newtree, internal_cols = _build_standard_fv_subtree(newtree, normal_fv_dacs, spine_time_field, from_source)
 
     if odfv_dacs:
-        newtree = _build_odfv_subtree(newtree, odfv_dacs)
+        newtree = _build_odfv_subtree(newtree, odfv_dacs, use_namespace_feature_prefix)
 
     # drop all internal cols
     if len(internal_cols) > 0:
         newtree = RenameColsNode(newtree, drop=list(internal_cols)).as_ref()
 
     return newtree
 
 
 def _build_spine_query_tree_temporal_or_feature_table(
-    spine_node: NodeRef, dac: FeatureDefinitionAndJoinConfig, data_delay_seconds: int, from_source: Optional[bool]
-):
+    spine_node: NodeRef,
+    dac: FeatureDefinitionAndJoinConfig,
+    data_delay_seconds: int,
+    from_source: Optional[bool],
+    use_namespace_feature_prefix: bool = True,
+) -> NodeRef:
     fdw = dac.feature_definition
     TIMESTAMP_PLUS_TTL = default_case("_timestamp_plus_ttl")
     base = build_get_features(fdw, from_source=from_source)
     batch_schedule_seconds = 0 if fdw.is_feature_table else fdw.batch_materialization_schedule.in_seconds()
     base = AddEffectiveTimestampNode(
         base,
         timestamp_field=fdw.timestamp_key,
-        effective_timestamp_name=default_case(EFFECTIVE_TIMESTAMP),
+        effective_timestamp_name=EFFECTIVE_TIMESTAMP,
         batch_schedule_seconds=batch_schedule_seconds,
         data_delay_seconds=data_delay_seconds,
         is_stream=fdw.is_stream,
         is_temporal_aggregate=False,
     ).as_ref()
     if fdw.serving_ttl is not None:
         base = AddDurationNode(
             base, timestamp_field=fdw.timestamp_key, duration=fdw.serving_ttl, new_column_name=TIMESTAMP_PLUS_TTL
         ).as_ref()
         # Calculate effective expiration time = window(feature_time + ttl, batch_schedule).end + data_delay
         batch_schedule_seconds = 0 if fdw.is_feature_table else fdw.batch_materialization_schedule.in_seconds()
         base = AddEffectiveTimestampNode(
             base,
             timestamp_field=TIMESTAMP_PLUS_TTL,
-            effective_timestamp_name=default_case(EXPIRATION_TIMESTAMP),
+            effective_timestamp_name=EXPIRATION_TIMESTAMP,
             batch_schedule_seconds=batch_schedule_seconds,
             data_delay_seconds=data_delay_seconds,
             is_stream=fdw.is_stream,
             is_temporal_aggregate=False,
         ).as_ref()
     rightside_join_prefix = default_case("_tecton_right")
     join_prefixed_feature_names = [f"{rightside_join_prefix}_{f}" for f in fdw.features]
+    prefix = f"{dac.namespace}{fdw.namespace_separator}" if use_namespace_feature_prefix else ""
     # we can't just ask for the correct right_prefix to begin with because the asofJoin always sticks an extra underscore in between
-    rename_map: Dict[str, Optional[str]] = {
-        f"{rightside_join_prefix}_{f}": f"{dac.namespace}{fdw.namespace_separator}{f}"
-        for f in fdw.features
-        if f in dac.features
-    }
+    rename_map: Dict[str, Optional[str]] = {}
     cols_to_drop = []
     for f in fdw.features:
         if f not in dac.features:
             cols_to_drop.append(f"{rightside_join_prefix}_{f}")
         else:
-            rename_map[f"{rightside_join_prefix}_{f}"] = f"{dac.namespace}{fdw.namespace_separator}{f}"
+            rename_map[f"{rightside_join_prefix}_{f}"] = f"{prefix}{f}"
 
-    expiration_timestamp_col = f"{rightside_join_prefix}_{default_case(EXPIRATION_TIMESTAMP)}"
+    expiration_timestamp_col = f"{rightside_join_prefix}_{EXPIRATION_TIMESTAMP}"
 
     cols_to_drop.append(f"{rightside_join_prefix}_{fdw.timestamp_key}")
-    cols_to_drop.append(f"{rightside_join_prefix}_{default_case(ANCHOR_TIME)}")
-    cols_to_drop.append(f"{rightside_join_prefix}_{default_case(EFFECTIVE_TIMESTAMP)}")
+    cols_to_drop.append(f"{rightside_join_prefix}_{ANCHOR_TIME}")
+    cols_to_drop.append(f"{rightside_join_prefix}_{EFFECTIVE_TIMESTAMP}")
     if fdw.serving_ttl is not None:
-        cols_to_drop.append(f"{rightside_join_prefix}_{default_case(TIMESTAMP_PLUS_TTL)}")
+        cols_to_drop.append(f"{rightside_join_prefix}_{TIMESTAMP_PLUS_TTL}")
         cols_to_drop.append(expiration_timestamp_col)
 
     if fdw.feature_start_timestamp is not None:
         base = RespectFeatureStartTimeNode(
             base, fdw.timestamp_key, fdw.feature_start_timestamp, fdw.features, fdw.get_feature_store_format_version
         ).as_ref()
 
@@ -569,15 +621,15 @@
         ).as_ref()
 
     base = AsofJoinNode(
         left_container=AsofJoinInputContainer(spine_node, fdw.timestamp_key),
         right_container=AsofJoinInputContainer(
             base,
             timestamp_field=fdw.timestamp_key,
-            effective_timestamp_field=default_case(EFFECTIVE_TIMESTAMP),
+            effective_timestamp_field=EFFECTIVE_TIMESTAMP,
             prefix=rightside_join_prefix,
             schema=fdw.view_schema,
         ),
         join_cols=fdw.join_keys,
     ).as_ref()
 
     if fdw.serving_ttl is not None:
@@ -604,24 +656,35 @@
     #     1. A Feature View with an aggregation_secondary_key: an aggregation_secondary_key is never in the spine,
     #     so we always need to explode the spine for it.
     #     2. A Feature View with a wild card join key: a wild card join key is optional in the spine, so we need to
     #     check if the wild card join key is not in the spine before exploding the spine for it.
     is_wildcard_join_key_not_in_spine = fdw.wildcard_join_key and fdw.wildcard_join_key not in spine_node.columns
     is_secondary_key_agg = fdw.aggregation_secondary_key is not None
     if is_wildcard_join_key_not_in_spine or is_secondary_key_agg:
+        # Add a unique id column if aggreagtion secondary key appears. The unique id column is used to make each spine
+        # row unique so later the secondary key aggregation rollup doesn't merge duplicate rows.
+        if is_secondary_key_agg:
+            augmented_spine = AddUniqueIdNode(augmented_spine).as_ref()
+
         return AsofSecondaryKeyExplodeNode(
-            augmented_spine, default_case(ANCHOR_TIME), partial_agg_node, default_case(ANCHOR_TIME), fdw
+            augmented_spine,
+            ANCHOR_TIME,
+            partial_agg_node,
+            ANCHOR_TIME,
+            fdw,
         ).as_ref()
 
     return augmented_spine
 
 
-def _rename_feature_columns_and_drop_non_feature_columns(dac: FeatureDefinitionAndJoinConfig, node: NodeRef) -> NodeRef:
+def _rename_feature_columns_and_drop_non_feature_columns(
+    dac: FeatureDefinitionAndJoinConfig, node: NodeRef, use_namespace_feature_prefix: bool = True
+) -> NodeRef:
     rename_map: Dict[str, Optional[str]] = {}
-    cols_to_drop = [default_case(ANCHOR_TIME)]
+    cols_to_drop = [ANCHOR_TIME]
     for f in dac.feature_definition.features:
         if f not in dac.features:
             cols_to_drop.append(f)
-        else:
+        elif use_namespace_feature_prefix:
             # TODO: make a helper
             rename_map[f] = f"{dac.namespace}{dac.feature_definition.namespace_separator}{f}"
     return RenameColsNode(node, mapping=rename_map, drop=cols_to_drop).as_ref()
```

### Comparing `tecton-0.8.0b4/tecton_core/query/node_interface.py` & `tecton-0.8.0b5/tecton_core/query/node_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import attrs
+import pandas as pd
 import pypika
 import sqlparse
 
 from tecton_core.vendor.treelib import Tree
 
 
 INDENT_BLOCK = "  "
@@ -76,19 +77,23 @@
             node_columns.append(f"<{unique_id}> " + f"{'|'.join(node.columns)}")
 
         return tree_str + "\n" + "\n".join(node_columns)
 
     def _to_query(self) -> pypika.Query:
         return self.node._to_query()
 
-    def to_sql(self) -> str:
+    def to_sql(self, pretty_sql: bool = False) -> str:
         """
         Attempts to recursively generate sql for this and child nodes.
+
+        Args:
+            pretty_sql: If True, the sql will be reformatted and returned as a more readable, multiline string. If False,
+            the SQL will be returned as a one line string. For long queries, using pretty_sql=False has better performance.
         """
-        return self.node.to_sql()
+        return self.node.to_sql(pretty_sql=pretty_sql)
 
     def create_tree(self, node_id: bool = True, name: bool = True, description: bool = True) -> Tree:
         """Creates a Tree to represent the query tree which has this NodeRef as the root node.
 
         The Tree is built so that it can immediately generate a string representation.
 
         Args:
@@ -105,15 +110,15 @@
         self,
         tree: Tree,
         prefix: str = "",
         parent_id: Optional[int] = None,
         node_id: bool = True,
         name: bool = True,
         description: bool = True,
-    ):
+    ) -> Tree:
         tag = ""
 
         # Node ids are assigned sequentially, starting with 1.
         unique_id = tree.size() + 1
         if node_id:
             tag += f"<{unique_id}> "
 
@@ -203,22 +208,29 @@
     @abstractmethod
     def as_str(self) -> str:
         """
         Prints contents of this node and calls recursively on its inputs.
         Used by tecton.TectonDataFrame.explain
         """
 
-    def to_sql(self) -> str:
+    def to_sql(self, pretty_sql: bool = False) -> str:
         """
         Attempts to recursively generate sql for this and child nodes.
+
+        Args:
+            pretty_sql: If True, the sql will be reformatted and returned as a more readable, multiline string. If False,
+            the SQL will be returned as a one line string. For long queries, using pretty_sql=False has better performance.
         """
         sql_str = self._to_query().get_sql()
-        return sqlparse.format(sql_str, reindent=True)
+        if pretty_sql:
+            # This can take a very long time for long queries
+            return sqlparse.format(sql_str, reindent=True)
+        return sql_str
 
-    def get_sql_views(self) -> List[Tuple[str, str]]:
+    def get_sql_views(self, pretty_sql: bool = False) -> List[Tuple[str, str]]:
         """
         Get optional sql views for this node. List of Tuple(view_name, view_sql)
         """
         return []
 
     @abstractmethod
     def _to_query(self) -> pypika.Query:
@@ -230,15 +242,15 @@
 class DataframeWrapper(ABC):
     """
     A wrapper around pyspark, pandas, snowflake, etc dataframes provides a common interface through which we
     can register views.
     """
 
     @property
-    def _dataframe(self) -> Any:
+    def _dataframe(self) -> Any:  # noqa: ANN401
         """
         The underlying dataframe
         """
         raise NotImplementedError
 
     @property
     def columns(self) -> List[str]:
@@ -257,15 +269,18 @@
     @property
     def _temp_table_name(self):
         """
         Gets the temp view name registered by register()
         """
         return f"TMP_TABLE_{id(self._dataframe)}"
 
+    def to_pandas(self) -> pd.DataFrame:
+        raise NotImplementedError
+
     def to_spark(self):
         raise NotImplementedError
 
 
-def recurse_query_tree(node_ref: NodeRef, f: Callable):
+def recurse_query_tree(node_ref: NodeRef, f: Callable) -> None:
     f(node_ref.node)
     for child in node_ref.inputs:
         recurse_query_tree(child, f)
```

### Comparing `tecton-0.8.0b4/tecton_core/query/nodes.py` & `tecton-0.8.0b5/tecton_core/query/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import attrs
 import pendulum
 import pypika
+import sqlparse
 from pypika import NULL
 from pypika import AliasedQuery
 from pypika import Case
 from pypika import Database
 from pypika import Field
 from pypika import Table
 from pypika import analytics as an
@@ -24,70 +25,90 @@
 from tecton_core import conf
 from tecton_core import specs
 from tecton_core import time_utils
 from tecton_core.errors import TectonAthenaNotImplementedError
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
 from tecton_core.materialization_context import BoundMaterializationContext
 from tecton_core.offline_store import TIME_PARTITION
+from tecton_core.offline_store import OfflineStorePartitionParams
+from tecton_core.offline_store import OfflineStoreType
 from tecton_core.offline_store import PartitionType
 from tecton_core.offline_store import get_offline_store_partition_params
+from tecton_core.offline_store import get_offline_store_type
 from tecton_core.offline_store import timestamp_to_partition_date_str
 from tecton_core.offline_store import timestamp_to_partition_epoch
 from tecton_core.pipeline_sql_builder import PipelineSqlBuilder
 from tecton_core.query.aggregation_plans import AGGREGATION_PLANS
 from tecton_core.query.aggregation_plans import QueryWindowSpec
+from tecton_core.query.executor_params import QueryTreeComputeType
 from tecton_core.query.node_interface import DataframeWrapper
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.node_interface import QueryNode
 from tecton_core.query.sql_compat import CustomQuery
+from tecton_core.query.sql_compat import Dialect
 from tecton_core.query.sql_compat import LastValue
 from tecton_core.query.sql_compat import Query
 from tecton_core.query.sql_compat import convert_epoch_seconds_to_feature_store_format_version
 from tecton_core.query.sql_compat import convert_epoch_term_in_seconds
 from tecton_core.query.sql_compat import date_add
 from tecton_core.query.sql_compat import default_case
+from tecton_core.query.sql_compat import dialect
 from tecton_core.query.sql_compat import from_unixtime
 from tecton_core.query.sql_compat import struct
 from tecton_core.query.sql_compat import struct_extract
 from tecton_core.query.sql_compat import to_timestamp
 from tecton_core.query.sql_compat import to_unixtime
 from tecton_core.query_consts import ANCHOR_TIME
+from tecton_core.query_consts import TECTON_UNIQUE_ID_COL
 from tecton_core.schema import Schema
 from tecton_core.time_utils import convert_duration_to_seconds
 from tecton_core.time_utils import convert_epoch_to_datetime
 from tecton_core.time_utils import convert_timedelta_for_version
 from tecton_proto.args.pipeline_pb2 import DataSourceNode
 from tecton_proto.common.data_source_type_pb2 import DataSourceType
-from tecton_proto.data.feature_view_pb2 import MaterializationTimeRangePolicy
+from tecton_proto.data import feature_view_pb2
+
+
+TECTON_CORE_QUERY_NODE_PARAM = "tecton_core_query_node_param"
+
+
+# If any attribute in a query node has TECTON_CORE_QUERY_NODE_PARAM set to True, that attribute isn't passed to the
+# exec node constructor.
+def exclude_query_node_params(attribute: attrs.Attribute, _) -> bool:
+    return not attribute.metadata.get(TECTON_CORE_QUERY_NODE_PARAM, False)
 
 
 @attrs.frozen
 class MultiOdfvPipelineNode(QueryNode):
     """
     Evaluates multiple ODFVs:
         - Dependent feature view columns are prefixed `udf_internal` (query_constants.UDF_INTERNAL).
         - Each ODFV has a namespace to ensure their features do not conflict with other features
     """
 
     input_node: NodeRef
     feature_definition_wrappers_namespaces: List[Tuple[FeatureDefinitionWrapper, str]]
+    use_namespace_feature_prefix: bool = True
 
     @property
     def columns(self) -> Tuple[str, ...]:
         output_columns = list(self.input_node.columns)
         for fdw, namespace in self.feature_definition_wrappers_namespaces:
             sep = fdw.namespace_separator
-            output_columns += [f"{namespace}{sep}{name}" for name in fdw.view_schema.column_names()]
+            output_columns += [
+                f"{namespace}{sep}{name}" if self.use_namespace_feature_prefix else name
+                for name in fdw.view_schema.column_names()
+            ]
         return tuple(output_columns)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         fdw_names = [fdw.name for fdw, _ in self.feature_definition_wrappers_namespaces]
         return f"Evaluate multiple on-demand feature views in pipeline '{fdw_names}'"
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
 
 
@@ -114,15 +135,15 @@
     def inputs(self) -> Tuple[NodeRef, ...]:
         return tuple(self.inputs_map.values())
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return list(self.inputs_map.keys())
 
-    def as_str(self):
+    def as_str(self) -> str:
         s = f"Evaluate feature view pipeline '{self.feature_definition_wrapper.name}'"
         if self.feature_time_limits:
             s += f" with feature time limits [{self.feature_time_limits.start}, {self.feature_time_limits.end})"
         return s
 
     def _to_query(self) -> pypika.Query:
         # maps input names to unique strings
@@ -144,14 +165,82 @@
         for t_node in queries[:-1]:
             query, alias = t_node
             res = res.with_(CustomQuery(query), alias)
         return res
 
 
 @attrs.frozen
+class StagingNode(QueryNode):
+    """
+    Executes upstream sql and stages (e.g. in S3)
+    """
+
+    input_node: NodeRef
+    staging_table_name: str
+    query_tree_stage: QueryTreeComputeType
+
+    @property
+    def columns(self) -> Tuple[str]:
+        return self.input_node.columns
+
+    @property
+    def inputs(self) -> Tuple[NodeRef, ...]:
+        return (self.input_node,)
+
+    def staging_table_name_unique(self) -> str:
+        return f"{self.staging_table_name}_{id(self)}"
+
+    def staging_path(self) -> str:
+        return f"{conf.get_or_none('STAGING_S3_PREFIX')}{self.staging_table_name_unique()}/"
+
+    def as_str(self):
+        return f"Staging data for {self.staging_table_name_unique()}"
+
+    def _to_staging_query_sql(self) -> str:
+        sql_str = self.input_node._to_query().get_sql()
+        if not conf.get_bool("DUCKDB_DEBUG"):
+            return sql_str
+        return sqlparse.format(sql_str, reindent=True)
+
+    def _to_query(self) -> pypika.Query:
+        # For non-DuckDB, this is just a passthrough
+        return self.input_node._to_query()
+
+
+@attrs.frozen
+class StagedTableScanNode(QueryNode):
+    staged_columns: Tuple[str]
+    staging_table_name: str
+    query_tree_stage: QueryTreeComputeType
+
+    @classmethod
+    def from_staging_node(cls, query_node: StagingNode) -> QueryNode:
+        return cls(
+            staged_columns=query_node.columns,
+            staging_table_name=query_node.staging_table_name_unique(),
+            query_tree_stage=query_node.query_tree_stage,
+        )
+
+    @property
+    def columns(self) -> Tuple[str]:
+        return self.staged_columns
+
+    @property
+    def inputs(self) -> Tuple[NodeRef, ...]:
+        return ()
+
+    def as_str(self):
+        return f"Scanning staged data from {self.staging_table_name}"
+
+    def _to_query(self) -> pypika.Query:
+        from_str = Database(self.staging_table_name)
+        return Query().from_(from_str).select("*")
+
+
+@attrs.frozen
 class DataSourceScanNode(QueryNode):
     """Scans a batch data source and applies the given time range filter, or reads a stream source.
 
     Attributes:
         ds: The data source to be scanned or read.
         ds_node: The DataSourceNode (proto object, not QueryNode) corresponding to the data source. Used for rewrites.
         is_stream: If True, the data source is a stream source.
@@ -175,24 +264,24 @@
         elif self.ds.type == DataSourceType.BATCH:
             return tuple(str(f.name) for f in self.ds.batch_source.spark_schema.fields)
         else:
             raise NotImplementedError
 
     # MyPy has a known issue on validators https://mypy.readthedocs.io/en/stable/additional_features.html#id1
     @is_stream.validator  # type: ignore
-    def check_no_time_filter(self, _, is_stream: bool):
+    def check_no_time_filter(self, _, is_stream: bool) -> None:
         if is_stream and (self.start_time is not None or self.end_time is not None):
             msg = "Raw data filtering cannot be run on a stream source"
             raise ValueError(msg)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
-        return tuple()
+        return ()
 
-    def as_str(self):
+    def as_str(self) -> str:
         verb = "Read stream source" if self.is_stream else "Scan data source"
         s = f"{verb} '{self.ds.name}'"
         if self.start_time and self.end_time:
             s += f" and apply time range filter [{self.start_time}, {self.end_time})"
         elif self.start_time:
             s += f" and filter by start time {self.start_time}"
         elif self.end_time:
@@ -238,17 +327,17 @@
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return tuple(f.name for f in self.ds.batch_source.spark_schema.fields)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
-        return tuple()
+        return ()
 
-    def as_str(self):
+    def as_str(self) -> str:
         if self.is_stream:
             return f"Read stream {self.ds.name}"
         else:
             return f"Scan data source '{self.ds.name} without applying a post processor"
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
@@ -263,60 +352,79 @@
 
     feature_definition_wrapper: FeatureDefinitionWrapper
     partition_time_filter: Optional[pendulum.Period] = None
 
     @property
     def columns(self) -> Tuple[str, ...]:
         offline_store_config = self.feature_definition_wrapper.offline_store_config
-        store_type = offline_store_config.WhichOneof("store_type")
+        store_type = get_offline_store_type(offline_store_config)
         cols = self.feature_definition_wrapper.materialization_schema.column_names()
-        if self.feature_definition_wrapper.is_temporal and store_type == "parquet":
+        if store_type == OfflineStoreType.SNOWFLAKE:
+            if self.feature_definition_wrapper.is_temporal_aggregate:
+                # Snowflake stores the timestamp_key instead of _anchor_time in offline store, but it's not used in QT for aggregates
+                cols.remove(default_case(self.feature_definition_wrapper.timestamp_key))
+            # anchor time is not included in m13n schema for any snowflake fvs
+            cols.append(ANCHOR_TIME)
+        if store_type == OfflineStoreType.PARQUET and self.feature_definition_wrapper.is_temporal:
             # anchor time is not included in m13n schema for bfv/sfv
-            cols.append(default_case(ANCHOR_TIME))
+            cols.append(ANCHOR_TIME)
         return cols
 
-    def as_str(self):
+    def as_str(self) -> str:
         s = f"Scan offline store for '{self.feature_definition_wrapper.name}'"
         if self.partition_time_filter:
             s += f" with feature time limits [{self.partition_time_filter.start}, {self.partition_time_filter.end}]"
         return s
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
-        return tuple()
+        return ()
 
     @property
     def store_type(self) -> str:
         return self.feature_definition_wrapper.offline_store_config.WhichOneof("store_type")
 
     def _to_query(self) -> pypika.Query:
-        workspace_prefix = self.feature_definition_wrapper.workspace.replace("-", "_")
         where_conds = self._get_partition_filters()
         fields = self._get_select_fields()
-        q = Query().from_(Table(f"{workspace_prefix}__{self.feature_definition_wrapper.name}")).select(*fields)
+        table_name = self._get_offline_table_name()
+        q = Query().from_(Table(table_name)).select(*fields)
         for w in where_conds:
             q = q.where(w)
         return q
 
     def _get_partition_filters(self) -> List[Term]:
         # Whenever the partition filtering logic is changed, also make sure the changes are applied to the spark
         # version in tecton_spark/offline_store.py
-
         if not self.partition_time_filter:
             return []
+
+        partition_filters = []
         partition_params = get_offline_store_partition_params(self.feature_definition_wrapper)
         partition_col = Field(partition_params.partition_by)
         if partition_params.partition_by == ANCHOR_TIME or (
             partition_params.partition_by == TIME_PARTITION and partition_params.partition_type == PartitionType.EPOCH
         ):
             partition_col = Cast(partition_col, "bigint")
+        partition_lower_bound, partition_upper_bound = self._get_partition_bounds(partition_params)
 
-        partition_filters = []
+        if partition_lower_bound:
+            partition_filters.append(partition_col >= partition_lower_bound)
+        if partition_upper_bound:
+            partition_filters.append(partition_col <= partition_upper_bound)
+        return partition_filters
+
+    def _get_partition_bounds(
+        self, partition_params: OfflineStorePartitionParams
+    ) -> Tuple[Optional[Union[int, str]], Optional[Union[int, str]]]:
+        if not self.partition_time_filter:
+            return None, None
         partition_lower_bound = None
         partition_upper_bound = None
+
         if partition_params.partition_type == PartitionType.DATE_STR:
             if self.partition_time_filter.start:
                 partition_lower_bound = timestamp_to_partition_date_str(
                     self.partition_time_filter.start, partition_params
                 )
             if self.partition_time_filter.end:
                 partition_upper_bound = timestamp_to_partition_date_str(
@@ -331,37 +439,58 @@
                 )
             if self.partition_time_filter.end:
                 partition_upper_bound = timestamp_to_partition_epoch(
                     self.partition_time_filter.end,
                     partition_params,
                     self.feature_definition_wrapper.get_feature_store_format_version,
                 )
+        elif partition_params.partition_type == PartitionType.RAW_TIMESTAMP:
+            if self.partition_time_filter.start:
+                partition_lower_bound = self.partition_time_filter.start
+            if self.partition_time_filter.end:
+                partition_upper_bound = self.partition_time_filter.end
 
-        if partition_lower_bound:
-            partition_filters.append(partition_col >= partition_lower_bound)
-        if partition_upper_bound:
-            partition_filters.append(partition_col <= partition_upper_bound)
-        return partition_filters
+        return partition_lower_bound, partition_upper_bound
 
     def _get_select_fields(self) -> List[Term]:
         offline_store_config = self.feature_definition_wrapper.offline_store_config
-        store_type = offline_store_config.WhichOneof("store_type")
+        store_type = get_offline_store_type(offline_store_config)
         fields = []
         for col in self.columns:
             if col == TIME_PARTITION:
                 continue
             elif col == ANCHOR_TIME:
+                if store_type == OfflineStoreType.SNOWFLAKE:
+                    # Convert the timestamp column to unixtime to create the anchor time column
+                    # For temporal fvs on snowflake: the offline table stores the event timestamp in the timestamp key column
+                    # For temporal aggregate fvs on snowflake: the offline table stores the start of the aggregation tile in the timestamp key column
+                    fields.append(
+                        convert_epoch_seconds_to_feature_store_format_version(
+                            to_unixtime(Field(self.feature_definition_wrapper.time_key)),
+                            self.feature_definition_wrapper.get_feature_store_format_version,
+                        ).as_(ANCHOR_TIME)
+                    )
                 # Only parquet store and bwafv delta store have _anchor_time column
                 # we probably dont need to actually keep this column in the general parquet case
-                if store_type == "parquet" or self.feature_definition_wrapper.is_temporal_aggregate:
+                elif store_type == OfflineStoreType.PARQUET or self.feature_definition_wrapper.is_temporal_aggregate:
                     fields.append(Cast(Field(ANCHOR_TIME), "bigint").as_(ANCHOR_TIME))
             else:
                 fields.append(col)
         return fields
 
+    def _get_offline_table_name(self) -> str:
+        sql_dialect = dialect()
+        if sql_dialect == Dialect.ATHENA:
+            workspace_prefix = self.feature_definition_wrapper.workspace.replace("-", "_")
+            return f"{workspace_prefix}__{self.feature_definition_wrapper.name}"
+        elif sql_dialect == Dialect.SNOWFLAKE:
+            return self.feature_definition_wrapper.fv_spec.snowflake_view_name
+        else:
+            raise NotImplementedError
+
 
 @attrs.frozen
 class JoinNode(QueryNode):
     """Join two inputs.
 
     Attributes:
         left: The left input of the join.
@@ -374,25 +503,25 @@
     right: NodeRef
     join_cols: List[str]
     how: str
 
     @property
     def columns(self) -> Tuple[str, ...]:
         right_nonjoin_cols = set(self.right.columns) - set(self.join_cols)
-        return tuple(list(self.left.columns) + sorted(list(right_nonjoin_cols)))
+        return tuple(list(self.left.columns) + sorted(right_nonjoin_cols))
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.left, self.right)
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return ["left", "right"]
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"{self.how.capitalize()} join on {self.join_cols}:"
 
     def _to_query(self) -> pypika.Query:
         left_q = self.left.node._to_query()
         if not conf.get_bool("QUERYTREE_SHORT_SQL_ENABLED"):
             right_q = self.right.node._to_query()
         else:
@@ -408,18 +537,18 @@
         elif self.how == "outer":
             join_q = join_q.outer_join(right_q)
         else:
             msg = f"Join Type {self.how} has not been implemented"
             raise NotImplementedError(msg)
         return join_q.using(*self.join_cols).select("*")
 
-    def get_sql_views(self) -> List[Tuple[str, str]]:
+    def get_sql_views(self, pretty_sql: bool = False) -> List[Tuple[str, str]]:
         if not conf.get_bool("QUERYTREE_SHORT_SQL_ENABLED"):
             return []
-        view_sql = self.right.node.to_sql()
+        view_sql = self.right.node.to_sql(pretty_sql=pretty_sql)
         return [(self._get_view_name(), view_sql)]
 
     def _get_view_name(self) -> str:
         return self.right.node.__class__.__name__ + "_" + str(id(self.right.node)) + "_" + "view"
 
 
 @attrs.frozen
@@ -443,15 +572,15 @@
         right_nonjoin_cols = set(self.right.columns) - set(self.join_cols)
         return tuple(list(self.left.columns) + list(right_nonjoin_cols))
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.left, self.right)
 
-    def as_str(self, verbose: bool):
+    def as_str(self, verbose: bool) -> str:
         return "Outer join (include nulls)" + (f" on {self.join_cols}:" if verbose else ":")
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
 
 
 @attrs.frozen
@@ -476,15 +605,15 @@
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.feature_data, self.entities)
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return ["feature_data", "entities"]
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Filter feature data by entities with respect to {self.entity_cols}:"
 
     def _to_query(self) -> pypika.Query:
         feature_data = self.feature_data._to_query()
         entities = self.entities._to_query()
         return Query().from_(feature_data).inner_join(entities).on_field(*self.entity_cols).select(*self.columns)
 
@@ -528,15 +657,15 @@
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.left_container.node, self.right_container.node)
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return ["left", "right"]
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Left asof join right, where the join condition is right.{self.right_container.effective_timestamp_field} <= left.{self.left_container.timestamp_field}"
 
     def _to_query(self) -> pypika.Query:
         ASOF_JOIN_TIMESTAMP_COL_1 = "_ASOF_JOIN_TIMESTAMP_1"
         ASOF_JOIN_TIMESTAMP_COL_2 = "_ASOF_JOIN_TIMESTAMP_2"
         IS_LEFT = "IS_LEFT"
         left_df = self.left_container.node._to_query()
@@ -581,28 +710,27 @@
         ]
         left_full_cols = (
             [LiteralValue(True).as_(IS_LEFT)]
             + [Field(x) for x in common_cols]
             + [Field(x) for x in left_nonjoin_cols]
             + [NULL.as_(self._right_struct_col)]
         )
-        mapping = {f"{self.right_container.prefix}_{x}": Field(x) for x in right_nonjoin_cols}
         right_full_cols = (
             [LiteralValue(False).as_(IS_LEFT)]
             + [Field(x) for x in common_cols]
             + [NULL.as_(x) for x in left_nonjoin_cols]
             + [struct(right_nonjoin_cols).as_(self._right_struct_col)]
         )
         left_df = Query().from_(left_df).select(*left_full_cols)
         right_df = Query().from_(right_df).select(*right_full_cols)
         union = left_df.union_all(right_df)
         right_window_funcs = []
         # Also order by IS_LEFT because we want spine rows to be after feature rows if
         # timestamps are the same
-        order_by_fields = timestamp_join_cols + [IS_LEFT]
+        order_by_fields = [*timestamp_join_cols, IS_LEFT]
         right_window_funcs.append(
             LastValue(Field(self._right_struct_col))
             .over(*[Field(x) for x in self.join_cols])
             .orderby(*[Field(x) for x in order_by_fields])
             .rows(an.Preceding(), an.CURRENT_ROW)
             .ignore_nulls()
             .as_(self._right_struct_col)
@@ -628,23 +756,29 @@
     Asof join full agg rollup
     """
 
     spine: NodeRef
     partial_agg_node: NodeRef
     fdw: FeatureDefinitionWrapper
 
+    # Whether QT should rewrite the subtree from this node to push down timestamps.
+    enable_spine_time_pushdown_rewrite: bool = attrs.field(metadata={TECTON_CORE_QUERY_NODE_PARAM: True})
+
+    # Whether QT should rewrite the subtree from this node to push down entity.
+    enable_spine_entity_pushdown_rewrite: bool = attrs.field(metadata={TECTON_CORE_QUERY_NODE_PARAM: True})
+
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.spine, self.partial_agg_node)
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return ["spine", "partial_aggregates"]
 
-    def as_str(self):
+    def as_str(self) -> str:
         return "Spine asof join partial aggregates, where the join condition is partial_aggregates._anchor_time <= spine._anchor_time and partial aggregates are rolled up to compute full aggregates"
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return tuple(list(self.spine.columns) + self.fdw.features)
 
     def _get_aggregations(self, window_order_col: str, partition_cols: List[str]) -> List[Term]:
@@ -661,15 +795,15 @@
                 tile_interval = self.fdw.get_tile_interval_for_version
             earliest_anchor_time = (
                 convert_timedelta_for_version(window_duration, feature_store_format_version) - tile_interval
             )
             # Adjust earliest_anchor_time by * 2 + 1 to account for the changes to TECTON_WINDOW_ORDER_COL
             earliest_anchor_time = an.Preceding(earliest_anchor_time * 2 + 1)
             aggregation_plan = AGGREGATION_PLANS.get(feature.function)
-            if conf.get_or_none("SQL_DIALECT") == "athena" and aggregation_plan is None:
+            if dialect() == Dialect.ATHENA and aggregation_plan is None:
                 msg = f"{feature.function} is not implemented in Athena"
                 raise TectonAthenaNotImplementedError(msg)
             names = aggregation_plan.materialized_column_names(feature.input_feature_name)
             query_window_spec = QueryWindowSpec(
                 partition_cols=partition_cols,
                 order_by_col=window_order_col,
                 range_start=earliest_anchor_time,
@@ -677,14 +811,16 @@
             )
             aggregations.append(
                 aggregation_plan.full_aggregation_query_term(names, query_window_spec).as_(feature.output_feature_name)
             )
         return aggregations
 
     def _to_query(self) -> pypika.Query:
+        # Snowflake has its own implementation of asof join, and this only works for Athena, DuckDB, and Spark
+        assert dialect() in (Dialect.ATHENA, Dialect.DUCKDB, Dialect.SPARK)
         left_df = self.spine.node._to_query()
         right_df = self.partial_agg_node.node._to_query()
         join_keys = self.fdw.join_keys
         timestamp_join_cols = [ANCHOR_TIME]
         common_cols = join_keys + timestamp_join_cols
         left_nonjoin_cols = list(set(self.spine.node.columns) - set(common_cols))
         left_prefix = "_tecton_left"
@@ -752,15 +888,14 @@
         anchor_0 - max_feature_agg_period (or ttl) < anchor_i <= anchor_0.
 
     Attributes:
          left: The spine node that misses the secondary key.
          left_ts: The timestamp column of the spine node.
          right: The feature value node that contains the secondary key.
          right_ts: The timestamp column of the feature value node.
-
     """
 
     left: NodeRef
     left_ts: str
     right: NodeRef
     right_ts: str
     fdw: FeatureDefinitionWrapper
@@ -769,23 +904,23 @@
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.left, self.right)
 
     @property
     def input_names(self) -> Optional[List[str]]:
         return ["left", "right"]
 
-    def as_str(self):
+    def as_str(self) -> str:
         return "Left asof wildcard match and explode right, where the join condition is left._anchor_time - ttl + 1 < right._anchor_time <= left._anchor_time."
 
     @property
     def columns(self) -> Tuple[str, ...]:
         if self.fdw.is_temporal_aggregate and self.fdw.aggregation_secondary_key:
-            return tuple(list(self.left.columns) + [self.fdw.aggregation_secondary_key])
+            return (*list(self.left.columns), self.fdw.aggregation_secondary_key)
 
-        return tuple(list(self.left.columns) + [self.fdw.wildcard_join_key])
+        return (*list(self.left.columns), self.fdw.wildcard_join_key)
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
 
 
 @attrs.frozen
 class AggregationSecondaryKeyExplodeNode(QueryNode):
@@ -796,15 +931,15 @@
     input_node: NodeRef
     fdw: FeatureDefinitionWrapper
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Use entities {self.fdw.join_keys} to find all values for aggregation secondary key '{self.fdw.aggregation_secondary_key}' to build a spine."
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     def _to_query(self) -> pypika.Query:
@@ -834,31 +969,35 @@
     fdw: FeatureDefinitionWrapper = attrs.field()
     window_start_column_name: str
     window_end_column_name: Optional[str] = None
     aggregation_anchor_time: Optional[datetime] = None
 
     @property
     def columns(self) -> Tuple[str, ...]:
-        cols = self.fdw.materialization_schema.column_names()
+        cols = list(self.fdw.materialization_schema.column_names())
+        # Snowflake stores timestamp key in offline store, so it has timestamp key in materialized schema.
+        # But we are returning _ANCHOR_TIME here for partial agg node.
+        if dialect() == Dialect.SNOWFLAKE:
+            cols = [col for col in cols if col != self.fdw.timestamp_key] + [ANCHOR_TIME]
         # TODO(Felix) this is janky
         if self.window_end_column_name is not None and not self.fdw.is_continuous:
             cols.append(self.window_end_column_name)
-        return cols
+        return tuple(cols)
 
     @fdw.validator
     def check_is_aggregate(self, _, value):
         if not value.is_temporal_aggregate:
             msg = "Cannot construct a PartialAggNode using a non-aggregate feature view."
             raise ValueError(msg)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         actions = [
             f"Perform partial aggregations with column '{self.window_start_column_name}' as the start time of tiles."
         ]
         if self.window_end_column_name:
             actions.append(f"Add column '{self.window_end_column_name}' as the end time of tiles.")
         if self.aggregation_anchor_time:
             actions.append(
@@ -899,20 +1038,19 @@
                 window_start, self.fdw.get_feature_store_format_version
             )
             window_end = convert_epoch_seconds_to_feature_store_format_version(
                 window_end, self.fdw.get_feature_store_format_version
             )
 
             select_cols = agg_cols + join_cols + [window_start.as_(self.window_start_column_name)]
-            group_by_cols = join_cols + [window_start]
+            group_by_cols = [*join_cols, window_start]
             group_by_cols.append(window_end)
             q = q.groupby(*group_by_cols)
             if self.window_end_column_name:
                 select_cols.append(window_end.as_(self.window_end_column_name))
-
         else:
             # Continuous
             select_cols = (
                 agg_cols
                 + join_cols
                 + [
                     timestamp_field,
@@ -920,15 +1058,18 @@
                         to_unixtime(Field(time_aggregation.time_key)), self.fdw.get_feature_store_format_version
                     ).as_(ANCHOR_TIME),
                 ]
             )
         res = q.select(*select_cols)
         return res
 
-    def _get_partial_agg_columns(self):
+    def _get_partial_agg_columns(self) -> List[Term]:
+        """
+        Snowflake overrides this method to use snowflake specific aggregation functions
+        """
         time_aggregation = self.fdw.trailing_time_window_aggregation
         agg_cols = []
         output_columns = set()
         for feature in time_aggregation.features:
             aggregation_plan = AGGREGATION_PLANS.get(feature.function)
             if time_aggregation.is_continuous:
                 agg_query_terms = aggregation_plan.continuous_aggregation_query_terms(feature.input_feature_name)
@@ -966,33 +1107,33 @@
     input_node: NodeRef
     feature_store_format_version: int
     batch_schedule: int
     timestamp_field: str
 
     @property
     def columns(self) -> Tuple[str, ...]:
-        return self.input_node.columns + [default_case(ANCHOR_TIME)]
+        return (*self.input_node.columns, ANCHOR_TIME)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return (
             "Add anchor time column '_anchor_time' to represent the materialization window. "
             f"It is calculated as window('{self.timestamp_field}', batch_schedule).start where batch_schedule = "
             f"{convert_duration_to_seconds(self.batch_schedule, self.feature_store_format_version)} seconds."
         )
 
     def _to_query(self) -> pypika.Query:
         input_query = self.input_node._to_query()
         uid = self.input_node.node.__class__.__name__ + "_" + str(id(self.input_node.node))
         secs = convert_duration_to_seconds(self.batch_schedule, self.feature_store_format_version)
         anchor_field = (to_unixtime(Field(self.timestamp_field)) - to_unixtime(Field(self.timestamp_field)) % secs).as_(
-            default_case(ANCHOR_TIME)
+            ANCHOR_TIME
         )
         return Query().with_(input_query, uid).from_(AliasedQuery(uid)).select("*", anchor_field)
 
 
 @attrs.frozen
 class AddRetrievalAnchorTimeNode(QueryNode):
     """Augment a dataframe with an anchor time column that represents the most recent features available for retrieval.
@@ -1033,25 +1174,25 @@
     input_node: NodeRef
     name: str
     feature_store_format_version: int
     batch_schedule: int
     tile_interval: int
     timestamp_field: str
     is_stream: bool
-    data_delay_seconds: Optional[int] = 0
+    data_delay_seconds: int = 0
 
     @property
     def columns(self) -> Tuple[str, ...]:
-        return tuple(list(self.input_node.columns) + [ANCHOR_TIME])
+        return (*list(self.input_node.columns), ANCHOR_TIME)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         base = (
             "Add anchor time column '_anchor_time' to represent the most recent feature data available for retrieval. "
             "The time at which feature data becomes available for retrieval depends on two factors: the frequency at "
             "which the feature view is materialized, and the data delay. "
         )
 
         if self.tile_interval == 0:  # Continuous
@@ -1093,32 +1234,24 @@
         data_delay_seconds = self.data_delay_seconds or 0
         anchor_time_field = convert_epoch_seconds_to_feature_store_format_version(
             to_unixtime(date_add("second", -data_delay_seconds, Field(self.timestamp_field))),
             self.feature_store_format_version,
         )
         if self.tile_interval == 0:
             return (
-                Query()
-                .with_(input_query, uid)
-                .from_(AliasedQuery(uid))
-                .select("*", anchor_time_field.as_(default_case(ANCHOR_TIME)))
+                Query().with_(input_query, uid).from_(AliasedQuery(uid)).select("*", anchor_time_field.as_(ANCHOR_TIME))
             )
         # For stream, we use the tile interval for bucketing since the data is available as soon as
         # the aggregation interval ends.
         # For BAFV, we use the batch schedule to get the last tile written.
         if self.is_stream:
             anchor_time_field = anchor_time_field - anchor_time_field % self.tile_interval - self.tile_interval
         else:
             anchor_time_field = anchor_time_field - anchor_time_field % self.batch_schedule - self.tile_interval
-        return (
-            Query()
-            .with_(input_query, uid)
-            .from_(AliasedQuery(uid))
-            .select("*", anchor_time_field.as_(default_case(ANCHOR_TIME)))
-        )
+        return Query().with_(input_query, uid).from_(AliasedQuery(uid)).select("*", anchor_time_field.as_(ANCHOR_TIME))
 
 
 @attrs.frozen
 class ConvertEpochToTimestampNode(QueryNode):
     """Convert epoch columns to timestamp columns.
 
     Attributes:
@@ -1135,15 +1268,15 @@
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return (
             f"Convert columns {list(self.feature_store_formats.keys())} from epoch (either seconds or ns) to timestamp."
         )
 
     def _to_query(self) -> pypika.Query:
         input_query = self.input_node._to_query()
         uid = self.input_node.node.__class__.__name__ + "_" + str(id(self.input_node.node))
@@ -1192,15 +1325,15 @@
                 newcols.append(col)
         return tuple(newcols)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         actions = []
         if self.mapping:
             actions.append(f"Rename columns with map {self.mapping}.")
         if self.drop:
             # NOTE: the order of drop columns is unimportant
             actions.append(f"Drop columns {sorted(self.drop)}.")
         if not actions:
@@ -1233,17 +1366,17 @@
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self.data.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
-        return tuple()
+        return ()
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"User provided data with columns {'|'.join(self.columns)}"
 
     def _to_query(self) -> pypika.Query:
         t = self.data._temp_table_name
         return Query().from_(Table(t)).select(*self.columns)
 
 
@@ -1265,15 +1398,15 @@
     start_time: Optional[datetime] = None
     end_time: Optional[datetime] = None
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.data,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         s = f"Read mock data source '{self.ds.name}'"
         if self.start_time:
             s += f" and filter by start time {self.start_time}"
         if self.end_time:
             s += f" and filter by end time {self.end_time}"
         return s
 
@@ -1342,15 +1475,15 @@
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         feature_start_time = (
             convert_epoch_to_datetime(self.feature_start_time, self.feature_store_format_version)
             if isinstance(self.feature_start_time, int)
             else self.feature_start_time
         )
         return (
             f"Respect the feature start time for all rows where '{self.retrieval_time_col}' < {feature_start_time} "
@@ -1392,15 +1525,15 @@
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Null out any values where '{self.retrieval_time_col}' > '{self.expiration_time_col}'"
 
     def _to_query(self) -> pypika.Query:
         input_query = self.input_node._to_query()
         cond = Field(self.retrieval_time_col) < Field(self.expiration_time_col)
         project_list = []
         for c in self.input_node.columns:
@@ -1418,15 +1551,15 @@
     input_node: NodeRef
     filter_str: str
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Apply filter: ({self.filter_str})"
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
     def _to_query(self) -> pypika.Query:
@@ -1442,34 +1575,40 @@
         feature_data_time_limits: The time limits to be applied.
         policy: The materialization policy to be used.
         timestamp_field: The column name of the feature timestamp field.
     """
 
     input_node: NodeRef
     feature_data_time_limits: pendulum.Period
-    policy: MaterializationTimeRangePolicy
+    policy: feature_view_pb2.MaterializationTimeRangePolicy
     timestamp_field: str
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         time_range_str = f"[{self.feature_data_time_limits.start}, {self.feature_data_time_limits.end})"
-        if self.policy == MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE:
+        if (
+            self.policy
+            == feature_view_pb2.MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE
+        ):
             return f"Assert all rows in column '{self.timestamp_field}' are in range {time_range_str}"
         else:
             return f"Apply time range filter {time_range_str} to column '{self.timestamp_field}'"
 
     def _to_query(self) -> pypika.Query:
-        if self.policy == MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE:
+        if (
+            self.policy
+            == feature_view_pb2.MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FAIL_IF_OUT_OF_RANGE
+        ):
             # snowflake/athena are post-fwv4
             raise NotImplementedError
         input_query = self.input_node._to_query()
         uid = self.input_node.node.__class__.__name__ + "_" + str(id(self.input_node.node))
         time_field = Field(self.timestamp_field)
         where_conds = []
         where_conds.append(time_field >= to_timestamp(self.feature_data_time_limits.start))
@@ -1492,15 +1631,15 @@
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return "Collect metrics on features"
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
 
 
 @attrs.frozen
@@ -1530,21 +1669,21 @@
     batch_schedule_seconds: int
     is_stream: bool
     data_delay_seconds: int
     is_temporal_aggregate: bool
 
     @property
     def columns(self) -> Tuple[str, ...]:
-        return tuple(list(self.input_node.columns) + [self.effective_timestamp_name])
+        return (*list(self.input_node.columns), self.effective_timestamp_name)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         if self.batch_schedule_seconds == 0 or self.is_stream:
             return f"Add effective timestamp column '{self.effective_timestamp_name}' that is equal to the timestamp column '{self.timestamp_field}'."
         else:
             result = (
                 f"Add effective timestamp column '{self.effective_timestamp_name}' that is equal to window('"
                 f"{self.timestamp_field}', batch_schedule).end where batch_schedule = "
                 f"{self.batch_schedule_seconds} seconds."
@@ -1586,21 +1725,21 @@
     input_node: NodeRef
     timestamp_field: str
     duration: pendulum.Duration
     new_column_name: str
 
     @property
     def columns(self) -> Tuple[str, ...]:
-        return tuple(list(self.input_node.columns) + [self.new_column_name])
+        return (*list(self.input_node.columns), self.new_column_name)
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Add {self.duration.in_words()} to '{self.timestamp_field}' as new column '{self.new_column_name}'"
 
     def _to_query(self) -> pypika.Query:
         input_query = self.input_node._to_query()
         uid = self.input_node.node.__class__.__name__ + "_" + str(id(self.input_node.node))
         return (
             Query()
@@ -1625,15 +1764,15 @@
     def columns(self) -> Tuple[str, ...]:
         return self.input_node.columns
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Set Stream Watermark {self.stream_watermark} on the DataFrame"
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
 
 
 @attrs.frozen
@@ -1641,15 +1780,15 @@
     input_node: NodeRef
     columns: List[str]
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.input_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Select distinct with columns {self.columns}."
 
     def _to_query(self) -> pypika.Query:
         input_query = self.input_node._to_query()
         uid = self.input_node.node.__class__.__name__ + "_" + str(id(self.input_node.node))
         fields = [Field(c) for c in self.columns]
         return Query().with_(input_query, uid).from_(AliasedQuery(uid)).select(*fields).distinct()
@@ -1659,27 +1798,54 @@
 class AggregationSecondaryKeyRollupNode(QueryNode):
     """
     Rollup aggregation secondary key and corresponding feature values for each distinct window.
 
     Attributes:
         full_aggregation_node: The input node, which is always a full aggregation node.
         fdw: The feature definition wrapper that contains the useful metadata.
+        group_by_columns: The columns to group by when rolling up the secondary key and its corresponding feature values.
     """
 
     full_aggregation_node: NodeRef
     fdw: FeatureDefinitionWrapper
+    group_by_columns: Tuple[str, ...]
 
     @property
     def inputs(self) -> Tuple[NodeRef, ...]:
         return (self.full_aggregation_node,)
 
-    def as_str(self):
+    def as_str(self) -> str:
         return f"Rollup aggregation secondary key '{self.fdw.aggregation_secondary_key}' and corresponding feature values for each distinct window."
 
     @property
     def columns(self) -> Tuple[str, ...]:
         return self.full_aggregation_node.columns + tuple(
             [o.name for o in self.fdw.fv_spec.secondary_key_rollup_outputs]
         )
 
     def _to_query(self) -> pypika.Query:
         raise NotImplementedError
+
+
+@attrs.frozen
+class AddUniqueIdNode(QueryNode):
+    """
+    Add a '_tecton_unique_id' column to the input node. This column is used to uniquely identify rows in the input node.
+
+    Warning: The generated unique ID is non-deterministic on Spark, so this column may not be safe to join on.
+    """
+
+    input_node: NodeRef
+
+    @property
+    def inputs(self) -> Tuple[NodeRef, ...]:
+        return (self.input_node,)
+
+    def as_str(self):
+        return f"Add a {TECTON_UNIQUE_ID_COL} column to the input node."
+
+    @property
+    def columns(self) -> Tuple[str, ...]:
+        return (*self.input_node.columns, TECTON_UNIQUE_ID_COL)
+
+    def _to_query(self) -> pypika.Query:
+        raise NotImplementedError
```

### Comparing `tecton-0.8.0b4/tecton_core/query/pandas/node.py` & `tecton-0.8.0b5/tecton_core/query/pandas/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,87 @@
 from __future__ import annotations
 
+import typing
 from abc import abstractmethod
+from typing import Callable
 from typing import List
+from typing import Optional
 
 import attrs
 import pandas
 
 from tecton_core.query import node_interface
 from tecton_core.query.pandas.sql import SqlExecutor
 
 
+if typing.TYPE_CHECKING:
+    import snowflake.snowpark
+
 # SqlExecNodes are responsible for executing the sql string produced by the query node and using its SqlExecutor to
 # output a pandas dataframe
+
+
 @attrs.frozen
 class SqlExecNode:
     columns: List[str]
     sql_string: str
     sql_executor: SqlExecutor
 
     @classmethod
-    def from_sql_inputs(cls, query_node: node_interface.QueryNode, sql_executor: SqlExecutor):
-        return cls(columns=query_node.columns, sql_string=query_node.to_sql(), sql_executor=sql_executor)  # type: ignore
+    def from_sql_inputs(
+        cls, query_node: node_interface.QueryNode, sql_executor: SqlExecutor, pretty_sql: bool = False
+    ) -> "SqlExecNode":
+        return cls(columns=query_node.columns, sql_string=query_node.to_sql(pretty_sql=pretty_sql), sql_executor=sql_executor)  # type: ignore
 
     def to_dataframe(self) -> pandas.DataFrame:
         df = self._to_dataframe()
-        if set([c.lower() for c in df.columns]) != set([c.lower() for c in self.columns]):
+        # TODO(TEC-15985): Because we do not refresh schemas on data sources, we can sometimes get different columns than what we have
+        # cached.
+        if {c.lower() for c in df.columns} != {c.lower() for c in self.columns}:
             pass
             # Because we do not refresh schemas on data sources, we can sometimes get different columns than what we have
             # cached. This is problematic but will require separate solution; don't fail for now
             # raise RuntimeError(f"Returned mismatch of columns: received: {df.columns}, expected: {self.columns}")
         return df
 
     def _to_dataframe(self) -> pandas.DataFrame:
-        if self.sql_executor is None:
-            msg = "SQL Executor must not be None"
-            raise ValueError(msg)
         pandas_df = self.sql_executor.read_sql(self.sql_string)
         return pandas_df
 
+    def to_snowpark(self) -> "snowflake.snowpark.DataFrame":
+        snowpark_df = self.sql_executor.sql_to_snowpark(self.sql_string)
+        return snowpark_df
+
 
 # PandasExecNodes are responsible for taking in a pandas dataframe, performing some pandas operation and outputting a
 # pandas dataframe
+
+
 @attrs.frozen
 class PandasExecNode:
     columns: List[str]
-    input_node: PandasExecNode
+    input_node: Optional[PandasExecNode]
+    column_name_updater: Optional[Callable[[str], str]]  # Snowflake uses this method to uppercase all column names
 
     @classmethod
-    def from_node_inputs(cls, query_node: node_interface.QueryNode, input_node: PandasExecNode):
+    def from_node_inputs(
+        cls,
+        query_node: node_interface.QueryNode,
+        input_node: Optional[PandasExecNode],
+        column_name_updater: Optional[Callable[[str], str]] = lambda x: x,
+    ) -> "PandasExecNode":
         kwargs = attrs.asdict(query_node, recurse=False)
         kwargs["input_node"] = input_node
         kwargs["columns"] = query_node.columns
+        kwargs["column_name_updater"] = column_name_updater
         return cls(**kwargs)
 
     def to_dataframe(self) -> pandas.DataFrame:
         df = self._to_dataframe()
-        if set([c.lower() for c in df.columns]) != set([c.lower() for c in self.columns]):
+        if {c.lower() for c in df.columns} != {c.lower() for c in self.columns}:
             pass
             # Because we do not refresh schemas on data sources, we can sometimes get different columns than what we have
             # cached. This is problematic but will require separate solution; don't fail for now
             # raise RuntimeError(f"Returned mismatch of columns: received: {df.columns}, expected: {self.columns}")
         return df
 
     @abstractmethod
```

### Comparing `tecton-0.8.0b4/tecton_core/query/pandas/nodes.py` & `tecton-0.8.0b5/tecton_core/query/pandas/nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,30 @@
     StringType(): "string",
     BoolType(): "bool",
     TimestampType(): "datetime64[ns]",
 }
 
 
 @attrs.frozen
+class PandasStagedTableScanNode(PandasExecNode):
+    input_df: pandas.DataFrame
+
+    def _to_dataframe(self) -> pandas.DataFrame:
+        return self.input_df
+
+    def to_dataframe(self) -> pandas.DataFrame:
+        # Ignore the super class check since this is a pass-through
+        return self._to_dataframe()
+
+
+@attrs.frozen
 class PandasMultiOdfvPipelineNode(PandasExecNode):
     input_node: Union[PandasExecNode, SqlExecNode]
     feature_definition_wrappers_namespaces: List[Tuple[FeatureDefinitionWrapper, str]]
+    use_namespace_feature_prefix: bool
 
     def _to_dataframe(self):
         output_df = self.input_node._to_dataframe()
         # Apply each ODFV sequentially. Note that attempting to apply ODFV
         # udfs in parallel as we traverse data rows does not meaningfully
         # speed up execution on Athena (unlike in Spark).
         for fdw, namespace in self.feature_definition_wrappers_namespaces:
@@ -58,15 +71,18 @@
         odfv_result_df = self._run_odfv(input_df, fdw)
         rename_map = {}
         datatypes = {}
         # Namespace ODFV outputs to this FV to avoid conflicts in output schemas
         # with other FV
         output_schema = fdw.view_schema.column_name_and_data_types()
         for column_name, datatype in output_schema:
-            mapped_name = f"{namespace}{fdw.namespace_separator}{column_name}"
+            if self.use_namespace_feature_prefix:
+                mapped_name = f"{namespace}{fdw.namespace_separator}{column_name}"
+            else:
+                mapped_name = column_name
             rename_map[column_name] = mapped_name
             if datatype in PRIMITIVE_TECTON_DATA_TYPE_TO_PANDAS_DATA_TYPE:
                 datatypes[mapped_name] = PRIMITIVE_TECTON_DATA_TYPE_TO_PANDAS_DATA_TYPE[datatype]
         odfv_result_df = odfv_result_df.rename(columns=rename_map)[[*rename_map.values()]].astype(datatypes)
         data_df = input_df.merge(odfv_result_df, left_index=True, right_index=True)
         return data_df
 
@@ -121,15 +137,15 @@
         odfv_transformation_node = odfv.pipeline.root.transformation_node
 
         for input in odfv_transformation_node.inputs:
             input_name = input.arg_name
 
             if input.node.HasField("request_data_source_node"):
                 request_context_schema = input.node.request_data_source_node.request_context.tecton_schema
-                request_context_fields = [c.name for c in request_context_schema.columns]
+                request_context_fields = [self.column_name_updater(c.name) for c in request_context_schema.columns]
 
                 for f in request_context_fields:
                     if f not in data_df.columns:
                         msg = f"ODFV {odfv.name} has a dependency on the Request Data Source named '{input_name}'. Field {f} of this Request Data Source is not found in the spine. Available columns: {list(data_df.columns)}"
                         raise TectonValidationError(msg)
 
                 input_df = data_df[request_context_fields]
@@ -137,16 +153,16 @@
                 fv_features = feature_set_config.find_dependent_feature_set_items(
                     odfv.fco_container, input.node, {}, odfv.id
                 )[0]
                 # Generate dependent column mappings since dependent FV have
                 # internal column names with _udf_internal
                 select_columns_and_rename_map = {}
                 for f in fv_features.features:
-                    column_name = f"{fv_features.namespace}__{f}"
-                    mapped_name = f
+                    column_name = self.column_name_updater(f"{fv_features.namespace}__{f}")
+                    mapped_name = self.column_name_updater(f)
                     select_columns_and_rename_map[column_name] = mapped_name
                 for f in select_columns_and_rename_map.keys():
                     if f not in data_df.columns:
                         msg = f"ODFV {odfv.name} has a dependency on the Feature View '{input_name}'. Feature {f} of this Feature View is not found in the retrieved historical data. Available columns: {list(data_df.columns)}"
                         raise TectonValidationError(msg)
                 # Let's select all of the features of the input FV from data_df
                 input_df = data_df.rename(columns=select_columns_and_rename_map)[
@@ -166,11 +182,12 @@
     mapping: Optional[Dict[str, str]]
     drop: Optional[List[str]]
 
     def _to_dataframe(self) -> pandas.DataFrame:
         input_df = self.input_node._to_dataframe()
         output_df = input_df
         if self.drop:
-            output_df = input_df.drop(columns=self.drop)
+            columns_to_drop = [self.column_name_updater(name) for name in self.drop]
+            output_df = input_df.drop(columns=columns_to_drop)
         if self.mapping:
             output_df = input_df.rename(self.mapping)
         return output_df
```

### Comparing `tecton-0.8.0b4/tecton_core/query/sql_compat.py` & `tecton-0.8.0b5/tecton_core/query/sql_compat.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,57 +9,84 @@
 from pypika import CustomFunction
 from pypika import Field
 from pypika import Interval
 from pypika import Table
 from pypika import analytics
 from pypika.dialects import MySQLQuery
 from pypika.dialects import PostgreSQLQuery
+from pypika.dialects import SnowflakeQuery
 from pypika.functions import Cast
 from pypika.functions import DateAdd
 from pypika.queries import Selectable
 from pypika.terms import AnalyticFunction
 from pypika.terms import Function
 from pypika.terms import LiteralValue
 from pypika.terms import Term
 from pypika.utils import format_alias_sql
 
 from tecton_core import conf
 from tecton_core.data_types import DataType
 from tecton_proto.data.feature_store_pb2 import FeatureStoreFormatVersion
 
 
+class CaseSensitiveSnowflakeQueryBuilder(pypika.dialects.SnowflakeQueryBuilder):
+    QUOTE_CHAR = '"'
+
+
 class CaseSensitiveSnowflakeQuery(pypika.queries.Query):
     @classmethod
-    def _builder(cls, **kwargs: Any) -> "CaseSensitiveSnowflakeQueryBuilder":
+    def _builder(cls, **kwargs: Any) -> CaseSensitiveSnowflakeQueryBuilder:
         return CaseSensitiveSnowflakeQueryBuilder(**kwargs)
 
 
-class CaseSensitiveSnowflakeQueryBuilder(pypika.dialects.SnowflakeQueryBuilder):
-    QUOTE_CHAR = '"'
+class DuckDBQuery(pypika.queries.Query):
+    @classmethod
+    def _builder(cls, **kwargs: Any) -> "DuckDBQuery":
+        return DuckDBQueryBuilder(**kwargs)
+
+
+class DuckDBQueryBuilder(pypika.dialects.PostgreSQLQueryBuilder):
+    ALIAS_QUOTE_CHAR = None
+
+    def __init__(self, **kwargs: Any) -> None:
+        super().__init__(as_keyword=True, **kwargs)
+
+
+class CaseInsensitiveSnowflakeQueryBuilder(pypika.dialects.SnowflakeQueryBuilder):
+    QUOTE_CHAR = None
+    ALIAS_QUOTE_CHAR = None
+    QUERY_ALIAS_QUOTE_CHAR = ""
+    QUERY_CLS = SnowflakeQuery
+
+
+class CaseInsensitiveSnowflakeQuery(pypika.queries.Query):
+    @classmethod
+    def _builder(cls, **kwargs: Any) -> CaseInsensitiveSnowflakeQueryBuilder:
+        return CaseInsensitiveSnowflakeQueryBuilder(**kwargs)
 
 
 class CustomQuery(pypika.queries.QueryBuilder):
     """
     Defines a custom-query class. It's needed for us to wrap some user-defined sql string from transformations in a QueryBuilder object.
     """
 
-    def __init__(self, sql: str):
+    def __init__(self, sql: str) -> None:
         super().__init__(self)
         self.sql = sql
         self.withs: List[Selectable] = []
 
-    def with_(self, selectable: Selectable, name: str):
+    def with_(self, selectable: Selectable, name: str) -> "CustomQuery":
         """
         overrides QueryBuilder.with_
         """
         t = AliasedQuery(name, selectable)
         self.withs.append(t)
         return self
 
-    def get_sql(self, with_alias: bool = False, subquery: bool = False, **kwargs):
+    def get_sql(self, with_alias: bool = False, subquery: bool = False, **kwargs: Any) -> str:
         """
         overrides QueryBuilder.get_sql
         """
         sql = ""
         if self.withs:
             sql += "WITH " + ",".join(
                 clause.name + " AS (" + clause.get_sql(subquery=False, with_alias=False, **kwargs) + ") "
@@ -80,23 +107,27 @@
     """
 
     def get_special_params_sql(self, **kwargs: Any) -> Optional[str]:
         if dialect() == Dialect.SPARK:
             # see: https://docs.databricks.com/sql/language-manual/functions/last_value.html
             # for sparkSQL syntax
             return f", {self._ignore_nulls}"
+        elif dialect() == Dialect.DUCKDB and self._ignore_nulls:
+            # see: https://duckdb.org/docs/sql/window_functions.html
+            # for DuckDB syntax
+            return " IGNORE NULLS"
         # Snowflake does not support adding a function param to indicate "ignore nulls"
         # It looks like LAST_VALUE(...) IGNORE NULLS OVER(...)
         # see: https://docs.snowflake.com/en/sql-reference/functions/last_value.html
         # Nor does Athena - Athena docs don't make this clear though.
         else:
             return None
 
     def get_function_sql(self, **kwargs: Any) -> str:
-        if dialect() == Dialect.SPARK:
+        if dialect() == Dialect.SPARK or dialect() == Dialect.DUCKDB:
             return super(LastValue, self).get_function_sql(**kwargs)
         else:
             function_sql = super(AnalyticFunction, self).get_function_sql(**kwargs)
             partition_sql = self.get_partition_sql(**kwargs)
 
             sql = function_sql
             if self._ignore_nulls:
@@ -106,14 +137,16 @@
             return sql
 
 
 class Dialect(str, enum.Enum):
     SNOWFLAKE = "snowflake"
     ATHENA = "athena"
     SPARK = "spark"
+    DUCKDB = "duckdb"
+    PANDAS = "pandas"
 
 
 def dialect() -> Dialect:
     # TODO(Daryl) - infer the sql dialect from the fv itself,
     # We just use the conf for now as athena transformations are still under development.
     d = conf.get_or_none("SQL_DIALECT")
     try:
@@ -121,29 +154,32 @@
     except Exception:
         msg = f"Unsupported sql dialect: set SQL_DIALECT to {[x.value for x in Dialect]}"
         raise Exception(msg)
 
 
 def Query():
     if dialect() == Dialect.SNOWFLAKE:
-        return CaseSensitiveSnowflakeQuery
+        # TODO(TEC-15831): support quoted identifiers
+        return CaseInsensitiveSnowflakeQuery
+    elif dialect() == Dialect.DUCKDB:
+        return DuckDBQuery
     elif dialect() == Dialect.SPARK:
         # Spark (similar to HiveSQL) uses backticks like MySQL
         return MySQLQuery
     else:
         # Athena (similar to PrestoSQL) uses doublequotes like Postgres
         return PostgreSQLQuery
 
 
 # Spark, Athena, and Snowflake use different versions of structs.
 class Struct(Function):
-    def __init__(self, dialect: Dialect, *args, **kwargs):
+    def __init__(self, dialect: Dialect, *args: Any, **kwargs: Any) -> None:
         if dialect == Dialect.SPARK:
             f = "struct"
-        elif dialect == Dialect.ATHENA:
+        elif dialect == Dialect.ATHENA or dialect == Dialect.DUCKDB:
             f = "row"
         elif dialect == Dialect.SNOWFLAKE:
             f = "array_construct"
         else:
             raise NotImplementedError
         super(Struct, self).__init__(f, *args, **kwargs)
 
@@ -161,15 +197,15 @@
         return field_name
 
 
 def struct_extract(name: str, field_names: List[str], aliases: List[str], schema: Dict[str, DataType]) -> List[Field]:
     """
     Returns list of fields that pull out all `field_names` from the struct object, and alias them to `aliases`
     """
-    if dialect() == Dialect.SPARK:
+    if dialect() == Dialect.SPARK or dialect() == Dialect.DUCKDB:
         assert len(field_names) == len(aliases)
         return [getattr(Table(name), (field)).as_(alias) for (field, alias) in zip(field_names, aliases)]
     elif dialect() == Dialect.ATHENA:
         return [getattr(Table(name), f"field{idx}").as_(aliases[idx]) for idx in range(len(aliases))]
     elif dialect() == Dialect.SNOWFLAKE:
         get = CustomFunction("get", ["array", "idx"])
         res = []
@@ -181,75 +217,91 @@
             res.append(val.as_(aliases[idx]))
         return res
     else:
         raise NotImplementedError
 
 
 def to_timestamp(time_str: str) -> Term:
-    if dialect() == Dialect.SNOWFLAKE or dialect() == Dialect.SPARK:
+    if dialect() == Dialect.DUCKDB:
+        return Cast(time_str, as_type="timestamp")
+    elif dialect() == Dialect.SNOWFLAKE or dialect() == Dialect.SPARK:
         c = CustomFunction("to_timestamp", ["time_str"])
     else:
         c = CustomFunction("from_iso8601_timestamp", ["time_str"])
     return c(time_str)
 
 
 def date_add(interval: str, amount: int, time_field: Term) -> Term:
     if dialect() == Dialect.SNOWFLAKE:
         # snowflake uses dateadd rather than date_add; https://docs.snowflake.com/en/sql-reference/functions/dateadd.html
         c = CustomFunction("dateadd", ["interval", "amount", "time_field"])
         # LiteralValue will not put quotes around.
         # So we get dateadd(second, ...)
         interval = LiteralValue(interval)
-    elif dialect() == Dialect.SPARK:
+    elif dialect() == Dialect.SPARK or dialect() == Dialect.DUCKDB:
         if interval == "second":
             return time_field + Interval(seconds=amount)
+        elif interval == "millisecond":
+            # Note: PyPika has a bug where for microseconds, it does not correctly respect negative values
+            if amount >= 0:
+                return time_field + Interval(microseconds=amount * 1000)
+            else:
+                return time_field - Interval(microseconds=abs(amount) * 1000)
         else:
-            raise NotImplementedError
+            msg = f"Unexpected date_add interval {interval}"
+            raise NotImplementedError(msg)
     else:
         c = DateAdd
         # For Athena, see: https://trino.io/docs/current/functions/datetime.html
         interval = f"'{interval}'"
     return c(interval, amount, time_field)
 
 
 def to_unixtime(timestamp: Term) -> Term:
     if dialect() == Dialect.SNOWFLAKE:
         c = CustomFunction("date_part", ["epoch", "timestamp"])
         return c(Field("epoch_second"), timestamp)
+    elif dialect() == Dialect.DUCKDB:
+        c = CustomFunction("date_part", ["epoch", "timestamp"])
+        return c("epoch", timestamp)
     elif dialect() == Dialect.SPARK:
         c = CustomFunction("unix_timestamp", ["timestamp"])
         return c(timestamp)
     else:
         c = CustomFunction("to_unixtime", ["timestamp"])
         return c(timestamp)
 
 
 def from_unixtime(unix_timestamp: Term) -> Term:
-    if dialect() == Dialect.SNOWFLAKE:
+    if dialect() == Dialect.SNOWFLAKE or dialect() == Dialect.DUCKDB:
         c = CustomFunction("to_timestamp", ["unix_timestamp"])
         return c(unix_timestamp)
     elif dialect() == Dialect.ATHENA:
         c = CustomFunction("from_unixtime", ["unix_timestamp"])
         return c(unix_timestamp)
     else:
         c = CustomFunction("from_unixtime", ["unix_timestamp"])
         return Cast(c(unix_timestamp), "timestamp")
 
 
-def convert_epoch_term_in_seconds(timestamp: Term, time_stamp_feature_store_format_version: FeatureStoreFormatVersion):
+def convert_epoch_term_in_seconds(
+    timestamp: Term, time_stamp_feature_store_format_version: FeatureStoreFormatVersion
+) -> Term:
     """
     Converts an epoch term to a timestamp column
     :param timestamp: epoch column [V0 : Seconds, V1 : Nanoseconds]
     :param time_stamp_feature_store_format_version: Feature Store Format Version
     :return: epoch in seconds
     """
     if time_stamp_feature_store_format_version == FeatureStoreFormatVersion.FEATURE_STORE_FORMAT_VERSION_DEFAULT:
         return timestamp
-    return timestamp / int(1e9)
+    # Cast explicitly to an integer (which is the expectation), since otherwise SQL will often treat integer division
+    # as outputting a double, which is incompatible with to_timestamp(epoch_seconds) functions
+    return Cast(timestamp / int(1e9), as_type="bigint")
 
 
 def convert_epoch_seconds_to_feature_store_format_version(
     timestamp: Term, feature_store_format_version: FeatureStoreFormatVersion
-):
+) -> Term:
     if feature_store_format_version == FeatureStoreFormatVersion.FEATURE_STORE_FORMAT_VERSION_DEFAULT:
         return timestamp
-    return timestamp * 1e9
+    return timestamp * int(1e9)
```

### Comparing `tecton-0.8.0b4/tecton_core/repo_file_handler.py` & `tecton-0.8.0b5/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/request_context.py` & `tecton-0.8.0b5/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/schema.py` & `tecton-0.8.0b5/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/schema_derivation_utils.py` & `tecton-0.8.0b5/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/__init__.py` & `tecton-0.8.0b5/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/data_source_spec.py` & `tecton-0.8.0b5/tecton_core/specs/data_source_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,16 +821,16 @@
         # use the serialized function over directly using the Python function.
         if proto.HasField("data_source_function"):
             data_source_function = function_deserialization.from_proto(proto.data_source_function)
         else:
             data_source_function = supplement.stream_data_source_function
 
         return cls(
-            deduplication_column_names=tuple(),
-            options=tuple(),
+            deduplication_column_names=(),
+            options=(),
             watermark_delay_threshold=pendulum.Duration(),
             spark_schema=supplement.stream_schema,
             function=data_source_function,
         )
 
 
 # Resolve forward type declarations.
```

### Comparing `tecton-0.8.0b4/tecton_core/specs/entity_spec.py` & `tecton-0.8.0b5/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/feature_service_spec.py` & `tecton-0.8.0b5/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/feature_view_spec.py` & `tecton-0.8.0b5/tecton_core/specs/feature_view_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         elif proto.HasField("temporal"):
             fv_type = MaterializedFeatureViewType.TEMPORAL
             is_continuous = proto.temporal.is_continuous
             data_source_type = utils.get_field_or_none(proto.temporal, "data_source_type")
             incremental_backfills = proto.temporal.incremental_backfills
             slide_interval = None
             ttl = utils.get_non_default_duration_field_or_none(proto.temporal, "serving_ttl")
-            aggregate_features = tuple()
+            aggregate_features = ()
             slide_interval_string = None
             aggregation_secondary_key = None
             secondary_key_rollup_outputs = None
         else:
             msg = f"Unexpected feature view type: {proto}"
             raise TypeError(msg)
 
@@ -344,15 +344,15 @@
             feature_start_time=feature_start_time,
             materialization_start_time=materialization_start_time,
             max_source_data_delay=_get_max_schedule_offset(proto.pipeline),
             aggregate_features=get_aggregate_features_from_feature_view_args(proto),
             slide_interval_string=slide_interval_string,
             materialized_data_path=None,
             time_range_policy=feature_view__data_pb2.MaterializationTimeRangePolicy.MATERIALIZATION_TIME_RANGE_POLICY_FILTER_TO_RANGE,
-            materialization_state_transitions=tuple(),
+            materialization_state_transitions=(),
             snowflake_view_name=None,
             validation_args=None,
             batch_cluster_config=utils.get_field_or_none(proto.materialized_feature_view_args, "batch_compute"),
             stream_cluster_config=utils.get_field_or_none(proto.materialized_feature_view_args, "stream_compute"),
             batch_trigger=get_batch_trigger_from_feature_view_args(proto),
             manual_trigger_backfill_end_time=utils.get_timestamp_field_or_none(
                 proto.materialized_feature_view_args, "manual_trigger_backfill_end_time"
@@ -409,17 +409,17 @@
     @classmethod
     @typechecked
     def from_args_proto(
         cls, proto: feature_view__args_pb2.FeatureViewArgs, supplement: FeatureViewSpecArgsSupplement
     ) -> "OnDemandFeatureViewSpec":
         return cls(
             metadata=tecton_object_spec.TectonObjectMetadataSpec.from_args_proto(proto.feature_view_id, proto.info),
-            entity_ids=tuple(),
-            join_keys=tuple(),
-            online_serving_keys=tuple(),
+            entity_ids=(),
+            join_keys=(),
+            online_serving_keys=(),
             view_schema=schema.Schema(supplement.view_schema),
             materialization_schema=schema.Schema(supplement.materialization_schema),
             feature_store_format_version=feature_store_pb2.FeatureStoreFormatVersion.FEATURE_STORE_FORMAT_VERSION_TIME_NANOSECONDS,
             materialization_enabled=False,
             online=False,
             offline=False,
             pipeline=utils.get_field_or_none(proto, "pipeline"),
@@ -515,15 +515,15 @@
             timestamp_field=_get_timestamp_column(supplement.view_schema),
             feature_store_format_version=feature_store_pb2.FeatureStoreFormatVersion.FEATURE_STORE_FORMAT_VERSION_TIME_NANOSECONDS,
             materialization_enabled=False,
             online=proto.online_enabled,
             offline=proto.offline_enabled,
             ttl=utils.get_duration_field_or_none(proto.feature_table_args, "serving_ttl"),
             materialized_data_path=None,
-            materialization_state_transitions=tuple(),
+            materialization_state_transitions=(),
             time_range_policy=None,
             validation_args=None,
             batch_cluster_config=utils.get_field_or_none(proto.feature_table_args, "batch_compute"),
             url=None,
         )
 
     @property
```

### Comparing `tecton-0.8.0b4/tecton_core/specs/tecton_object_spec.py` & `tecton-0.8.0b5/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/transformation_spec.py` & `tecton-0.8.0b5/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/specs/utils.py` & `tecton-0.8.0b5/tecton_core/specs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # An attrs metadata key use to indicate that a spec field is allowed and expected to diverge for the same object
 # definition between local and remote objects. This metadata used in testing and to codify fields where divergence is
 # permitted.
 LOCAL_REMOTE_DIVERGENCE_ALLOWED = "local_remote_divergence_allowed"
 
 
 @typeguard.typechecked
-def get_field_or_none(proto: protobuf.message.Message, field: str) -> Any:
+def get_field_or_none(proto: protobuf.message.Message, field: str) -> Any:  # noqa: ANN401
     """Get the proto message's field. Return None if the field is not set (instead of the default value).
 
     When filling specs, `None` should be typically filled when the underlying proto field is unset - except in cases
     where the proto default (e.g. 0) is the desired for the Python value.
     """
     if proto.HasField(field):
         return getattr(proto, field)
@@ -69,15 +69,15 @@
 
 
 @typeguard.typechecked
 def get_tuple_from_repeated_field(repeated_field: Iterable[T]) -> Tuple[T, ...]:
     return tuple(value for value in repeated_field)
 
 
-def type_validator(instance: Any, attribute: attrs.Attribute, value: Any):
+def type_validator(instance: Any, attribute: attrs.Attribute, value: Any) -> None:  # noqa: ANN401
     """An attrs validator that asserts that an attribute matches its declared type."""
     assert attribute.type is not None, "Type annotations are required."
 
     # It would be better to assert on the affirmative (e.g. `assert inspect.is_class(attribute.type)`), but generic
     # types (e.g. `Optional[str]`) are not classes and do not have a documented way to identify them.
     assert not isinstance(
         attribute.type, str
```

### Comparing `tecton-0.8.0b4/tecton_core/time_utils.py` & `tecton-0.8.0b5/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/__init__.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/misc.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/node.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/plugins.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/treelib/tree.py` & `tecton-0.8.0b5/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_core/vendor/vendor_treelib.py` & `tecton-0.8.0b5/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.8.0b5/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.8.0b5/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.8.0b5/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/basic_info_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/data_source_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/diff_options_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/diff_options_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/diff_options.proto\x12\x11tecton_proto.args\x1a google/protobuf/descriptor.proto\"]\n\x11\x46ieldRenameConfig\x12\x1f\n\x0b\x66ormer_name\x18\x01 \x01(\tR\nformerName\x12\'\n\x0f\x63utover_version\x18\x02 \x01(\tR\x0e\x63utoverVersion\"\xc9\x02\n\x0b\x44iffOptions\x12\x39\n\x06update\x18\x01 \x01(\x0e\x32!.tecton_proto.args.UpdateStrategyR\x06update\x12\x1b\n\thide_path\x18\x02 \x01(\x08R\x08hidePath\x12R\n\x0erendering_type\x18\x03 \x01(\x0e\x32+.tecton_proto.args.FcoPropertyRenderingTypeR\rrenderingType\x12P\n\x11\x63ustom_comparator\x18\x04 \x01(\x0e\x32#.tecton_proto.args.CustomComparatorR\x10\x63ustomComparator\x12<\n\x06rename\x18\x05 \x01(\x0b\x32$.tecton_proto.args.FieldRenameConfigR\x06rename*\xe9\x01\n\x0eUpdateStrategy\x12\x0c\n\x08RECREATE\x10\x00\x12\x0b\n\x07INPLACE\x10\x01\x12\x12\n\x0eINPLACE_ON_ADD\x10\x03\x12\x15\n\x11INPLACE_ON_REMOVE\x10\x04\x12\x0b\n\x07PASSIVE\x10\x05\x12\x1e\n\x1aRECREATE_UNLESS_SUPPRESSED\x10\x06\x12\x35\n1RECREATE_UNLESS_SUPPRESSED_INVALIDATE_CHECKPOINTS\x10\x07\x12-\n)RECREATE_UNLESS_SUPPRESSED_RESTART_STREAM\x10\x08*\xc1\x02\n\x18\x46\x63oPropertyRenderingType\x12+\n\'FCO_PROPERTY_RENDERING_TYPE_UNSPECIFIED\x10\x00\x12*\n&FCO_PROPERTY_RENDERING_TYPE_PLAIN_TEXT\x10\x01\x12&\n\"FCO_PROPERTY_RENDERING_TYPE_PYTHON\x10\x02\x12#\n\x1f\x46\x43O_PROPERTY_RENDERING_TYPE_SQL\x10\x03\x12-\n)FCO_PROPERTY_RENDERING_TYPE_ONLY_DECLARED\x10\x04\x12&\n\"FCO_PROPERTY_RENDERING_TYPE_HIDDEN\x10\x05\x12(\n$FCO_PROPERTY_RENDERING_TYPE_REDACTED\x10\x06*\x84\x02\n\x10\x43ustomComparator\x12\x1b\n\x17\x43USTOM_COMPARATOR_UNSET\x10\x00\x12&\n\"CUSTOM_COMPARATOR_AGGREGATION_NAME\x10\x01\x12\x31\n-CUSTOM_COMPARATOR_OPTION_VALUE_WITH_REDACTION\x10\x02\x12$\n CUSTOM_COMPARATOR_DISPLAY_NOTSET\x10\x03\x12$\n CUSTOM_COMPARATOR_REQUEST_SOURCE\x10\x04\x12,\n(CUSTOM_COMPARATOR_STREAM_PROCESSING_MODE\x10\x06:a\n\x0c\x64iff_options\x12\x1d.google.protobuf.FieldOptions\x18\xd2\t \x01(\x0b\x32\x1e.tecton_proto.args.DiffOptionsR\x0b\x64iffOptionsB\x13\n\x0f\x63om.tecton.argsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tecton_proto/args/diff_options.proto\x12\x11tecton_proto.args\x1a google/protobuf/descriptor.proto\"]\n\x11\x46ieldRenameConfig\x12\x1f\n\x0b\x66ormer_name\x18\x01 \x01(\tR\nformerName\x12\'\n\x0f\x63utover_version\x18\x02 \x01(\tR\x0e\x63utoverVersion\"\xc9\x02\n\x0b\x44iffOptions\x12\x39\n\x06update\x18\x01 \x01(\x0e\x32!.tecton_proto.args.UpdateStrategyR\x06update\x12\x1b\n\thide_path\x18\x02 \x01(\x08R\x08hidePath\x12R\n\x0erendering_type\x18\x03 \x01(\x0e\x32+.tecton_proto.args.FcoPropertyRenderingTypeR\rrenderingType\x12P\n\x11\x63ustom_comparator\x18\x04 \x01(\x0e\x32#.tecton_proto.args.CustomComparatorR\x10\x63ustomComparator\x12<\n\x06rename\x18\x05 \x01(\x0b\x32$.tecton_proto.args.FieldRenameConfigR\x06rename*\xe9\x01\n\x0eUpdateStrategy\x12\x0c\n\x08RECREATE\x10\x00\x12\x0b\n\x07INPLACE\x10\x01\x12\x12\n\x0eINPLACE_ON_ADD\x10\x03\x12\x15\n\x11INPLACE_ON_REMOVE\x10\x04\x12\x0b\n\x07PASSIVE\x10\x05\x12\x1e\n\x1aRECREATE_UNLESS_SUPPRESSED\x10\x06\x12\x35\n1RECREATE_UNLESS_SUPPRESSED_INVALIDATE_CHECKPOINTS\x10\x07\x12-\n)RECREATE_UNLESS_SUPPRESSED_RESTART_STREAM\x10\x08*\xc1\x02\n\x18\x46\x63oPropertyRenderingType\x12+\n\'FCO_PROPERTY_RENDERING_TYPE_UNSPECIFIED\x10\x00\x12*\n&FCO_PROPERTY_RENDERING_TYPE_PLAIN_TEXT\x10\x01\x12&\n\"FCO_PROPERTY_RENDERING_TYPE_PYTHON\x10\x02\x12#\n\x1f\x46\x43O_PROPERTY_RENDERING_TYPE_SQL\x10\x03\x12-\n)FCO_PROPERTY_RENDERING_TYPE_ONLY_DECLARED\x10\x04\x12&\n\"FCO_PROPERTY_RENDERING_TYPE_HIDDEN\x10\x05\x12(\n$FCO_PROPERTY_RENDERING_TYPE_REDACTED\x10\x06*\xba\x02\n\x10\x43ustomComparator\x12\x1b\n\x17\x43USTOM_COMPARATOR_UNSET\x10\x00\x12&\n\"CUSTOM_COMPARATOR_AGGREGATION_NAME\x10\x01\x12\x31\n-CUSTOM_COMPARATOR_OPTION_VALUE_WITH_REDACTION\x10\x02\x12$\n CUSTOM_COMPARATOR_DISPLAY_NOTSET\x10\x03\x12$\n CUSTOM_COMPARATOR_REQUEST_SOURCE\x10\x04\x12,\n(CUSTOM_COMPARATOR_STREAM_PROCESSING_MODE\x10\x06\x12\x34\n0CUSTOM_COMPARATOR_DIFF_OVERRIDE_JOIN_KEYS_AS_MAP\x10\x07:a\n\x0c\x64iff_options\x12\x1d.google.protobuf.FieldOptions\x18\xd2\t \x01(\x0b\x32\x1e.tecton_proto.args.DiffOptionsR\x0b\x64iffOptionsB\x13\n\x0f\x63om.tecton.argsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.args.diff_options_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(diff_options)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.argsP\001'
   _UPDATESTRATEGY._serialized_start=521
   _UPDATESTRATEGY._serialized_end=754
   _FCOPROPERTYRENDERINGTYPE._serialized_start=757
   _FCOPROPERTYRENDERINGTYPE._serialized_end=1078
   _CUSTOMCOMPARATOR._serialized_start=1081
-  _CUSTOMCOMPARATOR._serialized_end=1341
+  _CUSTOMCOMPARATOR._serialized_end=1395
   _FIELDRENAMECONFIG._serialized_start=93
   _FIELDRENAMECONFIG._serialized_end=186
   _DIFFOPTIONS._serialized_start=189
   _DIFFOPTIONS._serialized_end=518
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.8.0b4/tecton_proto/args/diff_test_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/entity_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/fco_args_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/feature_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/feature_service_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,32 +13,34 @@
 
 from tecton_proto.args import basic_info_pb2 as tecton__proto_dot_args_dot_basic__info__pb2
 from tecton_proto.args import diff_options_pb2 as tecton__proto_dot_args_dot_diff__options__pb2
 from tecton_proto.common import framework_version_pb2 as tecton__proto_dot_common_dot_framework__version__pb2
 from tecton_proto.common import id_pb2 as tecton__proto_dot_common_dot_id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tecton_proto/args/feature_service.proto\x12\x11tecton_proto.args\x1a\"tecton_proto/args/basic_info.proto\x1a$tecton_proto/args/diff_options.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\"d\n\x11LoggingConfigArgs\x12\x1f\n\x0bsample_rate\x18\x01 \x01(\x02R\nsampleRate\x12.\n\x13log_effective_times\x18\x02 \x01(\x08R\x11logEffectiveTimes\"V\n\nColumnPair\x12!\n\x0cspine_column\x18\x01 \x01(\tR\x0bspineColumn\x12%\n\x0e\x66\x65\x61ture_column\x18\x02 \x01(\tR\rfeatureColumn\"\xec\x01\n\x1c\x46\x65\x61tureServiceFeaturePackage\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12K\n\x12override_join_keys\x18\x02 \x03(\x0b\x32\x1d.tecton_proto.args.ColumnPairR\x10overrideJoinKeys\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x1a\n\x08\x66\x65\x61tures\x18\x04 \x03(\tR\x08\x66\x65\x61tures\"\x9f\x04\n\x12\x46\x65\x61tureServiceArgs\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x37\n\x04info\x18\x02 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x06 \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18\x07 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12Z\n\x10\x66\x65\x61ture_packages\x18\x03 \x03(\x0b\x32/.tecton_proto.args.FeatureServiceFeaturePackageR\x0f\x66\x65\x61turePackages\x12;\n\x16online_serving_enabled\x18\x04 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x14onlineServingEnabled\x12>\n\x07logging\x18\x05 \x01(\x0b\x32$.tecton_proto.args.LoggingConfigArgsR\x07logging\x12\x32\n\x15on_demand_environment\x18\t \x01(\tR\x13onDemandEnvironmentJ\x04\x08\x08\x10\tB\x13\n\x0f\x63om.tecton.argsP\x01')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tecton_proto/args/feature_service.proto\x12\x11tecton_proto.args\x1a\"tecton_proto/args/basic_info.proto\x1a$tecton_proto/args/diff_options.proto\x1a+tecton_proto/common/framework_version.proto\x1a\x1ctecton_proto/common/id.proto\"d\n\x11LoggingConfigArgs\x12\x1f\n\x0bsample_rate\x18\x01 \x01(\x02R\nsampleRate\x12.\n\x13log_effective_times\x18\x02 \x01(\x08R\x11logEffectiveTimes\"V\n\nColumnPair\x12!\n\x0cspine_column\x18\x01 \x01(\tR\x0bspineColumn\x12%\n\x0e\x66\x65\x61ture_column\x18\x02 \x01(\tR\rfeatureColumn\"\xf3\x01\n\x1c\x46\x65\x61tureServiceFeaturePackage\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12R\n\x12override_join_keys\x18\x02 \x03(\x0b\x32\x1d.tecton_proto.args.ColumnPairB\x05\x92M\x02 \x07R\x10overrideJoinKeys\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12\x1a\n\x08\x66\x65\x61tures\x18\x04 \x03(\tR\x08\x66\x65\x61tures\"\x9f\x04\n\x12\x46\x65\x61tureServiceArgs\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x37\n\x04info\x18\x02 \x01(\x0b\x32\x1c.tecton_proto.args.BasicInfoB\x05\x92M\x02\x10\x01R\x04info\x12\x46\n\x07version\x18\x06 \x01(\x0e\x32%.tecton_proto.common.FrameworkVersionB\x05\x92M\x02\x08\x05R\x07version\x12.\n\x0fprevent_destroy\x18\x07 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x0epreventDestroy\x12Z\n\x10\x66\x65\x61ture_packages\x18\x03 \x03(\x0b\x32/.tecton_proto.args.FeatureServiceFeaturePackageR\x0f\x66\x65\x61turePackages\x12;\n\x16online_serving_enabled\x18\x04 \x01(\x08\x42\x05\x92M\x02\x08\x01R\x14onlineServingEnabled\x12>\n\x07logging\x18\x05 \x01(\x0b\x32$.tecton_proto.args.LoggingConfigArgsR\x07logging\x12\x32\n\x15on_demand_environment\x18\t \x01(\tR\x13onDemandEnvironmentJ\x04\x08\x08\x10\tB\x13\n\x0f\x63om.tecton.argsP\x01')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.args.feature_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\017com.tecton.argsP\001'
+  _FEATURESERVICEFEATUREPACKAGE.fields_by_name['override_join_keys']._options = None
+  _FEATURESERVICEFEATUREPACKAGE.fields_by_name['override_join_keys']._serialized_options = b'\222M\002 \007'
   _FEATURESERVICEARGS.fields_by_name['info']._options = None
   _FEATURESERVICEARGS.fields_by_name['info']._serialized_options = b'\222M\002\020\001'
   _FEATURESERVICEARGS.fields_by_name['version']._options = None
   _FEATURESERVICEARGS.fields_by_name['version']._serialized_options = b'\222M\002\010\005'
   _FEATURESERVICEARGS.fields_by_name['prevent_destroy']._options = None
   _FEATURESERVICEARGS.fields_by_name['prevent_destroy']._serialized_options = b'\222M\002\010\001'
   _FEATURESERVICEARGS.fields_by_name['online_serving_enabled']._options = None
   _FEATURESERVICEARGS.fields_by_name['online_serving_enabled']._serialized_options = b'\222M\002\010\001'
   _LOGGINGCONFIGARGS._serialized_start=211
   _LOGGINGCONFIGARGS._serialized_end=311
   _COLUMNPAIR._serialized_start=313
   _COLUMNPAIR._serialized_end=399
   _FEATURESERVICEFEATUREPACKAGE._serialized_start=402
-  _FEATURESERVICEFEATUREPACKAGE._serialized_end=638
-  _FEATURESERVICEARGS._serialized_start=641
-  _FEATURESERVICEARGS._serialized_end=1184
+  _FEATURESERVICEFEATUREPACKAGE._serialized_end=645
+  _FEATURESERVICEARGS._serialized_start=648
+  _FEATURESERVICEARGS._serialized_end=1191
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.8.0b4/tecton_proto/args/feature_view_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/pipeline_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/transformation_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.8.0b5/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auditlog/metadata_pb2.py` & `tecton-0.8.0b5/tecton_proto/auditlog/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/acl_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/principal_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/resource_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/auth/service_pb2.py` & `tecton-0.8.0b5/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/canary/type_pb2.py` & `tecton-0.8.0b5/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/canary/update_pb2.py` & `tecton-0.8.0b5/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.8.0b5/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/column_type_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/container_image_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/data_type_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/framework_version_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/id_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/pair_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/schema_container_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/schema_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/secret_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.8.0b5/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.8.0b5/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/data_source_access_config_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/data_source_access_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/entity_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/fco_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/feature_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/feature_store_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/feature_view_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/onboarding_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/principal_group_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/serving_status_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/state_update_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/summary_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/transformation_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/user_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/data/workspace_pb2.py` & `tecton-0.8.0b5/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.8.0b5/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/config_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.8.0b5/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.8.0b5/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,52 +21,52 @@
 from tecton_proto.data import feature_service_pb2 as tecton__proto_dot_data_dot_feature__service__pb2
 from tecton_proto.data import feature_view_pb2 as tecton__proto_dot_data_dot_feature__view__pb2
 from tecton_proto.data import odfv_compute_pb2 as tecton__proto_dot_data_dot_odfv__compute__pb2
 from tecton_proto.data import tecton_api_key_pb2 as tecton__proto_dot_data_dot_tecton__api__key__pb2
 from tecton_proto.data import transformation_pb2 as tecton__proto_dot_data_dot_transformation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nLtecton_proto/feature_server/configuration/feature_server_configuration.proto\x12)tecton_proto.feature_server.configuration\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tecton_proto/args/pipeline.proto\x1a\x1btecton_proto/auth/acl.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a#tecton_proto/common/data_type.proto\x1a\x1ctecton_proto/common/id.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\"\xeb\x01\n\x0c\x46\x65\x61turesPlan\x12[\n\x0c\x66\x65\x61ture_plan\x18\x01 \x01(\x0b\x32\x36.tecton_proto.feature_server.configuration.FeaturePlanH\x00R\x0b\x66\x65\x61turePlan\x12x\n\x17on_demand_features_plan\x18\x02 \x01(\x0b\x32?.tecton_proto.feature_server.configuration.OnDemandFeaturesPlanH\x00R\x14onDemandFeaturesPlanB\x04\n\x02\x66p\"\xec\x01\n\x06\x43olumn\x12:\n\tdata_type\x18\x05 \x01(\x0b\x32\x1d.tecton_proto.common.DataTypeR\x08\x64\x61taType\x12\x35\n\x17\x66\x65\x61ture_view_space_name\x18\x02 \x01(\tR\x14\x66\x65\x61tureViewSpaceName\x12;\n\x1a\x66\x65\x61ture_service_space_name\x18\x03 \x01(\tR\x17\x66\x65\x61tureServiceSpaceName\x12,\n\x12\x66\x65\x61ture_view_index\x18\x04 \x01(\x05R\x10\x66\x65\x61tureViewIndexJ\x04\x08\x01\x10\x02\"\xab\x0b\n\x0b\x46\x65\x61turePlan\x12V\n\routput_column\x18\x04 \x01(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x0coutputColumn\x12V\n\rinput_columns\x18\x01 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x0cinputColumns\x12[\n\x14\x61ggregation_function\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x13\x61ggregationFunction\x12n\n\x1b\x61ggregation_function_params\x18\x06 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x19\x61ggregationFunctionParams\x12H\n\x12\x61ggregation_window\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11\x61ggregationWindow\x12N\n\tjoin_keys\x18\x07 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x08joinKeys\x12_\n\x12wildcard_join_keys\x18\x08 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x10wildcardJoinKeys\x12\x1d\n\ntable_name\x18\t \x01(\tR\ttableName\x12|\n\x19\x64\x61ta_table_timestamp_type\x18\x0f \x01(\x0e\x32\x41.tecton_proto.feature_server.configuration.DataTableTimestampTypeR\x16\x64\x61taTableTimestampType\x12\x82\x01\n\x1bstatus_table_timestamp_type\x18\x10 \x01(\x0e\x32\x43.tecton_proto.feature_server.configuration.StatusTableTimestampTypeR\x18statusTableTimestampType\x12#\n\rtimestamp_key\x18\x0c \x01(\tR\x0ctimestampKey\x12<\n\x0cslide_period\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bslidePeriod\x12:\n\x0bserving_ttl\x18\x0e \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12\x30\n\x14refresh_status_table\x18\x11 \x01(\x08R\x12refreshStatusTable\x12*\n\x11\x66\x65\x61ture_view_name\x18\x15 \x01(\tR\x0f\x66\x65\x61tureViewName\x12&\n\x0f\x66\x65\x61ture_view_id\x18\x17 \x01(\tR\rfeatureViewId\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x12 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12T\n\x13online_store_params\x18\x13 \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12.\n\x12\x64\x65letionTimeWindow\x18\x16 \x01(\x03R\x12\x64\x65letionTimeWindowJ\x04\x08\x02\x10\x03J\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x14\x10\x15\"g\n\x11\x46\x65\x61tureVectorPlan\x12R\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x36.tecton_proto.feature_server.configuration.FeaturePlanR\x08\x66\x65\x61tures\"\xc1\x05\n\x14OnDemandFeaturesPlan\x12l\n\x19\x61rgs_from_request_context\x18\x02 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x16\x61rgsFromRequestContext\x12K\n\x07outputs\x18\x03 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x07outputs\x12\x83\x01\n\x12\x66\x65\x61ture_set_inputs\x18\x05 \x03(\x0b\x32U.tecton_proto.feature_server.configuration.OnDemandFeaturesPlan.FeatureSetInputsEntryR\x10\x66\x65\x61tureSetInputs\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12K\n\x0ftransformations\x18\x07 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformations\x12*\n\x11\x66\x65\x61ture_view_name\x18\x08 \x01(\tR\x0f\x66\x65\x61tureViewName\x12&\n\x0f\x66\x65\x61ture_view_id\x18\t \x01(\tR\rfeatureViewId\x1a\x81\x01\n\x15\x46\x65\x61tureSetInputsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x05value\x18\x02 \x01(\x0b\x32<.tecton_proto.feature_server.configuration.FeatureVectorPlanR\x05value:\x02\x38\x01J\x04\x08\x01\x10\x02J\x04\x08\x04\x10\x05\"\x81\x01\n\rLoggingConfig\x12\x1f\n\x0bsample_rate\x18\x01 \x01(\x02R\nsampleRate\x12.\n\x13log_effective_times\x18\x02 \x01(\x08R\x11logEffectiveTimes\x12\x1f\n\x0b\x61vro_schema\x18\x03 \x01(\tR\navroSchema\"\xe9\x05\n\x12\x46\x65\x61tureServicePlan\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12?\n\x0f\x66\x65\x61ture_view_id\x18\n \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x30\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tR\x12\x66\x65\x61tureServiceName\x12*\n\x11\x66\x65\x61ture_view_name\x18\t \x01(\tR\x0f\x66\x65\x61tureViewName\x12%\n\x0eworkspace_name\x18\x08 \x01(\tR\rworkspaceName\x12^\n\x0e\x66\x65\x61tures_plans\x18\r \x03(\x0b\x32\x37.tecton_proto.feature_server.configuration.FeaturesPlanR\rfeaturesPlans\x12N\n\x11join_key_template\x18\x05 \x01(\x0b\x32\".tecton_proto.data.JoinKeyTemplateR\x0fjoinKeyTemplate\x12\x41\n\x10\x66\x65\x61ture_view_ids\x18\x06 \x03(\x0b\x32\x17.tecton_proto.common.IdR\x0e\x66\x65\x61tureViewIds\x12_\n\x0elogging_config\x18\x0c \x01(\x0b\x32\x38.tecton_proto.feature_server.configuration.LoggingConfigR\rloggingConfig\x12Z\n\x15on_demand_environment\x18\x0e \x01(\x0b\x32&.tecton_proto.data.OnlineComputeConfigR\x13onDemandEnvironmentJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x0b\x10\x0c\"\x80\x04\n\x11GlobalTableConfig\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12<\n\x0cslide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bslidePeriod\x12\x12\n\x04size\x18\x03 \x01(\x05R\x04size\x12\x82\x01\n\x1bstatus_table_timestamp_type\x18\x06 \x01(\x0e\x32\x43.tecton_proto.feature_server.configuration.StatusTableTimestampTypeR\x18statusTableTimestampType\x12\x30\n\x14refresh_status_table\x18\x07 \x01(\x08R\x12refreshStatusTable\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x08 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12T\n\x13online_store_params\x18\t \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParamsJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"\x87\x01\n\x12\x46\x65\x61tureServiceAcls\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12*\n\x04\x61\x63ls\x18\x02 \x03(\x0b\x32\x16.tecton_proto.auth.AclR\x04\x61\x63ls\"b\n\rWorkspaceAcls\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\x12*\n\x04\x61\x63ls\x18\x02 \x03(\x0b\x32\x16.tecton_proto.auth.AclR\x04\x61\x63ls\"\xe1\x01\n\x0c\x43\x61naryConfig\x12\x37\n\x18\x66\x65\x61ture_server_canary_id\x18\x01 \x01(\tR\x15\x66\x65\x61tureServerCanaryId\x12\x42\n\x1e\x66\x65\x61ture_server_canary_pod_name\x18\x02 \x01(\tR\x1a\x66\x65\x61tureServerCanaryPodName\x12T\n\'feature_server_canary_follower_endpoint\x18\x03 \x01(\tR#featureServerCanaryFollowerEndpoint\"\xef\x07\n\x1a\x46\x65\x61tureServerConfiguration\x12?\n\rcomputed_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63omputedTime\x12h\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32=.tecton_proto.feature_server.configuration.FeatureServicePlanR\x0f\x66\x65\x61tureServices\x12\xa0\x01\n\x1bglobal_table_config_by_name\x18\x03 \x03(\x0b\x32\x62.tecton_proto.feature_server.configuration.FeatureServerConfiguration.GlobalTableConfigByNameEntryR\x17globalTableConfigByName\x12O\n\x13\x61uthorized_api_keys\x18\x04 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x11\x61uthorizedApiKeys\x12o\n\x14\x66\x65\x61ture_service_acls\x18\x05 \x03(\x0b\x32=.tecton_proto.feature_server.configuration.FeatureServiceAclsR\x12\x66\x65\x61tureServiceAcls\x12_\n\x0eworkspace_acls\x18\x06 \x03(\x0b\x32\x38.tecton_proto.feature_server.configuration.WorkspaceAclsR\rworkspaceAcls\x12[\n\x17\x61ll_online_store_params\x18\x07 \x03(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x14\x61llOnlineStoreParams\x12x\n\x1c\x66\x65\x61ture_server_canary_config\x18\x08 \x01(\x0b\x32\x37.tecton_proto.feature_server.configuration.CanaryConfigR\x19\x66\x65\x61tureServerCanaryConfig\x1a\x88\x01\n\x1cGlobalTableConfigByNameEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x05value\x18\x02 \x01(\x0b\x32<.tecton_proto.feature_server.configuration.GlobalTableConfigR\x05value:\x02\x38\x01*\x90\x01\n\x16\x44\x61taTableTimestampType\x12%\n!DATA_TABLE_TIMESTAMP_TYPE_UNKNOWN\x10\x00\x12&\n\"DATA_TABLE_TIMESTAMP_TYPE_SORT_KEY\x10\x01\x12\'\n#DATA_TABLE_TIMESTAMP_TYPE_ATTRIBUTE\x10\x02*\x98\x01\n\x18StatusTableTimestampType\x12\'\n#STATUS_TABLE_TIMESTAMP_TYPE_UNKNOWN\x10\x00\x12(\n$STATUS_TABLE_TIMESTAMP_TYPE_SORT_KEY\x10\x01\x12)\n%STATUS_TABLE_TIMESTAMP_TYPE_ATTRIBUTE\x10\x02\x42l\n(com.tecton.feature_service.configurationP\x01Z>github.com/tecton-ai/tecton_proto/feature_server/configuration')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nLtecton_proto/feature_server/configuration/feature_server_configuration.proto\x12)tecton_proto.feature_server.configuration\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a tecton_proto/args/pipeline.proto\x1a\x1btecton_proto/auth/acl.proto\x1a.tecton_proto/common/aggregation_function.proto\x1a#tecton_proto/common/data_type.proto\x1a\x1ctecton_proto/common/id.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a$tecton_proto/data/odfv_compute.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\"\xeb\x01\n\x0c\x46\x65\x61turesPlan\x12[\n\x0c\x66\x65\x61ture_plan\x18\x01 \x01(\x0b\x32\x36.tecton_proto.feature_server.configuration.FeaturePlanH\x00R\x0b\x66\x65\x61turePlan\x12x\n\x17on_demand_features_plan\x18\x02 \x01(\x0b\x32?.tecton_proto.feature_server.configuration.OnDemandFeaturesPlanH\x00R\x14onDemandFeaturesPlanB\x04\n\x02\x66p\"\xec\x01\n\x06\x43olumn\x12:\n\tdata_type\x18\x05 \x01(\x0b\x32\x1d.tecton_proto.common.DataTypeR\x08\x64\x61taType\x12\x35\n\x17\x66\x65\x61ture_view_space_name\x18\x02 \x01(\tR\x14\x66\x65\x61tureViewSpaceName\x12;\n\x1a\x66\x65\x61ture_service_space_name\x18\x03 \x01(\tR\x17\x66\x65\x61tureServiceSpaceName\x12,\n\x12\x66\x65\x61ture_view_index\x18\x04 \x01(\x05R\x10\x66\x65\x61tureViewIndexJ\x04\x08\x01\x10\x02\"\xd1\x0c\n\x0b\x46\x65\x61turePlan\x12V\n\routput_column\x18\x04 \x01(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x0coutputColumn\x12V\n\rinput_columns\x18\x01 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x0cinputColumns\x12[\n\x14\x61ggregation_function\x18\x03 \x01(\x0e\x32(.tecton_proto.common.AggregationFunctionR\x13\x61ggregationFunction\x12n\n\x1b\x61ggregation_function_params\x18\x06 \x01(\x0b\x32..tecton_proto.common.AggregationFunctionParamsR\x19\x61ggregationFunctionParams\x12H\n\x12\x61ggregation_window\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x11\x61ggregationWindow\x12N\n\tjoin_keys\x18\x07 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x08joinKeys\x12_\n\x12wildcard_join_keys\x18\x08 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x10wildcardJoinKeys\x12m\n\x19\x61ggregation_secondary_key\x18\x18 \x01(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x17\x61ggregationSecondaryKey\x12\x35\n\x17is_secondary_key_output\x18\x19 \x01(\x08R\x14isSecondaryKeyOutput\x12\x1d\n\ntable_name\x18\t \x01(\tR\ttableName\x12|\n\x19\x64\x61ta_table_timestamp_type\x18\x0f \x01(\x0e\x32\x41.tecton_proto.feature_server.configuration.DataTableTimestampTypeR\x16\x64\x61taTableTimestampType\x12\x82\x01\n\x1bstatus_table_timestamp_type\x18\x10 \x01(\x0e\x32\x43.tecton_proto.feature_server.configuration.StatusTableTimestampTypeR\x18statusTableTimestampType\x12#\n\rtimestamp_key\x18\x0c \x01(\tR\x0ctimestampKey\x12<\n\x0cslide_period\x18\r \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bslidePeriod\x12:\n\x0bserving_ttl\x18\x0e \x01(\x0b\x32\x19.google.protobuf.DurationR\nservingTtl\x12\x30\n\x14refresh_status_table\x18\x11 \x01(\x08R\x12refreshStatusTable\x12*\n\x11\x66\x65\x61ture_view_name\x18\x15 \x01(\tR\x0f\x66\x65\x61tureViewName\x12&\n\x0f\x66\x65\x61ture_view_id\x18\x17 \x01(\tR\rfeatureViewId\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x12 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12T\n\x13online_store_params\x18\x13 \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParams\x12.\n\x12\x64\x65letionTimeWindow\x18\x16 \x01(\x03R\x12\x64\x65letionTimeWindowJ\x04\x08\x02\x10\x03J\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x14\x10\x15\"g\n\x11\x46\x65\x61tureVectorPlan\x12R\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x36.tecton_proto.feature_server.configuration.FeaturePlanR\x08\x66\x65\x61tures\"\xc1\x05\n\x14OnDemandFeaturesPlan\x12l\n\x19\x61rgs_from_request_context\x18\x02 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x16\x61rgsFromRequestContext\x12K\n\x07outputs\x18\x03 \x03(\x0b\x32\x31.tecton_proto.feature_server.configuration.ColumnR\x07outputs\x12\x83\x01\n\x12\x66\x65\x61ture_set_inputs\x18\x05 \x03(\x0b\x32U.tecton_proto.feature_server.configuration.OnDemandFeaturesPlan.FeatureSetInputsEntryR\x10\x66\x65\x61tureSetInputs\x12\x37\n\x08pipeline\x18\x06 \x01(\x0b\x32\x1b.tecton_proto.args.PipelineR\x08pipeline\x12K\n\x0ftransformations\x18\x07 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformations\x12*\n\x11\x66\x65\x61ture_view_name\x18\x08 \x01(\tR\x0f\x66\x65\x61tureViewName\x12&\n\x0f\x66\x65\x61ture_view_id\x18\t \x01(\tR\rfeatureViewId\x1a\x81\x01\n\x15\x46\x65\x61tureSetInputsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x05value\x18\x02 \x01(\x0b\x32<.tecton_proto.feature_server.configuration.FeatureVectorPlanR\x05value:\x02\x38\x01J\x04\x08\x01\x10\x02J\x04\x08\x04\x10\x05\"\x81\x01\n\rLoggingConfig\x12\x1f\n\x0bsample_rate\x18\x01 \x01(\x02R\nsampleRate\x12.\n\x13log_effective_times\x18\x02 \x01(\x08R\x11logEffectiveTimes\x12\x1f\n\x0b\x61vro_schema\x18\x03 \x01(\tR\navroSchema\"\xe9\x05\n\x12\x46\x65\x61tureServicePlan\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12?\n\x0f\x66\x65\x61ture_view_id\x18\n \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12\x30\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tR\x12\x66\x65\x61tureServiceName\x12*\n\x11\x66\x65\x61ture_view_name\x18\t \x01(\tR\x0f\x66\x65\x61tureViewName\x12%\n\x0eworkspace_name\x18\x08 \x01(\tR\rworkspaceName\x12^\n\x0e\x66\x65\x61tures_plans\x18\r \x03(\x0b\x32\x37.tecton_proto.feature_server.configuration.FeaturesPlanR\rfeaturesPlans\x12N\n\x11join_key_template\x18\x05 \x01(\x0b\x32\".tecton_proto.data.JoinKeyTemplateR\x0fjoinKeyTemplate\x12\x41\n\x10\x66\x65\x61ture_view_ids\x18\x06 \x03(\x0b\x32\x17.tecton_proto.common.IdR\x0e\x66\x65\x61tureViewIds\x12_\n\x0elogging_config\x18\x0c \x01(\x0b\x32\x38.tecton_proto.feature_server.configuration.LoggingConfigR\rloggingConfig\x12Z\n\x15on_demand_environment\x18\x0e \x01(\x0b\x32&.tecton_proto.data.OnlineComputeConfigR\x13onDemandEnvironmentJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08J\x04\x08\x0b\x10\x0c\"\x80\x04\n\x11GlobalTableConfig\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\x12<\n\x0cslide_period\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x0bslidePeriod\x12\x12\n\x04size\x18\x03 \x01(\x05R\x04size\x12\x82\x01\n\x1bstatus_table_timestamp_type\x18\x06 \x01(\x0e\x32\x43.tecton_proto.feature_server.configuration.StatusTableTimestampTypeR\x18statusTableTimestampType\x12\x30\n\x14refresh_status_table\x18\x07 \x01(\x08R\x12refreshStatusTable\x12?\n\x1c\x66\x65\x61ture_store_format_version\x18\x08 \x01(\x05R\x19\x66\x65\x61tureStoreFormatVersion\x12T\n\x13online_store_params\x18\t \x01(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x11onlineStoreParamsJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"\x87\x01\n\x12\x46\x65\x61tureServiceAcls\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12*\n\x04\x61\x63ls\x18\x02 \x03(\x0b\x32\x16.tecton_proto.auth.AclR\x04\x61\x63ls\"b\n\rWorkspaceAcls\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\x12*\n\x04\x61\x63ls\x18\x02 \x03(\x0b\x32\x16.tecton_proto.auth.AclR\x04\x61\x63ls\"\xe1\x01\n\x0c\x43\x61naryConfig\x12\x37\n\x18\x66\x65\x61ture_server_canary_id\x18\x01 \x01(\tR\x15\x66\x65\x61tureServerCanaryId\x12\x42\n\x1e\x66\x65\x61ture_server_canary_pod_name\x18\x02 \x01(\tR\x1a\x66\x65\x61tureServerCanaryPodName\x12T\n\'feature_server_canary_follower_endpoint\x18\x03 \x01(\tR#featureServerCanaryFollowerEndpoint\"\xef\x07\n\x1a\x46\x65\x61tureServerConfiguration\x12?\n\rcomputed_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63omputedTime\x12h\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32=.tecton_proto.feature_server.configuration.FeatureServicePlanR\x0f\x66\x65\x61tureServices\x12\xa0\x01\n\x1bglobal_table_config_by_name\x18\x03 \x03(\x0b\x32\x62.tecton_proto.feature_server.configuration.FeatureServerConfiguration.GlobalTableConfigByNameEntryR\x17globalTableConfigByName\x12O\n\x13\x61uthorized_api_keys\x18\x04 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x11\x61uthorizedApiKeys\x12o\n\x14\x66\x65\x61ture_service_acls\x18\x05 \x03(\x0b\x32=.tecton_proto.feature_server.configuration.FeatureServiceAclsR\x12\x66\x65\x61tureServiceAcls\x12_\n\x0eworkspace_acls\x18\x06 \x03(\x0b\x32\x38.tecton_proto.feature_server.configuration.WorkspaceAclsR\rworkspaceAcls\x12[\n\x17\x61ll_online_store_params\x18\x07 \x03(\x0b\x32$.tecton_proto.data.OnlineStoreParamsR\x14\x61llOnlineStoreParams\x12x\n\x1c\x66\x65\x61ture_server_canary_config\x18\x08 \x01(\x0b\x32\x37.tecton_proto.feature_server.configuration.CanaryConfigR\x19\x66\x65\x61tureServerCanaryConfig\x1a\x88\x01\n\x1cGlobalTableConfigByNameEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x05value\x18\x02 \x01(\x0b\x32<.tecton_proto.feature_server.configuration.GlobalTableConfigR\x05value:\x02\x38\x01*\x90\x01\n\x16\x44\x61taTableTimestampType\x12%\n!DATA_TABLE_TIMESTAMP_TYPE_UNKNOWN\x10\x00\x12&\n\"DATA_TABLE_TIMESTAMP_TYPE_SORT_KEY\x10\x01\x12\'\n#DATA_TABLE_TIMESTAMP_TYPE_ATTRIBUTE\x10\x02*\x98\x01\n\x18StatusTableTimestampType\x12\'\n#STATUS_TABLE_TIMESTAMP_TYPE_UNKNOWN\x10\x00\x12(\n$STATUS_TABLE_TIMESTAMP_TYPE_SORT_KEY\x10\x01\x12)\n%STATUS_TABLE_TIMESTAMP_TYPE_ATTRIBUTE\x10\x02\x42l\n(com.tecton.feature_service.configurationP\x01Z>github.com/tecton-ai/tecton_proto/feature_server/configuration')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.feature_server.configuration.feature_server_configuration_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n(com.tecton.feature_service.configurationP\001Z>github.com/tecton-ai/tecton_proto/feature_server/configuration'
   _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._options = None
   _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._serialized_options = b'8\001'
   _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._options = None
   _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._serialized_options = b'8\001'
-  _DATATABLETIMESTAMPTYPE._serialized_start=6179
-  _DATATABLETIMESTAMPTYPE._serialized_end=6323
-  _STATUSTABLETIMESTAMPTYPE._serialized_start=6326
-  _STATUSTABLETIMESTAMPTYPE._serialized_end=6478
+  _DATATABLETIMESTAMPTYPE._serialized_start=6345
+  _DATATABLETIMESTAMPTYPE._serialized_end=6489
+  _STATUSTABLETIMESTAMPTYPE._serialized_start=6492
+  _STATUSTABLETIMESTAMPTYPE._serialized_end=6644
   _FEATURESPLAN._serialized_start=564
   _FEATURESPLAN._serialized_end=799
   _COLUMN._serialized_start=802
   _COLUMN._serialized_end=1038
   _FEATUREPLAN._serialized_start=1041
-  _FEATUREPLAN._serialized_end=2492
-  _FEATUREVECTORPLAN._serialized_start=2494
-  _FEATUREVECTORPLAN._serialized_end=2597
-  _ONDEMANDFEATURESPLAN._serialized_start=2600
-  _ONDEMANDFEATURESPLAN._serialized_end=3305
-  _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._serialized_start=3164
-  _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._serialized_end=3293
-  _LOGGINGCONFIG._serialized_start=3308
-  _LOGGINGCONFIG._serialized_end=3437
-  _FEATURESERVICEPLAN._serialized_start=3440
-  _FEATURESERVICEPLAN._serialized_end=4185
-  _GLOBALTABLECONFIG._serialized_start=4188
-  _GLOBALTABLECONFIG._serialized_end=4700
-  _FEATURESERVICEACLS._serialized_start=4703
-  _FEATURESERVICEACLS._serialized_end=4838
-  _WORKSPACEACLS._serialized_start=4840
-  _WORKSPACEACLS._serialized_end=4938
-  _CANARYCONFIG._serialized_start=4941
-  _CANARYCONFIG._serialized_end=5166
-  _FEATURESERVERCONFIGURATION._serialized_start=5169
-  _FEATURESERVERCONFIGURATION._serialized_end=6176
-  _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._serialized_start=6040
-  _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._serialized_end=6176
+  _FEATUREPLAN._serialized_end=2658
+  _FEATUREVECTORPLAN._serialized_start=2660
+  _FEATUREVECTORPLAN._serialized_end=2763
+  _ONDEMANDFEATURESPLAN._serialized_start=2766
+  _ONDEMANDFEATURESPLAN._serialized_end=3471
+  _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._serialized_start=3330
+  _ONDEMANDFEATURESPLAN_FEATURESETINPUTSENTRY._serialized_end=3459
+  _LOGGINGCONFIG._serialized_start=3474
+  _LOGGINGCONFIG._serialized_end=3603
+  _FEATURESERVICEPLAN._serialized_start=3606
+  _FEATURESERVICEPLAN._serialized_end=4351
+  _GLOBALTABLECONFIG._serialized_start=4354
+  _GLOBALTABLECONFIG._serialized_end=4866
+  _FEATURESERVICEACLS._serialized_start=4869
+  _FEATURESERVICEACLS._serialized_end=5004
+  _WORKSPACEACLS._serialized_start=5006
+  _WORKSPACEACLS._serialized_end=5104
+  _CANARYCONFIG._serialized_start=5107
+  _CANARYCONFIG._serialized_end=5332
+  _FEATURESERVERCONFIGURATION._serialized_start=5335
+  _FEATURESERVERCONFIGURATION._serialized_end=6342
+  _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._serialized_start=6206
+  _FEATURESERVERCONFIGURATION_GLOBALTABLECONFIGBYNAMEENTRY._serialized_end=6342
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.8.0b4/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.8.0b5/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.8.0b5/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.8.0b5/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/materialization/params_pb2.py` & `tecton-0.8.0b5/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.8.0b5/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.8.0b5/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 from tecton_proto.dataobs import metric_pb2 as tecton__proto_dot_dataobs_dot_metric__pb2
 from tecton_proto.dataobs import validation_pb2 as tecton__proto_dot_dataobs_dot_validation__pb2
 from tecton_proto.materialization import materialization_states_pb2 as tecton__proto_dot_materialization_dot_materialization__states__pb2
 from tecton_proto.materialization import spark_cluster_pb2 as tecton__proto_dot_materialization_dot_spark__cluster__pb2
 from tecton_proto.validation import validator_pb2 as tecton__proto_dot_validation_dot_validator__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a!tecton_proto/auth/principal.proto\x1a$tecton_proto/auditlog/metadata.proto\x1a\x1ftecton_proto/auth/service.proto\x1a%tecton_proto/common/fco_locator.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/common/spark_schema.proto\x1a*tecton_proto/consumption/consumption.proto\x1a\x1etecton_proto/data/entity.proto\x1a\x1btecton_proto/data/fco.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a.tecton_proto/data/materialization_status.proto\x1a\"tecton_proto/data/onboarding.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a&tecton_proto/data/serving_status.proto\x1a$tecton_proto/data/state_update.proto\x1a\x1ftecton_proto/data/summary.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\x1a\x1ctecton_proto/data/user.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a\x39tecton_proto/materialization/materialization_states.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\x1a\'tecton_proto/validation/validator.proto\"\x90\x01\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x1e\n\ncomparison\x18\x03 \x01(\x03R\ncomparison\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\xbd\x01\n\x15ValidationResultToken\x12\x43\n\x0fvalidation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12\x34\n\tresult_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08resultId\x12)\n\x10\x65xpectation_name\x18\x03 \x01(\tR\x0f\x65xpectationName\"\xd3\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"`\n\x1cGetFeatureConsumptionRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"u\n\x1dGetFeatureConsumptionResponse\x12T\n\x10\x63onsumption_info\x18\x01 \x03(\x0b\x32).tecton_proto.consumption.ConsumptionInfoR\x0f\x63onsumptionInfo\"\xaf\x01\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x0finclude_deleted\x18\x02 \x01(\x08R\x0eincludeDeleted\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\xe0\x06\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12I\n\x08statuses\x18\x03 \x03(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\x08statuses\x12`\n\x16last_task_state_change\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x13lastTaskStateChange\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n$include_update_materialization_flags\x18\x0c \x01(\x08R!includeUpdateMaterializationFlags\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xb5\x05\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12K\n\ttaskState\x18\x02 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12-\n\x12manually_triggered\x18\t \x01(\x08R\x11manuallyTriggered\x12O\n\x16last_task_state_change\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13lastTaskStateChange\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"t\n!RestartMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\"\xa1\x01\n\"RestartMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\x12V\n\x1bnew_materialization_task_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x18newMaterializationTaskId\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"F\n\x12SparkClusterConfig\x12\x1a\n\x08original\x18\x01 \x01(\tR\x08original\x12\x14\n\x05\x66inal\x18\x02 \x01(\tR\x05\x66inal\"\xc4\x01\n\x16GetSparkConfigResponse\x12S\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0b\x62\x61tchConfig\x12U\n\rstream_config\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\xca\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xf3\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x04 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\xd0\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xe8\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"Z\n\x17\x46indFcoWorkspaceRequest\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xfd\x01\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xa9\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\xa5\x01\n\x16\x43reateWorkspaceRequest\x12.\n\x0eworkspace_name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\rworkspaceName\x12U\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"?\n\x16\x44\x65leteWorkspaceRequest\x12%\n\tworkspace\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"d\n\x13\x43reateApiKeyRequest\x12)\n\x0b\x64\x65scription\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12\"\n\x08is_admin\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07isAdmin\"Z\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"G\n\x13\x44\x65leteApiKeyRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\x9f\x02\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x36\n\x07\x63reator\x18\x05 \x01(\x0b\x32\x1c.tecton_proto.auth.PrincipalR\x07\x63reator\x12\x37\n\x05owner\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\x05owner\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"e\n\x1b\x43reateServiceAccountRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\"\xf9\x01\n\x1c\x43reateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\xa4\x01\n\x1bUpdateServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\"\xe0\x01\n\x1cUpdateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"6\n\x1b\x44\x65leteServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\"D\n\x18\x43reateClusterUserRequest\x12(\n\x0blogin_email\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\nloginEmail\"!\n\x19\x43reateClusterUserResponseJ\x04\x08\x01\x10\x02\"<\n\x18\x44\x65leteClusterUserRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\"!\n\x19\x44\x65leteClusterUserResponseJ\x04\x08\x01\x10\x02\"\x8f\x02\n\x18\x43lusterUserActionRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\x12\x41\n\x17resend_activation_email\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x15resendActivationEmail\x12*\n\x0bunlock_user\x18\x03 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\nunlockUser\x12*\n\x0bgrant_admin\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\ngrantAdmin\x12,\n\x0crevoke_admin\x18\x05 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"!\n\x19\x43lusterUserActionResponseJ\x04\x08\x01\x10\x02\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xf3\x01\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x31\n\x15online_join_keys_path\x18\x02 \x01(\tR\x12onlineJoinKeysPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offline\"\x18\n\x16\x44\x65leteEntitiesResponse\"\xfd\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"\\\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02*\x12\x41\x43TION_LIST_TABLES*\x17\x41\x43TION_GET_TABLE_SCHEMA\"\xe1\x01\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06resultJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\xc9\x01\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboardingJ\x04\x08\x01\x10\x02\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\xaf\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\x12\x1a\n\x05limit\x18\x06 \x01(\x05:\x04\x35\x30\x30\x30R\x05limit\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x80\x04\n!GetFeatureValidationResultRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12\x39\n\x19\x66ilter_feature_view_names\x18\x04 \x03(\tR\x16\x66ilterFeatureViewNames\x12\x38\n\x18\x66ilter_expectation_names\x18\x05 \x03(\tR\x16\x66ilterExpectationNames\x12[\n\x13\x66ilter_result_types\x18\x06 \x03(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x11\x66ilterResultTypes\x12O\n\npagination\x18\x07 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xb9\x01\n\"GetFeatureValidationResultResponse\x12\x41\n\x07results\x18\x02 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\x12P\n\npagination\x18\x03 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\x1f\n\x1dGetFeatureServerConfigRequest\"\x90\x01\n\x1eGetFeatureServerConfigResponse\x12\"\n\x0c\x63urrentCount\x18\x01 \x01(\rR\x0c\x63urrentCount\x12&\n\x0e\x61vailableCount\x18\x02 \x01(\rR\x0e\x61vailableCount\x12\"\n\x0c\x64\x65siredCount\x18\x03 \x01(\rR\x0c\x64\x65siredCount\"5\n\x1dSetFeatureServerConfigRequest\x12\x14\n\x05\x63ount\x18\x01 \x01(\rR\x05\x63ount*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\xc1\x92\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe5\x01\n\x1aRestartMaterializationTask\x12?.tecton_proto.metadataservice.RestartMaterializationTaskRequest\x1a@.tecton_proto.metadataservice.RestartMaterializationTaskResponse\"D\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/restart-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\x93\x02\n\x15GetFeatureConsumption\x12:.tecton_proto.metadataservice.GetFeatureConsumptionRequest\x1a;.tecton_proto.metadataservice.GetFeatureConsumptionResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-feature-view-consumption:\x01*\xa2\xbc\xe6\xc0\x05>\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*!tecton/workspace#read_consumption\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xbd\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#create_plan\x12\xbc\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#create_plan\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xaa\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xc8\x01\xa2\xbc\xe6\xc0\x05v*$tecton/organization#create_workspace2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x63reate_workspace\x1a\x01\x31\x12\xb5\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"T\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x64\x65lete_workspace\x1a\x01\x31\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xe5\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\"b\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\x9a\x02\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x63reate_service_account\x1a\x01\x31\x12\xec\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\"c\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xa5\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16update_service_account\x1a\x01\x31\x12\xa5\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x64\x65lete_service_account\x1a\x01\x31\x12\x8a\x02\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"\x92\x01\xa2\xbc\xe6\xc0\x05r**tecton/organization#create_service_account2B\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin8\x01\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x63reate_api_key\x1a\x01\x31\x12\xb4\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"Y\xa2\xbc\xe6\xc0\x05\x39\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account8\x01\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x64\x65lete_api_key\x1a\x01\x31\x12\xa4\x01\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"0\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xff\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x63reate_cluster_user\x1a\x01\x31\x12\xff\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x64\x65lete_cluster_user\x1a\x01\x31\x12\xff\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x63luster_user_action\x1a\x01\x31\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\x91\x02\n\x1aGetFeatureValidationResult\x12?.tecton_proto.metadataservice.GetFeatureValidationResultRequest\x1a@.tecton_proto.metadataservice.GetFeatureValidationResultResponse\"p\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-feature-validation-result:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xfe\x01\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"i\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_userBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a!tecton_proto/auth/principal.proto\x1a$tecton_proto/auditlog/metadata.proto\x1a\x1ftecton_proto/auth/service.proto\x1a%tecton_proto/common/fco_locator.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/common/spark_schema.proto\x1a*tecton_proto/consumption/consumption.proto\x1a\x1etecton_proto/data/entity.proto\x1a\x1btecton_proto/data/fco.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a.tecton_proto/data/materialization_status.proto\x1a\"tecton_proto/data/onboarding.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a&tecton_proto/data/serving_status.proto\x1a$tecton_proto/data/state_update.proto\x1a\x1ftecton_proto/data/summary.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\x1a\x1ctecton_proto/data/user.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a\x39tecton_proto/materialization/materialization_states.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\x1a\'tecton_proto/validation/validator.proto\"\x90\x01\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x1e\n\ncomparison\x18\x03 \x01(\x03R\ncomparison\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\xbd\x01\n\x15ValidationResultToken\x12\x43\n\x0fvalidation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12\x34\n\tresult_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08resultId\x12)\n\x10\x65xpectation_name\x18\x03 \x01(\tR\x0f\x65xpectationName\"\xd3\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"`\n\x1cGetFeatureConsumptionRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"u\n\x1dGetFeatureConsumptionResponse\x12T\n\x10\x63onsumption_info\x18\x01 \x03(\x0b\x32).tecton_proto.consumption.ConsumptionInfoR\x0f\x63onsumptionInfo\"\xaf\x01\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x0finclude_deleted\x18\x02 \x01(\x08R\x0eincludeDeleted\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\xac\x07\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12I\n\x08statuses\x18\x03 \x03(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\x08statuses\x12`\n\x16last_task_state_change\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x13lastTaskStateChange\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n$include_update_materialization_flags\x18\x0c \x01(\x08R!includeUpdateMaterializationFlags\x12#\n\rwrites_online\x18\r \x01(\x08R\x0cwritesOnline\x12%\n\x0ewrites_offline\x18\x0e \x01(\x08R\rwritesOffline\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xb5\x05\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12K\n\ttaskState\x18\x02 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12-\n\x12manually_triggered\x18\t \x01(\x08R\x11manuallyTriggered\x12O\n\x16last_task_state_change\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13lastTaskStateChange\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"t\n!RestartMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\"\xa1\x01\n\"RestartMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\x12V\n\x1bnew_materialization_task_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x18newMaterializationTaskId\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"F\n\x12SparkClusterConfig\x12\x1a\n\x08original\x18\x01 \x01(\tR\x08original\x12\x14\n\x05\x66inal\x18\x02 \x01(\tR\x05\x66inal\"\xc4\x01\n\x16GetSparkConfigResponse\x12S\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0b\x62\x61tchConfig\x12U\n\rstream_config\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\xca\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xf3\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x04 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\xd0\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xe8\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"Z\n\x17\x46indFcoWorkspaceRequest\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xfd\x01\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xa9\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\xa5\x01\n\x16\x43reateWorkspaceRequest\x12.\n\x0eworkspace_name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\rworkspaceName\x12U\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"?\n\x16\x44\x65leteWorkspaceRequest\x12%\n\tworkspace\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"d\n\x13\x43reateApiKeyRequest\x12)\n\x0b\x64\x65scription\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12\"\n\x08is_admin\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07isAdmin\"Z\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"G\n\x13\x44\x65leteApiKeyRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\x9f\x02\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12\x36\n\x07\x63reator\x18\x05 \x01(\x0b\x32\x1c.tecton_proto.auth.PrincipalR\x07\x63reator\x12\x37\n\x05owner\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\x05owner\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"e\n\x1b\x43reateServiceAccountRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\"\xf9\x01\n\x1c\x43reateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\xa4\x01\n\x1bUpdateServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\"\xe0\x01\n\x1cUpdateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"6\n\x1b\x44\x65leteServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\"D\n\x18\x43reateClusterUserRequest\x12(\n\x0blogin_email\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\nloginEmail\"!\n\x19\x43reateClusterUserResponseJ\x04\x08\x01\x10\x02\"<\n\x18\x44\x65leteClusterUserRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\"!\n\x19\x44\x65leteClusterUserResponseJ\x04\x08\x01\x10\x02\"\x8f\x02\n\x18\x43lusterUserActionRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\x12\x41\n\x17resend_activation_email\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x15resendActivationEmail\x12*\n\x0bunlock_user\x18\x03 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\nunlockUser\x12*\n\x0bgrant_admin\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\ngrantAdmin\x12,\n\x0crevoke_admin\x18\x05 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"!\n\x19\x43lusterUserActionResponseJ\x04\x08\x01\x10\x02\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xf3\x01\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x31\n\x15online_join_keys_path\x18\x02 \x01(\tR\x12onlineJoinKeysPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offline\"\x18\n\x16\x44\x65leteEntitiesResponse\"\xfd\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"\\\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02*\x12\x41\x43TION_LIST_TABLES*\x17\x41\x43TION_GET_TABLE_SCHEMA\"\xe1\x01\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06resultJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\xc9\x01\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboardingJ\x04\x08\x01\x10\x02\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\xaf\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\x12\x1a\n\x05limit\x18\x06 \x01(\x05:\x04\x35\x30\x30\x30R\x05limit\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x80\x04\n!GetFeatureValidationResultRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12\x39\n\x19\x66ilter_feature_view_names\x18\x04 \x03(\tR\x16\x66ilterFeatureViewNames\x12\x38\n\x18\x66ilter_expectation_names\x18\x05 \x03(\tR\x16\x66ilterExpectationNames\x12[\n\x13\x66ilter_result_types\x18\x06 \x03(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x11\x66ilterResultTypes\x12O\n\npagination\x18\x07 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xb9\x01\n\"GetFeatureValidationResultResponse\x12\x41\n\x07results\x18\x02 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\x12P\n\npagination\x18\x03 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\x1f\n\x1dGetFeatureServerConfigRequest\"\x90\x01\n\x1eGetFeatureServerConfigResponse\x12\"\n\x0c\x63urrentCount\x18\x01 \x01(\rR\x0c\x63urrentCount\x12&\n\x0e\x61vailableCount\x18\x02 \x01(\rR\x0e\x61vailableCount\x12\"\n\x0c\x64\x65siredCount\x18\x03 \x01(\rR\x0c\x64\x65siredCount\"5\n\x1dSetFeatureServerConfigRequest\x12\x14\n\x05\x63ount\x18\x01 \x01(\rR\x05\x63ount*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\xc1\x92\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe5\x01\n\x1aRestartMaterializationTask\x12?.tecton_proto.metadataservice.RestartMaterializationTaskRequest\x1a@.tecton_proto.metadataservice.RestartMaterializationTaskResponse\"D\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/restart-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\x93\x02\n\x15GetFeatureConsumption\x12:.tecton_proto.metadataservice.GetFeatureConsumptionRequest\x1a;.tecton_proto.metadataservice.GetFeatureConsumptionResponse\"\x80\x01\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-feature-view-consumption:\x01*\xa2\xbc\xe6\xc0\x05>\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*!tecton/workspace#read_consumption\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xbd\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#create_plan\x12\xbc\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#create_plan\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xaa\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xc8\x01\xa2\xbc\xe6\xc0\x05v*$tecton/organization#create_workspace2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x63reate_workspace\x1a\x01\x31\x12\xb5\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"T\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x64\x65lete_workspace\x1a\x01\x31\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xe5\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\"b\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\x9a\x02\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x63reate_service_account\x1a\x01\x31\x12\xec\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\"c\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xa5\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16update_service_account\x1a\x01\x31\x12\xa5\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x64\x65lete_service_account\x1a\x01\x31\x12\x8a\x02\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"\x92\x01\xa2\xbc\xe6\xc0\x05r**tecton/organization#create_service_account2B\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin8\x01\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x63reate_api_key\x1a\x01\x31\x12\xb4\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"Y\xa2\xbc\xe6\xc0\x05\x39\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account8\x01\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x64\x65lete_api_key\x1a\x01\x31\x12\xa4\x01\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"0\xa2\xbc\xe6\xc0\x05**(tecton/organization#list_service_account\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xff\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x63reate_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x64\x65lete_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x61\x63\x63ount_user_action\x1a\x01\x31\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\x91\x02\n\x1aGetFeatureValidationResult\x12?.tecton_proto.metadataservice.GetFeatureValidationResultRequest\x1a@.tecton_proto.metadataservice.GetFeatureValidationResultResponse\"p\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-feature-validation-result:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xfe\x01\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"i\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_userBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.metadataservice.metadata_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032com.tecton.metadataserviceB\024MetadataServiceProtoP\001Z1github.com/tecton-ai/tecton_proto/metadataservice'
@@ -249,19 +249,19 @@
   _METADATASERVICE.methods_by_name['GetNewIngestDataframeInfo']._options = None
   _METADATASERVICE.methods_by_name['GetNewIngestDataframeInfo']._serialized_options = b'\242\274\346\300\005\002@\001'
   _METADATASERVICE.methods_by_name['IngestDataframe']._options = None
   _METADATASERVICE.methods_by_name['IngestDataframe']._serialized_options = b'\242\274\346\300\0051\032\r\010\001\022\tworkspace* tecton/workspace#ingest_features'
   _METADATASERVICE.methods_by_name['GetClusterAdminInfo']._options = None
   _METADATASERVICE.methods_by_name['GetClusterAdminInfo']._serialized_options = b'\202\323\344\223\0020\"+/v1/metadata-service/get-cluster-admin-info:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['CreateClusterUser']._options = None
-  _METADATASERVICE.methods_by_name['CreateClusterUser']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/create-cluster-user:\001*\242\274\346\300\005!*\037tecton/organization#create_user\362\231\275F\032\010\001\022\023create_cluster_user\032\0011'
+  _METADATASERVICE.methods_by_name['CreateClusterUser']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/create-cluster-user:\001*\242\274\346\300\005!*\037tecton/organization#create_user\362\231\275F\032\010\001\022\023create_account_user\032\0011'
   _METADATASERVICE.methods_by_name['DeleteClusterUser']._options = None
-  _METADATASERVICE.methods_by_name['DeleteClusterUser']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/delete-cluster-user:\001*\242\274\346\300\005!*\037tecton/organization#manage_user\362\231\275F\032\010\001\022\023delete_cluster_user\032\0011'
+  _METADATASERVICE.methods_by_name['DeleteClusterUser']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/delete-cluster-user:\001*\242\274\346\300\005!*\037tecton/organization#manage_user\362\231\275F\032\010\001\022\023delete_account_user\032\0011'
   _METADATASERVICE.methods_by_name['ClusterUserAction']._options = None
-  _METADATASERVICE.methods_by_name['ClusterUserAction']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/cluster-user-action:\001*\242\274\346\300\005!*\037tecton/organization#manage_user\362\231\275F\032\010\001\022\023cluster_user_action\032\0011'
+  _METADATASERVICE.methods_by_name['ClusterUserAction']._serialized_options = b'\202\323\344\223\002-\"(/v1/metadata-service/cluster-user-action:\001*\242\274\346\300\005!*\037tecton/organization#manage_user\362\231\275F\032\010\001\022\023account_user_action\032\0011'
   _METADATASERVICE.methods_by_name['GetUserDeploymentSettings']._options = None
   _METADATASERVICE.methods_by_name['GetUserDeploymentSettings']._serialized_options = b'\202\323\344\223\0026\"1/v1/metadata-service/get-user-deployment-settings:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['UpdateUserDeploymentSettings']._options = None
   _METADATASERVICE.methods_by_name['UpdateUserDeploymentSettings']._serialized_options = b'\202\323\344\223\0029\"4/v1/metadata-service/update-user-deployment-settings:\001*\242\274\346\300\0050*.tecton/organization#manage_deployment_settings'
   _METADATASERVICE.methods_by_name['GetInternalSparkClusterStatus']._options = None
   _METADATASERVICE.methods_by_name['GetInternalSparkClusterStatus']._serialized_options = b'\202\323\344\223\002;\"6/v1/metadata-service/get-internal-spark-cluster-status:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['GetDeleteEntitiesInfo']._options = None
@@ -284,16 +284,16 @@
   _METADATASERVICE.methods_by_name['GetFeatureValidationResult']._serialized_options = b'\202\323\344\223\0027\"2/v1/metadata-service/get-feature-validation-result:\001*\242\274\346\300\005-\032\r\010\001\022\tworkspace*\034tecton/workspace#read_metric'
   _METADATASERVICE.methods_by_name['GetFeatureServerConfig']._options = None
   _METADATASERVICE.methods_by_name['GetFeatureServerConfig']._serialized_options = b'\202\323\344\223\0023\"./v1/metadata-service/get-feature-server-config:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['SetFeatureServerConfig']._options = None
   _METADATASERVICE.methods_by_name['SetFeatureServerConfig']._serialized_options = b'\202\323\344\223\0023\"./v1/metadata-service/set-feature-server-config:\001*\242\274\346\300\005**(tecton/organization#scale_feature_server'
   _METADATASERVICE.methods_by_name['GetUser']._options = None
   _METADATASERVICE.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002\"\"\035/v1/metadata-service/get-user:\001*\242\274\346\300\005\037*\035tecton/organization#list_user'
-  _SORTDIRECTION._serialized_start=25191
-  _SORTDIRECTION._serialized_end=25253
+  _SORTDIRECTION._serialized_start=25267
+  _SORTDIRECTION._serialized_end=25329
   _JOBSKEYSET._serialized_start=1614
   _JOBSKEYSET._serialized_end=1758
   _PAGINATIONREQUEST._serialized_start=1761
   _PAGINATIONREQUEST._serialized_end=1969
   _PAGINATIONRESPONSE._serialized_start=1972
   _PAGINATIONRESPONSE._serialized_end=2212
   _VALIDATIONRESULTTOKEN._serialized_start=2215
@@ -351,267 +351,267 @@
   _COUNTRANGE._serialized_start=5627
   _COUNTRANGE._serialized_end=5679
   _DURATIONRANGE._serialized_start=5681
   _DURATIONRANGE._serialized_end=5790
   _DATETIMERANGE._serialized_start=5792
   _DATETIMERANGE._serialized_end=5903
   _GETJOBSREQUEST._serialized_start=5906
-  _GETJOBSREQUEST._serialized_end=6770
-  _FEATUREVIEWMATERIALIZATIONSTATUS._serialized_start=6773
-  _FEATUREVIEWMATERIALIZATIONSTATUS._serialized_end=6970
-  _TASKWITHATTEMPTS._serialized_start=6973
-  _TASKWITHATTEMPTS._serialized_end=7666
-  _GETALLMATERIALIZATIONSTATUSINLIVEWORKSPACESRESPONSE._serialized_start=7669
-  _GETALLMATERIALIZATIONSTATUSINLIVEWORKSPACESRESPONSE._serialized_end=7866
-  _GETJOBSRESPONSE._serialized_start=7869
-  _GETJOBSRESPONSE._serialized_end=8062
-  _FORCERETRYMATERIALIZATIONTASKREQUEST._serialized_start=8065
-  _FORCERETRYMATERIALIZATIONTASKREQUEST._serialized_end=8225
-  _FORCERETRYMATERIALIZATIONTASKRESPONSE._serialized_start=8227
-  _FORCERETRYMATERIALIZATIONTASKRESPONSE._serialized_end=8303
-  _RESTARTMATERIALIZATIONTASKREQUEST._serialized_start=8305
-  _RESTARTMATERIALIZATIONTASKREQUEST._serialized_end=8421
-  _RESTARTMATERIALIZATIONTASKRESPONSE._serialized_start=8424
-  _RESTARTMATERIALIZATIONTASKRESPONSE._serialized_end=8585
-  _GETFCOSREQUEST._serialized_start=8587
-  _GETFCOSREQUEST._serialized_end=8633
-  _GETFCOSRESPONSE._serialized_start=8635
-  _GETFCOSRESPONSE._serialized_end=8722
-  _GETSPARKCONFIGREQUEST._serialized_start=8724
-  _GETSPARKCONFIGREQUEST._serialized_end=8821
-  _SPARKCLUSTERCONFIG._serialized_start=8823
-  _SPARKCLUSTERCONFIG._serialized_end=8893
-  _GETSPARKCONFIGRESPONSE._serialized_start=8896
-  _GETSPARKCONFIGRESPONSE._serialized_end=9092
-  _GETMETRICANDEXPECTATIONDEFINITIONREQUEST._serialized_start=9094
-  _GETMETRICANDEXPECTATIONDEFINITIONREQUEST._serialized_end=9210
-  _GETMETRICANDEXPECTATIONDEFINITIONRESPONSE._serialized_start=9213
-  _GETMETRICANDEXPECTATIONDEFINITIONRESPONSE._serialized_end=9569
-  _GETFEATUREVIEWREQUEST._serialized_start=9572
-  _GETFEATUREVIEWREQUEST._serialized_end=9774
-  _GETFEATUREVIEWRESPONSE._serialized_start=9776
-  _GETFEATUREVIEWRESPONSE._serialized_end=9870
-  _GETFEATUREVIEWSUMMARYREQUEST._serialized_start=9872
-  _GETFEATUREVIEWSUMMARYREQUEST._serialized_end=9968
-  _GETFEATUREVIEWSUMMARYRESPONSE._serialized_start=9970
-  _GETFEATUREVIEWSUMMARYRESPONSE._serialized_end=10065
-  _QUERYFEATUREVIEWSREQUEST._serialized_start=10067
-  _QUERYFEATUREVIEWSREQUEST._serialized_end=10149
-  _QUERYFEATUREVIEWSRESPONSE._serialized_start=10151
-  _QUERYFEATUREVIEWSRESPONSE._serialized_end=10248
-  _GETMATERIALIZINGFEATUREVIEWSINLIVEWORKSPACESRESPONSE._serialized_start=10250
-  _GETMATERIALIZINGFEATUREVIEWSINLIVEWORKSPACESRESPONSE._serialized_end=10373
-  _GETVIRTUALDATASOURCEREQUEST._serialized_start=10376
-  _GETVIRTUALDATASOURCEREQUEST._serialized_end=10619
-  _GETVIRTUALDATASOURCERESPONSE._serialized_start=10621
-  _GETVIRTUALDATASOURCERESPONSE._serialized_end=10721
-  _GETALLVIRTUALDATASOURCESREQUEST._serialized_start=10723
-  _GETALLVIRTUALDATASOURCESREQUEST._serialized_end=10786
-  _GETALLVIRTUALDATASOURCESRESPONSE._serialized_start=10788
-  _GETALLVIRTUALDATASOURCESRESPONSE._serialized_end=10910
-  _GETENTITYREQUEST._serialized_start=10913
-  _GETENTITYREQUEST._serialized_end=11121
-  _GETENTITYRESPONSE._serialized_start=11123
-  _GETENTITYRESPONSE._serialized_end=11212
-  _GETALLENTITIESREQUEST._serialized_start=11214
-  _GETALLENTITIESREQUEST._serialized_end=11267
-  _GETALLENTITIESRESPONSE._serialized_start=11269
-  _GETALLENTITIESRESPONSE._serialized_end=11348
-  _GETTRANSFORMATIONREQUEST._serialized_start=11351
-  _GETTRANSFORMATIONREQUEST._serialized_end=11583
-  _GETTRANSFORMATIONRESPONSE._serialized_start=11585
-  _GETTRANSFORMATIONRESPONSE._serialized_end=11688
-  _GETALLTRANSFORMATIONSREQUEST._serialized_start=11690
-  _GETALLTRANSFORMATIONSREQUEST._serialized_end=11750
-  _GETALLTRANSFORMATIONSRESPONSE._serialized_start=11752
-  _GETALLTRANSFORMATIONSRESPONSE._serialized_end=11866
-  _FINDFCOWORKSPACEREQUEST._serialized_start=11868
-  _FINDFCOWORKSPACEREQUEST._serialized_end=11958
-  _FINDFCOWORKSPACERESPONSE._serialized_start=11960
-  _FINDFCOWORKSPACERESPONSE._serialized_end=12016
-  _INGESTCLIENTLOGSREQUEST._serialized_start=12018
-  _INGESTCLIENTLOGSREQUEST._serialized_end=12140
-  _INGESTANALYTICSREQUEST._serialized_start=12142
-  _INGESTANALYTICSREQUEST._serialized_end=12260
-  _NEWSTATEUPDATEREQUEST._serialized_start=12263
-  _NEWSTATEUPDATEREQUEST._serialized_end=12454
-  _NEWSTATEUPDATEREQUESTV2._serialized_start=12457
-  _NEWSTATEUPDATEREQUESTV2._serialized_end=12710
-  _NEWSTATEUPDATERESPONSE._serialized_start=12713
-  _NEWSTATEUPDATERESPONSE._serialized_end=12944
-  _NEWSTATEUPDATERESPONSEV2._serialized_start=12947
-  _NEWSTATEUPDATERESPONSEV2._serialized_end=13182
-  _QUERYSTATEUPDATEREQUEST._serialized_start=13184
-  _QUERYSTATEUPDATEREQUEST._serialized_end=13291
-  _QUERYSTATEUPDATEREQUESTV2._serialized_start=13294
-  _QUERYSTATEUPDATEREQUESTV2._serialized_end=13463
-  _QUERYSTATEUPDATERESPONSE._serialized_start=13466
-  _QUERYSTATEUPDATERESPONSE._serialized_end=13806
-  _QUERYSTATEUPDATERESPONSEV2._serialized_start=13809
-  _QUERYSTATEUPDATERESPONSEV2._serialized_end=14170
-  _GETSTATEUPDATEPLANSUMMARYREQUEST._serialized_start=14172
-  _GETSTATEUPDATEPLANSUMMARYREQUEST._serialized_end=14256
-  _GETSTATEUPDATEPLANSUMMARYRESPONSE._serialized_start=14258
-  _GETSTATEUPDATEPLANSUMMARYRESPONSE._serialized_end=14356
-  _APPLYSTATEUPDATEREQUEST._serialized_start=14358
-  _APPLYSTATEUPDATEREQUEST._serialized_end=14470
-  _APPLYSTATEUPDATERESPONSE._serialized_start=14472
-  _APPLYSTATEUPDATERESPONSE._serialized_end=14498
-  _GETCONFIGSRESPONSE._serialized_start=14501
-  _GETCONFIGSRESPONSE._serialized_end=14679
-  _GETCONFIGSRESPONSE_KEYVALUESENTRY._serialized_start=14619
-  _GETCONFIGSRESPONSE_KEYVALUESENTRY._serialized_end=14679
-  _GETGLOBALSFORWEBUIRESPONSE._serialized_start=14682
-  _GETGLOBALSFORWEBUIRESPONSE._serialized_end=14876
-  _GETGLOBALSFORWEBUIRESPONSE_KEYVALUESENTRY._serialized_start=14619
-  _GETGLOBALSFORWEBUIRESPONSE_KEYVALUESENTRY._serialized_end=14679
-  _GETSTATEUPDATELOGREQUEST._serialized_start=14878
-  _GETSTATEUPDATELOGREQUEST._serialized_end=14956
-  _GETSTATEUPDATELOGRESPONSE._serialized_start=14958
-  _GETSTATEUPDATELOGRESPONSE._serialized_end=15048
-  _GETRESTOREINFOREQUEST._serialized_start=15050
-  _GETRESTOREINFOREQUEST._serialized_end=15132
-  _GETRESTOREINFORESPONSE._serialized_start=15135
-  _GETRESTOREINFORESPONSE._serialized_end=15285
-  _CREATEWORKSPACEREQUEST._serialized_start=15288
-  _CREATEWORKSPACEREQUEST._serialized_end=15453
-  _DELETEWORKSPACEREQUEST._serialized_start=15455
-  _DELETEWORKSPACEREQUEST._serialized_end=15518
-  _INTROSPECTAPIKEYREQUEST._serialized_start=15520
-  _INTROSPECTAPIKEYREQUEST._serialized_end=15570
-  _INTROSPECTAPIKEYRESPONSE._serialized_start=15573
-  _INTROSPECTAPIKEYRESPONSE._serialized_end=15776
-  _CREATEAPIKEYREQUEST._serialized_start=15778
-  _CREATEAPIKEYREQUEST._serialized_end=15878
-  _CREATEAPIKEYRESPONSE._serialized_start=15880
-  _CREATEAPIKEYRESPONSE._serialized_end=15970
-  _DELETEAPIKEYREQUEST._serialized_start=15972
-  _DELETEAPIKEYREQUEST._serialized_end=16043
-  _LISTAPIKEYSREQUEST._serialized_start=16045
-  _LISTAPIKEYSREQUEST._serialized_end=16108
-  _LISTAPIKEYSRESPONSE._serialized_start=16110
-  _LISTAPIKEYSRESPONSE._serialized_end=16191
-  _SERVICEACCOUNT._serialized_start=16194
-  _SERVICEACCOUNT._serialized_end=16481
-  _CREATESERVICEACCOUNTREQUEST._serialized_start=16483
-  _CREATESERVICEACCOUNTREQUEST._serialized_end=16584
-  _CREATESERVICEACCOUNTRESPONSE._serialized_start=16587
-  _CREATESERVICEACCOUNTRESPONSE._serialized_end=16836
-  _GETSERVICEACCOUNTSREQUEST._serialized_start=16838
-  _GETSERVICEACCOUNTSREQUEST._serialized_end=16907
-  _GETSERVICEACCOUNTSRESPONSE._serialized_start=16909
-  _GETSERVICEACCOUNTSRESPONSE._serialized_end=17026
-  _UPDATESERVICEACCOUNTREQUEST._serialized_start=17029
-  _UPDATESERVICEACCOUNTREQUEST._serialized_end=17193
-  _UPDATESERVICEACCOUNTRESPONSE._serialized_start=17196
-  _UPDATESERVICEACCOUNTRESPONSE._serialized_end=17420
-  _DELETESERVICEACCOUNTREQUEST._serialized_start=17422
-  _DELETESERVICEACCOUNTREQUEST._serialized_end=17476
-  _DELETESERVICEACCOUNTRESPONSE._serialized_start=17478
-  _DELETESERVICEACCOUNTRESPONSE._serialized_end=17508
-  _LISTWORKSPACESREQUEST._serialized_start=17510
-  _LISTWORKSPACESREQUEST._serialized_end=17533
-  _LISTWORKSPACESRESPONSE._serialized_start=17535
-  _LISTWORKSPACESRESPONSE._serialized_end=17621
-  _GETWORKSPACEREQUEST._serialized_start=17623
-  _GETWORKSPACEREQUEST._serialized_end=17683
-  _GETWORKSPACERESPONSE._serialized_start=17685
-  _GETWORKSPACERESPONSE._serialized_end=17767
-  _CREATESAVEDFEATUREDATAFRAMEREQUEST._serialized_start=17770
-  _CREATESAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18173
-  _CREATESAVEDFEATUREDATAFRAMERESPONSE._serialized_start=18176
-  _CREATESAVEDFEATUREDATAFRAMERESPONSE._serialized_end=18311
-  _ARCHIVESAVEDFEATUREDATAFRAMEREQUEST._serialized_start=18313
-  _ARCHIVESAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18436
-  _ARCHIVESAVEDFEATUREDATAFRAMERESPONSE._serialized_start=18438
-  _ARCHIVESAVEDFEATUREDATAFRAMERESPONSE._serialized_end=18476
-  _GETSAVEDFEATUREDATAFRAMEREQUEST._serialized_start=18479
-  _GETSAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18710
-  _GETCLUSTERADMININFORESPONSE._serialized_start=18713
-  _GETCLUSTERADMININFORESPONSE._serialized_end=18878
-  _CREATECLUSTERUSERREQUEST._serialized_start=18880
-  _CREATECLUSTERUSERREQUEST._serialized_end=18948
-  _CREATECLUSTERUSERRESPONSE._serialized_start=18950
-  _CREATECLUSTERUSERRESPONSE._serialized_end=18983
-  _DELETECLUSTERUSERREQUEST._serialized_start=18985
-  _DELETECLUSTERUSERREQUEST._serialized_end=19045
-  _DELETECLUSTERUSERRESPONSE._serialized_start=19047
-  _DELETECLUSTERUSERRESPONSE._serialized_end=19080
-  _CLUSTERUSERACTIONREQUEST._serialized_start=19083
-  _CLUSTERUSERACTIONREQUEST._serialized_end=19354
-  _CLUSTERUSERACTIONRESPONSE._serialized_start=19356
-  _CLUSTERUSERACTIONRESPONSE._serialized_end=19389
-  _GETSAVEDFEATUREDATAFRAMERESPONSE._serialized_start=19392
-  _GETSAVEDFEATUREDATAFRAMERESPONSE._serialized_end=19524
-  _GETALLSAVEDFEATUREDATAFRAMESREQUEST._serialized_start=19526
-  _GETALLSAVEDFEATUREDATAFRAMESREQUEST._serialized_end=19593
-  _GETALLSAVEDFEATUREDATAFRAMESRESPONSE._serialized_start=19596
-  _GETALLSAVEDFEATUREDATAFRAMESRESPONSE._serialized_end=19734
-  _INGESTDATAFRAMEREQUEST._serialized_start=19737
-  _INGESTDATAFRAMEREQUEST._serialized_end=19893
-  _INGESTDATAFRAMERESPONSE._serialized_start=19895
-  _INGESTDATAFRAMERESPONSE._serialized_end=19920
-  _GETNEWINGESTDATAFRAMEINFOREQUEST._serialized_start=19922
-  _GETNEWINGESTDATAFRAMEINFOREQUEST._serialized_end=20033
-  _GETNEWINGESTDATAFRAMEINFORESPONSE._serialized_start=20035
-  _GETNEWINGESTDATAFRAMEINFORESPONSE._serialized_end=20151
-  _GETUSERDEPLOYMENTSETTINGSRESPONSE._serialized_start=20154
-  _GETUSERDEPLOYMENTSETTINGSRESPONSE._serialized_end=20290
-  _UPDATEUSERDEPLOYMENTSETTINGSREQUEST._serialized_start=20293
-  _UPDATEUSERDEPLOYMENTSETTINGSREQUEST._serialized_end=20490
-  _UPDATEUSERDEPLOYMENTSETTINGSRESPONSE._serialized_start=20492
-  _UPDATEUSERDEPLOYMENTSETTINGSRESPONSE._serialized_end=20593
-  _GETINTERNALSPARKCLUSTERSTATUSRESPONSE._serialized_start=20595
-  _GETINTERNALSPARKCLUSTERSTATUSRESPONSE._serialized_end=20705
-  _GETDELETEENTITIESINFOREQUEST._serialized_start=20707
-  _GETDELETEENTITIESINFOREQUEST._serialized_end=20814
-  _GETDELETEENTITIESINFORESPONSE._serialized_start=20817
-  _GETDELETEENTITIESINFORESPONSE._serialized_end=21019
-  _DELETEENTITIESREQUEST._serialized_start=21022
-  _DELETEENTITIESREQUEST._serialized_end=21265
-  _DELETEENTITIESRESPONSE._serialized_start=21267
-  _DELETEENTITIESRESPONSE._serialized_end=21291
-  _GETHIVEMETADATAREQUEST._serialized_start=21294
-  _GETHIVEMETADATAREQUEST._serialized_end=21547
-  _GETHIVEMETADATAREQUEST_ACTION._serialized_start=21455
-  _GETHIVEMETADATAREQUEST_ACTION._serialized_end=21547
-  _GETHIVEMETADATARESPONSE._serialized_start=21550
-  _GETHIVEMETADATARESPONSE._serialized_end=21775
-  _VALIDATELOCALFCOREQUEST._serialized_start=21778
-  _VALIDATELOCALFCOREQUEST._serialized_end=21927
-  _VALIDATELOCALFCORESPONSE._serialized_start=21930
-  _VALIDATELOCALFCORESPONSE._serialized_end=22086
-  _GETONBOARDINGSTATUSREQUEST._serialized_start=22088
-  _GETONBOARDINGSTATUSREQUEST._serialized_end=22146
-  _GETONBOARDINGSTATUSRESPONSE._serialized_start=22149
-  _GETONBOARDINGSTATUSRESPONSE._serialized_end=22350
-  _GETDATAPLATFORMSETUPSTATUSRESPONSE._serialized_start=22353
-  _GETDATAPLATFORMSETUPSTATUSRESPONSE._serialized_end=22499
-  _GETOBSERVABILITYCONFIGREQUEST._serialized_start=22501
-  _GETOBSERVABILITYCONFIGREQUEST._serialized_end=22606
-  _GETOBSERVABILITYCONFIGRESPONSE._serialized_start=22609
-  _GETOBSERVABILITYCONFIGRESPONSE._serialized_end=22774
-  _QUERYMETRICREQUEST._serialized_start=22777
-  _QUERYMETRICREQUEST._serialized_end=23080
-  _QUERYMETRICRESPONSE._serialized_start=23083
-  _QUERYMETRICRESPONSE._serialized_end=23584
-  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_start=23587
-  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_end=24099
-  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_start=24102
-  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_end=24287
-  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_start=24290
-  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_end=24512
-  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_start=24515
-  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_end=24829
-  _GETUSERREQUEST._serialized_start=24831
-  _GETUSERREQUEST._serialized_end=24885
-  _GETUSERRESPONSE._serialized_start=24887
-  _GETUSERRESPONSE._serialized_end=24954
-  _GETFEATURESERVERCONFIGREQUEST._serialized_start=24956
-  _GETFEATURESERVERCONFIGREQUEST._serialized_end=24987
-  _GETFEATURESERVERCONFIGRESPONSE._serialized_start=24990
-  _GETFEATURESERVERCONFIGRESPONSE._serialized_end=25134
-  _SETFEATURESERVERCONFIGREQUEST._serialized_start=25136
-  _SETFEATURESERVERCONFIGREQUEST._serialized_end=25189
-  _METADATASERVICE._serialized_start=25257
-  _METADATASERVICE._serialized_end=44010
+  _GETJOBSREQUEST._serialized_end=6846
+  _FEATUREVIEWMATERIALIZATIONSTATUS._serialized_start=6849
+  _FEATUREVIEWMATERIALIZATIONSTATUS._serialized_end=7046
+  _TASKWITHATTEMPTS._serialized_start=7049
+  _TASKWITHATTEMPTS._serialized_end=7742
+  _GETALLMATERIALIZATIONSTATUSINLIVEWORKSPACESRESPONSE._serialized_start=7745
+  _GETALLMATERIALIZATIONSTATUSINLIVEWORKSPACESRESPONSE._serialized_end=7942
+  _GETJOBSRESPONSE._serialized_start=7945
+  _GETJOBSRESPONSE._serialized_end=8138
+  _FORCERETRYMATERIALIZATIONTASKREQUEST._serialized_start=8141
+  _FORCERETRYMATERIALIZATIONTASKREQUEST._serialized_end=8301
+  _FORCERETRYMATERIALIZATIONTASKRESPONSE._serialized_start=8303
+  _FORCERETRYMATERIALIZATIONTASKRESPONSE._serialized_end=8379
+  _RESTARTMATERIALIZATIONTASKREQUEST._serialized_start=8381
+  _RESTARTMATERIALIZATIONTASKREQUEST._serialized_end=8497
+  _RESTARTMATERIALIZATIONTASKRESPONSE._serialized_start=8500
+  _RESTARTMATERIALIZATIONTASKRESPONSE._serialized_end=8661
+  _GETFCOSREQUEST._serialized_start=8663
+  _GETFCOSREQUEST._serialized_end=8709
+  _GETFCOSRESPONSE._serialized_start=8711
+  _GETFCOSRESPONSE._serialized_end=8798
+  _GETSPARKCONFIGREQUEST._serialized_start=8800
+  _GETSPARKCONFIGREQUEST._serialized_end=8897
+  _SPARKCLUSTERCONFIG._serialized_start=8899
+  _SPARKCLUSTERCONFIG._serialized_end=8969
+  _GETSPARKCONFIGRESPONSE._serialized_start=8972
+  _GETSPARKCONFIGRESPONSE._serialized_end=9168
+  _GETMETRICANDEXPECTATIONDEFINITIONREQUEST._serialized_start=9170
+  _GETMETRICANDEXPECTATIONDEFINITIONREQUEST._serialized_end=9286
+  _GETMETRICANDEXPECTATIONDEFINITIONRESPONSE._serialized_start=9289
+  _GETMETRICANDEXPECTATIONDEFINITIONRESPONSE._serialized_end=9645
+  _GETFEATUREVIEWREQUEST._serialized_start=9648
+  _GETFEATUREVIEWREQUEST._serialized_end=9850
+  _GETFEATUREVIEWRESPONSE._serialized_start=9852
+  _GETFEATUREVIEWRESPONSE._serialized_end=9946
+  _GETFEATUREVIEWSUMMARYREQUEST._serialized_start=9948
+  _GETFEATUREVIEWSUMMARYREQUEST._serialized_end=10044
+  _GETFEATUREVIEWSUMMARYRESPONSE._serialized_start=10046
+  _GETFEATUREVIEWSUMMARYRESPONSE._serialized_end=10141
+  _QUERYFEATUREVIEWSREQUEST._serialized_start=10143
+  _QUERYFEATUREVIEWSREQUEST._serialized_end=10225
+  _QUERYFEATUREVIEWSRESPONSE._serialized_start=10227
+  _QUERYFEATUREVIEWSRESPONSE._serialized_end=10324
+  _GETMATERIALIZINGFEATUREVIEWSINLIVEWORKSPACESRESPONSE._serialized_start=10326
+  _GETMATERIALIZINGFEATUREVIEWSINLIVEWORKSPACESRESPONSE._serialized_end=10449
+  _GETVIRTUALDATASOURCEREQUEST._serialized_start=10452
+  _GETVIRTUALDATASOURCEREQUEST._serialized_end=10695
+  _GETVIRTUALDATASOURCERESPONSE._serialized_start=10697
+  _GETVIRTUALDATASOURCERESPONSE._serialized_end=10797
+  _GETALLVIRTUALDATASOURCESREQUEST._serialized_start=10799
+  _GETALLVIRTUALDATASOURCESREQUEST._serialized_end=10862
+  _GETALLVIRTUALDATASOURCESRESPONSE._serialized_start=10864
+  _GETALLVIRTUALDATASOURCESRESPONSE._serialized_end=10986
+  _GETENTITYREQUEST._serialized_start=10989
+  _GETENTITYREQUEST._serialized_end=11197
+  _GETENTITYRESPONSE._serialized_start=11199
+  _GETENTITYRESPONSE._serialized_end=11288
+  _GETALLENTITIESREQUEST._serialized_start=11290
+  _GETALLENTITIESREQUEST._serialized_end=11343
+  _GETALLENTITIESRESPONSE._serialized_start=11345
+  _GETALLENTITIESRESPONSE._serialized_end=11424
+  _GETTRANSFORMATIONREQUEST._serialized_start=11427
+  _GETTRANSFORMATIONREQUEST._serialized_end=11659
+  _GETTRANSFORMATIONRESPONSE._serialized_start=11661
+  _GETTRANSFORMATIONRESPONSE._serialized_end=11764
+  _GETALLTRANSFORMATIONSREQUEST._serialized_start=11766
+  _GETALLTRANSFORMATIONSREQUEST._serialized_end=11826
+  _GETALLTRANSFORMATIONSRESPONSE._serialized_start=11828
+  _GETALLTRANSFORMATIONSRESPONSE._serialized_end=11942
+  _FINDFCOWORKSPACEREQUEST._serialized_start=11944
+  _FINDFCOWORKSPACEREQUEST._serialized_end=12034
+  _FINDFCOWORKSPACERESPONSE._serialized_start=12036
+  _FINDFCOWORKSPACERESPONSE._serialized_end=12092
+  _INGESTCLIENTLOGSREQUEST._serialized_start=12094
+  _INGESTCLIENTLOGSREQUEST._serialized_end=12216
+  _INGESTANALYTICSREQUEST._serialized_start=12218
+  _INGESTANALYTICSREQUEST._serialized_end=12336
+  _NEWSTATEUPDATEREQUEST._serialized_start=12339
+  _NEWSTATEUPDATEREQUEST._serialized_end=12530
+  _NEWSTATEUPDATEREQUESTV2._serialized_start=12533
+  _NEWSTATEUPDATEREQUESTV2._serialized_end=12786
+  _NEWSTATEUPDATERESPONSE._serialized_start=12789
+  _NEWSTATEUPDATERESPONSE._serialized_end=13020
+  _NEWSTATEUPDATERESPONSEV2._serialized_start=13023
+  _NEWSTATEUPDATERESPONSEV2._serialized_end=13258
+  _QUERYSTATEUPDATEREQUEST._serialized_start=13260
+  _QUERYSTATEUPDATEREQUEST._serialized_end=13367
+  _QUERYSTATEUPDATEREQUESTV2._serialized_start=13370
+  _QUERYSTATEUPDATEREQUESTV2._serialized_end=13539
+  _QUERYSTATEUPDATERESPONSE._serialized_start=13542
+  _QUERYSTATEUPDATERESPONSE._serialized_end=13882
+  _QUERYSTATEUPDATERESPONSEV2._serialized_start=13885
+  _QUERYSTATEUPDATERESPONSEV2._serialized_end=14246
+  _GETSTATEUPDATEPLANSUMMARYREQUEST._serialized_start=14248
+  _GETSTATEUPDATEPLANSUMMARYREQUEST._serialized_end=14332
+  _GETSTATEUPDATEPLANSUMMARYRESPONSE._serialized_start=14334
+  _GETSTATEUPDATEPLANSUMMARYRESPONSE._serialized_end=14432
+  _APPLYSTATEUPDATEREQUEST._serialized_start=14434
+  _APPLYSTATEUPDATEREQUEST._serialized_end=14546
+  _APPLYSTATEUPDATERESPONSE._serialized_start=14548
+  _APPLYSTATEUPDATERESPONSE._serialized_end=14574
+  _GETCONFIGSRESPONSE._serialized_start=14577
+  _GETCONFIGSRESPONSE._serialized_end=14755
+  _GETCONFIGSRESPONSE_KEYVALUESENTRY._serialized_start=14695
+  _GETCONFIGSRESPONSE_KEYVALUESENTRY._serialized_end=14755
+  _GETGLOBALSFORWEBUIRESPONSE._serialized_start=14758
+  _GETGLOBALSFORWEBUIRESPONSE._serialized_end=14952
+  _GETGLOBALSFORWEBUIRESPONSE_KEYVALUESENTRY._serialized_start=14695
+  _GETGLOBALSFORWEBUIRESPONSE_KEYVALUESENTRY._serialized_end=14755
+  _GETSTATEUPDATELOGREQUEST._serialized_start=14954
+  _GETSTATEUPDATELOGREQUEST._serialized_end=15032
+  _GETSTATEUPDATELOGRESPONSE._serialized_start=15034
+  _GETSTATEUPDATELOGRESPONSE._serialized_end=15124
+  _GETRESTOREINFOREQUEST._serialized_start=15126
+  _GETRESTOREINFOREQUEST._serialized_end=15208
+  _GETRESTOREINFORESPONSE._serialized_start=15211
+  _GETRESTOREINFORESPONSE._serialized_end=15361
+  _CREATEWORKSPACEREQUEST._serialized_start=15364
+  _CREATEWORKSPACEREQUEST._serialized_end=15529
+  _DELETEWORKSPACEREQUEST._serialized_start=15531
+  _DELETEWORKSPACEREQUEST._serialized_end=15594
+  _INTROSPECTAPIKEYREQUEST._serialized_start=15596
+  _INTROSPECTAPIKEYREQUEST._serialized_end=15646
+  _INTROSPECTAPIKEYRESPONSE._serialized_start=15649
+  _INTROSPECTAPIKEYRESPONSE._serialized_end=15852
+  _CREATEAPIKEYREQUEST._serialized_start=15854
+  _CREATEAPIKEYREQUEST._serialized_end=15954
+  _CREATEAPIKEYRESPONSE._serialized_start=15956
+  _CREATEAPIKEYRESPONSE._serialized_end=16046
+  _DELETEAPIKEYREQUEST._serialized_start=16048
+  _DELETEAPIKEYREQUEST._serialized_end=16119
+  _LISTAPIKEYSREQUEST._serialized_start=16121
+  _LISTAPIKEYSREQUEST._serialized_end=16184
+  _LISTAPIKEYSRESPONSE._serialized_start=16186
+  _LISTAPIKEYSRESPONSE._serialized_end=16267
+  _SERVICEACCOUNT._serialized_start=16270
+  _SERVICEACCOUNT._serialized_end=16557
+  _CREATESERVICEACCOUNTREQUEST._serialized_start=16559
+  _CREATESERVICEACCOUNTREQUEST._serialized_end=16660
+  _CREATESERVICEACCOUNTRESPONSE._serialized_start=16663
+  _CREATESERVICEACCOUNTRESPONSE._serialized_end=16912
+  _GETSERVICEACCOUNTSREQUEST._serialized_start=16914
+  _GETSERVICEACCOUNTSREQUEST._serialized_end=16983
+  _GETSERVICEACCOUNTSRESPONSE._serialized_start=16985
+  _GETSERVICEACCOUNTSRESPONSE._serialized_end=17102
+  _UPDATESERVICEACCOUNTREQUEST._serialized_start=17105
+  _UPDATESERVICEACCOUNTREQUEST._serialized_end=17269
+  _UPDATESERVICEACCOUNTRESPONSE._serialized_start=17272
+  _UPDATESERVICEACCOUNTRESPONSE._serialized_end=17496
+  _DELETESERVICEACCOUNTREQUEST._serialized_start=17498
+  _DELETESERVICEACCOUNTREQUEST._serialized_end=17552
+  _DELETESERVICEACCOUNTRESPONSE._serialized_start=17554
+  _DELETESERVICEACCOUNTRESPONSE._serialized_end=17584
+  _LISTWORKSPACESREQUEST._serialized_start=17586
+  _LISTWORKSPACESREQUEST._serialized_end=17609
+  _LISTWORKSPACESRESPONSE._serialized_start=17611
+  _LISTWORKSPACESRESPONSE._serialized_end=17697
+  _GETWORKSPACEREQUEST._serialized_start=17699
+  _GETWORKSPACEREQUEST._serialized_end=17759
+  _GETWORKSPACERESPONSE._serialized_start=17761
+  _GETWORKSPACERESPONSE._serialized_end=17843
+  _CREATESAVEDFEATUREDATAFRAMEREQUEST._serialized_start=17846
+  _CREATESAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18249
+  _CREATESAVEDFEATUREDATAFRAMERESPONSE._serialized_start=18252
+  _CREATESAVEDFEATUREDATAFRAMERESPONSE._serialized_end=18387
+  _ARCHIVESAVEDFEATUREDATAFRAMEREQUEST._serialized_start=18389
+  _ARCHIVESAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18512
+  _ARCHIVESAVEDFEATUREDATAFRAMERESPONSE._serialized_start=18514
+  _ARCHIVESAVEDFEATUREDATAFRAMERESPONSE._serialized_end=18552
+  _GETSAVEDFEATUREDATAFRAMEREQUEST._serialized_start=18555
+  _GETSAVEDFEATUREDATAFRAMEREQUEST._serialized_end=18786
+  _GETCLUSTERADMININFORESPONSE._serialized_start=18789
+  _GETCLUSTERADMININFORESPONSE._serialized_end=18954
+  _CREATECLUSTERUSERREQUEST._serialized_start=18956
+  _CREATECLUSTERUSERREQUEST._serialized_end=19024
+  _CREATECLUSTERUSERRESPONSE._serialized_start=19026
+  _CREATECLUSTERUSERRESPONSE._serialized_end=19059
+  _DELETECLUSTERUSERREQUEST._serialized_start=19061
+  _DELETECLUSTERUSERREQUEST._serialized_end=19121
+  _DELETECLUSTERUSERRESPONSE._serialized_start=19123
+  _DELETECLUSTERUSERRESPONSE._serialized_end=19156
+  _CLUSTERUSERACTIONREQUEST._serialized_start=19159
+  _CLUSTERUSERACTIONREQUEST._serialized_end=19430
+  _CLUSTERUSERACTIONRESPONSE._serialized_start=19432
+  _CLUSTERUSERACTIONRESPONSE._serialized_end=19465
+  _GETSAVEDFEATUREDATAFRAMERESPONSE._serialized_start=19468
+  _GETSAVEDFEATUREDATAFRAMERESPONSE._serialized_end=19600
+  _GETALLSAVEDFEATUREDATAFRAMESREQUEST._serialized_start=19602
+  _GETALLSAVEDFEATUREDATAFRAMESREQUEST._serialized_end=19669
+  _GETALLSAVEDFEATUREDATAFRAMESRESPONSE._serialized_start=19672
+  _GETALLSAVEDFEATUREDATAFRAMESRESPONSE._serialized_end=19810
+  _INGESTDATAFRAMEREQUEST._serialized_start=19813
+  _INGESTDATAFRAMEREQUEST._serialized_end=19969
+  _INGESTDATAFRAMERESPONSE._serialized_start=19971
+  _INGESTDATAFRAMERESPONSE._serialized_end=19996
+  _GETNEWINGESTDATAFRAMEINFOREQUEST._serialized_start=19998
+  _GETNEWINGESTDATAFRAMEINFOREQUEST._serialized_end=20109
+  _GETNEWINGESTDATAFRAMEINFORESPONSE._serialized_start=20111
+  _GETNEWINGESTDATAFRAMEINFORESPONSE._serialized_end=20227
+  _GETUSERDEPLOYMENTSETTINGSRESPONSE._serialized_start=20230
+  _GETUSERDEPLOYMENTSETTINGSRESPONSE._serialized_end=20366
+  _UPDATEUSERDEPLOYMENTSETTINGSREQUEST._serialized_start=20369
+  _UPDATEUSERDEPLOYMENTSETTINGSREQUEST._serialized_end=20566
+  _UPDATEUSERDEPLOYMENTSETTINGSRESPONSE._serialized_start=20568
+  _UPDATEUSERDEPLOYMENTSETTINGSRESPONSE._serialized_end=20669
+  _GETINTERNALSPARKCLUSTERSTATUSRESPONSE._serialized_start=20671
+  _GETINTERNALSPARKCLUSTERSTATUSRESPONSE._serialized_end=20781
+  _GETDELETEENTITIESINFOREQUEST._serialized_start=20783
+  _GETDELETEENTITIESINFOREQUEST._serialized_end=20890
+  _GETDELETEENTITIESINFORESPONSE._serialized_start=20893
+  _GETDELETEENTITIESINFORESPONSE._serialized_end=21095
+  _DELETEENTITIESREQUEST._serialized_start=21098
+  _DELETEENTITIESREQUEST._serialized_end=21341
+  _DELETEENTITIESRESPONSE._serialized_start=21343
+  _DELETEENTITIESRESPONSE._serialized_end=21367
+  _GETHIVEMETADATAREQUEST._serialized_start=21370
+  _GETHIVEMETADATAREQUEST._serialized_end=21623
+  _GETHIVEMETADATAREQUEST_ACTION._serialized_start=21531
+  _GETHIVEMETADATAREQUEST_ACTION._serialized_end=21623
+  _GETHIVEMETADATARESPONSE._serialized_start=21626
+  _GETHIVEMETADATARESPONSE._serialized_end=21851
+  _VALIDATELOCALFCOREQUEST._serialized_start=21854
+  _VALIDATELOCALFCOREQUEST._serialized_end=22003
+  _VALIDATELOCALFCORESPONSE._serialized_start=22006
+  _VALIDATELOCALFCORESPONSE._serialized_end=22162
+  _GETONBOARDINGSTATUSREQUEST._serialized_start=22164
+  _GETONBOARDINGSTATUSREQUEST._serialized_end=22222
+  _GETONBOARDINGSTATUSRESPONSE._serialized_start=22225
+  _GETONBOARDINGSTATUSRESPONSE._serialized_end=22426
+  _GETDATAPLATFORMSETUPSTATUSRESPONSE._serialized_start=22429
+  _GETDATAPLATFORMSETUPSTATUSRESPONSE._serialized_end=22575
+  _GETOBSERVABILITYCONFIGREQUEST._serialized_start=22577
+  _GETOBSERVABILITYCONFIGREQUEST._serialized_end=22682
+  _GETOBSERVABILITYCONFIGRESPONSE._serialized_start=22685
+  _GETOBSERVABILITYCONFIGRESPONSE._serialized_end=22850
+  _QUERYMETRICREQUEST._serialized_start=22853
+  _QUERYMETRICREQUEST._serialized_end=23156
+  _QUERYMETRICRESPONSE._serialized_start=23159
+  _QUERYMETRICRESPONSE._serialized_end=23660
+  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_start=23663
+  _GETFEATUREVALIDATIONRESULTREQUEST._serialized_end=24175
+  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_start=24178
+  _GETFEATUREVALIDATIONRESULTRESPONSE._serialized_end=24363
+  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_start=24366
+  _GETFEATUREVALIDATIONSUMMARYREQUEST._serialized_end=24588
+  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_start=24591
+  _GETFEATUREVALIDATIONSUMMARYRESPONSE._serialized_end=24905
+  _GETUSERREQUEST._serialized_start=24907
+  _GETUSERREQUEST._serialized_end=24961
+  _GETUSERRESPONSE._serialized_start=24963
+  _GETUSERRESPONSE._serialized_end=25030
+  _GETFEATURESERVERCONFIGREQUEST._serialized_start=25032
+  _GETFEATURESERVERCONFIGREQUEST._serialized_end=25063
+  _GETFEATURESERVERCONFIGRESPONSE._serialized_start=25066
+  _GETFEATURESERVERCONFIGRESPONSE._serialized_end=25210
+  _SETFEATURESERVERCONFIGREQUEST._serialized_start=25212
+  _SETFEATURESERVERCONFIGREQUEST._serialized_end=25265
+  _METADATASERVICE._serialized_start=25333
+  _METADATASERVICE._serialized_end=44086
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.8.0b4/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.8.0b5/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.8.0b5/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.8.0b5/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.8.0b5/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/snowflake/location_pb2.py` & `tecton-0.8.0b5/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/spark_api/error_pb2.py` & `tecton-0.8.0b5/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.8.0b5/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.8.0b5/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.8.0b5/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_proto/validation/validator_pb2.py` & `tecton-0.8.0b5/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/pipeline_helper.py` & `tecton-0.8.0b5/tecton_snowflake/pipeline_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 def pipeline_to_sql_string(
     pipeline: Pipeline,
     data_sources: List[specs.DataSourceSpec],
     transformations: List[specs.TransformationSpec],
     materialization_context: BaseMaterializationContext,
-    mock_sql_inputs: Dict[str, str] = None,
+    mock_sql_inputs: Optional[Dict[str, str]] = None,
     session: "snowflake.snowpark.Session" = None,
 ) -> str:
     return format_sql(
         _PipelineBuilder(
             pipeline=pipeline,
             data_sources=data_sources,
             transformations=transformations,
```

### Comparing `tecton-0.8.0b4/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.8.0b5/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.8.0b5/tecton_snowflake/snowflake_type_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return tecton_types.Int64Type()
     elif snowflake_type.startswith("FLOAT"):
         return tecton_types.Float64Type()
     elif snowflake_type.startswith("BOOLEAN"):
         return tecton_types.BoolType()
     elif snowflake_type.startswith("TIMESTAMP_NTZ"):
         return tecton_types.TimestampType()
-    elif snowflake_type.startswith("TIMESTAMP_TZ") or snowflake_type.startswith("TIMESTAMP_LTZ"):
+    elif snowflake_type.startswith(("TIMESTAMP_TZ", "TIMESTAMP_LTZ")):
         msg = f"Timestamp type {snowflake_type} for column {column_name} is not supported because it contains a timezone.Please use TIMESTAMP_NTZ instead."
         raise errors.TectonValidationError(msg)
     else:
         msg = f"Unsupported Snowflake type {snowflake_type} for column {column_name}."
         raise errors.TectonValidationError(msg)
```

### Comparing `tecton-0.8.0b4/tecton_snowflake/sql_helper.py` & `tecton-0.8.0b5/tecton_snowflake/sql_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     # Get a list of all the join keys in the spine.
     spine_keys = {}
     for item in feature_set_items:
         fd = item.feature_definition
 
         if not fd.is_on_demand:
-            join_keys = {key: value for key, value in item.join_keys}
+            join_keys = dict(item.join_keys)
             spine_keys.update(join_keys)
 
     for item in feature_set_items:
         fd = item.feature_definition
         if fd.is_on_demand and not conf.get_bool("ALPHA_SNOWFLAKE_SNOWPARK_ENABLED"):
             msg = "On-demand features are only supported with Snowpark enabled"
             raise TectonSnowflakeNotImplementedError(msg)
@@ -155,23 +155,25 @@
         is_internal_udf_feature = item.namespace.startswith(UDF_INTERNAL)
         if is_internal_udf_feature:
             name = item.namespace.upper()
         else:
             name = fd.name
 
         if not fd.is_on_demand:
-            join_keys = {key: value for key, value in item.join_keys}
+            join_keys = dict(item.join_keys)
             features = [
                 col_name
                 for col_name in fd.view_schema.column_names()
-                if col_name not in (list(join_keys.keys()) + [fd.timestamp_key])
+                if col_name not in ([*list(join_keys.keys()), fd.timestamp_key])
             ]
             if len(fd.online_serving_index.join_keys) != len(fd.join_keys):
                 msg = "Wildcard is not supported for Snowflake"
                 raise TectonSnowflakeNotImplementedError(msg)
+            if fd.is_incremental_backfill and from_source:
+                raise errors.FV_BFC_SINGLE_FROM_SOURCE
             if start_time is None or (
                 fd.feature_start_timestamp is not None and start_time < fd.feature_start_timestamp
             ):
                 raw_data_start_time = fd.feature_start_timestamp
             else:
                 raw_data_start_time = start_time
 
@@ -475,17 +477,14 @@
 
     if from_source is None:
         from_source = not feature_definition.materialization_enabled or not feature_definition.writes_to_offline_store
 
     if from_source is False:
         if not feature_definition.materialization_enabled or not feature_definition.writes_to_offline_store:
             raise errors.FV_NEEDS_TO_BE_MATERIALIZED(feature_definition.name)
-    else:
-        if feature_definition.is_incremental_backfill:
-            raise errors.FV_BFC_SINGLE_FROM_SOURCE
 
     if from_source:
         pipeline_sql = pipeline_to_sql_string(
             pipeline=feature_definition.pipeline,
             data_sources=feature_definition.data_sources,
             transformations=feature_definition.transformations,
             materialization_context=materialization_context,
@@ -647,23 +646,23 @@
     query = get_materialization_query(
         source=source,
         feature_definition=feature_definition,
         feature_start_time=time_limits.start,
         feature_end_time=time_limits.end,
         offline_materialization=materialize_offline,
     )
-    common_context = dict(
-        source=query,
-        materialize_online=materialize_online,
-        materialize_offline=materialize_offline,
-        destination_stage=destination_stage,
-        materialization_schema=feature_definition.materialization_schema.to_proto(),
-        materialization_id=materialization_id,
-        cast_types=COPY_CASTS,
-    )
+    common_context = {
+        "source": query,
+        "materialize_online": materialize_online,
+        "materialize_offline": materialize_offline,
+        "destination_stage": destination_stage,
+        "materialization_schema": feature_definition.materialization_schema.to_proto(),
+        "materialization_id": materialization_id,
+        "cast_types": COPY_CASTS,
+    }
     if materialize_offline:
         view_name = feature_definition.fv_spec.snowflake_view_name
         database, schema, view = view_name.split(".")
         script_sql = MATERIALIZED_FEATURE_VIEW_TEMPLATE.render(
             destination_table=destination_table,
             workspace=f"{database}.{schema}",
             destination_view=view_name,
@@ -706,23 +705,23 @@
         timestamp_key=data_source.timestamp_field,
         start_time=start_time,
         end_time=end_time,
     )
     return session.sql(sql_str)
 
 
-def _get_feature_view_aggregations(feature_defintion: FeatureDefinition) -> Dict[str, Set[str]]:
+def _get_feature_view_aggregations(feature_definition: FeatureDefinition) -> Dict[str, Set[str]]:
     aggregations = defaultdict(set)
-    is_continuous = feature_defintion.is_continuous
+    is_continuous = feature_definition.is_continuous
     # For continuous features, we only keep one aggregation function for first/last non distinct n for each input feature
     if is_continuous:
         max_first_distinct_n_aggs = defaultdict(int)
         max_last_distinct_n_aggs = defaultdict(int)
 
-    for feature in feature_defintion.fv_spec.aggregate_features:
+    for feature in feature_definition.fv_spec.aggregate_features:
         aggregate_function_lambda = AGGREGATION_PLANS[feature.function]
         if not aggregate_function_lambda:
             msg = f"Unsupported aggregation function {feature.function} in snowflake pipeline"
             raise TectonSnowflakeNotImplementedError(msg)
         if feature.function == afpb.AGGREGATION_FUNCTION_LAST_NON_DISTINCT_N:
             if is_continuous:
                 max_last_distinct_n_aggs[feature.input_feature_name] = max(
```

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/historical_features.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates/time_limit.sql` & `tecton-0.8.0b5/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_snowflake/templates_utils.py` & `tecton-0.8.0b5/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/aggregation_plans.py` & `tecton-0.8.0b5/tecton_spark/aggregation_plans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable
 from typing import List
 from typing import Optional
+from typing import Union
 
 import attr
 import pyspark.sql.functions as F
 from pyspark import SparkContext
 from pyspark.sql import Column
 from pyspark.sql import WindowSpec
 from pyspark.sql import functions
@@ -91,15 +92,17 @@
     return lambda cols: [F.col(cols[0])]
 
 
 def _simple_full_aggregation_transform(spark_transform):
     return lambda cols, window: spark_transform(cols[0]).over(window)
 
 
-def _simple_aggregation_plan(aggregation_function: afpb.AggregationFunction, spark_transform):
+def _simple_aggregation_plan(
+    aggregation_function: afpb.AggregationFunction, spark_transform: Callable[[Union[Column, str]], Column]
+) -> AggregationPlan:
     return AggregationPlan(
         partial_aggregation_transform=_simple_partial_aggregation_transform(spark_transform),
         continuous_partial_aggregation_transform=_simple_continuous_partial_aggregation_transform(),
         full_aggregation_transform=_simple_full_aggregation_transform(spark_transform),
         materialized_column_prefixes=get_materialization_aggregation_column_prefixes(aggregation_function),
     )
 
@@ -108,15 +111,15 @@
     sc = SparkContext._active_spark_context
     udf_name = f"tecton_approx_percentile_partial_{precision}"
     sc._jvm.com.tecton.udfs.spark3.ApproxPercentilePartialRegister().register(udf_name, precision)
     columns = expr(f"{udf_name}({col})")
     return [columns.processedMeans, columns.processedWeights]
 
 
-def _make_approx_percentile_partial_aggregation(precision: int) -> Callable:
+def _make_approx_percentile_partial_aggregation(precision: int) -> Callable[[List[str]], List[Column]]:
     def _approx_percentile_partial_aggregation(cols: List[str]) -> List[Column]:
         return ApproxPercentilePartialAgg(cols[0], precision)
 
     return _approx_percentile_partial_aggregation
 
 
 def ApproxPercentileFullAgg(
@@ -128,15 +131,15 @@
     sc = SparkContext._active_spark_context
     percentile_str = str(percentile).replace(".", "_")
     udf_name = f"tecton_approx_percentile_full_{percentile_str}"
     sc._jvm.com.tecton.udfs.spark3.ApproxPercentileFullRegister().register(udf_name, precision, percentile)
     return expr(f"{udf_name}({processed_means}, {processed_weights})")
 
 
-def _make_approx_percentile_full_aggregation(percentile: float, precision: int) -> Callable:
+def _make_approx_percentile_full_aggregation(percentile: float, precision: int) -> Callable[[List[str]], WindowSpec]:
     def _approx_percentile_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
         processed_means, processed_weights = cols
         return (
             ApproxPercentileFullAgg(processed_means, processed_weights, percentile, precision).over(window).percentile
         )
 
     return _approx_percentile_full_aggregation
@@ -172,23 +175,23 @@
     sc = SparkContext._active_spark_context
     udf_name = "tecton_approx_count_distinct_partial"
     sc._jvm.com.tecton.udfs.spark3.ApproxCountDistinctPartialRegister().register(udf_name)
     columns = expr(f"{udf_name}({index}, {register})")
     return [columns.indices, columns.registers]
 
 
-def _make_approx_count_distinct_partial_aggregation() -> Callable:
+def _make_approx_count_distinct_partial_aggregation() -> Callable[[List[str]], Column]:
     def _approx_count_distinct_partial_aggregation(cols: List[str]) -> List[Column]:
         index, register = cols[0], cols[1]
         return ApproxCountDistinctPartialAgg(index, register)
 
     return _approx_count_distinct_partial_aggregation
 
 
-def _make_approx_count_distinct_partial_aggregation_helper(precision: int) -> Callable:
+def _make_approx_count_distinct_partial_aggregation_helper(precision: int) -> Callable[[str], List[Column]]:
     def _add_index_and_register_column(input_column: str) -> List[Column]:
         """Computes the index and register values and returns them as bigint columns.
 
         The input column is first hashed with the SHA256 hash function and truncated to 64 bits. Then:
         * The index is the first 'precision' bits of the hash.
         * The register value is 1 + (number of leading zeros in the final 64 - 'precision' bits of the hash).
 
@@ -225,15 +228,15 @@
 
     def _approx_count_distinct_partial_aggregation_helper(col: str) -> List[Column]:
         return _add_index_and_register_column(col)
 
     return _approx_count_distinct_partial_aggregation_helper
 
 
-def _mean_full_aggregation(cols: List[str], window: WindowSpec):
+def _mean_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
     # Window aggregation doesn't work with more than one built-in function like this
     #   sum(mean_clicked * count_clicked) / sum(count_clicked)
     # And it does not support UDFs on bounded windows (the kind we use)
     #   https://issues.apache.org/jira/browse/SPARK-22239
     # We work around this limitations by calculating ratio over two window aggregations
     mean_col, count_col = cols
     return functions.sum(functions.col(mean_col) * functions.col(count_col)).over(window) / functions.sum(
@@ -260,15 +263,15 @@
 def LastDistinctNAgg(col1: str, col2: str, n: int) -> Column:
     sc = SparkContext._active_spark_context
     udf_name = f"tecton_last_distinct_{n}_partial_aggregation"
     sc._jvm.com.tecton.udfs.spark3.LastNRegister().register(n, udf_name, True)
     return expr(f"{udf_name}({col1}, {col2}).values")
 
 
-def _make_last_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable:
+def _make_last_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable[[List[str]], List[Column]]:
     def _last_distinct_n_partial_aggregation(cols: List[str]) -> List[Column]:
         return [LastDistinctNAgg(time_key, cols[0], n)]
 
     return _last_distinct_n_partial_aggregation
 
 
 def _make_first_and_last_n_continuous_partial() -> Callable[[List[str]], List[Column]]:
@@ -286,42 +289,42 @@
         if keep_last_items
         else f"tecton_first_distinct_{n}_full_aggregation"
     )
     sc._jvm.com.tecton.udfs.spark3.LimitedListConcatRegister().register(n, udf_name, keep_last_items)
     return expr(f"{udf_name}({col1})")
 
 
-def _make_fixed_size_n_full_aggregation(n: int, keep_last_items: bool):
+def _make_fixed_size_n_full_aggregation(n: int, keep_last_items: bool) -> Callable[[List[str], WindowSpec], Column]:
     def _fixed_size_n_full_aggregation(column_name: List[str], window: WindowSpec) -> Column:
         col = (LimitedListConcatAgg(column_name[0], n, keep_last_items).over(window)).values
         return col
 
     return _fixed_size_n_full_aggregation
 
 
 # Full aggregator used by last non-distinct N.
-def _make_last_non_distinct_n_full_aggregation(n: int) -> Callable:
+def _make_last_non_distinct_n_full_aggregation(n: int) -> Callable[[List[str], WindowSpec], Column]:
     def _last_non_distinct_n_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
         return functions.reverse(
             functions.slice(functions.reverse(functions.flatten(functions.collect_list(cols[0]).over(window))), 1, n)
         )
 
     return _last_non_distinct_n_full_aggregation
 
 
 # Full aggregator used by first non-distinct N.
-def _make_first_non_distinct_n_full_aggregation(n: int) -> Callable:
+def _make_first_non_distinct_n_full_aggregation(n: int) -> Callable[[List[str], WindowSpec], Column]:
     def _first_non_distinct_n_full_aggregation(cols: List[Column], window: WindowSpec) -> Column:
         return functions.slice(functions.flatten(functions.collect_list(cols[0]).over(window)), 1, n)
 
     return _first_non_distinct_n_full_aggregation
 
 
 # Partial aggregator used by last non-distinct N.
-def _make_last_non_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable:
+def _make_last_non_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable[[List[str]], List[Column]]:
     def last_non_distinct_n_partial_aggregation(cols: List[str]) -> List[Column]:
         # Sort items in descending order based on timestamp.
         col = cols[0]
         sort_function = f"(left, right) -> case when left.{time_key} < right.{time_key} then 1 when left.{time_key} > right.{time_key} then -1 else 0 end)"
         return [
             functions.reverse(
                 functions.slice(
@@ -332,15 +335,15 @@
             )
         ]
 
     return last_non_distinct_n_partial_aggregation
 
 
 # Partial aggregator used by first non-distinct N.
-def _make_first_non_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable:
+def _make_first_non_distinct_n_partial_aggregation(time_key: str, n: int) -> Callable[[List[str]], List[Column]]:
     def first_non_distinct_n_partial_aggregation(cols: List[str]) -> List[Column]:
         # Sort items in ascending order based on timestamp.
         col = cols[0]
         sort_function = f"(left,right) -> case when left.{time_key} < right.{time_key} then -1 when left.{time_key} > right.{time_key} then 1 else 0 end)"
         return [
             functions.slice(
                 functions.expr(f"array_sort(collect_list(struct({col}, {time_key})), {sort_function}"),
@@ -348,54 +351,54 @@
                 n,
             ).getItem(col)
         ]
 
     return first_non_distinct_n_partial_aggregation
 
 
-def _sum_with_default(columns: List[str], window: WindowSpec):
+def _sum_with_default(columns: List[str], window: WindowSpec) -> Column:
     col = functions.sum(columns[0]).over(window)
     # Fill null
     col = functions.when(col.isNull(), functions.lit(0)).otherwise(col)
     return col
 
 
 # population variation equation: Σ(x^2)/n - μ^2
-def _var_pop_full_aggregation(cols: List[str], window: WindowSpec):
+def _var_pop_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
     sum_of_squares_col, count_col, sum_col = cols
     return functions.sum(sum_of_squares_col).over(window) / functions.sum(count_col).over(window) - functions.pow(
         functions.sum(sum_col).over(window) / functions.sum(count_col).over(window), 2
     )
 
 
-def _stddev_pop_full_aggregation(cols: List[str], window: WindowSpec):
+def _stddev_pop_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
     return functions.sqrt(_var_pop_full_aggregation(cols, window))
 
 
 # sample variation equation: (Σ(x^2) - (Σ(x)^2)/N)/N-1
-def _var_samp_full_aggregation(cols: List[str], window: WindowSpec):
+def _var_samp_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
     sum_of_squares_col, count_col, sum_col = cols
     total_count_col = functions.sum(count_col).over(window)
     # check if count is equal to 0 for divide by 0 errors
     var_samp_col = functions.when(
         total_count_col != 1,
         (
             functions.sum(sum_of_squares_col).over(window)
             - functions.pow(functions.sum(sum_col).over(window), 2) / total_count_col
         )
         / (total_count_col - functions.lit(1)),
     )
     return var_samp_col
 
 
-def _stddev_samp_full_aggregation(cols: List[str], window: WindowSpec):
+def _stddev_samp_full_aggregation(cols: List[str], window: WindowSpec) -> Column:
     return functions.sqrt(_var_samp_full_aggregation(cols, window))
 
 
-def _stddev_var_partial(col: List[str]):
+def _stddev_var_partial(col: List[str]) -> List[Column]:
     return [
         functions.sum(functions.pow(col, 2)),
         functions.count(col),
         functions.sum(functions.col(col)),
     ]
```

### Comparing `tecton-0.8.0b4/tecton_spark/data_observability.py` & `tecton-0.8.0b5/tecton_spark/data_observability.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 from typing import TYPE_CHECKING
+from typing import Optional
 
 from pyspark.sql import DataFrame
 from pyspark.sql import SparkSession
 
 
 if TYPE_CHECKING:
     from tecton_proto.materialization.params_pb2 import MaterializationTaskParams
@@ -46,16 +47,16 @@
     def publish(self):
         self._jvm_collector.publish()
 
 
 def create_feature_metrics_collector(
     spark: SparkSession,
     params: "MaterializationTaskParams",
-    feature_start_time: datetime = None,
-    feature_end_time: datetime = None,
+    feature_start_time: Optional[datetime] = None,
+    feature_end_time: Optional[datetime] = None,
 ) -> MetricsCollector:
     global _active_metrics_collector
 
     if not params.HasField("data_observability_config"):
         return NoopMetricsCollector()
 
     config = params.data_observability_config
```

### Comparing `tecton-0.8.0b4/tecton_spark/data_source_credentials.py` & `tecton-0.8.0b5/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/data_source_helper.py` & `tecton-0.8.0b5/tecton_spark/data_source_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from datetime import datetime
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Union
 
 import pendulum
+from pyspark.sql import Column
 from pyspark.sql import DataFrame
 from pyspark.sql import SparkSession
 from pyspark.sql import functions
 from pyspark.sql.functions import coalesce
 from pyspark.sql.functions import to_timestamp
 from pyspark.sql.types import ArrayType
+from pyspark.sql.types import DataType
 from pyspark.sql.types import DateType
 from pyspark.sql.types import MapType
 from pyspark.sql.types import StringType
 from pyspark.sql.types import StructField
 from pyspark.sql.types import StructType
 from typeguard import typechecked
 
@@ -90,15 +92,15 @@
         spark.sql(f"USE CATALOG {catalog}")
     spark.sql(f"USE {schema}")
     return spark.table(table)
 
 
 @typechecked
 def get_non_dsf_raw_dataframe(
-    spark: SparkSession, data_source: specs.BatchSourceSpec, called_for_schema_computation=False
+    spark: SparkSession, data_source: specs.BatchSourceSpec, called_for_schema_computation: bool = False
 ) -> DataFrame:
     """Returns a DataFrame of the raw, untranslated data defined by the given BatchDataSource proto.
 
     :param spark: Spark session.
     :param data_source: BatchDataSource proto. BatchDataSource must not be a data source function (spark_batch_config).
     :param called_for_schema_computation: If set, optimizations are applied for faster schema computations.
                                           i.e. FileDSConfig.schema_uri is used to avoid expensive partition discovery.
@@ -174,15 +176,15 @@
         raise ValueError(msg)
 
     return df
 
 
 @typechecked
 def get_table_dataframe(
-    spark: SparkSession, data_source: specs.BatchSourceSpec, called_for_schema_computation=False
+    spark: SparkSession, data_source: specs.BatchSourceSpec, called_for_schema_computation: bool = False
 ) -> DataFrame:
     """Returns a DataFrame for a table defined by given BatchDataSource proto.
 
     :param spark: Spark session.
     :param data_source: BatchDataSource proto. BatchDataSource must not be a data source function (spark_batch_config).
     :param called_for_schema_computation: If set, optimizations are applied for faster schema computations.
                                           i.e. FileDSConfig.schema_uri is used to avoid expensive partition discovery.
@@ -368,15 +370,15 @@
 #  --> (y = start.year & m = start.month & d >= start.day & d <= end.day)
 # (B)Time range: 2019 Dec 21 10:00:00 AM - 2020 Jan 10 5:00:00 AM
 #  --> ((y = start.year & m = start.month & d >= start.day) | (y = end.year & m = end.month & d <= end.day))
 def _build_partition_filter(
     datetime_partition_columns: specs.DatetimePartitionColumnSpec,
     start_time: Optional[Union[pendulum.DateTime, datetime]] = None,
     end_time: Optional[Union[pendulum.DateTime, datetime]] = None,
-):
+) -> Column:
     if not start_time and not end_time:
         return None
 
     range_duration = end_time - start_time if start_time and end_time else None
 
     # Filters relating to start_time and end_time
     start_filters = []
@@ -661,15 +663,15 @@
     """
     assert not isinstance(
         stream_data_source, specs.SparkStreamSourceSpec
     ), "get_stream_dataframe_with_options can not be used with data source function (spark_stream_config)."
 
     df = get_stream_dataframe(spark, stream_data_source, option_overrides)
 
-    dedup_columns = [column for column in stream_data_source.deduplication_column_names]
+    dedup_columns = list(stream_data_source.deduplication_column_names)
     if dedup_columns:
         df = df.dropDuplicates(dedup_columns)
 
     return df
 
 
 def _get_initial_stream_position(stream_data_source: specs.StreamSourceSpec) -> Optional[str]:
@@ -688,17 +690,17 @@
 @typechecked
 def get_ds_dataframe(
     spark: SparkSession,
     data_source: specs.DataSourceSpec,
     consume_streaming_data_source: bool,
     start_time: Optional[Union[pendulum.DateTime, datetime]] = None,
     end_time: Optional[Union[pendulum.DateTime, datetime]] = None,
-    called_for_schema_computation=False,
+    called_for_schema_computation: bool = False,
     stream_option_overrides: Optional[Dict[str, str]] = None,
-):
+) -> DataFrame:
     if consume_streaming_data_source and (start_time or end_time):
         msg = "Can't specify start or end time when consuming streaming data source"
         raise AssertionError(msg)
 
     if consume_streaming_data_source:
         assert (
             data_source.stream_source
@@ -738,33 +740,33 @@
     MapTypes or Arrays of non-StructTypes are not allowed.
 
     :param spark: Spark session.
     :param df: DataFrame input.
     :return: DataFrame with lowercase schema.
     """
 
-    def _get_lowercase_schema(datatype):
+    def _get_lowercase_schema(datatype: DataType) -> DataType:
         if type(datatype) == ArrayType:
             return _get_lowercase_array_schema(datatype)
         elif type(datatype) == StructType:
             return _get_lowercase_structtype_schema(datatype)
         elif type(col.dataType) == MapType:
             msg = "MapType not supported in JSON schema"
             raise TypeError(msg)
         return datatype
 
-    def _get_lowercase_structtype_schema(s) -> StructType:
+    def _get_lowercase_structtype_schema(s: StructType) -> StructType:
         assert type(s) == StructType, f"Invalid argument type {type(s)}, expected StructType"
         struct_fields = []
         for col in s:
             datatype = _get_lowercase_schema(col.dataType)
             struct_fields.append(StructField(col.name.lower(), datatype))
         return StructType(struct_fields)
 
-    def _get_lowercase_array_schema(c) -> ArrayType:
+    def _get_lowercase_array_schema(c: ArrayType) -> ArrayType:
         assert (
             type(c.elementType) == StructType
         ), f"Invalid ArrayType element type {type(c)}, expected StructType for valid JSON arrays."
         datatype = c.elementType
         struct_schema = _get_lowercase_structtype_schema(datatype)
         return ArrayType(struct_schema)
 
@@ -781,15 +783,15 @@
         elif type(col.dataType) is DateType:
             new_fields.append(functions.col(col.name).cast(StringType()).alias(col.name.lower()))
         else:
             new_fields.append(functions.col(col.name).alias(col.name.lower()))
     return df.select(new_fields)
 
 
-def validate_data_source_supports_time_filtering(data_source: specs.DataSourceSpec):
+def validate_data_source_supports_time_filtering(data_source: specs.DataSourceSpec) -> None:
     """
     Verifies the batch data_source has the timestamp_column_properties field or supports_time_filtering is True if it is a Data Source Function.
 
     :param data_source: a specs.DataSourceSpec containing a batch source.
     """
     batch_source = data_source.batch_source
     assert batch_source is not None
@@ -805,12 +807,12 @@
 
 
 def get_data_source_function_batch_dataframe(
     spark: SparkSession,
     data_source: specs.SparkBatchSourceSpec,
     start_time: Optional[datetime],
     end_time: Optional[datetime],
-):
+) -> DataFrame:
     if data_source.supports_time_filtering:
         filter_context = FilterContext(start_time, end_time)
         return data_source.function(spark, filter_context)
     return data_source.function(spark)
```

### Comparing `tecton-0.8.0b4/tecton_spark/feature_view_spark_utils.py` & `tecton-0.8.0b5/tecton_spark/feature_view_spark_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyspark.sql import DataFrame
 
 from tecton_core import errors
 from tecton_core.schema import Schema
 from tecton_spark.schema_spark_utils import schema_from_spark
 
 
-def validate_df_columns_and_feature_types(df: DataFrame, view_schema: Schema):
+def validate_df_columns_and_feature_types(df: DataFrame, view_schema: Schema) -> None:
     df_columns = schema_from_spark(df.schema).column_name_and_data_types()
     df_column_names = frozenset([x[0] for x in df_columns])
     fv_columns = view_schema.column_name_and_data_types()
     fv_column_names = frozenset([x[0] for x in fv_columns])
 
     if fv_column_names.difference(df_column_names):
         raise errors.INGEST_DF_MISSING_COLUMNS(list(fv_column_names.difference(df_column_names)))
```

### Comparing `tecton-0.8.0b4/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.8.0b5/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/materialization_plan.py` & `tecton-0.8.0b5/tecton_spark/materialization_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def from_querytree(cls, fd: FeatureDefinition, query_tree: NodeRef, spark: SparkSession) -> "MaterializationPlan":
         logger.info("Query Plan:")
         logger.info(query_tree.pretty_str())
         spark_df = translate.spark_convert(query_tree).to_dataframe(spark)
         return cls(fd=fd, base_data_frame=spark_df)
 
     @classmethod
-    def from_parquet(cls, fd: FeatureDefinition, path: str, spark: SparkSession):
+    def from_parquet(cls, fd: FeatureDefinition, path: str, spark: SparkSession) -> "MaterializationPlan":
         return cls(fd=fd, base_data_frame=spark.read.parquet(path))
 
     @property
     def offline_store_data_frame(self) -> DataFrame:
         return self.base_data_frame
 
     @property
```

### Comparing `tecton-0.8.0b4/tecton_spark/partial_aggregations.py` & `tecton-0.8.0b5/tecton_spark/partial_aggregations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from datetime import datetime
 from typing import Dict
+from typing import Iterator
 from typing import List
 from typing import Optional
+from typing import Tuple
 
 import pyspark
 import pyspark.sql.functions as F
+from pyspark.sql import Column
 
 from tecton_core.aggregation_utils import get_materialization_aggregation_column_prefixes
 from tecton_core.aggregation_utils import get_pretty_column_prefix
 from tecton_core.query_consts import ANCHOR_TIME
 from tecton_proto.data.feature_view_pb2 import TrailingTimeWindowAggregation
 from tecton_spark.aggregation_plans import AggregationPlan
 from tecton_spark.aggregation_plans import get_aggregation_plan
 from tecton_spark.time_utils import convert_timestamp_to_epoch
 from tecton_spark.time_utils import get_timestamp_in_seconds
 
 
 WINDOW_COLUMN_NAME = "window"
 
 
-def _get_feature_partial_aggregations(aggregation_plan: AggregationPlan, feature_name: str):
+def _get_feature_partial_aggregations(
+    aggregation_plan: AggregationPlan, feature_name: str
+) -> Iterator[Tuple[str, Column]]:
     column_names = set()
     input_columns = (
         aggregation_plan.intermediate_column_names(feature_name)
         if aggregation_plan.intermediate_column_prefixes is not None
         else [feature_name]
     )
 
@@ -75,15 +80,15 @@
     group_by_columns: List[str],
     time_aggregation: TrailingTimeWindowAggregation,
     version: int,
     window_start_column_name: Optional[str] = None,
     window_end_column_name: Optional[str] = None,
     convert_to_epoch: bool = True,
     aggregation_anchor_time: Optional[datetime] = None,
-):
+) -> pyspark.sql.DataFrame:
     """Constructs a dataframe that performs partial aggregations on the input dataframe.
 
     Also removes the default window column that is generated, and replaces it with a start time column, and optionally
     an end time column.
 
     If the time aggregation is continuous, no aggregations will be performed. Instead, a start time column will be added
     but will simply be the same as the timestamp column in the input dataframe.
@@ -123,17 +128,17 @@
             # an integer.
             anchor_time_epoch = get_timestamp_in_seconds(aggregation_anchor_time)
             slide_period_seconds = time_aggregation.aggregation_slide_period.seconds
             anchor_time_offset_seconds = anchor_time_epoch % slide_period_seconds
             anchor_time_offset_string = f"{anchor_time_offset_seconds} seconds"
 
         window_spec = F.window(time_aggregation.time_key, slide_str, slide_str, anchor_time_offset_string)
-        group_by_cols = [window_spec] + group_by_cols
+        group_by_cols = [window_spec, *group_by_cols]
         aggregations = []
-        intermediate_columns_added = set([])
+        intermediate_columns_added = set()
         for feature in time_aggregation.features:
             aggregation_plan = get_aggregation_plan(
                 feature.function, feature.function_params, time_aggregation.is_continuous, time_aggregation.time_key
             )
 
             if aggregation_plan.partial_aggregation_preprocessor is not None:
                 intermediate_columns = aggregation_plan.partial_aggregation_preprocessor(feature.input_feature_name)
@@ -147,15 +152,15 @@
                 if name in output_columns:
                     continue
                 output_columns.add(name)
                 aggregations.append(aggregation)
         output_df = df.groupBy(*group_by_cols).agg(*aggregations)
     else:
         columns_to_drop = set()
-        intermediate_columns_added = set([])
+        intermediate_columns_added = set()
         for feature in time_aggregation.features:
             aggregation_plan = get_aggregation_plan(
                 feature.function, feature.function_params, time_aggregation.is_continuous, time_aggregation.time_key
             )
 
             if aggregation_plan.partial_aggregation_preprocessor is not None:
                 intermediate_columns = aggregation_plan.partial_aggregation_preprocessor(feature.input_feature_name)
@@ -205,15 +210,15 @@
 
 
 def partial_aggregate_column_renames(
     slide_interval_string: str, trailing_time_window_aggregation: TrailingTimeWindowAggregation
 ) -> Dict[str, str]:
     """Rename partial aggregate columns to human readable format."""
     # Create a map from intermediate rollup column name to preferred column names.
-    renaming_map = dict()
+    renaming_map = {}
     for feature in trailing_time_window_aggregation.features:
         aggregation_plan = get_aggregation_plan(
             feature.function,
             feature.function_params,
             trailing_time_window_aggregation.is_continuous,
             trailing_time_window_aggregation.time_key,
         )
```

### Comparing `tecton-0.8.0b4/tecton_spark/pipeline_helper.py` & `tecton-0.8.0b5/tecton_spark/pipeline_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 MAX_INT64 = (2**63) - 1
 
 
 # TODO(TEC-8978): remove \. from namespace regex when FWv3 FVs are no longer supported.
 _NAMESPACE_SEPARATOR_REGEX = re.compile(r"__|\.")
 
 
-def feature_name(namespaced_feature_name: str):
+def feature_name(namespaced_feature_name: str) -> str:
     """Gets the base feature name from a namespaced_feature_name (e.g. feature_view__feature)
 
     Supports both `__` (fwv5) and `.` (fwv3) separators. Does two attempts at
     getting the feature name since `__` was allowed in feature view names in
     fwv3.
     """
 
@@ -69,15 +69,15 @@
     if len(spl) == 2:
         return spl[1]
 
     return namespaced_feature_name.split(".")[1]
 
 
 def build_odfv_udf_col(
-    input_df: DataFrame, fdw: FeatureDefinitionWrapper, namespace: str
+    input_df: DataFrame, fdw: FeatureDefinitionWrapper, namespace: str, use_namespace_feature_prefix: bool = True
 ) -> Tuple[Column, List[Column]]:
     """
     Builds a Spark udf for executing a specific ODFV. This runs an ODFV,
     which outputs a single temporary object (dict/map for python mode, json for
     pandas mode). We then deserialize this to get the feature columns.
 
     We use this function in two phases in parallel across multiple ODFVs:
@@ -119,18 +119,19 @@
         transformations=transformations,
         udf_arg_idx_map=udf_arg_idx_map,
         output_schema=output_schema,
     )
 
     from pyspark.sql.functions import col
 
-    output_columns = [
-        col(f"{odfv_tmp_output_name}.{c.name}").alias(f"{namespace}{namespace_separator}{c.name}")
-        for c in output_schema
-    ]
+    output_columns = []
+    for c in output_schema:
+        output_column_name = f"{namespace}{namespace_separator}{c.name}" if use_namespace_feature_prefix else c.name
+        output_columns.append(col(f"{odfv_tmp_output_name}.{c.name}").alias(output_column_name))
+
     from pyspark.sql.functions import from_json
     from pyspark.sql.functions import pandas_udf
     from pyspark.sql.functions import udf
 
     if builder.mode == "python":
         # Python features are output as a single dict / map column, so we
         # map that into individual columns
@@ -191,15 +192,15 @@
 
 def get_all_input_keys(node: PipelineNode) -> Set[str]:
     names_set = set()
     _get_all_input_keys_helper(node, names_set)
     return names_set
 
 
-def _get_all_input_keys_helper(node: PipelineNode, names_set: Set[str]):
+def _get_all_input_keys_helper(node: PipelineNode, names_set: Set[str]) -> Set[str]:
     if node.HasField("request_data_source_node"):
         names_set.add(node.request_data_source_node.input_name)
     elif node.HasField("data_source_node"):
         names_set.add(node.data_source_node.input_name)
     elif node.HasField("feature_view_node"):
         names_set.add(node.feature_view_node.input_name)
     elif node.HasField("transformation_node"):
@@ -210,15 +211,15 @@
 
 def get_fco_ids_to_input_keys(node: PipelineNode) -> Dict[str, str]:
     names_dict = {}
     _get_fco_ids_to_input_keys_helper(node, names_dict)
     return names_dict
 
 
-def _get_fco_ids_to_input_keys_helper(node: PipelineNode, names_dict: Dict[str, str]):
+def _get_fco_ids_to_input_keys_helper(node: PipelineNode, names_dict: Dict[str, str]) -> Dict[str, str]:
     if node.HasField("request_data_source_node"):
         # request data sources don't have fco ids
         pass
     elif node.HasField("data_source_node"):
         ds_node = node.data_source_node
         names_dict[IdHelper.to_string(ds_node.virtual_data_source_id)] = ds_node.input_name
     elif node.HasField("feature_view_node"):
@@ -232,26 +233,26 @@
 
 # Constructs empty data frames matching schema of DS inputs for the purpose of
 # schema-validating the transformation pipeline.
 def populate_empty_passed_in_inputs(
     node: PipelineNode,
     ds_map: Dict[str, specs.DataSourceSpec],
     spark: SparkSession,
-):
+) -> Dict[str, DataFrame]:
     empty_passed_in_inputs = {}
     _populate_empty_passed_in_inputs_helper(node, empty_passed_in_inputs, ds_map, spark)
     return empty_passed_in_inputs
 
 
 def _populate_empty_passed_in_inputs_helper(
     node: PipelineNode,
     empty_passed_in_inputs: Dict[str, DataFrame],
     ds_map: Dict[str, specs.DataSourceSpec],
     spark: SparkSession,
-):
+) -> None:
     if node.HasField("data_source_node"):
         ds_id = IdHelper.to_string(node.data_source_node.virtual_data_source_id)
         ds_spec = ds_map[ds_id]
         assert (
             ds_spec.type != DataSourceType.PUSH_NO_BATCH
         ), "This utility does not support FeatureView with PushSources that do not have a batch_config"
         ds_schema = ds_spec.batch_source.spark_schema
@@ -281,15 +282,15 @@
         # If None, we will compute inputs from raw data sources and apply time filtering.
         # Otherwise we will prefer these inputs instead
         passed_in_inputs: Optional[Dict[str, DataFrame]] = None,
         # output_schema is only used by python/pandas transformations during backfills.
         # Specifically, it applies for Stream feature views with push sources and batch config, during
         # the batch materialization jobs.
         output_schema: Optional[StructType] = None,
-    ):
+    ) -> None:
         self._spark = spark
         self._pipeline = pipeline
         self._output_schema = output_schema
         self._consume_streaming_data_sources = consume_streaming_data_sources
         self._feature_time_limits = feature_time_limits
         self._id_to_ds = {ds.id: ds for ds in data_sources}
         self._id_to_transformation = {t.id: t for t in transformations}
@@ -368,15 +369,15 @@
             else:
                 msg = f"Unknown argument type for Input node: {transformation_input}"
                 raise KeyError(msg)
 
         return self._apply_transformation_function(transformation_node, args, kwargs)
 
     def _apply_transformation_function(
-        self, transformation_node, args, kwargs
+        self, transformation_node: TransformationNode, args: List[Any], kwargs: Dict[str, Any]
     ) -> Union[Dict[str, Any], pd.DataFrame, DataFrame]:
         """For the given transformation node, returns the corresponding DataFrame transformation.
 
         If needed, resulted function is wrapped with a function that translates mode-specific input/output types to DataFrames.
         """
         transformation = self._id_to_transformation[IdHelper.to_string(transformation_node.transformation_id)]
         user_function = transformation.user_function
@@ -469,27 +470,27 @@
             ].name
             transformation_type_checker(transformation_name, sql_string, "spark_sql", self._possible_modes())
             return self._spark.sql(sql_string)
 
         return wrapped
 
     def _wrap_node_inputvalue(
-        self, node_input, value: _VALUE_TYPE
+        self, node_input: InputProto, value: _VALUE_TYPE
     ) -> Optional[Union[InputProto, str, int, float, bool]]:
         if node_input.node.HasField("constant_node"):
             assert value is None or isinstance(value, CONSTANT_TYPE_OBJECTS)
             return value
         elif node_input.node.HasField("materialization_context_node"):
             assert isinstance(value, BoundMaterializationContext)
             return value
         else:
             assert isinstance(value, DataFrame)
             return self._register_temp_table(self._node_name(node_input.node), value)
 
-    def _node_name(self, node) -> str:
+    def _node_name(self, node: PipelineNode) -> str:
         """Returns a human-readable name for the node."""
         if node.HasField("transformation_node"):
             name = self._id_to_transformation[IdHelper.to_string(node.transformation_node.transformation_id)].name
             return f"transformation_{name}_output"
         elif node.HasField("data_source_node"):
             if node.data_source_node.HasField("input_name"):
                 return node.data_source_node.input_name
@@ -552,15 +553,15 @@
         # maps input + feature name to arg index that udf function wrapper will be called with.
         # this is needed because we need to know which pd.Series that are inputs to this function correspond to the desired request context fields or dependent fv features that the customer-defined udf uses.
         udf_arg_idx_map: Dict[str, int],
         output_schema: StructType,
         # the id of this OnDemandFeatureView; only required to be set when reading from source data
         fv_id: Optional[str] = None,
         passed_in_inputs: Optional[Dict[str, Union[Dict[str, Any], pandas.DataFrame]]] = None,
-    ):
+    ) -> None:
         self._pipeline = pipeline
         self._name = name
         self._fv_id = fv_id
         self.udf_arg_idx_map = udf_arg_idx_map
         self._id_to_transformation = {t.id: t for t in transformations}
         self._output_schema = output_schema
         self._passed_in_inputs = passed_in_inputs
```

### Comparing `tecton-0.8.0b4/tecton_spark/query/data_source.py` & `tecton-0.8.0b5/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/query/filter.py` & `tecton-0.8.0b5/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/query/join.py` & `tecton-0.8.0b5/tecton_spark/query/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         cls,
         left_df: pyspark.sql.DataFrame,
         right_df: pyspark.sql.DataFrame,
         left_ts_cols: Sequence[str],
         right_ts_cols: Sequence[str],
         partition_cols: Sequence[str],
         use_window_range_between_value: bool,
-    ):
+    ) -> "_AsofJoinerAndWindowAggregator":
         if len(left_ts_cols) != len(right_ts_cols):
             msg = f"Timestamp columns are not equal length: left({left_ts_cols}), right({right_ts_cols})"
             raise RuntimeError(msg)
 
         timestamp_cols = [f"{cls._timestamp_prefix}_{i}" for i in range(len(left_ts_cols))]
 
         for new_col, old_col in zip(timestamp_cols, left_ts_cols):
@@ -183,15 +183,15 @@
             + [self._is_left_column_name]
         )
         selected = union.select(output_columns)
         return selected.filter(self._is_left_column_name).drop(self._is_left_column_name, *self.timestamp_cols)
 
     def get_range_between_window_spec(self, range_between_start, range_between_end):
         if range_between_start == spark_window.Window.unboundedPreceding:
-            order_by_cols = list(self.timestamp_cols) + [self._is_left_column_name]
+            order_by_cols = [*list(self.timestamp_cols), self._is_left_column_name]
         else:
             order_by_cols = [self._tecton_window_range_between_order_col]
 
         window_spec = (
             spark_window.Window.partitionBy(list(self.partition_cols))
             .orderBy([F.col(c).asc() for c in order_by_cols])
             .rangeBetween(range_between_start, range_between_end)
@@ -211,15 +211,15 @@
 
     left_container: AsofJoinInputSparkContainer
     right_container: AsofJoinInputSparkContainer
     join_cols: List[str]
 
     _right_struct_col: ClassVar[str] = "_right_values_struct"
 
-    def _structify_right(self, right_df, struct_col_name: str):
+    def _structify_right(self, right_df: pyspark.sql.DataFrame, struct_col_name: str) -> pyspark.sql.DataFrame:
         # we additionally include the right time field though we join on the left's time field.
         # This is so we can see how old the row we joined against is and later determine whether to exclude on basis of ttl
         right_nonjoin_cols = list(set(right_df.columns) - set(self.join_cols))
         # wrap fields on the right in a struct. This is to work around null feature values and ignorenulls
         # used during joining/window function.
         cols_to_wrap = [F.col(c).alias(f"{self.right_container.prefix}_{c}") for c in right_nonjoin_cols]
         right_df = right_df.withColumn(struct_col_name, F.struct(*cols_to_wrap))
@@ -280,15 +280,15 @@
     """
 
     spine: SparkExecNode
     partial_agg_node: SparkExecNode
     fdw: FeatureDefinitionWrapper
     TECTON_AGG_WINDOW_ORDER_COL: ClassVar[str] = "_tecton_agg_window_order_col"
 
-    def _get_aggregations(self, join_spec: _AsofJoinerAndWindowAggregator):
+    def _get_aggregations(self, join_spec: _AsofJoinerAndWindowAggregator) -> List[pyspark.sql.Column]:
         time_aggregation = self.fdw.trailing_time_window_aggregation
         aggregations = []
         for feature in time_aggregation.features:
             aggregation_plan = get_aggregation_plan(
                 feature.function, feature.function_params, time_aggregation.is_continuous, time_aggregation.time_key
             )
             names = aggregation_plan.materialized_column_names(feature.input_feature_name)
@@ -476,18 +476,20 @@
         |---------|-------------|-------------|--------------|--------------|-------------|
         | a       | [1, 2]      | [1, 2, 3]   | [1, 2]       | [11, 12, 13] | 1           |
         | a       | [1, 2]      | [1, 2]      | [1, 2]       | [21, 22]     | 2           |
 
     Attributes:
         full_aggregation_node: The input node, which is always a full aggregation node.
         fdw: The feature definition wrapper that contains the useful metadata.
+        group_by_columns: The columns to group by when rolling up the secondary key and its corresponding feature values.
     """
 
     full_aggregation_node: SparkExecNode
     fdw: FeatureDefinitionWrapper
+    group_by_columns: Tuple[str, ...]
     TECTON_TEMP_STRUCT_PREFIX: ClassVar[str] = "_tecton_internal_temp_struct"
 
     def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         df = self.full_aggregation_node.to_dataframe(spark)
 
         window_to_features = self._window_to_features_map
         # Put all columns in each distinct window into a struct column with name "_struct_{window}", and then collect
@@ -498,15 +500,15 @@
         temp_struct_column_names = [self._temp_struct_column_name(window) for window in window_to_features.keys()]
 
         # Rollup aggregation secondary keys and corresponding feature values by collecting struct values into a list so
         # that for each unique join keys and anchor time pair, we have a list of seoncdary keys and features for each
         # distinct window.
         df = (
             df.select(*df.columns, *temp_struct_columns)
-            .groupBy(*self.fdw.join_keys, ANCHOR_TIME)
+            .groupBy(*self.group_by_columns)
             .agg(*[F.collect_list(c).alias(c) for c in temp_struct_column_names])
         )
         return self._transform_temp_struct_to_feature_columns(df)
 
     @property
     def _window_to_features_map(self) -> Dict[str, List[str]]:
         window_to_features = {}
```

### Comparing `tecton-0.8.0b4/tecton_spark/query/node.py` & `tecton-0.8.0b5/tecton_spark/query/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from abc import abstractmethod
 from typing import List
 
 import attrs
 import pyspark
 
 from tecton_core.query import node_interface
+from tecton_core.query.nodes import exclude_query_node_params
 from tecton_spark.query import translate
 
 
 @attrs.frozen
 class SparkExecNode:
     columns: List[str]
 
     @classmethod
-    def from_query_node(cls, query_node: node_interface.QueryNode):
-        kwargs = attrs.asdict(query_node, value_serializer=translate.attrs_spark_converter, recurse=False)
+    def from_query_node(cls, query_node: node_interface.QueryNode) -> "SparkExecNode":
+        kwargs = attrs.asdict(
+            query_node,
+            value_serializer=translate.attrs_spark_converter,
+            recurse=False,
+            filter=exclude_query_node_params,
+        )
         kwargs["columns"] = query_node.columns
         return cls(**kwargs)
 
     def to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         df = self._to_dataframe(spark)
-        if set([c.lower() for c in df.columns]) != set([c.lower() for c in self.columns]):
+        if {c.lower() for c in df.columns} != {c.lower() for c in self.columns}:
             pass
             # Because we do not refresh schemas on data sources, we can sometimes get different columns than what we have
             # cached. This is problematic but will require separate solution; don't fail for now
             # raise RuntimeError(f"Returned mismatch of columns: received: {df.columns}, expected: {self.columns}")
         return df
 
     @abstractmethod
```

### Comparing `tecton-0.8.0b4/tecton_spark/query/pipeline.py` & `tecton-0.8.0b5/tecton_spark/query/pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,41 +5,45 @@
 from typing import Tuple
 
 import attrs
 import pendulum
 import pyspark
 
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
+from tecton_core.query.executor_params import QueryTreeComputeType
 from tecton_spark import data_observability
 from tecton_spark.partial_aggregations import construct_partial_time_aggregation_df
 from tecton_spark.pipeline_helper import _PipelineBuilder
 from tecton_spark.pipeline_helper import build_odfv_udf_col
 from tecton_spark.query.node import SparkExecNode
 from tecton_spark.schema_spark_utils import schema_to_spark
 
 
 @attrs.frozen
 class MultiOdfvPipelineSparkNode(SparkExecNode):
     input_node: SparkExecNode
     feature_definition_wrappers_namespaces: List[Tuple[FeatureDefinitionWrapper, str]]
+    use_namespace_feature_prefix: bool
 
     def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         """
         Executes multiple ODFV transformations on the same input dataframe.
 
         Note: If the user defines their transformation to produce extra columns
         (besides what's specified in output_schema), they will be ignored. If
         there are missing columns they will fail in this function during
         runtime.
         """
         udf_select_columns = []
         odfv_output_columns = []
         input_df = self.input_node.to_dataframe(spark)
         for fdw, namespace in self.feature_definition_wrappers_namespaces:
-            select_col, output_cols = build_odfv_udf_col(input_df, fdw, namespace)
+            select_col, output_cols = build_odfv_udf_col(
+                input_df, fdw, namespace, use_namespace_feature_prefix=self.use_namespace_feature_prefix
+            )
             udf_select_columns.append(select_col)
             odfv_output_columns.extend(output_cols)
 
         # Execute odfvs in parallel, then deserialize outputs into columns
         input_columns = [f"`{c.name}`" for c in input_df.schema]
         odfv_tmp_outputs = input_df.select(*input_columns, *udf_select_columns)
         return odfv_tmp_outputs.select(*input_columns, *odfv_output_columns)
@@ -94,7 +98,18 @@
     input_node: SparkExecNode
     metrics_collector: data_observability.MetricsCollector = attrs.field(
         factory=data_observability.get_active_metrics_collector
     )
 
     def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
         return self.metrics_collector.observe(self.input_node.to_dataframe(spark))
+
+
+@attrs.frozen
+class StagingSparkNode(SparkExecNode):
+    input_node: SparkExecNode
+    staging_table_name: str
+    query_tree_stage: QueryTreeComputeType
+
+    def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
+        # TODO(danny): consider implementing this in Spark, but for now this is unnecessary and is a passthrough
+        return self.input_node.to_dataframe(spark)
```

### Comparing `tecton-0.8.0b4/tecton_spark/query/projection.py` & `tecton-0.8.0b5/tecton_spark/query/projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pyspark
 import pyspark.sql.window as spark_window
 from pyspark.sql import functions
 from pyspark.sql.functions import expr
 
 from tecton_core.feature_definition_wrapper import FeatureDefinitionWrapper
 from tecton_core.query_consts import ANCHOR_TIME
+from tecton_core.query_consts import TECTON_UNIQUE_ID_COL
 from tecton_spark.query.node import SparkExecNode
 from tecton_spark.time_utils import convert_epoch_to_timestamp_column
 from tecton_spark.time_utils import convert_timestamp_to_epoch
 
 
 @attrs.frozen
 class AddAnchorTimeSparkNode(SparkExecNode):
@@ -198,7 +199,23 @@
             )
             .drop(self.fdw.aggregation_secondary_key)
             .distinct()
         )
         return input_df.withColumn(
             self.fdw.aggregation_secondary_key, functions.explode(self._tecton_temp_aggregation_secondary_key_col)
         )
+
+
+@attrs.frozen
+class AddUniqueIdSparkNode(SparkExecNode):
+    """
+    Add a '_tecton_unique_id' column to the input node. This column is used to uniquely identify rows in the input node.
+
+    Warning: The generated unique ID is non-deterministic on Spark, so this column may not be safe to join on.
+    """
+
+    input_node: SparkExecNode
+
+    def _to_dataframe(self, spark: pyspark.sql.SparkSession) -> pyspark.sql.DataFrame:
+        return self.input_node.to_dataframe(spark).withColumn(
+            TECTON_UNIQUE_ID_COL, functions.monotonically_increasing_id()
+        )
```

### Comparing `tecton-0.8.0b4/tecton_spark/query/translate.py` & `tecton-0.8.0b5/tecton_spark/query/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import attrs
 
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.nodes import AddAnchorTimeNode
 from tecton_core.query.nodes import AddDurationNode
 from tecton_core.query.nodes import AddEffectiveTimestampNode
 from tecton_core.query.nodes import AddRetrievalAnchorTimeNode
+from tecton_core.query.nodes import AddUniqueIdNode
 from tecton_core.query.nodes import AggregationSecondaryKeyExplodeNode
 from tecton_core.query.nodes import AggregationSecondaryKeyRollupNode
 from tecton_core.query.nodes import AsofJoinFullAggNode
 from tecton_core.query.nodes import AsofJoinInputContainer
 from tecton_core.query.nodes import AsofJoinNode
 from tecton_core.query.nodes import AsofSecondaryKeyExplodeNode
 from tecton_core.query.nodes import ConvertEpochToTimestampNode
@@ -27,14 +28,15 @@
 from tecton_core.query.nodes import OfflineStoreScanNode
 from tecton_core.query.nodes import PartialAggNode
 from tecton_core.query.nodes import RawDataSourceScanNode
 from tecton_core.query.nodes import RenameColsNode
 from tecton_core.query.nodes import RespectFeatureStartTimeNode
 from tecton_core.query.nodes import RespectTTLNode
 from tecton_core.query.nodes import SelectDistinctNode
+from tecton_core.query.nodes import StagingNode
 from tecton_core.query.nodes import StreamWatermarkNode
 from tecton_core.query.nodes import UserSpecifiedDataNode
 from tecton_core.query.nodes import WildcardJoinNode
 from tecton_spark.query import data_source
 from tecton_spark.query import filter
 from tecton_spark.query import join
 from tecton_spark.query import pipeline
@@ -79,24 +81,28 @@
         SelectDistinctNode: projection.SelectDistinctSparkNode,
         ConvertEpochToTimestampNode: projection.ConvertEpochToTimestampSparkNode,
         AddEffectiveTimestampNode: projection.AddEffectiveTimestampSparkNode,
         MetricsCollectorNode: pipeline.MetricsCollectorSparkNode,
         AddDurationNode: projection.AddDurationSparkNode,
         AggregationSecondaryKeyRollupNode: join.AggregationSecondaryKeyRollupSparkNode,
         AggregationSecondaryKeyExplodeNode: projection.AggregationSecondaryKeyExplodeSparkNode,
+        StagingNode: pipeline.StagingSparkNode,
+        AddUniqueIdNode: projection.AddUniqueIdSparkNode,
     }
 
     if logical_tree_node.__class__ in node_mapping:
         return node_mapping[logical_tree_node.__class__].from_query_node(logical_tree_node)
 
     msg = f"TODO: mapping for {logical_tree_node.__class__}"
     raise Exception(msg)
 
 
-def attrs_spark_converter(attrs_inst: typing.Any, attr: attrs.Attribute, item: typing.Any) -> typing.Any:
+def attrs_spark_converter(
+    attrs_inst: typing.Any, attr: attrs.Attribute, item: typing.Any  # noqa: ANN401
+) -> typing.Any:  # noqa: ANN401
     """
     This converts a NodeRef into a SparkNode if it's a NodeRef.
     """
     # Check if type is a typing wrapper.
     if get_origin(attr.type) is not None:
         if get_origin(attr.type) == typing.Union and NodeRef in get_args(attr.type) and isinstance(item, NodeRef):
             return spark_convert(item)
```

### Comparing `tecton-0.8.0b4/tecton_spark/schema_derivation_utils.py` & `tecton-0.8.0b5/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.8.0b4/tecton_spark/schema_spark_utils.py` & `tecton-0.8.0b5/tecton_spark/schema_spark_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import List
+from typing import Tuple
+
 import pyspark.sql.types as spark_types
 
 from tecton_core import schema_derivation_utils as core_schema_derivation_utils
 from tecton_core.data_types import ArrayType
 from tecton_core.data_types import BoolType
 from tecton_core.data_types import DataType
 from tecton_core.data_types import Float32Type
@@ -105,9 +108,9 @@
 def schema_to_spark(schema: Schema) -> spark_types.StructType:
     ret = spark_types.StructType()
     for col_name, col_spark_data_type in column_name_spark_data_types(schema):
         ret.add(col_name, col_spark_data_type)
     return ret
 
 
-def column_name_spark_data_types(schema: Schema):
+def column_name_spark_data_types(schema: Schema) -> List[Tuple[str, spark_types.DataType]]:
     return [(c[0], spark_data_type_from_tecton_data_type(c[1])) for c in schema.column_name_and_data_types()]
```

### Comparing `tecton-0.8.0b4/tecton_spark/spark_helper.py` & `tecton-0.8.0b5/tecton_spark/spark_helper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 from dataclasses import dataclass
+from typing import Any
 from typing import Optional
 
 from pyspark.sql import DataFrame
 
 from tecton_proto.args.feature_view_pb2 import ClusterConfig
 
 
@@ -14,15 +15,16 @@
 
 @dataclass
 class QueryPlanInfo:
     has_joins: bool
     has_aggregations: bool
 
 
-def _has_node(node, name: str):
+# Note: we use an Any for this type since it is difficult to ascertain the appropriate type of Pysparks internals.
+def _has_node(node: Any, name: str) -> bool:  # noqa: ANN401
     if node.nodeName() == name:
         return True
     else:
         children = node.children()
         for idx in range(children.size()):
             if _has_node(children.slice(idx, idx + 1).last(), name):
                 return True
@@ -31,15 +33,15 @@
 
 def get_query_plan_info_for_df(df: DataFrame) -> QueryPlanInfo:
     plan = df._jdf.queryExecution().logical()
     return QueryPlanInfo(has_joins=_has_node(plan, "Join"), has_aggregations=_has_node(plan, "Aggregate"))
 
 
 # Log if running on a different spark version than specified for the feature view's batch config
-def check_spark_version(config: Optional[ClusterConfig]):
+def check_spark_version(config: Optional[ClusterConfig]) -> None:
     if config is None:
         return
 
     if config.HasField("new_databricks") and config.new_databricks.HasField("pinned_spark_version"):
         expected_spark_version = config.new_databricks.pinned_spark_version
         # eg '9.1'
         actual_spark_version = os.environ.get("DATABRICKS_RUNTIME_VERSION")
```

### Comparing `tecton-0.8.0b4/tecton_spark/spark_schema_wrapper.py` & `tecton-0.8.0b5/tecton_spark/spark_schema_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 
 
 class SparkSchemaWrapper:
     """
     Wrapper around Spark schema (StructType).
     """
 
-    def __init__(self, schema: StructType):
+    def __init__(self, schema: StructType) -> None:
         """
         Creates a new SparkSchemaWrapper.
 
         :param schema: DataFrame schema.
         """
         self._schema = schema
 
     def to_proto(self) -> SparkSchema:
         return self.from_spark_schema(self._schema)
 
     @classmethod
-    def from_spark_schema(cls, schema) -> SparkSchema:
+    def from_spark_schema(cls, schema: StructType) -> SparkSchema:
         proto = SparkSchema()
         spark_dict = schema.jsonValue()
         for field in spark_dict["fields"]:
             proto_field = proto.fields.add()
             proto_field.name = field["name"]
             proto_field.structfield_json = json.dumps(field)
         return proto
```

### Comparing `tecton-0.8.0b4/tecton_spark/time_utils.py` & `tecton-0.8.0b5/tecton_spark/time_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from tecton_core.time_utils import strict_pytimeparse
 from tecton_proto.data.feature_store_pb2 import FeatureStoreFormatVersion
 
 
 WINDOW_UNBOUNDED_PRECEDING = "unbounded_preceding"
 
 
-def assert_valid_time_string(time_str: str, allow_unbounded=False):
+def assert_valid_time_string(time_str: str, allow_unbounded: bool = False) -> None:
     if allow_unbounded:
         if time_str.lower() != WINDOW_UNBOUNDED_PRECEDING and pytimeparse.parse(time_str) is None:
             msg = f"Time string {time_str} must either be `tecton.WINDOW_UNBOUNDED_PRECEDING` or a valid time string."
             raise TectonValidationError(msg)
     else:
         strict_pytimeparse(time_str)
```

### Comparing `tecton-0.8.0b4/tecton_spark/udfs.py` & `tecton-0.8.0b5/tecton_spark/udfs.py`

 * *Files identical despite different names*

