# Comparing `tmp/ondewo-vtsi-client-6.4.0.tar.gz` & `tmp/ondewo-vtsi-client-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.4.0.tar", last modified: Sat Aug  5 17:45:00 2023, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.5.0.tar", last modified: Tue Aug  8 15:25:39 2023, max compression
```

## Comparing `ondewo-vtsi-client-6.4.0.tar` & `ondewo-vtsi-client-6.5.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9088 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8516 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.142465 ondewo-vtsi-client-6.4.0/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73267 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    87204 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    28593 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16826 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     1592 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    10331 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14789 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    29810 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    71700 2023-08-05 17:44:43.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59591 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3354 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2.py
--rw-rw-r--   0 root         (0) root         (0)      158 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7876 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    11374 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     9514 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    10478 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     7450 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16562 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6634 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    65793 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    59122 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    19597 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    27124 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    20143 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    16902 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     6345 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2.py
--rw-rw-r--   0 root         (0) root         (0)     6508 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11401 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    13389 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38422 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10949 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    21323 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    31234 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    33144 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    47012 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    35863 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10991 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     5017 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services_container.py
--rw-rw-r--   0 root         (0) root         (0)    17177 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    14451 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9088 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2023-08-05 17:44:45.000000 ondewo-vtsi-client-6.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.147290 ondewo-vtsi-client-6.5.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-08 15:25:39.148290 ondewo-vtsi-client-6.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.143290 ondewo-vtsi-client-6.5.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.145290 ondewo-vtsi-client-6.5.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73267 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28593 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1592 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10331 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29810 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    71700 2023-08-08 15:25:21.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3354 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7876 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9514 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7450 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    65793 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19597 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20143 2023-08-08 15:25:21.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6345 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.145290 ondewo-vtsi-client-6.5.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11401 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.146290 ondewo-vtsi-client-6.5.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38422 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.146290 ondewo-vtsi-client-6.5.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10949 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    21323 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.146290 ondewo-vtsi-client-6.5.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31234 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.146290 ondewo-vtsi-client-6.5.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    47012 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    35863 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.147290 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.147290 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10991 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     5017 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-08-08 15:23:52.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    17264 2023-08-08 15:25:20.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14451 2023-08-08 15:25:19.000000 ondewo-vtsi-client-6.5.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:25:39.147290 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-08 15:25:39.000000 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-08-08 15:25:39.000000 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:25:39.000000 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-08-08 15:25:39.000000 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-08 15:25:39.000000 ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-08-08 15:25:39.148290 ondewo-vtsi-client-6.5.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-08-08 15:25:24.000000 ondewo-vtsi-client-6.5.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.4.0/LICENSE` & `ondewo-vtsi-client-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/PKG-INFO` & `ondewo-vtsi-client-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.4.0
+Version: 6.5.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.4.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.5.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.4.0/README.md` & `ondewo-vtsi-client-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/calls_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/calls.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/calls.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/projects.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/client/services/projects.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/projects_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aondewo/vtsi/projects.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa5\x03\n\x0bVtsiProject\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0bmax_callers\x18\x03 \x01(\x05\x12\x15\n\rmax_listeners\x18\x04 \x01(\x05\x12\x36\n\x10\x61sterisk_configs\x18\x05 \x01(\x0b\x32\x1c.ondewo.vtsi.AsteriskConfigs\x12;\n\x13vtsi_project_status\x18\x06 \x01(\x0e\x32\x1e.ondewo.vtsi.VtsiProjectStatus\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bmodified_by\x18\t \x01(\t\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x61\x63tive_callers\x18\x0b \x01(\x05\x12\x18\n\x10\x61\x63tive_listeners\x18\x0c \x01(\x05\x12\x15\n\rasterisk_port\x18\r \x01(\x05\"\xc1\x01\n\x18\x41steriskConfigsVariables\x12\x1a\n\x12sip_trunk_username\x18\x01 \x01(\t\x12\x1a\n\x12sip_trunk_password\x18\x02 \x01(\t\x12\x16\n\x0esip_trunk_host\x18\x03 \x01(\t\x12\x17\n\x0ftransfer_number\x18\x04 \x01(\t\x12\x1c\n\x14transfer_number_host\x18\x05 \x01(\t\x12\x1e\n\x16sip_trunk_phone_number\x18\x06 \x01(\t\"\x9c\x01\n\x14\x41steriskConfigsFiles\x12\x1c\n\x14sip_conf_file_string\x18\x01 \x01(\t\x12#\n\x1b\x65xtensions_conf_file_string\x18\x02 \x01(\t\x12\x1f\n\x17queues_conf_file_string\x18\x03 \x01(\t\x12 \n\x18modules_conf_file_string\x18\x04 \x01(\t\"\x86\x02\n\x0f\x41steriskConfigs\x12K\n\x1a\x61sterisk_configs_variables\x18\x01 \x01(\x0b\x32%.ondewo.vtsi.AsteriskConfigsVariablesH\x00\x12\x43\n\x16\x61sterisk_configs_files\x18\x02 \x01(\x0b\x32!.ondewo.vtsi.AsteriskConfigsFilesH\x00\x12\x30\n&asterisk_configs_target_directory_name\x18\x03 \x01(\tH\x00\x12\x15\n\rasterisk_port\x18\x04 \x01(\x05\x42\x18\n\x16\x61sterisk_configs_oneof\"a\n\x18\x43reateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"b\n\x19\x43reateVtsiProjectResponse\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"%\n\x15GetVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd7\x01\n\x17ListVtsiProjectsRequest\x12\x37\n\x11vtsi_project_view\x18\x01 \x01(\x0e\x32\x1c.ondewo.vtsi.VtsiProjectView\x12\x17\n\npage_token\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x42\n\x14vtsi_project_sorting\x18\x03 \x01(\x0b\x32\x1f.ondewo.vtsi.VtsiProjectSortingH\x01\x88\x01\x01\x42\r\n\x0b_page_tokenB\x17\n\x15_vtsi_project_sorting\"d\n\x18ListVtsiProjectsResponse\x12/\n\rvtsi_projects\x18\x01 \x03(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x9b\x03\n\x12VtsiProjectSorting\x12S\n\rsorting_field\x18\x01 \x01(\x0e\x32\x37.ondewo.vtsi.VtsiProjectSorting.VtsiProjectSortingFieldH\x00\x88\x01\x01\x12>\n\x0csorting_mode\x18\x02 \x01(\x0e\x32#.ondewo.vtsi.VtsiProjectSortingModeH\x01\x88\x01\x01\"\xcc\x01\n\x17VtsiProjectSortingField\x12\x1b\n\x17NO_VTSI_PROJECT_SORTING\x10\x00\x12\x1d\n\x19SORT_VTSI_PROJECT_BY_NAME\x10\x01\x12%\n!SORT_VTSI_PROJECT_BY_DISPLAY_NAME\x10\x02\x12&\n\"SORT_VTSI_PROJECT_BY_CREATION_DATE\x10\x03\x12&\n\"SORT_VTSI_PROJECT_BY_LAST_MODIFIED\x10\x04\x42\x10\n\x0e_sorting_fieldB\x0f\n\r_sorting_mode\"J\n\x18UpdateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\"@\n\x19UpdateVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65leteVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65leteVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65ployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65ployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"*\n\x1aUndeployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"B\n\x1bUndeployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x8b\x01\n\x11VtsiProjectStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nUNDEPLOYED\x10\x01\x12\x0c\n\x08UPDATING\x10\x02\x12\r\n\tDEPLOYING\x10\x03\x12\x0c\n\x08\x44\x45PLOYED\x10\x04\x12\x0f\n\x0bUNDEPLOYING\x10\x05\x12\x0c\n\x08\x44\x45LETING\x10\x06\x12\x0b\n\x07\x44\x45LETED\x10\x07*7\n\x16VtsiProjectSortingMode\x12\r\n\tASCENDING\x10\x00\x12\x0e\n\nDESCENDING\x10\x01*\x8e\x01\n\x0fVtsiProjectView\x12!\n\x1dVTSI_PROJECT_VIEW_UNSPECIFIED\x10\x00\x12\x1a\n\x16VTSI_PROJECT_VIEW_FULL\x10\x01\x12\x1d\n\x19VTSI_PROJECT_VIEW_SHALLOW\x10\x02\x12\x1d\n\x19VTSI_PROJECT_VIEW_MINIMUM\x10\x03\x32\xb5\x05\n\x08Projects\x12\x62\n\x11\x43reateVtsiProject\x12%.ondewo.vtsi.CreateVtsiProjectRequest\x1a&.ondewo.vtsi.CreateVtsiProjectResponse\x12N\n\x0eGetVtsiProject\x12\".ondewo.vtsi.GetVtsiProjectRequest\x1a\x18.ondewo.vtsi.VtsiProject\x12\x62\n\x11UpdateVtsiProject\x12%.ondewo.vtsi.UpdateVtsiProjectRequest\x1a&.ondewo.vtsi.UpdateVtsiProjectResponse\x12\x62\n\x11\x44\x65leteVtsiProject\x12%.ondewo.vtsi.DeleteVtsiProjectRequest\x1a&.ondewo.vtsi.DeleteVtsiProjectResponse\x12\x62\n\x11\x44\x65ployVtsiProject\x12%.ondewo.vtsi.DeployVtsiProjectRequest\x1a&.ondewo.vtsi.DeployVtsiProjectResponse\x12h\n\x13UndeployVtsiProject\x12\'.ondewo.vtsi.UndeployVtsiProjectRequest\x1a(.ondewo.vtsi.UndeployVtsiProjectResponse\x12_\n\x10ListVtsiProjects\x12$.ondewo.vtsi.ListVtsiProjectsRequest\x1a%.ondewo.vtsi.ListVtsiProjectsResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aondewo/vtsi/projects.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xbe\x03\n\x0bVtsiProject\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0bmax_callers\x18\x03 \x01(\x05\x12\x15\n\rmax_listeners\x18\x04 \x01(\x05\x12\x36\n\x10\x61sterisk_configs\x18\x05 \x01(\x0b\x32\x1c.ondewo.vtsi.AsteriskConfigs\x12;\n\x13vtsi_project_status\x18\x06 \x01(\x0e\x32\x1e.ondewo.vtsi.VtsiProjectStatus\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bmodified_by\x18\t \x01(\t\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x61\x63tive_callers\x18\x0b \x01(\x05\x12\x18\n\x10\x61\x63tive_listeners\x18\x0c \x01(\x05\x12\x15\n\rasterisk_port\x18\r \x01(\x05\x12\x17\n\x0fnlu_agent_names\x18\x0e \x03(\t\"\xc1\x01\n\x18\x41steriskConfigsVariables\x12\x1a\n\x12sip_trunk_username\x18\x01 \x01(\t\x12\x1a\n\x12sip_trunk_password\x18\x02 \x01(\t\x12\x16\n\x0esip_trunk_host\x18\x03 \x01(\t\x12\x17\n\x0ftransfer_number\x18\x04 \x01(\t\x12\x1c\n\x14transfer_number_host\x18\x05 \x01(\t\x12\x1e\n\x16sip_trunk_phone_number\x18\x06 \x01(\t\"\x9c\x01\n\x14\x41steriskConfigsFiles\x12\x1c\n\x14sip_conf_file_string\x18\x01 \x01(\t\x12#\n\x1b\x65xtensions_conf_file_string\x18\x02 \x01(\t\x12\x1f\n\x17queues_conf_file_string\x18\x03 \x01(\t\x12 \n\x18modules_conf_file_string\x18\x04 \x01(\t\"\x86\x02\n\x0f\x41steriskConfigs\x12K\n\x1a\x61sterisk_configs_variables\x18\x01 \x01(\x0b\x32%.ondewo.vtsi.AsteriskConfigsVariablesH\x00\x12\x43\n\x16\x61sterisk_configs_files\x18\x02 \x01(\x0b\x32!.ondewo.vtsi.AsteriskConfigsFilesH\x00\x12\x30\n&asterisk_configs_target_directory_name\x18\x03 \x01(\tH\x00\x12\x15\n\rasterisk_port\x18\x04 \x01(\x05\x42\x18\n\x16\x61sterisk_configs_oneof\"a\n\x18\x43reateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"b\n\x19\x43reateVtsiProjectResponse\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"%\n\x15GetVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xf0\x01\n\x17ListVtsiProjectsRequest\x12\x37\n\x11vtsi_project_view\x18\x01 \x01(\x0e\x32\x1c.ondewo.vtsi.VtsiProjectView\x12\x17\n\npage_token\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x42\n\x14vtsi_project_sorting\x18\x03 \x01(\x0b\x32\x1f.ondewo.vtsi.VtsiProjectSortingH\x01\x88\x01\x01\x12\x17\n\x0fnlu_agent_names\x18\x04 \x03(\tB\r\n\x0b_page_tokenB\x17\n\x15_vtsi_project_sorting\"d\n\x18ListVtsiProjectsResponse\x12/\n\rvtsi_projects\x18\x01 \x03(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x9b\x03\n\x12VtsiProjectSorting\x12S\n\rsorting_field\x18\x01 \x01(\x0e\x32\x37.ondewo.vtsi.VtsiProjectSorting.VtsiProjectSortingFieldH\x00\x88\x01\x01\x12>\n\x0csorting_mode\x18\x02 \x01(\x0e\x32#.ondewo.vtsi.VtsiProjectSortingModeH\x01\x88\x01\x01\"\xcc\x01\n\x17VtsiProjectSortingField\x12\x1b\n\x17NO_VTSI_PROJECT_SORTING\x10\x00\x12\x1d\n\x19SORT_VTSI_PROJECT_BY_NAME\x10\x01\x12%\n!SORT_VTSI_PROJECT_BY_DISPLAY_NAME\x10\x02\x12&\n\"SORT_VTSI_PROJECT_BY_CREATION_DATE\x10\x03\x12&\n\"SORT_VTSI_PROJECT_BY_LAST_MODIFIED\x10\x04\x42\x10\n\x0e_sorting_fieldB\x0f\n\r_sorting_mode\"J\n\x18UpdateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\"@\n\x19UpdateVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65leteVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65leteVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65ployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65ployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"*\n\x1aUndeployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"B\n\x1bUndeployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x8b\x01\n\x11VtsiProjectStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nUNDEPLOYED\x10\x01\x12\x0c\n\x08UPDATING\x10\x02\x12\r\n\tDEPLOYING\x10\x03\x12\x0c\n\x08\x44\x45PLOYED\x10\x04\x12\x0f\n\x0bUNDEPLOYING\x10\x05\x12\x0c\n\x08\x44\x45LETING\x10\x06\x12\x0b\n\x07\x44\x45LETED\x10\x07*7\n\x16VtsiProjectSortingMode\x12\r\n\tASCENDING\x10\x00\x12\x0e\n\nDESCENDING\x10\x01*\x8e\x01\n\x0fVtsiProjectView\x12!\n\x1dVTSI_PROJECT_VIEW_UNSPECIFIED\x10\x00\x12\x1a\n\x16VTSI_PROJECT_VIEW_FULL\x10\x01\x12\x1d\n\x19VTSI_PROJECT_VIEW_SHALLOW\x10\x02\x12\x1d\n\x19VTSI_PROJECT_VIEW_MINIMUM\x10\x03\x32\xb5\x05\n\x08Projects\x12\x62\n\x11\x43reateVtsiProject\x12%.ondewo.vtsi.CreateVtsiProjectRequest\x1a&.ondewo.vtsi.CreateVtsiProjectResponse\x12N\n\x0eGetVtsiProject\x12\".ondewo.vtsi.GetVtsiProjectRequest\x1a\x18.ondewo.vtsi.VtsiProject\x12\x62\n\x11UpdateVtsiProject\x12%.ondewo.vtsi.UpdateVtsiProjectRequest\x1a&.ondewo.vtsi.UpdateVtsiProjectResponse\x12\x62\n\x11\x44\x65leteVtsiProject\x12%.ondewo.vtsi.DeleteVtsiProjectRequest\x1a&.ondewo.vtsi.DeleteVtsiProjectResponse\x12\x62\n\x11\x44\x65ployVtsiProject\x12%.ondewo.vtsi.DeployVtsiProjectRequest\x1a&.ondewo.vtsi.DeployVtsiProjectResponse\x12h\n\x13UndeployVtsiProject\x12\'.ondewo.vtsi.UndeployVtsiProjectRequest\x1a(.ondewo.vtsi.UndeployVtsiProjectResponse\x12_\n\x10ListVtsiProjects\x12$.ondewo.vtsi.ListVtsiProjectsRequest\x1a%.ondewo.vtsi.ListVtsiProjectsResponseb\x06proto3')
 
 _VTSIPROJECTSTATUS = DESCRIPTOR.enum_types_by_name['VtsiProjectStatus']
 VtsiProjectStatus = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTSTATUS)
 _VTSIPROJECTSORTINGMODE = DESCRIPTOR.enum_types_by_name['VtsiProjectSortingMode']
 VtsiProjectSortingMode = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTSORTINGMODE)
 _VTSIPROJECTVIEW = DESCRIPTOR.enum_types_by_name['VtsiProjectView']
 VtsiProjectView = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTVIEW)
@@ -184,54 +184,54 @@
 })
 _sym_db.RegisterMessage(UndeployVtsiProjectResponse)
 
 _PROJECTS = DESCRIPTOR.services_by_name['Projects']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _VTSIPROJECTSTATUS._serialized_start=2593
-    _VTSIPROJECTSTATUS._serialized_end=2732
-    _VTSIPROJECTSORTINGMODE._serialized_start=2734
-    _VTSIPROJECTSORTINGMODE._serialized_end=2789
-    _VTSIPROJECTVIEW._serialized_start=2792
-    _VTSIPROJECTVIEW._serialized_end=2934
+    _VTSIPROJECTSTATUS._serialized_start=2643
+    _VTSIPROJECTSTATUS._serialized_end=2782
+    _VTSIPROJECTSORTINGMODE._serialized_start=2784
+    _VTSIPROJECTSORTINGMODE._serialized_end=2839
+    _VTSIPROJECTVIEW._serialized_start=2842
+    _VTSIPROJECTVIEW._serialized_end=2984
     _VTSIPROJECT._serialized_start=107
-    _VTSIPROJECT._serialized_end=528
-    _ASTERISKCONFIGSVARIABLES._serialized_start=531
-    _ASTERISKCONFIGSVARIABLES._serialized_end=724
-    _ASTERISKCONFIGSFILES._serialized_start=727
-    _ASTERISKCONFIGSFILES._serialized_end=883
-    _ASTERISKCONFIGS._serialized_start=886
-    _ASTERISKCONFIGS._serialized_end=1148
-    _CREATEVTSIPROJECTREQUEST._serialized_start=1150
-    _CREATEVTSIPROJECTREQUEST._serialized_end=1247
-    _CREATEVTSIPROJECTRESPONSE._serialized_start=1249
-    _CREATEVTSIPROJECTRESPONSE._serialized_end=1347
-    _GETVTSIPROJECTREQUEST._serialized_start=1349
-    _GETVTSIPROJECTREQUEST._serialized_end=1386
-    _LISTVTSIPROJECTSREQUEST._serialized_start=1389
-    _LISTVTSIPROJECTSREQUEST._serialized_end=1604
-    _LISTVTSIPROJECTSRESPONSE._serialized_start=1606
-    _LISTVTSIPROJECTSRESPONSE._serialized_end=1706
-    _VTSIPROJECTSORTING._serialized_start=1709
-    _VTSIPROJECTSORTING._serialized_end=2120
-    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_start=1881
-    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_end=2085
-    _UPDATEVTSIPROJECTREQUEST._serialized_start=2122
-    _UPDATEVTSIPROJECTREQUEST._serialized_end=2196
-    _UPDATEVTSIPROJECTRESPONSE._serialized_start=2198
-    _UPDATEVTSIPROJECTRESPONSE._serialized_end=2262
-    _DELETEVTSIPROJECTREQUEST._serialized_start=2264
-    _DELETEVTSIPROJECTREQUEST._serialized_end=2304
-    _DELETEVTSIPROJECTRESPONSE._serialized_start=2306
-    _DELETEVTSIPROJECTRESPONSE._serialized_end=2370
-    _DEPLOYVTSIPROJECTREQUEST._serialized_start=2372
-    _DEPLOYVTSIPROJECTREQUEST._serialized_end=2412
-    _DEPLOYVTSIPROJECTRESPONSE._serialized_start=2414
-    _DEPLOYVTSIPROJECTRESPONSE._serialized_end=2478
-    _UNDEPLOYVTSIPROJECTREQUEST._serialized_start=2480
-    _UNDEPLOYVTSIPROJECTREQUEST._serialized_end=2522
-    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_start=2524
-    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_end=2590
-    _PROJECTS._serialized_start=2937
-    _PROJECTS._serialized_end=3630
+    _VTSIPROJECT._serialized_end=553
+    _ASTERISKCONFIGSVARIABLES._serialized_start=556
+    _ASTERISKCONFIGSVARIABLES._serialized_end=749
+    _ASTERISKCONFIGSFILES._serialized_start=752
+    _ASTERISKCONFIGSFILES._serialized_end=908
+    _ASTERISKCONFIGS._serialized_start=911
+    _ASTERISKCONFIGS._serialized_end=1173
+    _CREATEVTSIPROJECTREQUEST._serialized_start=1175
+    _CREATEVTSIPROJECTREQUEST._serialized_end=1272
+    _CREATEVTSIPROJECTRESPONSE._serialized_start=1274
+    _CREATEVTSIPROJECTRESPONSE._serialized_end=1372
+    _GETVTSIPROJECTREQUEST._serialized_start=1374
+    _GETVTSIPROJECTREQUEST._serialized_end=1411
+    _LISTVTSIPROJECTSREQUEST._serialized_start=1414
+    _LISTVTSIPROJECTSREQUEST._serialized_end=1654
+    _LISTVTSIPROJECTSRESPONSE._serialized_start=1656
+    _LISTVTSIPROJECTSRESPONSE._serialized_end=1756
+    _VTSIPROJECTSORTING._serialized_start=1759
+    _VTSIPROJECTSORTING._serialized_end=2170
+    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_start=1931
+    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_end=2135
+    _UPDATEVTSIPROJECTREQUEST._serialized_start=2172
+    _UPDATEVTSIPROJECTREQUEST._serialized_end=2246
+    _UPDATEVTSIPROJECTRESPONSE._serialized_start=2248
+    _UPDATEVTSIPROJECTRESPONSE._serialized_end=2312
+    _DELETEVTSIPROJECTREQUEST._serialized_start=2314
+    _DELETEVTSIPROJECTREQUEST._serialized_end=2354
+    _DELETEVTSIPROJECTRESPONSE._serialized_start=2356
+    _DELETEVTSIPROJECTRESPONSE._serialized_end=2420
+    _DEPLOYVTSIPROJECTREQUEST._serialized_start=2422
+    _DEPLOYVTSIPROJECTREQUEST._serialized_end=2462
+    _DEPLOYVTSIPROJECTRESPONSE._serialized_start=2464
+    _DEPLOYVTSIPROJECTRESPONSE._serialized_end=2528
+    _UNDEPLOYVTSIPROJECTREQUEST._serialized_start=2530
+    _UNDEPLOYVTSIPROJECTREQUEST._serialized_end=2572
+    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_start=2574
+    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_end=2640
+    _PROJECTS._serialized_start=2987
+    _PROJECTS._serialized_end=3680
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-6.5.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.4.0
+Version: 6.5.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.4.0 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.5.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.5.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.4.0/setup.py` & `ondewo-vtsi-client-6.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.4.0',
+    version='6.5.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
```

