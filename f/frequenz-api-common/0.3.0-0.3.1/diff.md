# Comparing `tmp/frequenz-api-common-0.3.0.tar.gz` & `tmp/frequenz-api-common-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-common-0.3.0.tar", last modified: Tue Jun  6 09:33:28 2023, max compression
+gzip compressed data, was "frequenz-api-common-0.3.1.tar", last modified: Tue Aug  8 14:31:32 2023, max compression
```

## Comparing `frequenz-api-common-0.3.0.tar` & `frequenz-api-common-0.3.1.tar`

### file list

```diff
@@ -1,103 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.612018 frequenz-api-common-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 09:33:28.612018 frequenz-api-common-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/.cookiecutter-replay.json
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     5450 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1886 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)    57278 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/mkdocstrings_autoapi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2920 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     3557 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/proto/frequenz/api/common/components.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/proto/frequenz/api/common/location.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.642884 frequenz-api-common-0.3.1/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/py/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/py/frequenz/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/py/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/py/frequenz/api/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/py/frequenz/api/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1886 2023-08-08 14:31:32.000000 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-08-08 14:31:32.000000 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 14:31:32.000000 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-08-08 14:31:32.000000 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-08-08 14:31:32.000000 frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-08-08 14:31:11.000000 frequenz-api-common-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 14:31:32.646884 frequenz-api-common-0.3.1/setup.cfg
```

### Comparing `frequenz-api-common-0.3.0/LICENSE` & `frequenz-api-common-0.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Frequenz Energy-as-a-Service GmbH
+Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `frequenz-api-common-0.3.0/PKG-INFO` & `frequenz-api-common-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.3.0
+Version: 0.3.1
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
-Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
+Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
-Keywords: frequenz,api,microgrid,grpc,common
+Keywords: frequenz,python,api,grpc,protobuf,rpc,common
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev-docstrings
 Provides-Extra: dev-formatting
+Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
 Provides-Extra: dev
 License-File: LICENSE
 
-# frequenz-api-common
-Common definitions for frequenz GRPC APIs
+# Frequenz Common API
+
+[![Build Status](https://github.com/frequenz-floss/frequenz-api-common/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-api-common/actions/workflows/ci.yaml)
+[![PyPI Package](https://img.shields.io/pypi/v/frequenz-api-common)](https://pypi.org/project/frequenz-api-common/)
+[![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-api-common/)
+
+## Introduction
+
+Frequenz common gRPC API and bindings
+
+## Contributing
+
+If you want to know how to build this project and contribute to it, please
+check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-api-common-0.3.0/proto/frequenz/api/common/components.proto` & `frequenz-api-common-0.3.1/proto/frequenz/api/common/components.proto`

 * *Files 26% similar despite different names*

```diff
@@ -41,14 +41,29 @@
   COMPONENT_CATEGORY_CRYPTO_MINER = 8;
 
   // An electrolyzer for converting water into hydrogen and oxygen.
   COMPONENT_CATEGORY_ELECTROLYZER = 9;
 
   // A heat and power combustion plant (CHP stands for combined heat and power).
   COMPONENT_CATEGORY_CHP = 10;
+
+  // A relay.
+  // Relays generally have two states: open (connected) and closed
+  // (disconnected).
+  // They are generally placed in front of a component, e.g., an inverter, to
+  // control whether the component is connected to the grid or not.
+  COMPONENT_CATEGORY_RELAY = 11;
+
+  // A precharge module.
+  // Precharging involves gradually ramping up the DC voltage to prevent any
+  // potential damage to sensitive electrical components like capacitors.
+  // While many inverters and batteries come equipped with in-built precharging
+  // mechanisms, some may lack this feature. In such cases, we need to use
+  // external precharging modules.
+  COMPONENT_CATEGORY_PRECHARGE_MODULE = 12;
 }
 
 // Enumerated battery types.
 enum BatteryType {
   // Unspecified.
   BATTERY_TYPE_UNSPECIFIED = 0;
```

### Comparing `frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-common-0.3.1/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics.proto` & `frequenz-api-common-0.3.1/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/PKG-INFO` & `frequenz-api-common-0.3.1/py/frequenz_api_common.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.3.0
+Version: 0.3.1
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
-Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
+Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
-Keywords: frequenz,api,microgrid,grpc,common
+Keywords: frequenz,python,api,grpc,protobuf,rpc,common
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev-docstrings
 Provides-Extra: dev-formatting
+Provides-Extra: dev-mkdocs
 Provides-Extra: dev-mypy
 Provides-Extra: dev-noxfile
 Provides-Extra: dev-pylint
 Provides-Extra: dev-pytest
 Provides-Extra: dev
 License-File: LICENSE
 
