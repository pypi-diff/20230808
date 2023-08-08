# Comparing `tmp/formal-sdk-1.0.7.tar.gz` & `tmp/formal-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-1.0.7.tar", last modified: Sun Aug  6 23:45:24 2023, max compression
+gzip compressed data, was "formal-sdk-1.0.8.tar", last modified: Tue Aug  8 21:41:02 2023, max compression
```

## Comparing `formal-sdk-1.0.7.tar` & `formal-sdk-1.0.8.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.811936 formal-sdk-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-06 23:45:24.811936 formal-sdk-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 23:45:24.811936 formal-sdk-1.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.747934 formal-sdk-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.759934 formal-sdk-1.0.7/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/cord.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.747934 formal-sdk-1.0.7/src/formal_sdk/gen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.747934 formal-sdk-1.0.7/src/formal_sdk/gen/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.787935 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34739 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33522 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34680 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.747934 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.811936 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/column_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/group_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/key_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.747934 formal-sdk-1.0.7/src/formal_sdk/gen/validate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.811936 formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/validate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/validate_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/identities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_code_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_datahub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_external_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_incident.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/integration_sso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/native_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/satellite.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-06 23:45:10.000000 formal-sdk-1.0.7/src/formal_sdk/work_os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 23:45:24.759934 formal-sdk-1.0.7/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-06 23:45:24.000000 formal-sdk-1.0.7/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-06 23:45:24.000000 formal-sdk-1.0.7/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 23:45:24.000000 formal-sdk-1.0.7/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-06 23:45:24.000000 formal-sdk-1.0.7/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-06 23:45:24.000000 formal-sdk-1.0.7/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.123916 formal-sdk-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-08 21:41:02.123916 formal-sdk-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:41:02.123916 formal-sdk-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.095914 formal-sdk-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.099914 formal-sdk-1.0.8/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/cord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.095914 formal-sdk-1.0.8/src/formal_sdk/gen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.095914 formal-sdk-1.0.8/src/formal_sdk/gen/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.115915 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11526 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30635 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32368 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34407 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27261 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.095914 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.123916 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/column_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/group_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/key_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.095914 formal-sdk-1.0.8/src/formal_sdk/gen/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.123916 formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/validate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/validate_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/identities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_code_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_datahub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_external_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_incident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/integration_sso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/native_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/satellite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-08 21:40:46.000000 formal-sdk-1.0.8/src/formal_sdk/work_os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:41:02.099914 formal-sdk-1.0.8/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-08 21:41:02.000000 formal-sdk-1.0.8/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-08 21:41:02.000000 formal-sdk-1.0.8/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:41:02.000000 formal-sdk-1.0.8/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-08 21:41:02.000000 formal-sdk-1.0.8/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 21:41:02.000000 formal-sdk-1.0.8/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-1.0.7/LICENSE` & `formal-sdk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/PKG-INFO` & `formal-sdk-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-1.0.7/README.md` & `formal-sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/pyproject.toml` & `formal-sdk-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-sdk-1.0.7/src/example.py` & `formal-sdk-1.0.8/src/example.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/__init__.py` & `formal-sdk-1.0.8/src/formal_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/admin.py` & `formal-sdk-1.0.8/src/formal_sdk/admin.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/audit.py` & `formal-sdk-1.0.8/src/formal_sdk/audit.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/cord.py` & `formal-sdk-1.0.8/src/formal_sdk/cord.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/datastore.py` & `formal-sdk-1.0.8/src/formal_sdk/datastore.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/encryption.py` & `formal-sdk-1.0.8/src/formal_sdk/encryption.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/audit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/cord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/datastore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/encryption_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/identities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_cloud_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_code_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_datahub_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_external_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_github_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_incident_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_kms_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_slack_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/integration_sso_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .types.v1 import domain_pb2 as admin_dot_v1_dot_types_dot_v1_dot_domain__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from ...validate.v1 import validate_pb2 as validate_dot_v1_dot_validate__pb2
 from .types.v1 import list_metadata_pb2 as admin_dot_v1_dot_types_dot_v1_dot_list__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61\x64min/v1/inventory.proto\x12\x08\x61\x64min.v1\x1a\x1e\x61\x64min/v1/types/v1/domain.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1avalidate/v1/validate.proto\x1a%admin/v1/types/v1/list_metadata.proto\"\x1c\n\x1aGetInventoryFlatOldRequest\"\xa6\x04\n\tColumnOld\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12*\n\x11table_physical_id\x18\x06 \x01(\tR\x0ftablePhysicalId\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x14\n\x05\x61lias\x18\t \x01(\tR\x05\x61lias\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\"P\n\x1bGetInventoryFlatOldResponse\x12\x31\n\tinventory\x18\x01 \x03(\x0b\x32\x13.admin.v1.ColumnOldR\tinventory\"\x94\x03\n\"UpdateColumnFieldEncryptionRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12l\n\x16\x65ncryption_key_storage\x18\x03 \x01(\tB6\xfa\x42\x33r1R\x12\x63ontrol_plane_onlyR\x1b\x63ontrol_plane_and_with_dataR\x14\x65ncryptionKeyStorage\x12*\n\x11\x65ncryption_key_id\x18\x04 \x01(\tR\x0f\x65ncryptionKeyId\x12W\n\x14\x65ncryption_algorithm\x18\x05 \x01(\tB$\xfa\x42!r\x1fR\x11\x61\x65s_deterministicR\naes_randomR\x13\x65ncryptionAlgorithm\x12\x32\n\x15\x65ncrypt_existing_data\x18\x06 \x01(\x08R\x13\x65ncryptExistingData\"%\n#UpdateColumnFieldEncryptionResponse\"d\n\x19GetInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\"F\n\x1aGetInventoryObjectResponse\x12(\n\x06\x63olumn\x18\x01 \x01(\x0b\x32\x10.admin.v1.ColumnR\x06\x63olumn\"!\n\x1fGetInventoryHierarchicalRequest\"\x92\x07\n GetInventoryHierarchicalResponse\x12R\n\tinventory\x18\x01 \x03(\x0b\x32\x34.admin.v1.GetInventoryHierarchicalResponse.DatastoreR\tinventory\x1a\x90\x01\n\tDatastore\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ntechnology\x18\x03 \x01(\tR\ntechnology\x12?\n\x03\x64\x62s\x18\x04 \x03(\x0b\x32-.admin.v1.GetInventoryHierarchicalResponse.DbR\x03\x64\x62s\x1a\xe6\x01\n\x02\x44\x62\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12K\n\x07schemas\x18\x04 \x03(\x0b\x32\x31.admin.v1.GetInventoryHierarchicalResponse.SchemaR\x07schemas\x12H\n\x06tables\x18\x05 \x03(\x0b\x32\x30.admin.v1.GetInventoryHierarchicalResponse.TableR\x06tables\x1a\x93\x01\n\x06Schema\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12H\n\x06tables\x18\x04 \x03(\x0b\x32\x30.admin.v1.GetInventoryHierarchicalResponse.TableR\x06tables\x1a\xb6\x01\n\x05Table\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\x1f\n\x0bschema_path\x18\x04 \x01(\tR\nschemaPath\x12K\n\x07\x63olumns\x18\x05 \x03(\x0b\x32\x31.admin.v1.GetInventoryHierarchicalResponse.ColumnR\x07\x63olumns\x1aO\n\x06\x43olumn\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1d\n\ntable_path\x18\x03 \x01(\tR\ttablePath\"G\n(GetInventoryHierarchicalPaginatedRequest\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\"\xd1\x07\n)GetInventoryHierarchicalPaginatedResponse\x12[\n\tinventory\x18\x01 \x03(\x0b\x32=.admin.v1.GetInventoryHierarchicalPaginatedResponse.DatastoreR\tinventory\x1a\x99\x01\n\tDatastore\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ntechnology\x18\x03 \x01(\tR\ntechnology\x12H\n\x03\x64\x62s\x18\x04 \x03(\x0b\x32\x36.admin.v1.GetInventoryHierarchicalPaginatedResponse.DbR\x03\x64\x62s\x1a\xf8\x01\n\x02\x44\x62\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12T\n\x07schemas\x18\x04 \x03(\x0b\x32:.admin.v1.GetInventoryHierarchicalPaginatedResponse.SchemaR\x07schemas\x12Q\n\x06tables\x18\x05 \x03(\x0b\x32\x39.admin.v1.GetInventoryHierarchicalPaginatedResponse.TableR\x06tables\x1a\x9c\x01\n\x06Schema\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12Q\n\x06tables\x18\x04 \x03(\x0b\x32\x39.admin.v1.GetInventoryHierarchicalPaginatedResponse.TableR\x06tables\x1a\xbf\x01\n\x05Table\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\x1f\n\x0bschema_path\x18\x04 \x01(\tR\nschemaPath\x12T\n\x07\x63olumns\x18\x05 \x03(\x0b\x32:.admin.v1.GetInventoryHierarchicalPaginatedResponse.ColumnR\x07\x63olumns\x1aO\n\x06\x43olumn\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1d\n\ntable_path\x18\x03 \x01(\tR\ttablePath\"s\n\x17GetInventoryFlatRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x14\n\x05\x61\x66ter\x18\x02 \x01(\tR\x05\x61\x66ter\x12\x16\n\x06\x62\x65\x66ore\x18\x03 \x01(\tR\x06\x62\x65\x66ore\x12\x14\n\x05order\x18\x04 \x01(\tR\x05order\"\xb3\x04\n\x06\x43olumn\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12*\n\x11table_physical_id\x18\x06 \x01(\tR\x0ftablePhysicalId\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x14\n\x05\x61lias\x18\t \x01(\tR\x05\x61lias\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\x12\x0e\n\x02id\x18\x11 \x01(\tR\x02id\"h\n\x02\x44s\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ntechnology\x18\x03 \x01(\tR\ntechnology\x12\x1e\n\x03\x64\x62s\x18\x04 \x03(\x0b\x32\x0c.admin.v1.DbR\x03\x64\x62s\"\xb4\x01\n\x02\x44\x62\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12*\n\x07schemas\x18\x04 \x03(\x0b\x32\x10.admin.v1.SchemaR\x07schemas\x12\'\n\x06tables\x18\x05 \x03(\x0b\x32\x0f.admin.v1.TableR\x06tables\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\"\x82\x01\n\x06Schema\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\'\n\x06tables\x18\x04 \x03(\x0b\x32\x0f.admin.v1.TableR\x06tables\x12\x0e\n\x02id\x18\x05 \x01(\tR\x02id\"\xa5\x01\n\x05Table\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\x1f\n\x0bschema_path\x18\x04 \x01(\tR\nschemaPath\x12*\n\x07\x63olumns\x18\x05 \x03(\x0b\x32\x10.admin.v1.ColumnR\x07\x63olumns\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\"\xbe\x03\n\tSubColumn\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\x12\x0e\n\x02id\x18\x11 \x01(\tR\x02id\"\xa0\x02\n\x0fInventoryObject\x12,\n\tdatastore\x18\x01 \x01(\x0b\x32\x0c.admin.v1.DsH\x00R\tdatastore\x12\x1e\n\x02\x64\x62\x18\x02 \x01(\x0b\x32\x0c.admin.v1.DbH\x00R\x02\x64\x62\x12*\n\x06schema\x18\x03 \x01(\x0b\x32\x10.admin.v1.SchemaH\x00R\x06schema\x12\'\n\x05table\x18\x04 \x01(\x0b\x32\x0f.admin.v1.TableH\x00R\x05table\x12*\n\x06\x63olumn\x18\x05 \x01(\x0b\x32\x10.admin.v1.ColumnH\x00R\x06\x63olumn\x12\x34\n\nsub_column\x18\x06 \x01(\x0b\x32\x13.admin.v1.SubColumnH\x00R\tsubColumnB\x08\n\x06object\"\x99\x01\n\x18GetInventoryFlatResponse\x12\x37\n\tinventory\x18\x01 \x03(\x0b\x32\x19.admin.v1.InventoryObjectR\tinventory\x12\x44\n\rlist_metadata\x18\x02 \x01(\x0b\x32\x1f.admin.v1.types.v1.ListMetadataR\x0clistMetadata\"\x86\x01\n\x1dUpdateColumnLockStatusRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1c\n\tvalidated\x18\x03 \x01(\x08R\tvalidated\" \n\x1eUpdateColumnLockStatusResponse\"\x86\x01\n\x1cUpdateColumnDataLabelRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1d\n\ndata_label\x18\x03 \x01(\tR\tdataLabel\"\x1f\n\x1dUpdateColumnDataLabelResponse\"\x9f\x07\n\x1c\x43reateInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12M\n\x0bobject_type\x18\x02 \x01(\tB,\xfa\x42)r\'R\x02\x64\x62R\x06schemaR\x05tableR\x06\x63olumnR\nsub-columnR\nobjectType\x12\x39\n\x02\x64\x62\x18\x03 \x01(\x0b\x32).admin.v1.CreateInventoryObjectRequest.DbR\x02\x64\x62\x12\x45\n\x06schema\x18\x04 \x01(\x0b\x32-.admin.v1.CreateInventoryObjectRequest.SchemaR\x06schema\x12\x42\n\x05table\x18\x05 \x01(\x0b\x32,.admin.v1.CreateInventoryObjectRequest.TableR\x05table\x12\x45\n\x06\x63olumn\x18\x06 \x01(\x0b\x32-.admin.v1.CreateInventoryObjectRequest.ColumnR\x06\x63olumn\x12O\n\nsub_column\x18\x07 \x01(\x0b\x32\x30.admin.v1.CreateInventoryObjectRequest.SubColumnR\tsubColumn\x1a>\n\x02\x44\x62\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1a\x42\n\x06Schema\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1a\x41\n\x05Table\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1ah\n\x06\x43olumn\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12$\n\tdata_type\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x64\x61taType\x1au\n\tSubColumn\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12.\n\x08sub_type\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0eR\x06hstoreR\x04jsonR\x07subType\"\x1f\n\x1d\x43reateInventoryObjectResponse\"g\n\x1c\x44\x65leteInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\"\x1f\n\x1d\x44\x65leteInventoryObjectResponse\"w\n\x03Tag\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12\x43\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01R\tcreatedAt\"8\n\x19\x43reateInventoryTagRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\"=\n\x1a\x43reateInventoryTagResponse\x12\x1f\n\x03tag\x18\x01 \x01(\x0b\x32\r.admin.v1.TagR\x03tag\"s\n\x17GetInventoryTagsRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x14\n\x05\x61\x66ter\x18\x02 \x01(\tR\x05\x61\x66ter\x12\x16\n\x06\x62\x65\x66ore\x18\x03 \x01(\tR\x06\x62\x65\x66ore\x12\x14\n\x05order\x18\x04 \x01(\tR\x05order\"\x83\x01\n\x18GetInventoryTagsResponse\x12!\n\x04tags\x18\x01 \x03(\x0b\x32\r.admin.v1.TagR\x04tags\x12\x44\n\rlist_metadata\x18\x02 \x01(\x0b\x32\x1f.admin.v1.types.v1.ListMetadataR\x0clistMetadata\"\x7f\n UpdateInventoryObjectTagsRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x12\n\x04tags\x18\x03 \x03(\tR\x04tags\"\xce\x04\n!UpdateInventoryObjectTagsResponse\x12S\n\x06object\x18\x01 \x01(\x0b\x32;.admin.v1.UpdateInventoryObjectTagsResponse.InventoryObjectR\x06object\x1a\xd3\x03\n\x0fInventoryObject\x12!\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tR\x0b\x64\x61tastoreId\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x17\n\x07\x64\x62_path\x18\x04 \x01(\tR\x06\x64\x62Path\x12\x1d\n\ntable_path\x18\x05 \x01(\tR\ttablePath\x12\x1f\n\x0bschema_path\x18\x06 \x01(\tR\nschemaPath\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x1b\n\tdata_type\x18\x08 \x01(\tR\x08\x64\x61taType\x12\x1d\n\ndata_label\x18\t \x01(\tR\tdataLabel\x12\x1d\n\nupdated_at\x18\n \x01(\x03R\tupdatedAt\x12\x1d\n\ncreated_at\x18\x0b \x01(\x03R\tcreatedAt\x12&\n\x0f\x64\x61ta_store_name\x18\x0c \x01(\tR\rdataStoreName\x12\x12\n\x04name\x18\r \x01(\tR\x04name\x12\x1c\n\tvalidated\x18\x0e \x01(\x08R\tvalidated\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\"4\n\x19\x44\x65leteInventoryTagRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x02id\"?\n\x1a\x44\x65leteInventoryTagResponse\x12!\n\x04tags\x18\x01 \x03(\x0b\x32\r.admin.v1.TagR\x04tags\"\xcf\x01\n\x17\x43reateDataDomainRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x30\n\x06owners\x18\x03 \x03(\x0b\x32\x18.admin.v1.types.v1.OwnerR\x06owners\x12%\n\x0e\x65xcluded_paths\x18\x04 \x03(\tR\rexcludedPaths\x12%\n\x0eincluded_paths\x18\x05 \x03(\tR\rincludedPaths\"*\n\x18\x43reateDataDomainResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x17\n\x15GetDataDomainsRequest\"M\n\x16GetDataDomainsResponse\x12\x33\n\x07\x64omains\x18\x01 \x03(\x0b\x32\x19.admin.v1.types.v1.DomainR\x07\x64omains\"*\n\x18GetDataDomainByIdRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"N\n\x19GetDataDomainByIdResponse\x12\x31\n\x06\x64omain\x18\x01 \x01(\x0b\x32\x19.admin.v1.types.v1.DomainR\x06\x64omain\"\xdf\x01\n\x17UpdateDataDomainRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x30\n\x06owners\x18\x04 \x03(\x0b\x32\x18.admin.v1.types.v1.OwnerR\x06owners\x12%\n\x0e\x65xcluded_paths\x18\x05 \x03(\tR\rexcludedPaths\x12%\n\x0eincluded_paths\x18\x06 \x03(\tR\rincludedPaths\"M\n\x18UpdateDataDomainResponse\x12\x31\n\x06\x64omain\x18\x01 \x01(\x0b\x32\x19.admin.v1.types.v1.DomainR\x06\x64omain\")\n\x17\x44\x65leteDataDomainRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1a\n\x18\x44\x65leteDataDomainResponse2\xce\x0f\n\x10InventoryService\x12s\n\x18GetInventoryHierarchical\x12).admin.v1.GetInventoryHierarchicalRequest\x1a*.admin.v1.GetInventoryHierarchicalResponse\"\x00\x12\x8e\x01\n!GetInventoryHierarchicalPaginated\x12\x32.admin.v1.GetInventoryHierarchicalPaginatedRequest\x1a\x33.admin.v1.GetInventoryHierarchicalPaginatedResponse\"\x00\x12[\n\x10GetInventoryFlat\x12!.admin.v1.GetInventoryFlatRequest\x1a\".admin.v1.GetInventoryFlatResponse\"\x00\x12\x64\n\x13GetInventoryFlatOld\x12$.admin.v1.GetInventoryFlatOldRequest\x1a%.admin.v1.GetInventoryFlatOldResponse\"\x00\x12\x61\n\x12GetInventoryObject\x12#.admin.v1.GetInventoryObjectRequest\x1a$.admin.v1.GetInventoryObjectResponse\"\x00\x12m\n\x16UpdateColumnLockStatus\x12\'.admin.v1.UpdateColumnLockStatusRequest\x1a(.admin.v1.UpdateColumnLockStatusResponse\"\x00\x12j\n\x15UpdateColumnDataLabel\x12&.admin.v1.UpdateColumnDataLabelRequest\x1a\'.admin.v1.UpdateColumnDataLabelResponse\"\x00\x12|\n\x1bUpdateColumnFieldEncryption\x12,.admin.v1.UpdateColumnFieldEncryptionRequest\x1a-.admin.v1.UpdateColumnFieldEncryptionResponse\"\x00\x12v\n\x19UpdateInventoryObjectTags\x12*.admin.v1.UpdateInventoryObjectTagsRequest\x1a+.admin.v1.UpdateInventoryObjectTagsResponse\"\x00\x12j\n\x15\x43reateInventoryObject\x12&.admin.v1.CreateInventoryObjectRequest\x1a\'.admin.v1.CreateInventoryObjectResponse\"\x00\x12j\n\x15\x44\x65leteInventoryObject\x12&.admin.v1.DeleteInventoryObjectRequest\x1a\'.admin.v1.DeleteInventoryObjectResponse\"\x00\x12\x61\n\x12\x43reateInventoryTag\x12#.admin.v1.CreateInventoryTagRequest\x1a$.admin.v1.CreateInventoryTagResponse\"\x00\x12[\n\x10GetInventoryTags\x12!.admin.v1.GetInventoryTagsRequest\x1a\".admin.v1.GetInventoryTagsResponse\"\x00\x12\x61\n\x12\x44\x65leteInventoryTag\x12#.admin.v1.DeleteInventoryTagRequest\x1a$.admin.v1.DeleteInventoryTagResponse\"\x00\x12Y\n\x10\x43reateDataDomain\x12!.admin.v1.CreateDataDomainRequest\x1a\".admin.v1.CreateDataDomainResponse\x12S\n\x0eGetDataDomains\x12\x1f.admin.v1.GetDataDomainsRequest\x1a .admin.v1.GetDataDomainsResponse\x12\\\n\x11GetDataDomainById\x12\".admin.v1.GetDataDomainByIdRequest\x1a#.admin.v1.GetDataDomainByIdResponse\x12Y\n\x10UpdateDataDomain\x12!.admin.v1.UpdateDataDomainRequest\x1a\".admin.v1.UpdateDataDomainResponse\x12Y\n\x10\x44\x65leteDataDomain\x12!.admin.v1.DeleteDataDomainRequest\x1a\".admin.v1.DeleteDataDomainResponseB\xa9\x01\n\x0c\x63om.admin.v1B\x0eInventoryProtoP\x01ZHgithub.com/formalco/control-plane/backend/admin-api/gen/admin/v1;adminv1\xa2\x02\x03\x41XX\xaa\x02\x08\x41\x64min.V1\xca\x02\x08\x41\x64min\\V1\xe2\x02\x14\x41\x64min\\V1\\GPBMetadata\xea\x02\tAdmin::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x61\x64min/v1/inventory.proto\x12\x08\x61\x64min.v1\x1a\x1e\x61\x64min/v1/types/v1/domain.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1avalidate/v1/validate.proto\x1a%admin/v1/types/v1/list_metadata.proto\"\x1c\n\x1aGetInventoryFlatOldRequest\"\xa6\x04\n\tColumnOld\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12*\n\x11table_physical_id\x18\x06 \x01(\tR\x0ftablePhysicalId\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x14\n\x05\x61lias\x18\t \x01(\tR\x05\x61lias\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\"P\n\x1bGetInventoryFlatOldResponse\x12\x31\n\tinventory\x18\x01 \x03(\x0b\x32\x13.admin.v1.ColumnOldR\tinventory\"\x94\x03\n\"UpdateColumnFieldEncryptionRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12l\n\x16\x65ncryption_key_storage\x18\x03 \x01(\tB6\xfa\x42\x33r1R\x12\x63ontrol_plane_onlyR\x1b\x63ontrol_plane_and_with_dataR\x14\x65ncryptionKeyStorage\x12*\n\x11\x65ncryption_key_id\x18\x04 \x01(\tR\x0f\x65ncryptionKeyId\x12W\n\x14\x65ncryption_algorithm\x18\x05 \x01(\tB$\xfa\x42!r\x1fR\x11\x61\x65s_deterministicR\naes_randomR\x13\x65ncryptionAlgorithm\x12\x32\n\x15\x65ncrypt_existing_data\x18\x06 \x01(\x08R\x13\x65ncryptExistingData\"%\n#UpdateColumnFieldEncryptionResponse\"d\n\x19GetInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\"F\n\x1aGetInventoryObjectResponse\x12(\n\x06\x63olumn\x18\x01 \x01(\x0b\x32\x10.admin.v1.ColumnR\x06\x63olumn\"!\n\x1fGetInventoryHierarchicalRequest\"\x92\x07\n GetInventoryHierarchicalResponse\x12R\n\tinventory\x18\x01 \x03(\x0b\x32\x34.admin.v1.GetInventoryHierarchicalResponse.DatastoreR\tinventory\x1a\x90\x01\n\tDatastore\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ntechnology\x18\x03 \x01(\tR\ntechnology\x12?\n\x03\x64\x62s\x18\x04 \x03(\x0b\x32-.admin.v1.GetInventoryHierarchicalResponse.DbR\x03\x64\x62s\x1a\xe6\x01\n\x02\x44\x62\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12K\n\x07schemas\x18\x04 \x03(\x0b\x32\x31.admin.v1.GetInventoryHierarchicalResponse.SchemaR\x07schemas\x12H\n\x06tables\x18\x05 \x03(\x0b\x32\x30.admin.v1.GetInventoryHierarchicalResponse.TableR\x06tables\x1a\x93\x01\n\x06Schema\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12H\n\x06tables\x18\x04 \x03(\x0b\x32\x30.admin.v1.GetInventoryHierarchicalResponse.TableR\x06tables\x1a\xb6\x01\n\x05Table\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\x1f\n\x0bschema_path\x18\x04 \x01(\tR\nschemaPath\x12K\n\x07\x63olumns\x18\x05 \x03(\x0b\x32\x31.admin.v1.GetInventoryHierarchicalResponse.ColumnR\x07\x63olumns\x1aO\n\x06\x43olumn\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1d\n\ntable_path\x18\x03 \x01(\tR\ttablePath\"\xaa\x01\n\x13GetInventoryRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x14\n\x05\x61\x66ter\x18\x02 \x01(\tR\x05\x61\x66ter\x12\x16\n\x06\x62\x65\x66ore\x18\x03 \x01(\tR\x06\x62\x65\x66ore\x12\x14\n\x05order\x18\x04 \x01(\tR\x05order\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12%\n\x0e\x65xcluded_paths\x18\x06 \x03(\tR\rexcludedPaths\"\x95\x01\n\x14GetInventoryResponse\x12\x37\n\tinventory\x18\x01 \x03(\x0b\x32\x19.admin.v1.InventoryObjectR\tinventory\x12\x44\n\rlist_metadata\x18\x02 \x01(\x0b\x32\x1f.admin.v1.types.v1.ListMetadataR\x0clistMetadata\"s\n\x17GetInventoryFlatRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x14\n\x05\x61\x66ter\x18\x02 \x01(\tR\x05\x61\x66ter\x12\x16\n\x06\x62\x65\x66ore\x18\x03 \x01(\tR\x06\x62\x65\x66ore\x12\x14\n\x05order\x18\x04 \x01(\tR\x05order\"\xb3\x04\n\x06\x43olumn\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12*\n\x11table_physical_id\x18\x06 \x01(\tR\x0ftablePhysicalId\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x14\n\x05\x61lias\x18\t \x01(\tR\x05\x61lias\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\x12\x0e\n\x02id\x18\x11 \x01(\tR\x02id\"h\n\x02\x44s\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x1e\n\ntechnology\x18\x03 \x01(\tR\ntechnology\x12\x1e\n\x03\x64\x62s\x18\x04 \x03(\x0b\x32\x0c.admin.v1.DbR\x03\x64\x62s\"\xb4\x01\n\x02\x44\x62\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12*\n\x07schemas\x18\x04 \x03(\x0b\x32\x10.admin.v1.SchemaR\x07schemas\x12\'\n\x06tables\x18\x05 \x03(\x0b\x32\x0f.admin.v1.TableR\x06tables\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\"\x82\x01\n\x06Schema\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\'\n\x06tables\x18\x04 \x03(\x0b\x32\x0f.admin.v1.TableR\x06tables\x12\x0e\n\x02id\x18\x05 \x01(\tR\x02id\"\xa5\x01\n\x05Table\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x17\n\x07\x64\x62_path\x18\x03 \x01(\tR\x06\x64\x62Path\x12\x1f\n\x0bschema_path\x18\x04 \x01(\tR\nschemaPath\x12*\n\x07\x63olumns\x18\x05 \x03(\x0b\x32\x10.admin.v1.ColumnR\x07\x63olumns\x12\x0e\n\x02id\x18\x06 \x01(\tR\x02id\"\xbe\x03\n\tSubColumn\x12\x1d\n\ncreated_at\x18\x01 \x01(\x03R\tcreatedAt\x12\x1d\n\nupdated_at\x18\x02 \x01(\x03R\tupdatedAt\x12!\n\x0c\x64\x61tastore_id\x18\x03 \x01(\tR\x0b\x64\x61tastoreId\x12%\n\x0e\x64\x61tastore_name\x18\x04 \x01(\tR\rdatastoreName\x12\x12\n\x04path\x18\x05 \x01(\tR\x04path\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x1d\n\ntable_path\x18\n \x01(\tR\ttablePath\x12\x1d\n\ndata_label\x18\x0b \x01(\tR\tdataLabel\x12\x1b\n\tdata_type\x18\x0c \x01(\tR\x08\x64\x61taType\x12\"\n\rdata_type_oid\x18\r \x01(\rR\x0b\x64\x61taTypeOid\x12@\n\x1d\x64\x61ta_label_locked_for_sidecar\x18\x0e \x01(\x08R\x19\x64\x61taLabelLockedForSidecar\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\x12\x1c\n\tencrypted\x18\x10 \x01(\x08R\tencrypted\x12\x0e\n\x02id\x18\x11 \x01(\tR\x02id\"\xa0\x02\n\x0fInventoryObject\x12,\n\tdatastore\x18\x01 \x01(\x0b\x32\x0c.admin.v1.DsH\x00R\tdatastore\x12\x1e\n\x02\x64\x62\x18\x02 \x01(\x0b\x32\x0c.admin.v1.DbH\x00R\x02\x64\x62\x12*\n\x06schema\x18\x03 \x01(\x0b\x32\x10.admin.v1.SchemaH\x00R\x06schema\x12\'\n\x05table\x18\x04 \x01(\x0b\x32\x0f.admin.v1.TableH\x00R\x05table\x12*\n\x06\x63olumn\x18\x05 \x01(\x0b\x32\x10.admin.v1.ColumnH\x00R\x06\x63olumn\x12\x34\n\nsub_column\x18\x06 \x01(\x0b\x32\x13.admin.v1.SubColumnH\x00R\tsubColumnB\x08\n\x06object\"\x99\x01\n\x18GetInventoryFlatResponse\x12\x37\n\tinventory\x18\x01 \x03(\x0b\x32\x19.admin.v1.InventoryObjectR\tinventory\x12\x44\n\rlist_metadata\x18\x02 \x01(\x0b\x32\x1f.admin.v1.types.v1.ListMetadataR\x0clistMetadata\"\x86\x01\n\x1dUpdateColumnLockStatusRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1c\n\tvalidated\x18\x03 \x01(\x08R\tvalidated\" \n\x1eUpdateColumnLockStatusResponse\"\x86\x01\n\x1cUpdateColumnDataLabelRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1d\n\ndata_label\x18\x03 \x01(\tR\tdataLabel\"\x1f\n\x1dUpdateColumnDataLabelResponse\"\x9f\x07\n\x1c\x43reateInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12M\n\x0bobject_type\x18\x02 \x01(\tB,\xfa\x42)r\'R\x02\x64\x62R\x06schemaR\x05tableR\x06\x63olumnR\nsub-columnR\nobjectType\x12\x39\n\x02\x64\x62\x18\x03 \x01(\x0b\x32).admin.v1.CreateInventoryObjectRequest.DbR\x02\x64\x62\x12\x45\n\x06schema\x18\x04 \x01(\x0b\x32-.admin.v1.CreateInventoryObjectRequest.SchemaR\x06schema\x12\x42\n\x05table\x18\x05 \x01(\x0b\x32,.admin.v1.CreateInventoryObjectRequest.TableR\x05table\x12\x45\n\x06\x63olumn\x18\x06 \x01(\x0b\x32-.admin.v1.CreateInventoryObjectRequest.ColumnR\x06\x63olumn\x12O\n\nsub_column\x18\x07 \x01(\x0b\x32\x30.admin.v1.CreateInventoryObjectRequest.SubColumnR\tsubColumn\x1a>\n\x02\x44\x62\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1a\x42\n\x06Schema\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1a\x41\n\x05Table\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x1ah\n\x06\x43olumn\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12$\n\tdata_type\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x08\x64\x61taType\x1au\n\tSubColumn\x12\x1b\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12.\n\x08sub_type\x18\x03 \x01(\tB\x13\xfa\x42\x10r\x0eR\x06hstoreR\x04jsonR\x07subType\"\x1f\n\x1d\x43reateInventoryObjectResponse\"g\n\x1c\x44\x65leteInventoryObjectRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\"\x1f\n\x1d\x44\x65leteInventoryObjectResponse\"w\n\x03Tag\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\x12\x43\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x08\xfa\x42\x05\xb2\x01\x02\x08\x01R\tcreatedAt\"8\n\x19\x43reateInventoryTagRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04name\"=\n\x1a\x43reateInventoryTagResponse\x12\x1f\n\x03tag\x18\x01 \x01(\x0b\x32\r.admin.v1.TagR\x03tag\"s\n\x17GetInventoryTagsRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x14\n\x05\x61\x66ter\x18\x02 \x01(\tR\x05\x61\x66ter\x12\x16\n\x06\x62\x65\x66ore\x18\x03 \x01(\tR\x06\x62\x65\x66ore\x12\x14\n\x05order\x18\x04 \x01(\tR\x05order\"\x83\x01\n\x18GetInventoryTagsResponse\x12!\n\x04tags\x18\x01 \x03(\x0b\x32\r.admin.v1.TagR\x04tags\x12\x44\n\rlist_metadata\x18\x02 \x01(\x0b\x32\x1f.admin.v1.types.v1.ListMetadataR\x0clistMetadata\"\x7f\n UpdateInventoryObjectTagsRequest\x12*\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x0b\x64\x61tastoreId\x12\x1b\n\x04path\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x04path\x12\x12\n\x04tags\x18\x03 \x03(\tR\x04tags\"\xce\x04\n!UpdateInventoryObjectTagsResponse\x12S\n\x06object\x18\x01 \x01(\x0b\x32;.admin.v1.UpdateInventoryObjectTagsResponse.InventoryObjectR\x06object\x1a\xd3\x03\n\x0fInventoryObject\x12!\n\x0c\x64\x61tastore_id\x18\x01 \x01(\tR\x0b\x64\x61tastoreId\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x17\n\x07\x64\x62_path\x18\x04 \x01(\tR\x06\x64\x62Path\x12\x1d\n\ntable_path\x18\x05 \x01(\tR\ttablePath\x12\x1f\n\x0bschema_path\x18\x06 \x01(\tR\nschemaPath\x12\x34\n\x16table_attribute_number\x18\x07 \x01(\x04R\x14tableAttributeNumber\x12\x1b\n\tdata_type\x18\x08 \x01(\tR\x08\x64\x61taType\x12\x1d\n\ndata_label\x18\t \x01(\tR\tdataLabel\x12\x1d\n\nupdated_at\x18\n \x01(\x03R\tupdatedAt\x12\x1d\n\ncreated_at\x18\x0b \x01(\x03R\tcreatedAt\x12&\n\x0f\x64\x61ta_store_name\x18\x0c \x01(\tR\rdataStoreName\x12\x12\n\x04name\x18\r \x01(\tR\x04name\x12\x1c\n\tvalidated\x18\x0e \x01(\x08R\tvalidated\x12\x12\n\x04tags\x18\x0f \x03(\tR\x04tags\"4\n\x19\x44\x65leteInventoryTagRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01R\x02id\"?\n\x1a\x44\x65leteInventoryTagResponse\x12!\n\x04tags\x18\x01 \x03(\x0b\x32\r.admin.v1.TagR\x04tags\"\xcf\x01\n\x17\x43reateDataDomainRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x30\n\x06owners\x18\x03 \x03(\x0b\x32\x18.admin.v1.types.v1.OwnerR\x06owners\x12%\n\x0e\x65xcluded_paths\x18\x04 \x03(\tR\rexcludedPaths\x12%\n\x0eincluded_paths\x18\x05 \x03(\tR\rincludedPaths\"*\n\x18\x43reateDataDomainResponse\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x17\n\x15GetDataDomainsRequest\"M\n\x16GetDataDomainsResponse\x12\x33\n\x07\x64omains\x18\x01 \x03(\x0b\x32\x19.admin.v1.types.v1.DomainR\x07\x64omains\"*\n\x18GetDataDomainByIdRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"N\n\x19GetDataDomainByIdResponse\x12\x31\n\x06\x64omain\x18\x01 \x01(\x0b\x32\x19.admin.v1.types.v1.DomainR\x06\x64omain\"\xdf\x01\n\x17UpdateDataDomainRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x30\n\x06owners\x18\x04 \x03(\x0b\x32\x18.admin.v1.types.v1.OwnerR\x06owners\x12%\n\x0e\x65xcluded_paths\x18\x05 \x03(\tR\rexcludedPaths\x12%\n\x0eincluded_paths\x18\x06 \x03(\tR\rincludedPaths\"M\n\x18UpdateDataDomainResponse\x12\x31\n\x06\x64omain\x18\x01 \x01(\x0b\x32\x19.admin.v1.types.v1.DomainR\x06\x64omain\")\n\x17\x44\x65leteDataDomainRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\x1a\n\x18\x44\x65leteDataDomainResponse2\x8e\x0f\n\x10InventoryService\x12s\n\x18GetInventoryHierarchical\x12).admin.v1.GetInventoryHierarchicalRequest\x1a*.admin.v1.GetInventoryHierarchicalResponse\"\x00\x12O\n\x0cGetInventory\x12\x1d.admin.v1.GetInventoryRequest\x1a\x1e.admin.v1.GetInventoryResponse\"\x00\x12[\n\x10GetInventoryFlat\x12!.admin.v1.GetInventoryFlatRequest\x1a\".admin.v1.GetInventoryFlatResponse\"\x00\x12\x64\n\x13GetInventoryFlatOld\x12$.admin.v1.GetInventoryFlatOldRequest\x1a%.admin.v1.GetInventoryFlatOldResponse\"\x00\x12\x61\n\x12GetInventoryObject\x12#.admin.v1.GetInventoryObjectRequest\x1a$.admin.v1.GetInventoryObjectResponse\"\x00\x12m\n\x16UpdateColumnLockStatus\x12\'.admin.v1.UpdateColumnLockStatusRequest\x1a(.admin.v1.UpdateColumnLockStatusResponse\"\x00\x12j\n\x15UpdateColumnDataLabel\x12&.admin.v1.UpdateColumnDataLabelRequest\x1a\'.admin.v1.UpdateColumnDataLabelResponse\"\x00\x12|\n\x1bUpdateColumnFieldEncryption\x12,.admin.v1.UpdateColumnFieldEncryptionRequest\x1a-.admin.v1.UpdateColumnFieldEncryptionResponse\"\x00\x12v\n\x19UpdateInventoryObjectTags\x12*.admin.v1.UpdateInventoryObjectTagsRequest\x1a+.admin.v1.UpdateInventoryObjectTagsResponse\"\x00\x12j\n\x15\x43reateInventoryObject\x12&.admin.v1.CreateInventoryObjectRequest\x1a\'.admin.v1.CreateInventoryObjectResponse\"\x00\x12j\n\x15\x44\x65leteInventoryObject\x12&.admin.v1.DeleteInventoryObjectRequest\x1a\'.admin.v1.DeleteInventoryObjectResponse\"\x00\x12\x61\n\x12\x43reateInventoryTag\x12#.admin.v1.CreateInventoryTagRequest\x1a$.admin.v1.CreateInventoryTagResponse\"\x00\x12[\n\x10GetInventoryTags\x12!.admin.v1.GetInventoryTagsRequest\x1a\".admin.v1.GetInventoryTagsResponse\"\x00\x12\x61\n\x12\x44\x65leteInventoryTag\x12#.admin.v1.DeleteInventoryTagRequest\x1a$.admin.v1.DeleteInventoryTagResponse\"\x00\x12Y\n\x10\x43reateDataDomain\x12!.admin.v1.CreateDataDomainRequest\x1a\".admin.v1.CreateDataDomainResponse\x12S\n\x0eGetDataDomains\x12\x1f.admin.v1.GetDataDomainsRequest\x1a .admin.v1.GetDataDomainsResponse\x12\\\n\x11GetDataDomainById\x12\".admin.v1.GetDataDomainByIdRequest\x1a#.admin.v1.GetDataDomainByIdResponse\x12Y\n\x10UpdateDataDomain\x12!.admin.v1.UpdateDataDomainRequest\x1a\".admin.v1.UpdateDataDomainResponse\x12Y\n\x10\x44\x65leteDataDomain\x12!.admin.v1.DeleteDataDomainRequest\x1a\".admin.v1.DeleteDataDomainResponseB\xa9\x01\n\x0c\x63om.admin.v1B\x0eInventoryProtoP\x01ZHgithub.com/formalco/control-plane/backend/admin-api/gen/admin/v1;adminv1\xa2\x02\x03\x41XX\xaa\x02\x08\x41\x64min.V1\xca\x02\x08\x41\x64min\\V1\xe2\x02\x14\x41\x64min\\V1\\GPBMetadata\xea\x02\tAdmin::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'admin.v1.inventory_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -34,16 +34,14 @@
   _UPDATECOLUMNFIELDENCRYPTIONREQUEST.fields_by_name['encryption_key_storage']._serialized_options = b'\372B3r1R\022control_plane_onlyR\033control_plane_and_with_data'
   _UPDATECOLUMNFIELDENCRYPTIONREQUEST.fields_by_name['encryption_algorithm']._options = None
   _UPDATECOLUMNFIELDENCRYPTIONREQUEST.fields_by_name['encryption_algorithm']._serialized_options = b'\372B!r\037R\021aes_deterministicR\naes_random'
   _GETINVENTORYOBJECTREQUEST.fields_by_name['datastore_id']._options = None
   _GETINVENTORYOBJECTREQUEST.fields_by_name['datastore_id']._serialized_options = b'\372B\004r\002\020\001'
   _GETINVENTORYOBJECTREQUEST.fields_by_name['path']._options = None
   _GETINVENTORYOBJECTREQUEST.fields_by_name['path']._serialized_options = b'\372B\004r\002\020\001'
-  _GETINVENTORYHIERARCHICALPAGINATEDREQUEST.fields_by_name['path']._options = None
-  _GETINVENTORYHIERARCHICALPAGINATEDREQUEST.fields_by_name['path']._serialized_options = b'\372B\004r\002\020\001'
   _UPDATECOLUMNLOCKSTATUSREQUEST.fields_by_name['datastore_id']._options = None
   _UPDATECOLUMNLOCKSTATUSREQUEST.fields_by_name['datastore_id']._serialized_options = b'\372B\004r\002\020\001'
   _UPDATECOLUMNLOCKSTATUSREQUEST.fields_by_name['path']._options = None
   _UPDATECOLUMNLOCKSTATUSREQUEST.fields_by_name['path']._serialized_options = b'\372B\004r\002\020\001'
   _UPDATECOLUMNDATALABELREQUEST.fields_by_name['datastore_id']._options = None
   _UPDATECOLUMNDATALABELREQUEST.fields_by_name['datastore_id']._serialized_options = b'\372B\004r\002\020\001'
   _UPDATECOLUMNDATALABELREQUEST.fields_by_name['path']._options = None
@@ -116,108 +114,98 @@
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_DB']._serialized_end=1989
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_SCHEMA']._serialized_start=1992
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_SCHEMA']._serialized_end=2139
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_TABLE']._serialized_start=2142
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_TABLE']._serialized_end=2324
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_COLUMN']._serialized_start=2326
   _globals['_GETINVENTORYHIERARCHICALRESPONSE_COLUMN']._serialized_end=2405
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDREQUEST']._serialized_start=2407
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDREQUEST']._serialized_end=2478
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE']._serialized_start=2481
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE']._serialized_end=3458
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_DATASTORE']._serialized_start=2620
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_DATASTORE']._serialized_end=2773
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_DB']._serialized_start=2776
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_DB']._serialized_end=3024
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_SCHEMA']._serialized_start=3027
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_SCHEMA']._serialized_end=3183
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_TABLE']._serialized_start=3186
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_TABLE']._serialized_end=3377
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_COLUMN']._serialized_start=2326
-  _globals['_GETINVENTORYHIERARCHICALPAGINATEDRESPONSE_COLUMN']._serialized_end=2405
-  _globals['_GETINVENTORYFLATREQUEST']._serialized_start=3460
-  _globals['_GETINVENTORYFLATREQUEST']._serialized_end=3575
-  _globals['_COLUMN']._serialized_start=3578
-  _globals['_COLUMN']._serialized_end=4141
-  _globals['_DS']._serialized_start=4143
-  _globals['_DS']._serialized_end=4247
-  _globals['_DB']._serialized_start=4250
-  _globals['_DB']._serialized_end=4430
-  _globals['_SCHEMA']._serialized_start=4433
-  _globals['_SCHEMA']._serialized_end=4563
-  _globals['_TABLE']._serialized_start=4566
-  _globals['_TABLE']._serialized_end=4731
-  _globals['_SUBCOLUMN']._serialized_start=4734
-  _globals['_SUBCOLUMN']._serialized_end=5180
-  _globals['_INVENTORYOBJECT']._serialized_start=5183
-  _globals['_INVENTORYOBJECT']._serialized_end=5471
-  _globals['_GETINVENTORYFLATRESPONSE']._serialized_start=5474
-  _globals['_GETINVENTORYFLATRESPONSE']._serialized_end=5627
-  _globals['_UPDATECOLUMNLOCKSTATUSREQUEST']._serialized_start=5630
-  _globals['_UPDATECOLUMNLOCKSTATUSREQUEST']._serialized_end=5764
-  _globals['_UPDATECOLUMNLOCKSTATUSRESPONSE']._serialized_start=5766
-  _globals['_UPDATECOLUMNLOCKSTATUSRESPONSE']._serialized_end=5798
-  _globals['_UPDATECOLUMNDATALABELREQUEST']._serialized_start=5801
-  _globals['_UPDATECOLUMNDATALABELREQUEST']._serialized_end=5935
-  _globals['_UPDATECOLUMNDATALABELRESPONSE']._serialized_start=5937
-  _globals['_UPDATECOLUMNDATALABELRESPONSE']._serialized_end=5968
-  _globals['_CREATEINVENTORYOBJECTREQUEST']._serialized_start=5971
-  _globals['_CREATEINVENTORYOBJECTREQUEST']._serialized_end=6898
-  _globals['_CREATEINVENTORYOBJECTREQUEST_DB']._serialized_start=6476
-  _globals['_CREATEINVENTORYOBJECTREQUEST_DB']._serialized_end=6538
-  _globals['_CREATEINVENTORYOBJECTREQUEST_SCHEMA']._serialized_start=6540
-  _globals['_CREATEINVENTORYOBJECTREQUEST_SCHEMA']._serialized_end=6606
-  _globals['_CREATEINVENTORYOBJECTREQUEST_TABLE']._serialized_start=6608
-  _globals['_CREATEINVENTORYOBJECTREQUEST_TABLE']._serialized_end=6673
-  _globals['_CREATEINVENTORYOBJECTREQUEST_COLUMN']._serialized_start=6675
-  _globals['_CREATEINVENTORYOBJECTREQUEST_COLUMN']._serialized_end=6779
-  _globals['_CREATEINVENTORYOBJECTREQUEST_SUBCOLUMN']._serialized_start=6781
-  _globals['_CREATEINVENTORYOBJECTREQUEST_SUBCOLUMN']._serialized_end=6898
-  _globals['_CREATEINVENTORYOBJECTRESPONSE']._serialized_start=6900
-  _globals['_CREATEINVENTORYOBJECTRESPONSE']._serialized_end=6931
-  _globals['_DELETEINVENTORYOBJECTREQUEST']._serialized_start=6933
-  _globals['_DELETEINVENTORYOBJECTREQUEST']._serialized_end=7036
-  _globals['_DELETEINVENTORYOBJECTRESPONSE']._serialized_start=7038
-  _globals['_DELETEINVENTORYOBJECTRESPONSE']._serialized_end=7069
-  _globals['_TAG']._serialized_start=7071
-  _globals['_TAG']._serialized_end=7190
-  _globals['_CREATEINVENTORYTAGREQUEST']._serialized_start=7192
-  _globals['_CREATEINVENTORYTAGREQUEST']._serialized_end=7248
-  _globals['_CREATEINVENTORYTAGRESPONSE']._serialized_start=7250
-  _globals['_CREATEINVENTORYTAGRESPONSE']._serialized_end=7311
-  _globals['_GETINVENTORYTAGSREQUEST']._serialized_start=7313
-  _globals['_GETINVENTORYTAGSREQUEST']._serialized_end=7428
-  _globals['_GETINVENTORYTAGSRESPONSE']._serialized_start=7431
-  _globals['_GETINVENTORYTAGSRESPONSE']._serialized_end=7562
-  _globals['_UPDATEINVENTORYOBJECTTAGSREQUEST']._serialized_start=7564
-  _globals['_UPDATEINVENTORYOBJECTTAGSREQUEST']._serialized_end=7691
-  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE']._serialized_start=7694
-  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE']._serialized_end=8284
-  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE_INVENTORYOBJECT']._serialized_start=7817
-  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE_INVENTORYOBJECT']._serialized_end=8284
-  _globals['_DELETEINVENTORYTAGREQUEST']._serialized_start=8286
-  _globals['_DELETEINVENTORYTAGREQUEST']._serialized_end=8338
-  _globals['_DELETEINVENTORYTAGRESPONSE']._serialized_start=8340
-  _globals['_DELETEINVENTORYTAGRESPONSE']._serialized_end=8403
-  _globals['_CREATEDATADOMAINREQUEST']._serialized_start=8406
-  _globals['_CREATEDATADOMAINREQUEST']._serialized_end=8613
-  _globals['_CREATEDATADOMAINRESPONSE']._serialized_start=8615
-  _globals['_CREATEDATADOMAINRESPONSE']._serialized_end=8657
-  _globals['_GETDATADOMAINSREQUEST']._serialized_start=8659
-  _globals['_GETDATADOMAINSREQUEST']._serialized_end=8682
-  _globals['_GETDATADOMAINSRESPONSE']._serialized_start=8684
-  _globals['_GETDATADOMAINSRESPONSE']._serialized_end=8761
-  _globals['_GETDATADOMAINBYIDREQUEST']._serialized_start=8763
-  _globals['_GETDATADOMAINBYIDREQUEST']._serialized_end=8805
-  _globals['_GETDATADOMAINBYIDRESPONSE']._serialized_start=8807
-  _globals['_GETDATADOMAINBYIDRESPONSE']._serialized_end=8885
-  _globals['_UPDATEDATADOMAINREQUEST']._serialized_start=8888
-  _globals['_UPDATEDATADOMAINREQUEST']._serialized_end=9111
-  _globals['_UPDATEDATADOMAINRESPONSE']._serialized_start=9113
-  _globals['_UPDATEDATADOMAINRESPONSE']._serialized_end=9190
-  _globals['_DELETEDATADOMAINREQUEST']._serialized_start=9192
-  _globals['_DELETEDATADOMAINREQUEST']._serialized_end=9233
-  _globals['_DELETEDATADOMAINRESPONSE']._serialized_start=9235
-  _globals['_DELETEDATADOMAINRESPONSE']._serialized_end=9261
-  _globals['_INVENTORYSERVICE']._serialized_start=9264
-  _globals['_INVENTORYSERVICE']._serialized_end=11262
+  _globals['_GETINVENTORYREQUEST']._serialized_start=2408
+  _globals['_GETINVENTORYREQUEST']._serialized_end=2578
+  _globals['_GETINVENTORYRESPONSE']._serialized_start=2581
+  _globals['_GETINVENTORYRESPONSE']._serialized_end=2730
+  _globals['_GETINVENTORYFLATREQUEST']._serialized_start=2732
+  _globals['_GETINVENTORYFLATREQUEST']._serialized_end=2847
+  _globals['_COLUMN']._serialized_start=2850
+  _globals['_COLUMN']._serialized_end=3413
+  _globals['_DS']._serialized_start=3415
+  _globals['_DS']._serialized_end=3519
+  _globals['_DB']._serialized_start=3522
+  _globals['_DB']._serialized_end=3702
+  _globals['_SCHEMA']._serialized_start=3705
+  _globals['_SCHEMA']._serialized_end=3835
+  _globals['_TABLE']._serialized_start=3838
+  _globals['_TABLE']._serialized_end=4003
+  _globals['_SUBCOLUMN']._serialized_start=4006
+  _globals['_SUBCOLUMN']._serialized_end=4452
+  _globals['_INVENTORYOBJECT']._serialized_start=4455
+  _globals['_INVENTORYOBJECT']._serialized_end=4743
+  _globals['_GETINVENTORYFLATRESPONSE']._serialized_start=4746
+  _globals['_GETINVENTORYFLATRESPONSE']._serialized_end=4899
+  _globals['_UPDATECOLUMNLOCKSTATUSREQUEST']._serialized_start=4902
+  _globals['_UPDATECOLUMNLOCKSTATUSREQUEST']._serialized_end=5036
+  _globals['_UPDATECOLUMNLOCKSTATUSRESPONSE']._serialized_start=5038
+  _globals['_UPDATECOLUMNLOCKSTATUSRESPONSE']._serialized_end=5070
+  _globals['_UPDATECOLUMNDATALABELREQUEST']._serialized_start=5073
+  _globals['_UPDATECOLUMNDATALABELREQUEST']._serialized_end=5207
+  _globals['_UPDATECOLUMNDATALABELRESPONSE']._serialized_start=5209
+  _globals['_UPDATECOLUMNDATALABELRESPONSE']._serialized_end=5240
+  _globals['_CREATEINVENTORYOBJECTREQUEST']._serialized_start=5243
+  _globals['_CREATEINVENTORYOBJECTREQUEST']._serialized_end=6170
+  _globals['_CREATEINVENTORYOBJECTREQUEST_DB']._serialized_start=5748
+  _globals['_CREATEINVENTORYOBJECTREQUEST_DB']._serialized_end=5810
+  _globals['_CREATEINVENTORYOBJECTREQUEST_SCHEMA']._serialized_start=5812
+  _globals['_CREATEINVENTORYOBJECTREQUEST_SCHEMA']._serialized_end=5878
+  _globals['_CREATEINVENTORYOBJECTREQUEST_TABLE']._serialized_start=5880
+  _globals['_CREATEINVENTORYOBJECTREQUEST_TABLE']._serialized_end=5945
+  _globals['_CREATEINVENTORYOBJECTREQUEST_COLUMN']._serialized_start=5947
+  _globals['_CREATEINVENTORYOBJECTREQUEST_COLUMN']._serialized_end=6051
+  _globals['_CREATEINVENTORYOBJECTREQUEST_SUBCOLUMN']._serialized_start=6053
+  _globals['_CREATEINVENTORYOBJECTREQUEST_SUBCOLUMN']._serialized_end=6170
+  _globals['_CREATEINVENTORYOBJECTRESPONSE']._serialized_start=6172
+  _globals['_CREATEINVENTORYOBJECTRESPONSE']._serialized_end=6203
+  _globals['_DELETEINVENTORYOBJECTREQUEST']._serialized_start=6205
+  _globals['_DELETEINVENTORYOBJECTREQUEST']._serialized_end=6308
+  _globals['_DELETEINVENTORYOBJECTRESPONSE']._serialized_start=6310
+  _globals['_DELETEINVENTORYOBJECTRESPONSE']._serialized_end=6341
+  _globals['_TAG']._serialized_start=6343
+  _globals['_TAG']._serialized_end=6462
+  _globals['_CREATEINVENTORYTAGREQUEST']._serialized_start=6464
+  _globals['_CREATEINVENTORYTAGREQUEST']._serialized_end=6520
+  _globals['_CREATEINVENTORYTAGRESPONSE']._serialized_start=6522
+  _globals['_CREATEINVENTORYTAGRESPONSE']._serialized_end=6583
+  _globals['_GETINVENTORYTAGSREQUEST']._serialized_start=6585
+  _globals['_GETINVENTORYTAGSREQUEST']._serialized_end=6700
+  _globals['_GETINVENTORYTAGSRESPONSE']._serialized_start=6703
+  _globals['_GETINVENTORYTAGSRESPONSE']._serialized_end=6834
+  _globals['_UPDATEINVENTORYOBJECTTAGSREQUEST']._serialized_start=6836
+  _globals['_UPDATEINVENTORYOBJECTTAGSREQUEST']._serialized_end=6963
+  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE']._serialized_start=6966
+  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE']._serialized_end=7556
+  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE_INVENTORYOBJECT']._serialized_start=7089
+  _globals['_UPDATEINVENTORYOBJECTTAGSRESPONSE_INVENTORYOBJECT']._serialized_end=7556
+  _globals['_DELETEINVENTORYTAGREQUEST']._serialized_start=7558
+  _globals['_DELETEINVENTORYTAGREQUEST']._serialized_end=7610
+  _globals['_DELETEINVENTORYTAGRESPONSE']._serialized_start=7612
+  _globals['_DELETEINVENTORYTAGRESPONSE']._serialized_end=7675
+  _globals['_CREATEDATADOMAINREQUEST']._serialized_start=7678
+  _globals['_CREATEDATADOMAINREQUEST']._serialized_end=7885
+  _globals['_CREATEDATADOMAINRESPONSE']._serialized_start=7887
+  _globals['_CREATEDATADOMAINRESPONSE']._serialized_end=7929
+  _globals['_GETDATADOMAINSREQUEST']._serialized_start=7931
+  _globals['_GETDATADOMAINSREQUEST']._serialized_end=7954
+  _globals['_GETDATADOMAINSRESPONSE']._serialized_start=7956
+  _globals['_GETDATADOMAINSRESPONSE']._serialized_end=8033
+  _globals['_GETDATADOMAINBYIDREQUEST']._serialized_start=8035
+  _globals['_GETDATADOMAINBYIDREQUEST']._serialized_end=8077
+  _globals['_GETDATADOMAINBYIDRESPONSE']._serialized_start=8079
+  _globals['_GETDATADOMAINBYIDRESPONSE']._serialized_end=8157
+  _globals['_UPDATEDATADOMAINREQUEST']._serialized_start=8160
+  _globals['_UPDATEDATADOMAINREQUEST']._serialized_end=8383
+  _globals['_UPDATEDATADOMAINRESPONSE']._serialized_start=8385
+  _globals['_UPDATEDATADOMAINRESPONSE']._serialized_end=8462
+  _globals['_DELETEDATADOMAINREQUEST']._serialized_start=8464
+  _globals['_DELETEDATADOMAINREQUEST']._serialized_end=8505
+  _globals['_DELETEDATADOMAINRESPONSE']._serialized_start=8507
+  _globals['_DELETEDATADOMAINRESPONSE']._serialized_end=8533
+  _globals['_INVENTORYSERVICE']._serialized_start=8536
+  _globals['_INVENTORYSERVICE']._serialized_end=10470
 # @@protoc_insertion_point(module_scope)
```

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -152,82 +152,37 @@
         name: str
         table_path: str
         def __init__(self, path: _Optional[str] = ..., name: _Optional[str] = ..., table_path: _Optional[str] = ...) -> None: ...
     INVENTORY_FIELD_NUMBER: _ClassVar[int]
     inventory: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalResponse.Datastore]
     def __init__(self, inventory: _Optional[_Iterable[_Union[GetInventoryHierarchicalResponse.Datastore, _Mapping]]] = ...) -> None: ...
 
-class GetInventoryHierarchicalPaginatedRequest(_message.Message):
-    __slots__ = ["path"]
+class GetInventoryRequest(_message.Message):
+    __slots__ = ["limit", "after", "before", "order", "path", "excluded_paths"]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    AFTER_FIELD_NUMBER: _ClassVar[int]
+    BEFORE_FIELD_NUMBER: _ClassVar[int]
+    ORDER_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
+    EXCLUDED_PATHS_FIELD_NUMBER: _ClassVar[int]
+    limit: int
+    after: str
+    before: str
+    order: str
     path: str
-    def __init__(self, path: _Optional[str] = ...) -> None: ...
+    excluded_paths: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, limit: _Optional[int] = ..., after: _Optional[str] = ..., before: _Optional[str] = ..., order: _Optional[str] = ..., path: _Optional[str] = ..., excluded_paths: _Optional[_Iterable[str]] = ...) -> None: ...
 
-class GetInventoryHierarchicalPaginatedResponse(_message.Message):
-    __slots__ = ["inventory"]
-    class Datastore(_message.Message):
-        __slots__ = ["id", "name", "technology", "dbs"]
-        ID_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        TECHNOLOGY_FIELD_NUMBER: _ClassVar[int]
-        DBS_FIELD_NUMBER: _ClassVar[int]
-        id: str
-        name: str
-        technology: str
-        dbs: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Db]
-        def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., technology: _Optional[str] = ..., dbs: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Db, _Mapping]]] = ...) -> None: ...
-    class Db(_message.Message):
-        __slots__ = ["path", "name", "datastore_id", "schemas", "tables"]
-        PATH_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        DATASTORE_ID_FIELD_NUMBER: _ClassVar[int]
-        SCHEMAS_FIELD_NUMBER: _ClassVar[int]
-        TABLES_FIELD_NUMBER: _ClassVar[int]
-        path: str
-        name: str
-        datastore_id: str
-        schemas: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Schema]
-        tables: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Table]
-        def __init__(self, path: _Optional[str] = ..., name: _Optional[str] = ..., datastore_id: _Optional[str] = ..., schemas: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Schema, _Mapping]]] = ..., tables: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Table, _Mapping]]] = ...) -> None: ...
-    class Schema(_message.Message):
-        __slots__ = ["path", "name", "db_path", "tables"]
-        PATH_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        DB_PATH_FIELD_NUMBER: _ClassVar[int]
-        TABLES_FIELD_NUMBER: _ClassVar[int]
-        path: str
-        name: str
-        db_path: str
-        tables: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Table]
-        def __init__(self, path: _Optional[str] = ..., name: _Optional[str] = ..., db_path: _Optional[str] = ..., tables: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Table, _Mapping]]] = ...) -> None: ...
-    class Table(_message.Message):
-        __slots__ = ["path", "name", "db_path", "schema_path", "columns"]
-        PATH_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        DB_PATH_FIELD_NUMBER: _ClassVar[int]
-        SCHEMA_PATH_FIELD_NUMBER: _ClassVar[int]
-        COLUMNS_FIELD_NUMBER: _ClassVar[int]
-        path: str
-        name: str
-        db_path: str
-        schema_path: str
-        columns: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Column]
-        def __init__(self, path: _Optional[str] = ..., name: _Optional[str] = ..., db_path: _Optional[str] = ..., schema_path: _Optional[str] = ..., columns: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Column, _Mapping]]] = ...) -> None: ...
-    class Column(_message.Message):
-        __slots__ = ["path", "name", "table_path"]
-        PATH_FIELD_NUMBER: _ClassVar[int]
-        NAME_FIELD_NUMBER: _ClassVar[int]
-        TABLE_PATH_FIELD_NUMBER: _ClassVar[int]
-        path: str
-        name: str
-        table_path: str
-        def __init__(self, path: _Optional[str] = ..., name: _Optional[str] = ..., table_path: _Optional[str] = ...) -> None: ...
+class GetInventoryResponse(_message.Message):
+    __slots__ = ["inventory", "list_metadata"]
     INVENTORY_FIELD_NUMBER: _ClassVar[int]
-    inventory: _containers.RepeatedCompositeFieldContainer[GetInventoryHierarchicalPaginatedResponse.Datastore]
-    def __init__(self, inventory: _Optional[_Iterable[_Union[GetInventoryHierarchicalPaginatedResponse.Datastore, _Mapping]]] = ...) -> None: ...
+    LIST_METADATA_FIELD_NUMBER: _ClassVar[int]
+    inventory: _containers.RepeatedCompositeFieldContainer[InventoryObject]
+    list_metadata: _list_metadata_pb2.ListMetadata
+    def __init__(self, inventory: _Optional[_Iterable[_Union[InventoryObject, _Mapping]]] = ..., list_metadata: _Optional[_Union[_list_metadata_pb2.ListMetadata, _Mapping]] = ...) -> None: ...
 
 class GetInventoryFlatRequest(_message.Message):
     __slots__ = ["limit", "after", "before", "order"]
     LIMIT_FIELD_NUMBER: _ClassVar[int]
     AFTER_FIELD_NUMBER: _ClassVar[int]
     BEFORE_FIELD_NUMBER: _ClassVar[int]
     ORDER_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/inventory_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
             channel: A grpc.Channel.
         """
         self.GetInventoryHierarchical = channel.unary_unary(
                 '/admin.v1.InventoryService/GetInventoryHierarchical',
                 request_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalRequest.SerializeToString,
                 response_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalResponse.FromString,
                 )
-        self.GetInventoryHierarchicalPaginated = channel.unary_unary(
-                '/admin.v1.InventoryService/GetInventoryHierarchicalPaginated',
-                request_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedRequest.SerializeToString,
-                response_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedResponse.FromString,
+        self.GetInventory = channel.unary_unary(
+                '/admin.v1.InventoryService/GetInventory',
+                request_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryRequest.SerializeToString,
+                response_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryResponse.FromString,
                 )
         self.GetInventoryFlat = channel.unary_unary(
                 '/admin.v1.InventoryService/GetInventoryFlat',
                 request_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryFlatRequest.SerializeToString,
                 response_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryFlatResponse.FromString,
                 )
         self.GetInventoryFlatOld = channel.unary_unary(
@@ -116,15 +116,15 @@
 
     def GetInventoryHierarchical(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetInventoryHierarchicalPaginated(self, request, context):
+    def GetInventory(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetInventoryFlat(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -232,18 +232,18 @@
 def add_InventoryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetInventoryHierarchical': grpc.unary_unary_rpc_method_handler(
                     servicer.GetInventoryHierarchical,
                     request_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalRequest.FromString,
                     response_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalResponse.SerializeToString,
             ),
-            'GetInventoryHierarchicalPaginated': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetInventoryHierarchicalPaginated,
-                    request_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedRequest.FromString,
-                    response_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedResponse.SerializeToString,
+            'GetInventory': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetInventory,
+                    request_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryRequest.FromString,
+                    response_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryResponse.SerializeToString,
             ),
             'GetInventoryFlat': grpc.unary_unary_rpc_method_handler(
                     servicer.GetInventoryFlat,
                     request_deserializer=admin_dot_v1_dot_inventory__pb2.GetInventoryFlatRequest.FromString,
                     response_serializer=admin_dot_v1_dot_inventory__pb2.GetInventoryFlatResponse.SerializeToString,
             ),
             'GetInventoryFlatOld': grpc.unary_unary_rpc_method_handler(
@@ -350,27 +350,27 @@
         return grpc.experimental.unary_unary(request, target, '/admin.v1.InventoryService/GetInventoryHierarchical',
             admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalRequest.SerializeToString,
             admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetInventoryHierarchicalPaginated(request,
+    def GetInventory(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/admin.v1.InventoryService/GetInventoryHierarchicalPaginated',
-            admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedRequest.SerializeToString,
-            admin_dot_v1_dot_inventory__pb2.GetInventoryHierarchicalPaginatedResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/admin.v1.InventoryService/GetInventory',
+            admin_dot_v1_dot_inventory__pb2.GetInventoryRequest.SerializeToString,
+            admin_dot_v1_dot_inventory__pb2.GetInventoryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetInventoryFlat(request,
             target,
             options=(),
```

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/metrics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/native_user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/outputs_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/policies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/registry_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/satellite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/search_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/sidecar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/coderepo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/column_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/datahub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/domain_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/external_id_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/flat_dataplane_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/github_repository_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/group_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/incident_account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/integration_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/list_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_link_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/organization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/policy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/satellite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/search_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_link_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/sidecar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/types/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/admin/v1/work_os_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/validate_pb2.py` & `formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/gen/validate/v1/validate_pb2.pyi` & `formal-sdk-1.0.8/src/formal_sdk/gen/validate/v1/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/identities.py` & `formal-sdk-1.0.8/src/formal_sdk/identities.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_app.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_app.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_cloud.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_cloud.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_code_repository.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_code_repository.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_datahub.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_datahub.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_external_api.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_external_api.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_github.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_github.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_incident.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_incident.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_kms.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_kms.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_log.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_log.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_slack.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_slack.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/integration_sso.py` & `formal-sdk-1.0.8/src/formal_sdk/integration_sso.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/inventory.py` & `formal-sdk-1.0.8/src/formal_sdk/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 	GetInventoryFlatOldResponse,
 	UpdateColumnFieldEncryptionRequest,
 	UpdateColumnFieldEncryptionResponse,
 	GetInventoryObjectRequest,
 	GetInventoryObjectResponse,
 	GetInventoryHierarchicalRequest,
 	GetInventoryHierarchicalResponse,
-	GetInventoryHierarchicalPaginatedRequest,
-	GetInventoryHierarchicalPaginatedResponse,
+	GetInventoryRequest,
+	GetInventoryResponse,
 	GetInventoryFlatRequest,
 	Column,
 	Ds,
 	Db,
 	Schema,
 	Table,
 	SubColumn,
@@ -58,16 +58,16 @@
 		self.channel = grpc.secure_channel(self.base_url, grpc.ssl_channel_credentials())
 		self.stub = InventoryServiceStub(self.channel)
 		self.headers = [('x-api-key', token)]
 
 	def GetInventoryHierarchical(self, request: GetInventoryHierarchicalRequest) -> GetInventoryHierarchicalResponse:
 		return self.stub.GetInventoryHierarchical(request, metadata=self.headers)
 
-	def GetInventoryHierarchicalPaginated(self, request: GetInventoryHierarchicalPaginatedRequest) -> GetInventoryHierarchicalPaginatedResponse:
-		return self.stub.GetInventoryHierarchicalPaginated(request, metadata=self.headers)
+	def GetInventory(self, request: GetInventoryRequest) -> GetInventoryResponse:
+		return self.stub.GetInventory(request, metadata=self.headers)
 
 	def GetInventoryFlat(self, request: GetInventoryFlatRequest) -> GetInventoryFlatResponse:
 		return self.stub.GetInventoryFlat(request, metadata=self.headers)
 
 	def GetInventoryFlatOld(self, request: GetInventoryFlatOldRequest) -> GetInventoryFlatOldResponse:
 		return self.stub.GetInventoryFlatOld(request, metadata=self.headers)
```

### Comparing `formal-sdk-1.0.7/src/formal_sdk/metrics.py` & `formal-sdk-1.0.8/src/formal_sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/native_user.py` & `formal-sdk-1.0.8/src/formal_sdk/native_user.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/outputs.py` & `formal-sdk-1.0.8/src/formal_sdk/outputs.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/policies.py` & `formal-sdk-1.0.8/src/formal_sdk/policies.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/registry.py` & `formal-sdk-1.0.8/src/formal_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/satellite.py` & `formal-sdk-1.0.8/src/formal_sdk/satellite.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/search.py` & `formal-sdk-1.0.8/src/formal_sdk/search.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/sidecar.py` & `formal-sdk-1.0.8/src/formal_sdk/sidecar.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk/work_os.py` & `formal-sdk-1.0.8/src/formal_sdk/work_os.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-1.0.7/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-1.0.8/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-1.0.7/src/formal_sdk.egg-info/SOURCES.txt` & `formal-sdk-1.0.8/src/formal_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

