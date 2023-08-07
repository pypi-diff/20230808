# Comparing `tmp/modelaapi-0.6.236.tar.gz` & `tmp/modelaapi-0.6.238.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.236.tar", last modified: Mon Aug  7 20:54:48 2023, max compression
+gzip compressed data, was "modelaapi-0.6.238.tar", last modified: Mon Aug  7 22:23:49 2023, max compression
```

## Comparing `modelaapi-0.6.236.tar` & `modelaapi-0.6.238.tar`

### file list

```diff
@@ -1,581 +1,581 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.528544 modelaapi-0.6.236/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.236/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.236/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.236/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.236/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.236/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.236/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 20:54:48.528544 modelaapi-0.6.236/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.236/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    55414 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    97242 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.496544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    61593 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    65270 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   104658 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11708 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7194 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    20179 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.500543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.484543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.484543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.504543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.484543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.508544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.512544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.516543 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-07 20:54:39.000000 modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/annotations_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/http_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/apps/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/apps/v1/generated_pb2.pyi
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.520544 modelaapi-0.6.236/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/core/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/api/rbac/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.488543 modelaapi-0.6.236/k8s/io/apps/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/apps/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.488543 modelaapi-0.6.236/k8s/io/core/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/k8s/io/pkg/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.488543 modelaapi-0.6.236/k8s/io/pkg/api/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/k8s/io/pkg/apis/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/k8s/io/pkg/apis/meta/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/k8s/io/pkg/util/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.492543 modelaapi-0.6.236/k8s/io/rbac/
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/k8s/io/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 20:54:39.000000 modelaapi-0.6.236/k8s/io/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.524544 modelaapi-0.6.236/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.236/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.236/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.236/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.236/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.236/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-07 20:54:46.000000 modelaapi-0.6.236/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 20:54:48.528544 modelaapi-0.6.236/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.236/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-07 20:54:48.000000 modelaapi-0.6.236/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.236/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-07 20:54:48.528544 modelaapi-0.6.236/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.236/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.238/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.238/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.238/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.238/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.238/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.238/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 22:23:49.774961 modelaapi-0.6.238/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.238/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24765 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    41839 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    52674 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    91844 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.730960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    55414 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    97242 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.734960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12353 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17866 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11572 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7286 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20675 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    61485 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    65084 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   104658 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.738960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11708 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7194 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20179 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9651 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5903 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.742960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.746960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.722960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.722960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.750960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.722960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.754960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.758960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.762961 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.766960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-08-07 22:23:28.000000 modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/annotations_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/http_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/apps/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/apps/v1/generated_pb2.pyi
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/core/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/api/rbac/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.770960 modelaapi-0.6.238/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/apps/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/apps/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/core/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/pkg/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/pkg/api/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/pkg/apis/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/pkg/apis/meta/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/pkg/util/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.726960 modelaapi-0.6.238/k8s/io/rbac/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/k8s/io/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-08-07 22:23:28.000000 modelaapi-0.6.238/k8s/io/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.238/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.238/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.238/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.238/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.238/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-08-07 22:23:41.000000 modelaapi-0.6.238/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-08-07 22:23:49.774961 modelaapi-0.6.238/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.238/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-08-07 22:23:49.000000 modelaapi-0.6.238/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.238/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-08-07 22:23:49.774961 modelaapi-0.6.238/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.238/setup.py
```

### Comparing `modelaapi-0.6.236/CONTRIBUTING.rst` & `modelaapi-0.6.238/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/LICENSE.txt` & `modelaapi-0.6.238/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/Makefile` & `modelaapi-0.6.238/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/PKG-INFO` & `modelaapi-0.6.238/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.236
+Version: 0.6.238
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.236
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.238
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.236
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.238
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.236/README.md` & `modelaapi-0.6.238/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi` & `modelaapi-0.6.238/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=github.com/metaprov/modelaapi/services/common/v1/common.proto\x12\x30github.com.metaprov.modelaapi.services.common.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xe2\x03\n\x0e\x44\x61tasetProfile\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x0c\n\x04rows\x18\x02 \x01(\x05\x12\x10\n\x08\x66ilesize\x18\x03 \x01(\x05\x12\x11\n\timbalance\x18\x04 \x01(\x08\x12\x45\n\x05plots\x18\x05 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12P\n\x07\x63olumns\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.services.common.v1.ColumnProfile\x12J\n\x05table\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x0c\n\x04hash\x18\x08 \x01(\t\x12K\n\x06groups\x18\n \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12O\n\x02ts\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.services.common.v1.TimeSeriesProfile\"\xc1\x06\n\x0cModelProfile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x45\n\x05plots\x18\x02 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12\x62\n\nimportance\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.common.v1.ModelProfile.ImportanceEntry\x12J\n\x06rocauc\x18\x04 \x01(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.ROCCurve\x12R\n\x02pr\x18\x05 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.services.common.v1.PrecisionRecallCurve\x12T\n\x10multiclassRocAuc\x18\x06 \x03(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.ROCCurve\x12\\\n\x0cmulticlassPR\x18\x07 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.services.common.v1.PrecisionRecallCurve\x12U\n\x04\x61lgs\x18\x08 \x03(\x0b\x32G.github.com.metaprov.modelaapi.services.common.v1.ForecastingAlgProfile\x12M\n\x08\x66\x65\x61tures\x18\n \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12K\n\x06groups\x18\x0b \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x1a\x31\n\x0fImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x95\x05\n\x15\x46orecastingAlgProfile\x12\x11\n\talgorithm\x18\x01 \x01(\t\x12K\n\x06series\x18\x02 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12L\n\x08timeStat\x18\x03 \x01(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.TimeStat\x12N\n\tvalueStat\x18\x04 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12G\n\x02\x63v\x18\x05 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12M\n\x08\x66orecast\x18\x06 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12L\n\x07metrics\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12Q\n\x0c\x63hangePoints\x18\x08 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x45\n\x05plots\x18\n \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\xa4\x02\n\x08TimeStat\x12I\n\x04gaps\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x18\n\x10\x61\x64\x64\x65\x64_timepoints\x18\x02 \x01(\x05\x12\x1a\n\x12\x64ropped_timepoints\x18\x03 \x01(\x05\x12\x13\n\x0b\x64\x61ta_points\x18\x04 \x01(\x05\x12\x1c\n\x14mean_increments_secs\x18\x05 \x01(\x02\x12\x31\n\rmin_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rmax_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\\\n\x08ROCCurve\x12\x11\n\tclassname\x18\x01 \x01(\t\x12\x0f\n\x07\x63lassid\x18\x02 \x01(\x05\x12\x0b\n\x03\x66pr\x18\x03 \x03(\x01\x12\x0b\n\x03tpr\x18\x04 \x03(\x01\x12\x12\n\nthresholds\x18\x05 \x03(\x01\"q\n\x14PrecisionRecallCurve\x12\x11\n\tclassname\x18\x01 \x01(\t\x12\x0f\n\x07\x63lassid\x18\x02 \x01(\x05\x12\x11\n\tprecision\x18\x03 \x03(\x01\x12\x0e\n\x06recall\x18\x04 \x03(\x01\x12\x12\n\nthresholds\x18\x05 \x03(\x01\"\x9a\x06\n\x11TimeSeriesProfile\x12\x44\n\x04kpss\x18\x01 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.KPSS\x12\x42\n\x03\x61\x64\x66\x18\x02 \x01(\x0b\x32\x35.github.com.metaprov.modelaapi.services.common.v1.ADF\x12L\n\x05zivot\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.services.common.v1.ZivotAndrew\x12N\n\x07kendall\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.services.common.v1.MannKendall\x12J\n\x02\x64w\x18\x05 \x01(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.DurbinWatson\x12\x0b\n\x03key\x18\x06 \x01(\t\x12K\n\x06series\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12N\n\tvalueStat\x18\x08 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12Q\n\x0c\x66\x65\x61turesView\x18\t \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x63\n\x08\x66\x65\x61tures\x18\n \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.common.v1.TimeSeriesProfile.FeaturesEntry\x1a/\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xb4\x01\n\x04KPSS\x12\x11\n\tkpss_stat\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12\x0c\n\x04lags\x18\x03 \x01(\x02\x12N\n\x04\x63rit\x18\x04 \x03(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.KPSS.CritEntry\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xbd\x01\n\x03\x41\x44\x46\x12\x0b\n\x03\x61\x64\x66\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12\x0f\n\x07usedlag\x18\x03 \x01(\x05\x12\x0c\n\x04nobs\x18\x04 \x01(\x05\x12M\n\x04\x63rit\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.services.common.v1.ADF.CritEntry\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xd1\x01\n\x0bZivotAndrew\x12\x0e\n\x06zastat\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12U\n\x04\x63rit\x18\x03 \x03(\x0b\x32G.github.com.metaprov.modelaapi.services.common.v1.ZivotAndrew.CritEntry\x12\x0f\n\x07\x62\x61selag\x18\x04 \x01(\x05\x12\r\n\x05\x62pidx\x18\x05 \x01(\x05\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x86\x01\n\x0bMannKendall\x12\r\n\x05trend\x18\x01 \x01(\t\x12\t\n\x01h\x18\x02 \x01(\x02\x12\t\n\x01p\x18\x03 \x01(\x02\x12\t\n\x01z\x18\x04 \x01(\x02\x12\x0b\n\x03tau\x18\x05 \x01(\x02\x12\t\n\x01s\x18\x06 \x01(\x02\x12\r\n\x05var_s\x18\x07 \x01(\x02\x12\r\n\x05slope\x18\x08 \x01(\x02\x12\x11\n\tintercept\x18\t \x01(\x02\"\x1a\n\x0c\x44urbinWatson\x12\n\n\x02\x64w\x18\x01 \x01(\x02\"f\n\x0f\x46orecastProfile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x45\n\x05plots\x18\x02 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\xe8\x01\n\x0cStudyProfile\x12\x45\n\x05plots\x18\x01 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12N\n\x06models\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.ModelProfile\x12\x14\n\x0ctrainingHash\x18\x03 \x01(\t\x12\x13\n\x0btestingHash\x18\x04 \x01(\t\x12\x16\n\x0evalidationHash\x18\x05 \x01(\t\"L\n\x04Plot\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0b\n\x03img\x18\x03 \x01(\x0c\x12\r\n\x05\x66name\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\"\xd3\x07\n\rColumnProfile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x05\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x16\n\x0epercentMissing\x18\x05 \x01(\x02\x12\x10\n\x08\x64istinct\x18\x06 \x01(\x05\x12\x0c\n\x04mean\x18\x07 \x01(\x01\x12\x0c\n\x04mode\x18\x08 \x01(\t\x12\x0e\n\x06stddev\x18\t \x01(\x01\x12\x10\n\x08variance\x18\n \x01(\x01\x12\x0b\n\x03min\x18\x0b \x01(\x01\x12\x0b\n\x03max\x18\x0c \x01(\x01\x12\x10\n\x08kurtosis\x18\r \x01(\x01\x12\x10\n\x08skewness\x18\x0e \x01(\x01\x12\x0b\n\x03sum\x18\x0f \x01(\x01\x12\x0b\n\x03mad\x18\x10 \x01(\x01\x12\r\n\x05zeros\x18\x11 \x01(\x01\x12\x0b\n\x03p25\x18\x12 \x01(\x01\x12\x0b\n\x03p50\x18\x13 \x01(\x01\x12\x0b\n\x03p75\x18\x14 \x01(\x01\x12\x0c\n\x04p100\x18\x15 \x01(\x01\x12\x0b\n\x03iqr\x18\x16 \x01(\x01\x12\n\n\x02\x63v\x18\x17 \x01(\x01\x12\x0b\n\x03top\x18\x18 \x01(\x05\x12\x0c\n\x04\x66req\x18\x19 \x01(\x05\x12\x0e\n\x06ignore\x18\x1a \x01(\x08\x12\x0e\n\x06target\x18\x1b \x01(\x08\x12N\n\thistogram\x18\x1c \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.Histogram\x12\x0f\n\x07invalid\x18\x1d \x01(\x05\x12\x12\n\nimportance\x18\x1e \x01(\x01\x12\x10\n\x08nullable\x18\x1f \x01(\x08\x12\x17\n\x0fhighCardinality\x18  \x01(\x08\x12!\n\x19highCorrWithOtherFeatures\x18! \x01(\x08\x12\x19\n\x11lowCorrWithTarget\x18\" \x01(\x08\x12\x16\n\x0ehighMissingPct\x18# \x01(\x08\x12\x0e\n\x06skewed\x18$ \x01(\x08\x12\n\n\x02id\x18% \x01(\x08\x12\x10\n\x08\x63onstant\x18& \x01(\x08\x12\x11\n\tduplicate\x18\' \x01(\x08\x12\x10\n\x08reserved\x18( \x01(\x08\x12\x15\n\routliersUpper\x18) \x01(\x05\x12\x15\n\routliersLower\x18* \x01(\x05\x12\x17\n\x0foutliersPercent\x18+ \x01(\x02\x12\x14\n\x0c\x63ompleteness\x18, \x01(\x01\x12\x1a\n\x12\x64istinctValueCount\x18- \x01(\x01\x12\x1b\n\x13mostFreqValuesRatio\x18. \x01(\x01\x12\x1a\n\x12indexOfPeculiarity\x18/ \x01(\x01\x12\x0e\n\x06values\x18\x30 \x03(\t\x12\x14\n\x0c\x63orrToTarget\x18\x31 \x01(\x01\x12\r\n\x05index\x18\x32 \x01(\x05\"=\n\tHistogram\x12\x0e\n\x06values\x18\x01 \x03(\x01\x12\x0c\n\x04\x62ins\x18\x02 \x03(\x01\x12\x12\n\ncategories\x18\x03 \x03(\t\"\xf6\x02\n\rNamespaceInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.github.com.metaprov.modelaapi.services.common.v1.NamespaceInfo.NamespaceType\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08\x61\x63\x63ounts\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uckets\x18\x04 \x01(\x05\x12\x0c\n\x04labs\x18\x05 \x01(\x05\x12\x14\n\x0cservingsites\x18\x06 \x01(\x05\x12\x10\n\x08\x64\x61tasets\x18\x07 \x01(\x05\x12\x13\n\x0b\x64\x61tasources\x18\x08 \x01(\x05\x12\x0f\n\x07studies\x18\t \x01(\x05\x12\x0e\n\x06models\x18\n \x01(\x05\"k\n\rNamespaceType\x12\n\n\x06TENANT\x10\x00\x12\x0f\n\x0b\x44\x41TAPRODUCT\x10\x01\x12\x07\n\x03LAB\x10\x02\x12\x0f\n\x0bSERVINGSITE\x10\x03\x12\x10\n\x0cMODELASYSTEM\x10\x04\x12\x11\n\rMODELACATALOG\x10\x05\"\xba\x01\n\tTableView\x12\x0c\n\x04\x63ols\x18\x01 \x03(\t\x12L\n\x04rows\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.TableViewRow\x12Q\n\x08profiles\x18\x03 \x03(\x0b\x32?.github.com.metaprov.modelaapi.services.common.v1.ColumnProfile\"\x1e\n\x0cTableViewRow\x12\x0e\n\x06values\x18\x02 \x03(\tB2Z0github.com/metaprov/modelaapi/services/common/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n=github.com/metaprov/modelaapi/services/common/v1/common.proto\x12\x30github.com.metaprov.modelaapi.services.common.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\"\xea\x03\n\x0e\x44\x61tasetProfile\x12\x0c\n\x04\x63ols\x18\x01 \x01(\x05\x12\x0c\n\x04rows\x18\x02 \x01(\x05\x12\x10\n\x08\x66ilesize\x18\x03 \x01(\x05\x12\x11\n\timbalance\x18\x04 \x01(\x08\x12\x45\n\x05plots\x18\x05 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12X\n\x07\x63olumns\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureStatistics\x12J\n\x05table\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x0c\n\x04hash\x18\x08 \x01(\t\x12K\n\x06groups\x18\n \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12O\n\x02ts\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.services.common.v1.TimeSeriesProfile\"\xc1\x06\n\x0cModelProfile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x45\n\x05plots\x18\x02 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12\x62\n\nimportance\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.common.v1.ModelProfile.ImportanceEntry\x12J\n\x06rocauc\x18\x04 \x01(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.ROCCurve\x12R\n\x02pr\x18\x05 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.services.common.v1.PrecisionRecallCurve\x12T\n\x10multiclassRocAuc\x18\x06 \x03(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.ROCCurve\x12\\\n\x0cmulticlassPR\x18\x07 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.services.common.v1.PrecisionRecallCurve\x12U\n\x04\x61lgs\x18\x08 \x03(\x0b\x32G.github.com.metaprov.modelaapi.services.common.v1.ForecastingAlgProfile\x12M\n\x08\x66\x65\x61tures\x18\n \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12K\n\x06groups\x18\x0b \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x1a\x31\n\x0fImportanceEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x95\x05\n\x15\x46orecastingAlgProfile\x12\x11\n\talgorithm\x18\x01 \x01(\t\x12K\n\x06series\x18\x02 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12L\n\x08timeStat\x18\x03 \x01(\x0b\x32:.github.com.metaprov.modelaapi.services.common.v1.TimeStat\x12N\n\tvalueStat\x18\x04 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12G\n\x02\x63v\x18\x05 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12M\n\x08\x66orecast\x18\x06 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12L\n\x07metrics\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12Q\n\x0c\x63hangePoints\x18\x08 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x45\n\x05plots\x18\n \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\xa4\x02\n\x08TimeStat\x12I\n\x04gaps\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x18\n\x10\x61\x64\x64\x65\x64_timepoints\x18\x02 \x01(\x05\x12\x1a\n\x12\x64ropped_timepoints\x18\x03 \x01(\x05\x12\x13\n\x0b\x64\x61ta_points\x18\x04 \x01(\x05\x12\x1c\n\x14mean_increments_secs\x18\x05 \x01(\x02\x12\x31\n\rmin_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rmax_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\\\n\x08ROCCurve\x12\x11\n\tclassname\x18\x01 \x01(\t\x12\x0f\n\x07\x63lassid\x18\x02 \x01(\x05\x12\x0b\n\x03\x66pr\x18\x03 \x03(\x01\x12\x0b\n\x03tpr\x18\x04 \x03(\x01\x12\x12\n\nthresholds\x18\x05 \x03(\x01\"q\n\x14PrecisionRecallCurve\x12\x11\n\tclassname\x18\x01 \x01(\t\x12\x0f\n\x07\x63lassid\x18\x02 \x01(\x05\x12\x11\n\tprecision\x18\x03 \x03(\x01\x12\x0e\n\x06recall\x18\x04 \x03(\x01\x12\x12\n\nthresholds\x18\x05 \x03(\x01\"\x9a\x06\n\x11TimeSeriesProfile\x12\x44\n\x04kpss\x18\x01 \x01(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.KPSS\x12\x42\n\x03\x61\x64\x66\x18\x02 \x01(\x0b\x32\x35.github.com.metaprov.modelaapi.services.common.v1.ADF\x12L\n\x05zivot\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.services.common.v1.ZivotAndrew\x12N\n\x07kendall\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.services.common.v1.MannKendall\x12J\n\x02\x64w\x18\x05 \x01(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.DurbinWatson\x12\x0b\n\x03key\x18\x06 \x01(\t\x12K\n\x06series\x18\x07 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12N\n\tvalueStat\x18\x08 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12Q\n\x0c\x66\x65\x61turesView\x18\t \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\x12\x63\n\x08\x66\x65\x61tures\x18\n \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.common.v1.TimeSeriesProfile.FeaturesEntry\x1a/\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xb4\x01\n\x04KPSS\x12\x11\n\tkpss_stat\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12\x0c\n\x04lags\x18\x03 \x01(\x02\x12N\n\x04\x63rit\x18\x04 \x03(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.KPSS.CritEntry\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xbd\x01\n\x03\x41\x44\x46\x12\x0b\n\x03\x61\x64\x66\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12\x0f\n\x07usedlag\x18\x03 \x01(\x05\x12\x0c\n\x04nobs\x18\x04 \x01(\x05\x12M\n\x04\x63rit\x18\x05 \x03(\x0b\x32?.github.com.metaprov.modelaapi.services.common.v1.ADF.CritEntry\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xd1\x01\n\x0bZivotAndrew\x12\x0e\n\x06zastat\x18\x01 \x01(\x02\x12\x0e\n\x06pvalue\x18\x02 \x01(\x02\x12U\n\x04\x63rit\x18\x03 \x03(\x0b\x32G.github.com.metaprov.modelaapi.services.common.v1.ZivotAndrew.CritEntry\x12\x0f\n\x07\x62\x61selag\x18\x04 \x01(\x05\x12\r\n\x05\x62pidx\x18\x05 \x01(\x05\x1a+\n\tCritEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\x86\x01\n\x0bMannKendall\x12\r\n\x05trend\x18\x01 \x01(\t\x12\t\n\x01h\x18\x02 \x01(\x02\x12\t\n\x01p\x18\x03 \x01(\x02\x12\t\n\x01z\x18\x04 \x01(\x02\x12\x0b\n\x03tau\x18\x05 \x01(\x02\x12\t\n\x01s\x18\x06 \x01(\x02\x12\r\n\x05var_s\x18\x07 \x01(\x02\x12\r\n\x05slope\x18\x08 \x01(\x02\x12\x11\n\tintercept\x18\t \x01(\x02\"\x1a\n\x0c\x44urbinWatson\x12\n\n\x02\x64w\x18\x01 \x01(\x02\"f\n\x0f\x46orecastProfile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x45\n\x05plots\x18\x02 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\"\xe8\x01\n\x0cStudyProfile\x12\x45\n\x05plots\x18\x01 \x03(\x0b\x32\x36.github.com.metaprov.modelaapi.services.common.v1.Plot\x12N\n\x06models\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.ModelProfile\x12\x14\n\x0ctrainingHash\x18\x03 \x01(\t\x12\x13\n\x0btestingHash\x18\x04 \x01(\t\x12\x16\n\x0evalidationHash\x18\x05 \x01(\t\"L\n\x04Plot\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x0b\n\x03img\x18\x03 \x01(\x0c\x12\r\n\x05\x66name\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\"=\n\tHistogram\x12\x0e\n\x06values\x18\x01 \x03(\x01\x12\x0c\n\x04\x62ins\x18\x02 \x03(\x01\x12\x12\n\ncategories\x18\x03 \x03(\t\"\xf6\x02\n\rNamespaceInfo\x12[\n\x04type\x18\x01 \x01(\x0e\x32M.github.com.metaprov.modelaapi.services.common.v1.NamespaceInfo.NamespaceType\x12\x0c\n\x04Name\x18\x02 \x01(\t\x12\x10\n\x08\x61\x63\x63ounts\x18\x03 \x01(\x05\x12\x0f\n\x07\x62uckets\x18\x04 \x01(\x05\x12\x0c\n\x04labs\x18\x05 \x01(\x05\x12\x14\n\x0cservingsites\x18\x06 \x01(\x05\x12\x10\n\x08\x64\x61tasets\x18\x07 \x01(\x05\x12\x13\n\x0b\x64\x61tasources\x18\x08 \x01(\x05\x12\x0f\n\x07studies\x18\t \x01(\x05\x12\x0e\n\x06models\x18\n \x01(\x05\"k\n\rNamespaceType\x12\n\n\x06TENANT\x10\x00\x12\x0f\n\x0b\x44\x41TAPRODUCT\x10\x01\x12\x07\n\x03LAB\x10\x02\x12\x0f\n\x0bSERVINGSITE\x10\x03\x12\x10\n\x0cMODELASYSTEM\x10\x04\x12\x11\n\rMODELACATALOG\x10\x05\"\xc2\x01\n\tTableView\x12\x0c\n\x04\x63ols\x18\x01 \x03(\t\x12L\n\x04rows\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.services.common.v1.TableViewRow\x12Y\n\x08profiles\x18\x03 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureStatistics\"\x1e\n\x0cTableViewRow\x12\x0e\n\x06values\x18\x01 \x03(\tB2Z0github.com/metaprov/modelaapi/services/common/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.common.v1.common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z0github.com/metaprov/modelaapi/services/common/v1'
@@ -29,60 +30,58 @@
   _TIMESERIESPROFILE_FEATURESENTRY._serialized_options = b'8\001'
   _KPSS_CRITENTRY._options = None
   _KPSS_CRITENTRY._serialized_options = b'8\001'
   _ADF_CRITENTRY._options = None
   _ADF_CRITENTRY._serialized_options = b'8\001'
   _ZIVOTANDREW_CRITENTRY._options = None
   _ZIVOTANDREW_CRITENTRY._serialized_options = b'8\001'
-  _DATASETPROFILE._serialized_start=181
-  _DATASETPROFILE._serialized_end=663
-  _MODELPROFILE._serialized_start=666
-  _MODELPROFILE._serialized_end=1499
-  _MODELPROFILE_IMPORTANCEENTRY._serialized_start=1450
-  _MODELPROFILE_IMPORTANCEENTRY._serialized_end=1499
-  _FORECASTINGALGPROFILE._serialized_start=1502
-  _FORECASTINGALGPROFILE._serialized_end=2163
-  _TIMESTAT._serialized_start=2166
-  _TIMESTAT._serialized_end=2458
-  _ROCCURVE._serialized_start=2460
-  _ROCCURVE._serialized_end=2552
-  _PRECISIONRECALLCURVE._serialized_start=2554
-  _PRECISIONRECALLCURVE._serialized_end=2667
-  _TIMESERIESPROFILE._serialized_start=2670
-  _TIMESERIESPROFILE._serialized_end=3464
-  _TIMESERIESPROFILE_FEATURESENTRY._serialized_start=3417
-  _TIMESERIESPROFILE_FEATURESENTRY._serialized_end=3464
-  _KPSS._serialized_start=3467
-  _KPSS._serialized_end=3647
-  _KPSS_CRITENTRY._serialized_start=3604
-  _KPSS_CRITENTRY._serialized_end=3647
-  _ADF._serialized_start=3650
-  _ADF._serialized_end=3839
-  _ADF_CRITENTRY._serialized_start=3604
-  _ADF_CRITENTRY._serialized_end=3647
-  _ZIVOTANDREW._serialized_start=3842
-  _ZIVOTANDREW._serialized_end=4051
-  _ZIVOTANDREW_CRITENTRY._serialized_start=3604
-  _ZIVOTANDREW_CRITENTRY._serialized_end=3647
-  _MANNKENDALL._serialized_start=4054
-  _MANNKENDALL._serialized_end=4188
-  _DURBINWATSON._serialized_start=4190
-  _DURBINWATSON._serialized_end=4216
-  _FORECASTPROFILE._serialized_start=4218
-  _FORECASTPROFILE._serialized_end=4320
-  _STUDYPROFILE._serialized_start=4323
-  _STUDYPROFILE._serialized_end=4555
-  _PLOT._serialized_start=4557
-  _PLOT._serialized_end=4633
-  _COLUMNPROFILE._serialized_start=4636
-  _COLUMNPROFILE._serialized_end=5615
-  _HISTOGRAM._serialized_start=5617
-  _HISTOGRAM._serialized_end=5678
-  _NAMESPACEINFO._serialized_start=5681
-  _NAMESPACEINFO._serialized_end=6055
-  _NAMESPACEINFO_NAMESPACETYPE._serialized_start=5948
-  _NAMESPACEINFO_NAMESPACETYPE._serialized_end=6055
-  _TABLEVIEW._serialized_start=6058
-  _TABLEVIEW._serialized_end=6244
-  _TABLEVIEWROW._serialized_start=6246
-  _TABLEVIEWROW._serialized_end=6276
+  _DATASETPROFILE._serialized_start=251
+  _DATASETPROFILE._serialized_end=741
+  _MODELPROFILE._serialized_start=744
+  _MODELPROFILE._serialized_end=1577
+  _MODELPROFILE_IMPORTANCEENTRY._serialized_start=1528
+  _MODELPROFILE_IMPORTANCEENTRY._serialized_end=1577
+  _FORECASTINGALGPROFILE._serialized_start=1580
+  _FORECASTINGALGPROFILE._serialized_end=2241
+  _TIMESTAT._serialized_start=2244
+  _TIMESTAT._serialized_end=2536
+  _ROCCURVE._serialized_start=2538
+  _ROCCURVE._serialized_end=2630
+  _PRECISIONRECALLCURVE._serialized_start=2632
+  _PRECISIONRECALLCURVE._serialized_end=2745
+  _TIMESERIESPROFILE._serialized_start=2748
+  _TIMESERIESPROFILE._serialized_end=3542
+  _TIMESERIESPROFILE_FEATURESENTRY._serialized_start=3495
+  _TIMESERIESPROFILE_FEATURESENTRY._serialized_end=3542
+  _KPSS._serialized_start=3545
+  _KPSS._serialized_end=3725
+  _KPSS_CRITENTRY._serialized_start=3682
+  _KPSS_CRITENTRY._serialized_end=3725
+  _ADF._serialized_start=3728
+  _ADF._serialized_end=3917
+  _ADF_CRITENTRY._serialized_start=3682
+  _ADF_CRITENTRY._serialized_end=3725
+  _ZIVOTANDREW._serialized_start=3920
+  _ZIVOTANDREW._serialized_end=4129
+  _ZIVOTANDREW_CRITENTRY._serialized_start=3682
+  _ZIVOTANDREW_CRITENTRY._serialized_end=3725
+  _MANNKENDALL._serialized_start=4132
+  _MANNKENDALL._serialized_end=4266
+  _DURBINWATSON._serialized_start=4268
+  _DURBINWATSON._serialized_end=4294
+  _FORECASTPROFILE._serialized_start=4296
+  _FORECASTPROFILE._serialized_end=4398
+  _STUDYPROFILE._serialized_start=4401
+  _STUDYPROFILE._serialized_end=4633
+  _PLOT._serialized_start=4635
+  _PLOT._serialized_end=4711
+  _HISTOGRAM._serialized_start=4713
+  _HISTOGRAM._serialized_end=4774
+  _NAMESPACEINFO._serialized_start=4777
+  _NAMESPACEINFO._serialized_end=5151
+  _NAMESPACEINFO_NAMESPACETYPE._serialized_start=5044
+  _NAMESPACEINFO_NAMESPACETYPE._serialized_end=5151
+  _TABLEVIEW._serialized_start=5154
+  _TABLEVIEW._serialized_end=5348
+  _TABLEVIEWROW._serialized_start=5350
+  _TABLEVIEWROW._serialized_end=5380
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as _generated_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -25,141 +26,37 @@
     adf: float
     crit: _containers.ScalarMap[str, float]
     nobs: int
     pvalue: float
     usedlag: int
     def __init__(self, adf: _Optional[float] = ..., pvalue: _Optional[float] = ..., usedlag: _Optional[int] = ..., nobs: _Optional[int] = ..., crit: _Optional[_Mapping[str, float]] = ...) -> None: ...
 
-class ColumnProfile(_message.Message):
-    __slots__ = ["completeness", "constant", "corrToTarget", "count", "cv", "distinct", "distinctValueCount", "duplicate", "freq", "highCardinality", "highCorrWithOtherFeatures", "highMissingPct", "histogram", "id", "ignore", "importance", "index", "indexOfPeculiarity", "invalid", "iqr", "kurtosis", "lowCorrWithTarget", "mad", "max", "mean", "min", "missing", "mode", "mostFreqValuesRatio", "name", "nullable", "outliersLower", "outliersPercent", "outliersUpper", "p100", "p25", "p50", "p75", "percentMissing", "reserved", "skewed", "skewness", "stddev", "sum", "target", "top", "type", "values", "variance", "zeros"]
-    COMPLETENESS_FIELD_NUMBER: _ClassVar[int]
-    CONSTANT_FIELD_NUMBER: _ClassVar[int]
-    CORRTOTARGET_FIELD_NUMBER: _ClassVar[int]
-    COUNT_FIELD_NUMBER: _ClassVar[int]
-    CV_FIELD_NUMBER: _ClassVar[int]
-    DISTINCTVALUECOUNT_FIELD_NUMBER: _ClassVar[int]
-    DISTINCT_FIELD_NUMBER: _ClassVar[int]
-    DUPLICATE_FIELD_NUMBER: _ClassVar[int]
-    FREQ_FIELD_NUMBER: _ClassVar[int]
-    HIGHCARDINALITY_FIELD_NUMBER: _ClassVar[int]
-    HIGHCORRWITHOTHERFEATURES_FIELD_NUMBER: _ClassVar[int]
-    HIGHMISSINGPCT_FIELD_NUMBER: _ClassVar[int]
-    HISTOGRAM_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    IGNORE_FIELD_NUMBER: _ClassVar[int]
-    IMPORTANCE_FIELD_NUMBER: _ClassVar[int]
-    INDEXOFPECULIARITY_FIELD_NUMBER: _ClassVar[int]
-    INDEX_FIELD_NUMBER: _ClassVar[int]
-    INVALID_FIELD_NUMBER: _ClassVar[int]
-    IQR_FIELD_NUMBER: _ClassVar[int]
-    KURTOSIS_FIELD_NUMBER: _ClassVar[int]
-    LOWCORRWITHTARGET_FIELD_NUMBER: _ClassVar[int]
-    MAD_FIELD_NUMBER: _ClassVar[int]
-    MAX_FIELD_NUMBER: _ClassVar[int]
-    MEAN_FIELD_NUMBER: _ClassVar[int]
-    MIN_FIELD_NUMBER: _ClassVar[int]
-    MISSING_FIELD_NUMBER: _ClassVar[int]
-    MODE_FIELD_NUMBER: _ClassVar[int]
-    MOSTFREQVALUESRATIO_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    NULLABLE_FIELD_NUMBER: _ClassVar[int]
-    OUTLIERSLOWER_FIELD_NUMBER: _ClassVar[int]
-    OUTLIERSPERCENT_FIELD_NUMBER: _ClassVar[int]
-    OUTLIERSUPPER_FIELD_NUMBER: _ClassVar[int]
-    P100_FIELD_NUMBER: _ClassVar[int]
-    P25_FIELD_NUMBER: _ClassVar[int]
-    P50_FIELD_NUMBER: _ClassVar[int]
-    P75_FIELD_NUMBER: _ClassVar[int]
-    PERCENTMISSING_FIELD_NUMBER: _ClassVar[int]
-    RESERVED_FIELD_NUMBER: _ClassVar[int]
-    SKEWED_FIELD_NUMBER: _ClassVar[int]
-    SKEWNESS_FIELD_NUMBER: _ClassVar[int]
-    STDDEV_FIELD_NUMBER: _ClassVar[int]
-    SUM_FIELD_NUMBER: _ClassVar[int]
-    TARGET_FIELD_NUMBER: _ClassVar[int]
-    TOP_FIELD_NUMBER: _ClassVar[int]
-    TYPE_FIELD_NUMBER: _ClassVar[int]
-    VALUES_FIELD_NUMBER: _ClassVar[int]
-    VARIANCE_FIELD_NUMBER: _ClassVar[int]
-    ZEROS_FIELD_NUMBER: _ClassVar[int]
-    completeness: float
-    constant: bool
-    corrToTarget: float
-    count: int
-    cv: float
-    distinct: int
-    distinctValueCount: float
-    duplicate: bool
-    freq: int
-    highCardinality: bool
-    highCorrWithOtherFeatures: bool
-    highMissingPct: bool
-    histogram: Histogram
-    id: bool
-    ignore: bool
-    importance: float
-    index: int
-    indexOfPeculiarity: float
-    invalid: int
-    iqr: float
-    kurtosis: float
-    lowCorrWithTarget: bool
-    mad: float
-    max: float
-    mean: float
-    min: float
-    missing: int
-    mode: str
-    mostFreqValuesRatio: float
-    name: str
-    nullable: bool
-    outliersLower: int
-    outliersPercent: float
-    outliersUpper: int
-    p100: float
-    p25: float
-    p50: float
-    p75: float
-    percentMissing: float
-    reserved: bool
-    skewed: bool
-    skewness: float
-    stddev: float
-    sum: float
-    target: bool
-    top: int
-    type: str
-    values: _containers.RepeatedScalarFieldContainer[str]
-    variance: float
-    zeros: float
-    def __init__(self, name: _Optional[str] = ..., count: _Optional[int] = ..., type: _Optional[str] = ..., missing: _Optional[int] = ..., percentMissing: _Optional[float] = ..., distinct: _Optional[int] = ..., mean: _Optional[float] = ..., mode: _Optional[str] = ..., stddev: _Optional[float] = ..., variance: _Optional[float] = ..., min: _Optional[float] = ..., max: _Optional[float] = ..., kurtosis: _Optional[float] = ..., skewness: _Optional[float] = ..., sum: _Optional[float] = ..., mad: _Optional[float] = ..., zeros: _Optional[float] = ..., p25: _Optional[float] = ..., p50: _Optional[float] = ..., p75: _Optional[float] = ..., p100: _Optional[float] = ..., iqr: _Optional[float] = ..., cv: _Optional[float] = ..., top: _Optional[int] = ..., freq: _Optional[int] = ..., ignore: bool = ..., target: bool = ..., histogram: _Optional[_Union[Histogram, _Mapping]] = ..., invalid: _Optional[int] = ..., importance: _Optional[float] = ..., nullable: bool = ..., highCardinality: bool = ..., highCorrWithOtherFeatures: bool = ..., lowCorrWithTarget: bool = ..., highMissingPct: bool = ..., skewed: bool = ..., id: bool = ..., constant: bool = ..., duplicate: bool = ..., reserved: bool = ..., outliersUpper: _Optional[int] = ..., outliersLower: _Optional[int] = ..., outliersPercent: _Optional[float] = ..., completeness: _Optional[float] = ..., distinctValueCount: _Optional[float] = ..., mostFreqValuesRatio: _Optional[float] = ..., indexOfPeculiarity: _Optional[float] = ..., values: _Optional[_Iterable[str]] = ..., corrToTarget: _Optional[float] = ..., index: _Optional[int] = ...) -> None: ...
-
 class DatasetProfile(_message.Message):
     __slots__ = ["cols", "columns", "filesize", "groups", "hash", "imbalance", "plots", "rows", "table", "ts"]
     COLS_FIELD_NUMBER: _ClassVar[int]
     COLUMNS_FIELD_NUMBER: _ClassVar[int]
     FILESIZE_FIELD_NUMBER: _ClassVar[int]
     GROUPS_FIELD_NUMBER: _ClassVar[int]
     HASH_FIELD_NUMBER: _ClassVar[int]
     IMBALANCE_FIELD_NUMBER: _ClassVar[int]
     PLOTS_FIELD_NUMBER: _ClassVar[int]
     ROWS_FIELD_NUMBER: _ClassVar[int]
     TABLE_FIELD_NUMBER: _ClassVar[int]
     TS_FIELD_NUMBER: _ClassVar[int]
     cols: int
-    columns: _containers.RepeatedCompositeFieldContainer[ColumnProfile]
+    columns: _containers.RepeatedCompositeFieldContainer[_generated_pb2.FeatureStatistics]
     filesize: int
     groups: TableView
     hash: str
     imbalance: bool
     plots: _containers.RepeatedCompositeFieldContainer[Plot]
     rows: int
     table: TableView
     ts: TimeSeriesProfile
-    def __init__(self, cols: _Optional[int] = ..., rows: _Optional[int] = ..., filesize: _Optional[int] = ..., imbalance: bool = ..., plots: _Optional[_Iterable[_Union[Plot, _Mapping]]] = ..., columns: _Optional[_Iterable[_Union[ColumnProfile, _Mapping]]] = ..., table: _Optional[_Union[TableView, _Mapping]] = ..., hash: _Optional[str] = ..., groups: _Optional[_Union[TableView, _Mapping]] = ..., ts: _Optional[_Union[TimeSeriesProfile, _Mapping]] = ...) -> None: ...
+    def __init__(self, cols: _Optional[int] = ..., rows: _Optional[int] = ..., filesize: _Optional[int] = ..., imbalance: bool = ..., plots: _Optional[_Iterable[_Union[Plot, _Mapping]]] = ..., columns: _Optional[_Iterable[_Union[_generated_pb2.FeatureStatistics, _Mapping]]] = ..., table: _Optional[_Union[TableView, _Mapping]] = ..., hash: _Optional[str] = ..., groups: _Optional[_Union[TableView, _Mapping]] = ..., ts: _Optional[_Union[TimeSeriesProfile, _Mapping]] = ...) -> None: ...
 
 class DurbinWatson(_message.Message):
     __slots__ = ["dw"]
     DW_FIELD_NUMBER: _ClassVar[int]
     dw: float
     def __init__(self, dw: _Optional[float] = ...) -> None: ...
 
@@ -365,17 +262,17 @@
 
 class TableView(_message.Message):
     __slots__ = ["cols", "profiles", "rows"]
     COLS_FIELD_NUMBER: _ClassVar[int]
     PROFILES_FIELD_NUMBER: _ClassVar[int]
     ROWS_FIELD_NUMBER: _ClassVar[int]
     cols: _containers.RepeatedScalarFieldContainer[str]
-    profiles: _containers.RepeatedCompositeFieldContainer[ColumnProfile]
+    profiles: _containers.RepeatedCompositeFieldContainer[_generated_pb2.FeatureStatistics]
     rows: _containers.RepeatedCompositeFieldContainer[TableViewRow]
-    def __init__(self, cols: _Optional[_Iterable[str]] = ..., rows: _Optional[_Iterable[_Union[TableViewRow, _Mapping]]] = ..., profiles: _Optional[_Iterable[_Union[ColumnProfile, _Mapping]]] = ...) -> None: ...
+    def __init__(self, cols: _Optional[_Iterable[str]] = ..., rows: _Optional[_Iterable[_Union[TableViewRow, _Mapping]]] = ..., profiles: _Optional[_Iterable[_Union[_generated_pb2.FeatureStatistics, _Mapping]]] = ...) -> None: ...
 
 class TableViewRow(_message.Message):
     __slots__ = ["values"]
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_inference_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x06 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\t \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\n \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xc8\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe6\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe7\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe8\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x08 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\n \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\x0b \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xd2\x03\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12U\n\x06target\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x06 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xcf\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12^\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12]\n\x0etestingDataset\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x80\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\r\n\x05rungs\x18\x05 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xea\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc1\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe4\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc2\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x07 \x01(\x05\x12\x11\n\tdefaultHP\x18\x08 \x01(\x08\x12\x11\n\talgorithm\x18\t \x01(\t\x12V\n\nalgorithms\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe0\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xae\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x10\n\x08\x61lgnames\x18\x07 \x03(\t\x12\x0b\n\x03\x61ll\x18\x08 \x01(\x08\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb5\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xbc\x03\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"m\n\x12\x44sSnapshotResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n9github.com/metaprov/modelaapi/services/data/v1/data.proto\x12.github.com.metaprov.modelaapi.services.data.v1\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1aIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1a\"k8s.io/api/core/v1/generated.proto\"\xa2\x03\n\x11\x44sReadFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12]\n\x06secret\x18\x06 \x03(\x0b\x32M.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xa8\x03\n\x14\x44sReadFeatureRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12`\n\x06secret\x18\x06 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xf4\x03\n\x12\x44sWriteFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x07\x63ontent\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x05 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x07 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xd0\x02\n\x12\x44sReadAudioRequest\x12T\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12^\n\x06secret\x18\x03 \x03(\x0b\x32N.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xae\x03\n\x17\x44sReadTextCorpusRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x05 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadTextCorpusRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xfd\x03\n\x17\x44sReadFromStoreResponse\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12M\n\x06result\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12U\n\nconnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x06secret\x18\x06 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"p\n\x18\x44sRunDataPipelineRequest\x12T\n\x08pipeline\x18\x01 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataPipeline\"j\n\x19\x44sRunDataPipelineResponse\x12M\n\x06result\x18\x01 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"\xf6\x07\n\x12\x44sRunRecipeRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\x06\x62ucket\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\\\n\x11storageConnection\x18\x05 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\rstorageSecret\x18\x06 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x62\n\x08\x64\x62Secret\x18\x08 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest.DbSecretEntry\x12L\n\x06recipe\x18\t \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\x12R\n\treciperun\x18\n \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.RecipeRun\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"c\n\x13\x44sRunRecipeResponse\x12L\n\x06result\x18\x01 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Recipe\"\x14\n\x12\x44\x61taSourceResponse\"\x11\n\x0f\x44\x61tasetResponse\"\xc8\x03\n\x1d\x44sCreateDatasetProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"\xb3\x02\n\x1e\x44sCreateDatasetProfileResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0f\x61nomalyLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xe6\x04\n\x1b\x44sCreateModelProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"~\n\x1c\x44sCreateModelProfileResponse\x12^\n\x0fprofileLocation\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x83\x08\n\x1a\x44sMergeForecastFileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x08 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x66\n\x06secret\x18\n \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.SecretEntry\x12\x11\n\tforecasts\x18\x0b \x03(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12j\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32X.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"*\n\x1b\x44sMergeForecastFileResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xe7\x04\n\x1b\x44sCreateStudyProfileRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"~\n\x1c\x44sCreateStudyProfileResponse\x12^\n\x0fprofileLocation\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x91\x06\n\x13RunTestSuiteRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12N\n\x05study\x18\x04 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12Y\n\thistogram\x18\x07 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12\\\n\x0crefHistogram\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureHistogram\x12Q\n\x05suite\x18\t \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"p\n\x14RunTestSuiteResponse\x12X\n\x06result\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\"\xd2\x03\n\x18\x44sGenerateDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12U\n\x06target\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0c\n\x04rows\x18\x06 \x01(\x05\"r\n\x19\x44sGenerateDatasetResponse\x12U\n\x06target\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xcf\x05\n\x15\x44sSplitDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12^\n\x0ftrainingDataset\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12]\n\x0etestingDataset\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"\xc3\x03\n\x16\x44sSplitDatasetResponse\x12\x10\n\x08training\x18\x01 \x01(\x05\x12\x0f\n\x07testing\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x14\n\x0ctrainingHash\x18\x04 \x01(\t\x12\x13\n\x0btestingHash\x18\x05 \x01(\t\x12\x16\n\x0evalidationHash\x18\x06 \x01(\t\x12\x11\n\tindexFile\x18\x07 \x01(\t\x12\\\n\rtrainLocation\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12[\n\x0ctestLocation\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x61\n\x12validationLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\x80\x03\n\x1c\x44sSplitDatasetToRungsRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\r\n\x05rungs\x18\x05 \x01(\x05\"\x1f\n\x1d\x44sSplitDatasetToRungsResponse\"\xea\x02\n\x15GroupByDatasetRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"%\n\x16GroupByDatasetResponse\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\xd5\x01\n\x14\x44sInferSchemaRequest\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"j\n\x15\x44sInferSchemaResponse\x12Q\n\x07profile\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.services.common.v1.DatasetProfile\"\xdc\x01\n\x15\x44sGetTableViewRequest\x12Z\n\x08\x66latfile\x18\x01 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x0e\n\x06tenant\x18\x03 \x01(\t\"h\n\x16\x44sGetTableViewResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\x86\x04\n\x18\x43reateModelReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xd7\x08\n\x1b\x43reateForecastReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12T\n\ndatasource\x18\x05 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12Q\n\x08\x66orecast\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12U\n\nconnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12g\n\x06secret\x18\x08 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.SecretEntry\x12T\n\x06\x62ucket\x18\t \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12P\n\x06report\x18\n \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\x12\r\n\x05group\x18\x0b \x01(\x08\x12W\n\x0c\x64\x62\x43onnection\x18\x0c \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12k\n\x08\x64\x62Secret\x18\r \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest.DbSecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\xc3\x01\n\x1a\x43reateSummaryReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12Q\n\x07reports\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"#\n\x14\x43reateReportResponse\x12\x0b\n\x03pdf\x18\x01 \x01(\x0c\"\xc1\x03\n\x1a\x43reateDatasetReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12P\n\x06report\x18\x06 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe4\x04\n\x18\x43reateStudyReportRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12S\n\x06models\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelList\x12P\n\x06report\x18\x07 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xc2\x04\n\x0f\x41skModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x07 \x01(\x05\x12\x11\n\tdefaultHP\x18\x08 \x01(\x08\x12\x11\n\talgorithm\x18\t \x01(\t\x12V\n\nalgorithms\x18\n \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xeb\x02\n\x1fGetTimeSeriesDatasetKeysRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\"0\n GetTimeSeriesDatasetKeysResponse\x12\x0c\n\x04keys\x18\x01 \x03(\t\"\xc9\x03\n\x17\x41skForecastModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12\x0c\n\x04keys\x18\x06 \x03(\t\x12V\n\nalgorithms\x18\x07 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"j\n\x18\x41skForecastModelResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xe0\x04\n\x12\x41skEnsembleRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12O\n\x06models\x18\x07 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skEnsembleResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xae\x04\n\x12\x41skBaselineRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x03 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x04 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x10\n\x08\x61lgnames\x18\x07 \x03(\t\x12\x0b\n\x03\x61ll\x18\x08 \x01(\x08\x12V\n\nalgorithms\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"e\n\x13\x41skBaselineResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xb5\x04\n\x1a\x41skAllModelsForTaskRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12\x0e\n\x06\x62udget\x18\x06 \x01(\x05\x12\x0c\n\x04task\x18\x07 \x01(\t\x12V\n\nalgorithms\x18\x08 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"m\n\x1b\x41skAllModelsForTaskResponse\x12N\n\x05model\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\x95\x04\n\x10TellModelRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\x12N\n\x05model\x18\x06 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12\x0e\n\x06\x66\x61iled\x18\x07 \x01(\x08\"#\n\x11TellModelResponse\x12\x0e\n\x06pruned\x18\x01 \x01(\x08\"\x13\n\x11\x44sShutdownRequest\"\x14\n\x12\x44sShutdownResponse\"\xda\x02\n\x17\x44sTestConnectionRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12\x63\n\x06secret\x18\x03 \x03(\x0b\x32S.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest.SecretEntry\x1a-\n\x0bSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"7\n\x18\x44sTestConnectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x08\x12\x0b\n\x03msg\x18\x02 \x01(\t\"\xb9\x01\n\x13\x44sStudyEndedRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\x16\n\x14\x44sStudyEndedResponse\"\x92\x02\n\x16SaveOptimizerDBRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12T\n\x06\x62ucket\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\"r\n\x17SaveOptimizerDBResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"n\n\x15\x44sGetDatabasesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"+\n\x16\x44sGetDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\t\"k\n\x12\x44sGetTablesRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"%\n\x13\x44sGetTablesResponse\x12\x0e\n\x06tables\x18\x01 \x03(\t\"y\n\x13\x44sExecuteSqlRequest\x12U\n\nconnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x0b\n\x03sql\x18\x04 \x01(\t\"f\n\x14\x44sExecuteSqlResponse\x12N\n\ttableview\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView\"\xbc\x03\n\x11\x44sSnapshotRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\x06\x62ucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12T\n\ndatasource\x18\x03 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x04 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12W\n\x08snapshot\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DatasetSnapshot\"m\n\x12\x44sSnapshotResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"b\n\x10\x41skModelResponse\x12N\n\x05model\x18\x01 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"\xca\x03\n\x16GenTrainingDataRequest\x12R\n\x07product\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelClass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelClassRun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x08\x65ntities\x18\x04 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\"r\n\x17GenTrainingDataResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\"\xeb\x06\n\x16SyncOnlineStoreRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12p\n\rstorageSecret\x18\x03 \x03(\x0b\x32Y.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x66\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32T.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"\x19\n\x17SyncOnlineStoreResponse\"\xfd\x06\n\x1cGenOnlineStoreDatasetRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12v\n\rstorageSecret\x18\x03 \x03(\x0b\x32_.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12l\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Z.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest.DbSecretEntry\x12S\n\x05model\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x02\x66g\x18\x07 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x08location\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"x\n\x1dGenOnlineStoreDatasetResponse\x12W\n\x08location\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x8d\x08\n\x13\x42\x61tchPredictRequest\x12\\\n\x11storageConnection\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12[\n\rstorageBucket\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.VirtualBucket\x12m\n\rstorageSecret\x18\x03 \x03(\x0b\x32V.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.StorageSecretEntry\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\x12\x63\n\x08\x64\x62Secret\x18\x05 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest.DbSecretEntry\x12X\n\nmodelclass\x18\x06 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12N\n\x05model\x18\x07 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12N\n\x08\x65ntities\x18\x08 \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Entity\x12R\n\x06groups\x18\t \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12Y\n\nprediction\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x1a\x34\n\x12StorageSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\x1a/\n\rDbSecretEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x0c:\x02\x38\x01\"$\n\x14\x42\x61tchPredictResponse\x12\x0c\n\x04rows\x18\x01 \x01(\x05\"\xa5\x04\n\x12SaveDatasetRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12N\n\x07\x64\x61taset\x18\x03 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Dataset\x12X\n\nmodelclass\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x05 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xf1\x04\n\x10SaveModelRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12N\n\x05study\x18\x02 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\x12X\n\nmodelclass\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x04 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12N\n\x05model\x18\x05 \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\x12R\n\x06groups\x18\x06 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureGroup\x12W\n\x0c\x64\x62\x43onnection\x18\x07 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xb6\x04\n\x15SavePredictionRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12^\n\rmodelclassrun\x18\x03 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\x12W\n\tpredictor\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\x12Y\n\nprediction\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x06 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\xfb\x02\n\x14SavePredictorRequest\x12V\n\x0b\x64\x61taproduct\x18\x01 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataProduct\x12X\n\nmodelclass\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\x12X\n\tpredictor\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\x12W\n\x0c\x64\x62\x43onnection\x18\x04 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x84\x01\n\x19\x43reateMetricsStoreRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12W\n\x0c\x64\x62\x43onnection\x18\x02 \x01(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1.Connection\"\x1c\n\x1a\x43reateMetricsStoreResponse\"\x1c\n\x0cSaveResponse\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\x05\x32\xf0?\n\x0b\x44\x61taService\x12\x98\x01\n\x08ReadFile\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsReadFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9e\x01\n\x0bReadFeature\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsReadFeatureRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\x9a\x01\n\tReadAudio\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsReadAudioRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fRunDataPipeline\x12H.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsRunDataPipelineResponse\"\x00\x12\x96\x01\n\tRunRecipe\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsRunRecipeResponse\"\x00\x12\x9a\x01\n\tWriteFile\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsWriteFileRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.DsReadFromStoreResponse\"\x00\x12\xa8\x01\n\x0fGenerateDataset\x12H.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetRequest\x1aI.github.com.metaprov.modelaapi.services.data.v1.DsGenerateDatasetResponse\"\x00\x12\x9f\x01\n\x0cSplitDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetResponse\"\x00\x12\x9c\x01\n\x0bInferSchema\x12\x44.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaRequest\x1a\x45.github.com.metaprov.modelaapi.services.data.v1.DsInferSchemaResponse\"\x00\x12\x9f\x01\n\x0cGetTableView\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetTableViewResponse\"\x00\x12\xb4\x01\n\x13SplitDatasetToRungs\x12L.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.DsSplitDatasetToRungsResponse\"\x00\x12\xb7\x01\n\x14\x43reateDatasetProfile\x12M.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileRequest\x1aN.github.com.metaprov.modelaapi.services.data.v1.DsCreateDatasetProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateModelProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateModelProfileResponse\"\x00\x12\xb1\x01\n\x12\x43reateStudyProfile\x12K.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileRequest\x1aL.github.com.metaprov.modelaapi.services.data.v1.DsCreateStudyProfileResponse\"\x00\x12\xa5\x01\n\x11\x43reateModelReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateModelReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa5\x01\n\x11\x43reateStudyReport\x12H.github.com.metaprov.modelaapi.services.data.v1.CreateStudyReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateDatasetReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateDatasetReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xab\x01\n\x14\x43reateForecastReport\x12K.github.com.metaprov.modelaapi.services.data.v1.CreateForecastReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\xa9\x01\n\x13\x43reateSummaryReport\x12J.github.com.metaprov.modelaapi.services.data.v1.CreateSummaryReportRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.CreateReportResponse\"\x00\x12\x8c\x01\n\x05\x41skFE\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\x98\x01\n\x0b\x41skBaseline\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskBaselineRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskBaselineResponse\"\x00\x12\x98\x01\n\x0b\x41skEnsemble\x12\x42.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.AskEnsembleResponse\"\x00\x12\xa7\x01\n\x10\x41skForecastModel\x12G.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.AskForecastModelResponse\"\x00\x12\x8f\x01\n\x08\x41skModel\x12?.github.com.metaprov.modelaapi.services.data.v1.AskModelRequest\x1a@.github.com.metaprov.modelaapi.services.data.v1.AskModelResponse\"\x00\x12\xb0\x01\n\x13\x41skAllModelsForTask\x12J.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.AskAllModelsForTaskResponse\"\x00\x12\x99\x01\n\x10TellPartialModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\x92\x01\n\tTellModel\x12@.github.com.metaprov.modelaapi.services.data.v1.TellModelRequest\x1a\x41.github.com.metaprov.modelaapi.services.data.v1.TellModelResponse\"\x00\x12\xae\x01\n\x11MergeForecastFile\x12J.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileRequest\x1aK.github.com.metaprov.modelaapi.services.data.v1.DsMergeForecastFileResponse\"\x00\x12\xa7\x01\n\x10\x44sTestConnection\x12G.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionRequest\x1aH.github.com.metaprov.modelaapi.services.data.v1.DsTestConnectionResponse\"\x00\x12\x93\x01\n\x08ShutDown\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsShutdownRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsShutdownResponse\"\x00\x12\x99\x01\n\nStudyEnded\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsStudyEndedResponse\"\x00\x12\xa4\x01\n\x0fSaveOptimizerDB\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SaveOptimizerDBResponse\"\x00\x12\x9f\x01\n\x0cGetDatabases\x12\x45.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.DsGetDatabasesResponse\"\x00\x12\x96\x01\n\tGetTables\x12\x42.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesRequest\x1a\x43.github.com.metaprov.modelaapi.services.data.v1.DsGetTablesResponse\"\x00\x12\x99\x01\n\nExecuteSql\x12\x43.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.DsExecuteSqlResponse\"\x00\x12\x93\x01\n\x08Snapshot\x12\x41.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotRequest\x1a\x42.github.com.metaprov.modelaapi.services.data.v1.DsSnapshotResponse\"\x00\x12\x9e\x01\n\x0fUnitTestDataset\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9c\x01\n\rUnitTestModel\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\x9f\x01\n\x10UnitTestFeedback\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa7\x01\n\x18UnitTestFeatureHistogram\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa0\x01\n\x11UnitTestPredictor\x12\x43.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.RunTestSuiteResponse\"\x00\x12\xa1\x01\n\x0eGroupByDataset\x12\x45.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetRequest\x1a\x46.github.com.metaprov.modelaapi.services.data.v1.GroupByDatasetResponse\"\x00\x12\xa4\x01\n\x0fSyncOnlineStore\x12\x46.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.SyncOnlineStoreResponse\"\x00\x12\xa4\x01\n\x0fGenTrainingData\x12\x46.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataRequest\x1aG.github.com.metaprov.modelaapi.services.data.v1.GenTrainingDataResponse\"\x00\x12\xb6\x01\n\x15GenOnlineStoreDataset\x12L.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetRequest\x1aM.github.com.metaprov.modelaapi.services.data.v1.GenOnlineStoreDatasetResponse\"\x00\x12\x9b\x01\n\x0c\x42\x61tchPredict\x12\x43.github.com.metaprov.modelaapi.services.data.v1.BatchPredictRequest\x1a\x44.github.com.metaprov.modelaapi.services.data.v1.BatchPredictResponse\"\x00\x12\x91\x01\n\x0bSaveDataSet\x12\x42.github.com.metaprov.modelaapi.services.data.v1.SaveDatasetRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x8d\x01\n\tSaveModel\x12@.github.com.metaprov.modelaapi.services.data.v1.SaveModelRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\x97\x01\n\x0eSavePrediction\x12\x45.github.com.metaprov.modelaapi.services.data.v1.SavePredictionRequest\x1a<.github.com.metaprov.modelaapi.services.data.v1.SaveResponse\"\x00\x12\xad\x01\n\x12\x43reateMetricsStore\x12I.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreRequest\x1aJ.github.com.metaprov.modelaapi.services.data.v1.CreateMetricsStoreResponse\"\x00\x42\x30Z.github.com/metaprov/modelaapi/services/data/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.data.v1.data_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z.github.com/metaprov/modelaapi/services/data/v1'
@@ -123,157 +123,157 @@
   _DSMERGEFORECASTFILERESPONSE._serialized_start=7131
   _DSMERGEFORECASTFILERESPONSE._serialized_end=7173
   _DSCREATESTUDYPROFILEREQUEST._serialized_start=7176
   _DSCREATESTUDYPROFILEREQUEST._serialized_end=7791
   _DSCREATESTUDYPROFILERESPONSE._serialized_start=7793
   _DSCREATESTUDYPROFILERESPONSE._serialized_end=7919
   _RUNTESTSUITEREQUEST._serialized_start=7922
-  _RUNTESTSUITEREQUEST._serialized_end=8794
-  _RUNTESTSUITERESPONSE._serialized_start=8796
-  _RUNTESTSUITERESPONSE._serialized_end=8908
-  _DSGENERATEDATASETREQUEST._serialized_start=8911
-  _DSGENERATEDATASETREQUEST._serialized_end=9377
-  _DSGENERATEDATASETRESPONSE._serialized_start=9379
-  _DSGENERATEDATASETRESPONSE._serialized_end=9493
-  _DSSPLITDATASETREQUEST._serialized_start=9496
-  _DSSPLITDATASETREQUEST._serialized_end=10215
-  _DSSPLITDATASETRESPONSE._serialized_start=10218
-  _DSSPLITDATASETRESPONSE._serialized_end=10669
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=10672
-  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=11056
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=11058
-  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=11089
-  _GROUPBYDATASETREQUEST._serialized_start=11092
-  _GROUPBYDATASETREQUEST._serialized_end=11454
-  _GROUPBYDATASETRESPONSE._serialized_start=11456
-  _GROUPBYDATASETRESPONSE._serialized_end=11493
-  _DSINFERSCHEMAREQUEST._serialized_start=11496
-  _DSINFERSCHEMAREQUEST._serialized_end=11709
-  _DSINFERSCHEMARESPONSE._serialized_start=11711
-  _DSINFERSCHEMARESPONSE._serialized_end=11817
-  _DSGETTABLEVIEWREQUEST._serialized_start=11820
-  _DSGETTABLEVIEWREQUEST._serialized_end=12040
-  _DSGETTABLEVIEWRESPONSE._serialized_start=12042
-  _DSGETTABLEVIEWRESPONSE._serialized_end=12146
-  _CREATEMODELREPORTREQUEST._serialized_start=12149
-  _CREATEMODELREPORTREQUEST._serialized_end=12667
-  _CREATEFORECASTREPORTREQUEST._serialized_start=12670
-  _CREATEFORECASTREPORTREQUEST._serialized_end=13781
+  _RUNTESTSUITEREQUEST._serialized_end=8707
+  _RUNTESTSUITERESPONSE._serialized_start=8709
+  _RUNTESTSUITERESPONSE._serialized_end=8821
+  _DSGENERATEDATASETREQUEST._serialized_start=8824
+  _DSGENERATEDATASETREQUEST._serialized_end=9290
+  _DSGENERATEDATASETRESPONSE._serialized_start=9292
+  _DSGENERATEDATASETRESPONSE._serialized_end=9406
+  _DSSPLITDATASETREQUEST._serialized_start=9409
+  _DSSPLITDATASETREQUEST._serialized_end=10128
+  _DSSPLITDATASETRESPONSE._serialized_start=10131
+  _DSSPLITDATASETRESPONSE._serialized_end=10582
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_start=10585
+  _DSSPLITDATASETTORUNGSREQUEST._serialized_end=10969
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_start=10971
+  _DSSPLITDATASETTORUNGSRESPONSE._serialized_end=11002
+  _GROUPBYDATASETREQUEST._serialized_start=11005
+  _GROUPBYDATASETREQUEST._serialized_end=11367
+  _GROUPBYDATASETRESPONSE._serialized_start=11369
+  _GROUPBYDATASETRESPONSE._serialized_end=11406
+  _DSINFERSCHEMAREQUEST._serialized_start=11409
+  _DSINFERSCHEMAREQUEST._serialized_end=11622
+  _DSINFERSCHEMARESPONSE._serialized_start=11624
+  _DSINFERSCHEMARESPONSE._serialized_end=11730
+  _DSGETTABLEVIEWREQUEST._serialized_start=11733
+  _DSGETTABLEVIEWREQUEST._serialized_end=11953
+  _DSGETTABLEVIEWRESPONSE._serialized_start=11955
+  _DSGETTABLEVIEWRESPONSE._serialized_end=12059
+  _CREATEMODELREPORTREQUEST._serialized_start=12062
+  _CREATEMODELREPORTREQUEST._serialized_end=12580
+  _CREATEFORECASTREPORTREQUEST._serialized_start=12583
+  _CREATEFORECASTREPORTREQUEST._serialized_end=13694
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_start=945
   _CREATEFORECASTREPORTREQUEST_SECRETENTRY._serialized_end=990
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_start=4396
   _CREATEFORECASTREPORTREQUEST_DBSECRETENTRY._serialized_end=4443
-  _CREATESUMMARYREPORTREQUEST._serialized_start=13784
-  _CREATESUMMARYREPORTREQUEST._serialized_end=13979
-  _CREATEREPORTRESPONSE._serialized_start=13981
-  _CREATEREPORTRESPONSE._serialized_end=14016
-  _CREATEDATASETREPORTREQUEST._serialized_start=14019
-  _CREATEDATASETREPORTREQUEST._serialized_end=14468
-  _CREATESTUDYREPORTREQUEST._serialized_start=14471
-  _CREATESTUDYREPORTREQUEST._serialized_end=15083
-  _ASKMODELREQUEST._serialized_start=15086
-  _ASKMODELREQUEST._serialized_end=15664
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=15667
-  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=16030
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=16032
-  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=16080
-  _ASKFORECASTMODELREQUEST._serialized_start=16083
-  _ASKFORECASTMODELREQUEST._serialized_end=16540
-  _ASKFORECASTMODELRESPONSE._serialized_start=16542
-  _ASKFORECASTMODELRESPONSE._serialized_end=16648
-  _ASKENSEMBLEREQUEST._serialized_start=16651
-  _ASKENSEMBLEREQUEST._serialized_end=17259
-  _ASKENSEMBLERESPONSE._serialized_start=17261
-  _ASKENSEMBLERESPONSE._serialized_end=17362
-  _ASKBASELINEREQUEST._serialized_start=17365
-  _ASKBASELINEREQUEST._serialized_end=17923
-  _ASKBASELINERESPONSE._serialized_start=17925
-  _ASKBASELINERESPONSE._serialized_end=18026
-  _ASKALLMODELSFORTASKREQUEST._serialized_start=18029
-  _ASKALLMODELSFORTASKREQUEST._serialized_end=18594
-  _ASKALLMODELSFORTASKRESPONSE._serialized_start=18596
-  _ASKALLMODELSFORTASKRESPONSE._serialized_end=18705
-  _TELLMODELREQUEST._serialized_start=18708
-  _TELLMODELREQUEST._serialized_end=19241
-  _TELLMODELRESPONSE._serialized_start=19243
-  _TELLMODELRESPONSE._serialized_end=19278
-  _DSSHUTDOWNREQUEST._serialized_start=19280
-  _DSSHUTDOWNREQUEST._serialized_end=19299
-  _DSSHUTDOWNRESPONSE._serialized_start=19301
-  _DSSHUTDOWNRESPONSE._serialized_end=19321
-  _DSTESTCONNECTIONREQUEST._serialized_start=19324
-  _DSTESTCONNECTIONREQUEST._serialized_end=19670
+  _CREATESUMMARYREPORTREQUEST._serialized_start=13697
+  _CREATESUMMARYREPORTREQUEST._serialized_end=13892
+  _CREATEREPORTRESPONSE._serialized_start=13894
+  _CREATEREPORTRESPONSE._serialized_end=13929
+  _CREATEDATASETREPORTREQUEST._serialized_start=13932
+  _CREATEDATASETREPORTREQUEST._serialized_end=14381
+  _CREATESTUDYREPORTREQUEST._serialized_start=14384
+  _CREATESTUDYREPORTREQUEST._serialized_end=14996
+  _ASKMODELREQUEST._serialized_start=14999
+  _ASKMODELREQUEST._serialized_end=15577
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_start=15580
+  _GETTIMESERIESDATASETKEYSREQUEST._serialized_end=15943
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_start=15945
+  _GETTIMESERIESDATASETKEYSRESPONSE._serialized_end=15993
+  _ASKFORECASTMODELREQUEST._serialized_start=15996
+  _ASKFORECASTMODELREQUEST._serialized_end=16453
+  _ASKFORECASTMODELRESPONSE._serialized_start=16455
+  _ASKFORECASTMODELRESPONSE._serialized_end=16561
+  _ASKENSEMBLEREQUEST._serialized_start=16564
+  _ASKENSEMBLEREQUEST._serialized_end=17172
+  _ASKENSEMBLERESPONSE._serialized_start=17174
+  _ASKENSEMBLERESPONSE._serialized_end=17275
+  _ASKBASELINEREQUEST._serialized_start=17278
+  _ASKBASELINEREQUEST._serialized_end=17836
+  _ASKBASELINERESPONSE._serialized_start=17838
+  _ASKBASELINERESPONSE._serialized_end=17939
+  _ASKALLMODELSFORTASKREQUEST._serialized_start=17942
+  _ASKALLMODELSFORTASKREQUEST._serialized_end=18507
+  _ASKALLMODELSFORTASKRESPONSE._serialized_start=18509
+  _ASKALLMODELSFORTASKRESPONSE._serialized_end=18618
+  _TELLMODELREQUEST._serialized_start=18621
+  _TELLMODELREQUEST._serialized_end=19154
+  _TELLMODELRESPONSE._serialized_start=19156
+  _TELLMODELRESPONSE._serialized_end=19191
+  _DSSHUTDOWNREQUEST._serialized_start=19193
+  _DSSHUTDOWNREQUEST._serialized_end=19212
+  _DSSHUTDOWNRESPONSE._serialized_start=19214
+  _DSSHUTDOWNRESPONSE._serialized_end=19234
+  _DSTESTCONNECTIONREQUEST._serialized_start=19237
+  _DSTESTCONNECTIONREQUEST._serialized_end=19583
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_start=945
   _DSTESTCONNECTIONREQUEST_SECRETENTRY._serialized_end=990
-  _DSTESTCONNECTIONRESPONSE._serialized_start=19672
-  _DSTESTCONNECTIONRESPONSE._serialized_end=19727
-  _DSSTUDYENDEDREQUEST._serialized_start=19730
-  _DSSTUDYENDEDREQUEST._serialized_end=19915
-  _DSSTUDYENDEDRESPONSE._serialized_start=19917
-  _DSSTUDYENDEDRESPONSE._serialized_end=19939
-  _SAVEOPTIMIZERDBREQUEST._serialized_start=19942
-  _SAVEOPTIMIZERDBREQUEST._serialized_end=20216
-  _SAVEOPTIMIZERDBRESPONSE._serialized_start=20218
-  _SAVEOPTIMIZERDBRESPONSE._serialized_end=20332
-  _DSGETDATABASESREQUEST._serialized_start=20334
-  _DSGETDATABASESREQUEST._serialized_end=20444
-  _DSGETDATABASESRESPONSE._serialized_start=20446
-  _DSGETDATABASESRESPONSE._serialized_end=20489
-  _DSGETTABLESREQUEST._serialized_start=20491
-  _DSGETTABLESREQUEST._serialized_end=20598
-  _DSGETTABLESRESPONSE._serialized_start=20600
-  _DSGETTABLESRESPONSE._serialized_end=20637
-  _DSEXECUTESQLREQUEST._serialized_start=20639
-  _DSEXECUTESQLREQUEST._serialized_end=20760
-  _DSEXECUTESQLRESPONSE._serialized_start=20762
-  _DSEXECUTESQLRESPONSE._serialized_end=20864
-  _DSSNAPSHOTREQUEST._serialized_start=20867
-  _DSSNAPSHOTREQUEST._serialized_end=21311
-  _DSSNAPSHOTRESPONSE._serialized_start=21313
-  _DSSNAPSHOTRESPONSE._serialized_end=21422
-  _ASKMODELRESPONSE._serialized_start=21424
-  _ASKMODELRESPONSE._serialized_end=21522
-  _GENTRAININGDATAREQUEST._serialized_start=21525
-  _GENTRAININGDATAREQUEST._serialized_end=21983
-  _GENTRAININGDATARESPONSE._serialized_start=21985
-  _GENTRAININGDATARESPONSE._serialized_end=22099
-  _SYNCONLINESTOREREQUEST._serialized_start=22102
-  _SYNCONLINESTOREREQUEST._serialized_end=22977
+  _DSTESTCONNECTIONRESPONSE._serialized_start=19585
+  _DSTESTCONNECTIONRESPONSE._serialized_end=19640
+  _DSSTUDYENDEDREQUEST._serialized_start=19643
+  _DSSTUDYENDEDREQUEST._serialized_end=19828
+  _DSSTUDYENDEDRESPONSE._serialized_start=19830
+  _DSSTUDYENDEDRESPONSE._serialized_end=19852
+  _SAVEOPTIMIZERDBREQUEST._serialized_start=19855
+  _SAVEOPTIMIZERDBREQUEST._serialized_end=20129
+  _SAVEOPTIMIZERDBRESPONSE._serialized_start=20131
+  _SAVEOPTIMIZERDBRESPONSE._serialized_end=20245
+  _DSGETDATABASESREQUEST._serialized_start=20247
+  _DSGETDATABASESREQUEST._serialized_end=20357
+  _DSGETDATABASESRESPONSE._serialized_start=20359
+  _DSGETDATABASESRESPONSE._serialized_end=20402
+  _DSGETTABLESREQUEST._serialized_start=20404
+  _DSGETTABLESREQUEST._serialized_end=20511
+  _DSGETTABLESRESPONSE._serialized_start=20513
+  _DSGETTABLESRESPONSE._serialized_end=20550
+  _DSEXECUTESQLREQUEST._serialized_start=20552
+  _DSEXECUTESQLREQUEST._serialized_end=20673
+  _DSEXECUTESQLRESPONSE._serialized_start=20675
+  _DSEXECUTESQLRESPONSE._serialized_end=20777
+  _DSSNAPSHOTREQUEST._serialized_start=20780
+  _DSSNAPSHOTREQUEST._serialized_end=21224
+  _DSSNAPSHOTRESPONSE._serialized_start=21226
+  _DSSNAPSHOTRESPONSE._serialized_end=21335
+  _ASKMODELRESPONSE._serialized_start=21337
+  _ASKMODELRESPONSE._serialized_end=21435
+  _GENTRAININGDATAREQUEST._serialized_start=21438
+  _GENTRAININGDATAREQUEST._serialized_end=21896
+  _GENTRAININGDATARESPONSE._serialized_start=21898
+  _GENTRAININGDATARESPONSE._serialized_end=22012
+  _SYNCONLINESTOREREQUEST._serialized_start=22015
+  _SYNCONLINESTOREREQUEST._serialized_end=22890
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _SYNCONLINESTOREREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_start=4396
   _SYNCONLINESTOREREQUEST_DBSECRETENTRY._serialized_end=4443
-  _SYNCONLINESTORERESPONSE._serialized_start=22979
-  _SYNCONLINESTORERESPONSE._serialized_end=23004
-  _GENONLINESTOREDATASETREQUEST._serialized_start=23007
-  _GENONLINESTOREDATASETREQUEST._serialized_end=23900
+  _SYNCONLINESTORERESPONSE._serialized_start=22892
+  _SYNCONLINESTORERESPONSE._serialized_end=22917
+  _GENONLINESTOREDATASETREQUEST._serialized_start=22920
+  _GENONLINESTOREDATASETREQUEST._serialized_end=23813
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _GENONLINESTOREDATASETREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_start=4396
   _GENONLINESTOREDATASETREQUEST_DBSECRETENTRY._serialized_end=4443
-  _GENONLINESTOREDATASETRESPONSE._serialized_start=23902
-  _GENONLINESTOREDATASETRESPONSE._serialized_end=24022
-  _BATCHPREDICTREQUEST._serialized_start=24025
-  _BATCHPREDICTREQUEST._serialized_end=25062
+  _GENONLINESTOREDATASETRESPONSE._serialized_start=23815
+  _GENONLINESTOREDATASETRESPONSE._serialized_end=23935
+  _BATCHPREDICTREQUEST._serialized_start=23938
+  _BATCHPREDICTREQUEST._serialized_end=24975
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_start=4342
   _BATCHPREDICTREQUEST_STORAGESECRETENTRY._serialized_end=4394
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_start=4396
   _BATCHPREDICTREQUEST_DBSECRETENTRY._serialized_end=4443
-  _BATCHPREDICTRESPONSE._serialized_start=25064
-  _BATCHPREDICTRESPONSE._serialized_end=25100
-  _SAVEDATASETREQUEST._serialized_start=25103
-  _SAVEDATASETREQUEST._serialized_end=25652
-  _SAVEMODELREQUEST._serialized_start=25655
-  _SAVEMODELREQUEST._serialized_end=26280
-  _SAVEPREDICTIONREQUEST._serialized_start=26283
-  _SAVEPREDICTIONREQUEST._serialized_end=26849
-  _SAVEPREDICTORREQUEST._serialized_start=26852
-  _SAVEPREDICTORREQUEST._serialized_end=27231
-  _CREATEMETRICSSTOREREQUEST._serialized_start=27234
-  _CREATEMETRICSSTOREREQUEST._serialized_end=27366
-  _CREATEMETRICSSTORERESPONSE._serialized_start=27368
-  _CREATEMETRICSSTORERESPONSE._serialized_end=27396
-  _SAVERESPONSE._serialized_start=27398
-  _SAVERESPONSE._serialized_end=27426
-  _DATASERVICE._serialized_start=27429
-  _DATASERVICE._serialized_end=35605
+  _BATCHPREDICTRESPONSE._serialized_start=24977
+  _BATCHPREDICTRESPONSE._serialized_end=25013
+  _SAVEDATASETREQUEST._serialized_start=25016
+  _SAVEDATASETREQUEST._serialized_end=25565
+  _SAVEMODELREQUEST._serialized_start=25568
+  _SAVEMODELREQUEST._serialized_end=26193
+  _SAVEPREDICTIONREQUEST._serialized_start=26196
+  _SAVEPREDICTIONREQUEST._serialized_end=26762
+  _SAVEPREDICTORREQUEST._serialized_start=26765
+  _SAVEPREDICTORREQUEST._serialized_end=27144
+  _CREATEMETRICSSTOREREQUEST._serialized_start=27147
+  _CREATEMETRICSSTOREREQUEST._serialized_end=27279
+  _CREATEMETRICSSTORERESPONSE._serialized_start=27281
+  _CREATEMETRICSSTORERESPONSE._serialized_end=27309
+  _SAVERESPONSE._serialized_start=27311
+  _SAVERESPONSE._serialized_end=27339
+  _DATASERVICE._serialized_start=27342
+  _DATASERVICE._serialized_end=35518
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -908,36 +908,34 @@
 class GroupByDatasetResponse(_message.Message):
     __slots__ = ["uri"]
     URI_FIELD_NUMBER: _ClassVar[int]
     uri: str
     def __init__(self, uri: _Optional[str] = ...) -> None: ...
 
 class RunTestSuiteRequest(_message.Message):
-    __slots__ = ["bucket", "connection", "dataset", "datasource", "histogram", "model", "product", "refHistogram", "study", "suite"]
+    __slots__ = ["bucket", "dataset", "datasource", "histogram", "model", "product", "refHistogram", "study", "suite"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
-    CONNECTION_FIELD_NUMBER: _ClassVar[int]
     DATASET_FIELD_NUMBER: _ClassVar[int]
     DATASOURCE_FIELD_NUMBER: _ClassVar[int]
     HISTOGRAM_FIELD_NUMBER: _ClassVar[int]
     MODEL_FIELD_NUMBER: _ClassVar[int]
     PRODUCT_FIELD_NUMBER: _ClassVar[int]
     REFHISTOGRAM_FIELD_NUMBER: _ClassVar[int]
     STUDY_FIELD_NUMBER: _ClassVar[int]
     SUITE_FIELD_NUMBER: _ClassVar[int]
     bucket: _generated_pb2_1_1_1.VirtualBucket
-    connection: _generated_pb2_1_1_1.Connection
     dataset: _generated_pb2.Dataset
     datasource: _generated_pb2.DataSource
     histogram: _generated_pb2.FeatureHistogram
     model: _generated_pb2_1.Model
     product: _generated_pb2.DataProduct
     refHistogram: _generated_pb2.FeatureHistogram
     study: _generated_pb2_1.Study
     suite: _generated_pb2_1_1_1_1.TestSuite
-    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., connection: _Optional[_Union[_generated_pb2_1_1_1.Connection, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., histogram: _Optional[_Union[_generated_pb2.FeatureHistogram, _Mapping]] = ..., refHistogram: _Optional[_Union[_generated_pb2.FeatureHistogram, _Mapping]] = ..., suite: _Optional[_Union[_generated_pb2_1_1_1_1.TestSuite, _Mapping]] = ...) -> None: ...
+    def __init__(self, product: _Optional[_Union[_generated_pb2.DataProduct, _Mapping]] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., dataset: _Optional[_Union[_generated_pb2.Dataset, _Mapping]] = ..., study: _Optional[_Union[_generated_pb2_1.Study, _Mapping]] = ..., model: _Optional[_Union[_generated_pb2_1.Model, _Mapping]] = ..., bucket: _Optional[_Union[_generated_pb2_1_1_1.VirtualBucket, _Mapping]] = ..., histogram: _Optional[_Union[_generated_pb2.FeatureHistogram, _Mapping]] = ..., refHistogram: _Optional[_Union[_generated_pb2.FeatureHistogram, _Mapping]] = ..., suite: _Optional[_Union[_generated_pb2_1_1_1_1.TestSuite, _Mapping]] = ...) -> None: ...
 
 class RunTestSuiteResponse(_message.Message):
     __slots__ = ["result"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     result: _generated_pb2_1_1_1_1.TestSuiteResult
     def __init__(self, result: _Optional[_Union[_generated_pb2_1_1_1_1.TestSuiteResult, _Mapping]] = ...) -> None: ...
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.pkg.apis.infra.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_infra_dot_v1alpha1_dot_generated__pb2
 from github.com.metaprov.modelaapi.services.common.v1 import common_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_services_dot_common_dot_v1_dot_common__pb2
 from github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_catalog_dot_v1alpha1_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/services/datasource/v1/datasource.proto\x12\x34github.com.metaprov.modelaapi.services.datasource.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\"\xfb\x01\n\x15ListDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12g\n\x06labels\x18\x02 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x8c\x01\n\x16ListDataSourceResponse\x12Y\n\x0b\x64\x61tasources\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x14GetDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"{\n\x15GetDataSourceResponse\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"\x9f\x01\n\x17UpdateDataSourceRequest\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x1a\n\x18UpdateDataSourceResponse\"o\n\x17\x43reateDataSourceRequest\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x1a\n\x18\x43reateDataSourceResponse\":\n\x17\x44\x65leteDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1a\n\x18\x44\x65leteDataSourceResponse\"\xd3\x01\n\x12InferSchemaRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"g\n\x13InferSchemaResponse\x12P\n\x07\x63olumns\x18\x01 \x03(\x0b\x32?.github.com.metaprov.modelaapi.services.common.v1.ColumnProfile\"\xd8\x01\n\x13GetTableViewRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12X\n\x06\x66ormat\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"b\n\x14GetTableViewResponse\x12J\n\x05table\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView2\xa2\x0c\n\x11\x44\x61taSourceService\x12\xd1\x01\n\x0fListDataSources\x12K.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceRequest\x1aL.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/datasources/{namespace}\x12\xcd\x01\n\x10\x43reateDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.CreateDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.CreateDataSourceResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/datasources:\x01*\x12\xd4\x01\n\rGetDataSource\x12J.github.com.metaprov.modelaapi.services.datasource.v1.GetDataSourceRequest\x1aK.github.com.metaprov.modelaapi.services.datasource.v1.GetDataSourceResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/datasources/{namespace}/{name}\x12\x88\x02\n\x10UpdateDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.UpdateDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.UpdateDataSourceResponse\"U\x82\xd3\xe4\x93\x02O\x1aJ/v1/datasources/{datasource.metadata.namespace}/{datasource.metadata.name}:\x01*\x12\xdd\x01\n\x10\x44\x65leteDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.DeleteDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.DeleteDataSourceResponse\"*\x82\xd3\xe4\x93\x02$*\"/v1/datasources/{namespace}/{name}\x12\xfc\x01\n\x0bInferSchema\x12H.github.com.metaprov.modelaapi.services.datasource.v1.InferSchemaRequest\x1aI.github.com.metaprov.modelaapi.services.datasource.v1.InferSchemaResponse\"X\x82\xd3\xe4\x93\x02R\"P/v1/datasources/{datasource.metadata.namespace}/{datasource.metadata.name}:infer\x12\xa7\x01\n\x0cGetTableView\x12I.github.com.metaprov.modelaapi.services.datasource.v1.GetTableViewRequest\x1aJ.github.com.metaprov.modelaapi.services.datasource.v1.GetTableViewResponse\"\x00\x42\x36Z4github.com/metaprov/modelaapi/services/datasource/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nEgithub.com/metaprov/modelaapi/services/datasource/v1/datasource.proto\x12\x34github.com.metaprov.modelaapi.services.datasource.v1\x1a google/protobuf/field_mask.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\x45github.com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated.proto\x1a=github.com/metaprov/modelaapi/services/common/v1/common.proto\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\"\xfb\x01\n\x15ListDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12g\n\x06labels\x18\x02 \x03(\x0b\x32W.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceRequest.LabelsEntry\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\x12\x10\n\x08order_by\x18\x05 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x8c\x01\n\x16ListDataSourceResponse\x12Y\n\x0b\x64\x61tasources\x18\x01 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSourceList\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"7\n\x14GetDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"{\n\x15GetDataSourceResponse\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12\x0c\n\x04yaml\x18\x02 \x01(\t\"\x9f\x01\n\x17UpdateDataSourceRequest\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12.\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\"\x1a\n\x18UpdateDataSourceResponse\"o\n\x17\x43reateDataSourceRequest\x12T\n\ndatasource\x18\x01 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\"\x1a\n\x18\x43reateDataSourceResponse\":\n\x17\x44\x65leteDataSourceRequest\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1a\n\x18\x44\x65leteDataSourceResponse\"\xd3\x01\n\x12InferSchemaRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12T\n\ndatasource\x18\x02 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataSource\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"p\n\x13InferSchemaResponse\x12Y\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FeatureStatistics\"\xd8\x01\n\x13GetTableViewRequest\x12\x0e\n\x06tenant\x18\x01 \x01(\t\x12X\n\x06\x66ormat\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"b\n\x14GetTableViewResponse\x12J\n\x05table\x18\x01 \x01(\x0b\x32;.github.com.metaprov.modelaapi.services.common.v1.TableView2\xa2\x0c\n\x11\x44\x61taSourceService\x12\xd1\x01\n\x0fListDataSources\x12K.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceRequest\x1aL.github.com.metaprov.modelaapi.services.datasource.v1.ListDataSourceResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/datasources/{namespace}\x12\xcd\x01\n\x10\x43reateDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.CreateDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.CreateDataSourceResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\"\x0f/v1/datasources:\x01*\x12\xd4\x01\n\rGetDataSource\x12J.github.com.metaprov.modelaapi.services.datasource.v1.GetDataSourceRequest\x1aK.github.com.metaprov.modelaapi.services.datasource.v1.GetDataSourceResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/datasources/{namespace}/{name}\x12\x88\x02\n\x10UpdateDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.UpdateDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.UpdateDataSourceResponse\"U\x82\xd3\xe4\x93\x02O\x1aJ/v1/datasources/{datasource.metadata.namespace}/{datasource.metadata.name}:\x01*\x12\xdd\x01\n\x10\x44\x65leteDataSource\x12M.github.com.metaprov.modelaapi.services.datasource.v1.DeleteDataSourceRequest\x1aN.github.com.metaprov.modelaapi.services.datasource.v1.DeleteDataSourceResponse\"*\x82\xd3\xe4\x93\x02$*\"/v1/datasources/{namespace}/{name}\x12\xfc\x01\n\x0bInferSchema\x12H.github.com.metaprov.modelaapi.services.datasource.v1.InferSchemaRequest\x1aI.github.com.metaprov.modelaapi.services.datasource.v1.InferSchemaResponse\"X\x82\xd3\xe4\x93\x02R\"P/v1/datasources/{datasource.metadata.namespace}/{datasource.metadata.name}:infer\x12\xa7\x01\n\x0cGetTableView\x12I.github.com.metaprov.modelaapi.services.datasource.v1.GetTableViewRequest\x1aJ.github.com.metaprov.modelaapi.services.datasource.v1.GetTableViewResponse\"\x00\x42\x36Z4github.com/metaprov/modelaapi/services/datasource/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.datasource.v1.datasource_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/metaprov/modelaapi/services/datasource/v1'
@@ -62,15 +62,15 @@
   _DELETEDATASOURCEREQUEST._serialized_start=1378
   _DELETEDATASOURCEREQUEST._serialized_end=1436
   _DELETEDATASOURCERESPONSE._serialized_start=1438
   _DELETEDATASOURCERESPONSE._serialized_end=1464
   _INFERSCHEMAREQUEST._serialized_start=1467
   _INFERSCHEMAREQUEST._serialized_end=1678
   _INFERSCHEMARESPONSE._serialized_start=1680
-  _INFERSCHEMARESPONSE._serialized_end=1783
-  _GETTABLEVIEWREQUEST._serialized_start=1786
-  _GETTABLEVIEWREQUEST._serialized_end=2002
-  _GETTABLEVIEWRESPONSE._serialized_start=2004
-  _GETTABLEVIEWRESPONSE._serialized_end=2102
-  _DATASOURCESERVICE._serialized_start=2105
-  _DATASOURCESERVICE._serialized_end=3675
+  _INFERSCHEMARESPONSE._serialized_end=1792
+  _GETTABLEVIEWREQUEST._serialized_start=1795
+  _GETTABLEVIEWREQUEST._serialized_end=2011
+  _GETTABLEVIEWRESPONSE._serialized_start=2013
+  _GETTABLEVIEWRESPONSE._serialized_end=2111
+  _DATASOURCESERVICE._serialized_start=2114
+  _DATASOURCESERVICE._serialized_end=3684
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -72,18 +72,18 @@
     TENANT_FIELD_NUMBER: _ClassVar[int]
     datasource: _generated_pb2.DataSource
     location: _generated_pb2_1_1.DataLocation
     tenant: str
     def __init__(self, tenant: _Optional[str] = ..., datasource: _Optional[_Union[_generated_pb2.DataSource, _Mapping]] = ..., location: _Optional[_Union[_generated_pb2_1_1.DataLocation, _Mapping]] = ...) -> None: ...
 
 class InferSchemaResponse(_message.Message):
-    __slots__ = ["columns"]
-    COLUMNS_FIELD_NUMBER: _ClassVar[int]
-    columns: _containers.RepeatedCompositeFieldContainer[_common_pb2.ColumnProfile]
-    def __init__(self, columns: _Optional[_Iterable[_Union[_common_pb2.ColumnProfile, _Mapping]]] = ...) -> None: ...
+    __slots__ = ["features"]
+    FEATURES_FIELD_NUMBER: _ClassVar[int]
+    features: _containers.RepeatedCompositeFieldContainer[_generated_pb2.FeatureStatistics]
+    def __init__(self, features: _Optional[_Iterable[_Union[_generated_pb2.FeatureStatistics, _Mapping]]] = ...) -> None: ...
 
 class ListDataSourceRequest(_message.Message):
     __slots__ = ["labels", "namespace", "order_by", "page_size", "page_token"]
     class LabelsEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.238/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/google/api/annotations_pb2.py` & `modelaapi-0.6.238/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/google/api/http_pb2.py` & `modelaapi-0.6.238/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/google/api/http_pb2.pyi` & `modelaapi-0.6.238/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/apps/v1/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/api/apps/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/core/v1/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/api/core/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/api/rbac/v1/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/api/rbac/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi` & `modelaapi-0.6.238/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/modelaapi/consts.py` & `modelaapi-0.6.238/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/modelaapi/custom_transformers.py` & `modelaapi-0.6.238/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/modelaapi/graykite_model.py` & `modelaapi-0.6.238/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/modelaapi/ts.py` & `modelaapi-0.6.238/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/modelaapi/version.py` & `modelaapi-0.6.238/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 236,
+    "micro": 238,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.236/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.238/modelaapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.236
+Version: 0.6.238
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.236
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.238
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.236
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.238
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.236/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.238/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/setup.cfg` & `modelaapi-0.6.238/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.236/setup.py` & `modelaapi-0.6.238/setup.py`

 * *Files identical despite different names*