-# frequenz-api-common
-Common definitions for frequenz GRPC APIs
+# Frequenz Common API
+
+[![Build Status](https://github.com/frequenz-floss/frequenz-api-common/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-api-common/actions/workflows/ci.yaml)
+[![PyPI Package](https://img.shields.io/pypi/v/frequenz-api-common)](https://pypi.org/project/frequenz-api-common/)
+[![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-api-common/)
+
+## Introduction
+
+Frequenz common gRPC API and bindings
+
+## Contributing
+
+If you want to know how to build this project and contribute to it, please
+check out the [Contributing Guide](CONTRIBUTING.md).
```

### Comparing `frequenz-api-common-0.3.0/pyproject.toml` & `frequenz-api-common-0.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,115 @@
+# License: MIT
+# Copyright © 2023 Frequenz Energy-as-a-Service GmbH
+
 [build-system]
 requires = [
   "setuptools == 67.7.2",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[api] == 0.2.0",
+  "frequenz-repo-config[api] == 0.4.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-api-common"
 description = "Frequenz common gRPC API and bindings"
 readme = "README.md"
 license = { text = "MIT" }
-keywords = ["frequenz", "api", "microgrid", "grpc", "common"]
+keywords = ["frequenz", "python", "api", "grpc", "protobuf", "rpc", "common"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
+  "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
   "googleapis-common-protos >= 1.56.2, < 2",
   "grpcio >= 1.51.1, < 2",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
-dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
-dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
+dev-docstrings = [
+  "pydocstyle == 6.3.0",
+  "darglint == 1.8.1",
+  "tomli == 2.0.1",      # Needed by pydocstyle to read pyproject.toml
+]
+dev-formatting = ["black == 23.7.0", "isort == 5.12.0"]
+dev-mkdocs = [
+  "mike == 1.1.2",
+  "mkdocs-gen-files == 0.5.0",
+  "mkdocs-literate-nav == 0.6.0",
+  "mkdocs-material == 9.1.21",
+  "mkdocs-section-index == 0.3.5",
+  "mkdocstrings[python] == 0.22.0",
+  "frequenz-repo-config[api] == 0.4.0",
+]
 dev-mypy = [
-  "mypy == 1.3.0",
-  # For checking the noxfile and tests
-  "frequenz-api-common[dev-noxfile,dev-pytest]",
+  "mypy == 1.4.1",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[api] == 0.2.0"]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[api] == 0.4.0"]
 dev-pylint = [
-  "pylint == 2.17.4",
-  # For checking the noxfile and tests
-  "frequenz-api-common[dev-noxfile,dev-pytest]",
+  "pylint == 2.17.5",
+  # For checking the noxfile, docs/ script, and tests
+  "frequenz-api-common[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-pytest = ["pytest == 7.3.1"]
+dev-pytest = ["pytest == 7.4.0"]
 dev = [
-  "frequenz-api-common[dev-docstrings,dev-formatting,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
+  "frequenz-api-common[dev-mkdocs,dev-docstrings,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-api-common/releases"
-Repository = "https://github.com/frequenz-floss/frequenz-api-common"
 Issues = "https://github.com/frequenz-floss/frequenz-api-common/issues"
+Repository = "https://github.com/frequenz-floss/frequenz-api-common"
 Support = "https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support"
 
+[tool.black]
+line-length = 88
+target-version = ['py311']
+
+[tool.isort]
+profile = "black"
+line_length = 88
+src_paths = ["benchmarks", "examples", "src", "tests"]
+
+[tool.frequenz-repo-config.protobuf]
+include_paths = ["submodules/api-common-protos"]
+
+[tool.pylint.similarities]
+ignore-comments = ['yes']
+ignore-docstrings = ['yes']
+ignore-imports = ['no']
+min-similarity-lines = 40
+
+[tool.pylint.messages_control]
+disable = [
+  "too-few-public-methods",
+  # disabled because it conflicts with isort
+  "wrong-import-order",
+  "ungrouped-imports",
+  # pylint's unsubscriptable check is buggy and is not needed because
+  # it is a type-check, for which we already have mypy.
+  "unsubscriptable-object",
+]
+
+[tool.pytest.ini_options]
+testpaths = ["pytests"]
+
 [tool.setuptools.package-dir]
 "" = "py"
 
 [tool.setuptools.package-data]
 "*" = ["*.pyi"]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
-
-[tools.pytest.ini_options]
-testpaths = ["pytests"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

