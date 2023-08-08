# Comparing `tmp/devcycle-python-server-sdk-3.3.4.tar.gz` & `tmp/devcycle-python-server-sdk-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.4.tar", last modified: Thu Jul 27 14:39:11 2023, max compression
+gzip compressed data, was "dist/devcycle-python-server-sdk-3.3.5.tar", last modified: Tue Aug  8 14:35:42 2023, max compression
```

## Comparing `devcycle-python-server-sdk-3.3.4.tar` & `devcycle-python-server-sdk-3.3.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/backoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/platform_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/cloud_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/example/local_bucketing_client_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_bucketing_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_config_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/api/test_local_bucketing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/fixture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/fixture/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/managers/test_event_queue_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/models/test_bucketed_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/test_cloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/test_local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:39:11.000000 devcycle-python-server-sdk-3.3.4/test/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-27 14:38:53.000000 devcycle-python-server-sdk-3.3.4/test/util/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-08 14:35:41.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 14:35:41.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-08 14:35:41.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 14:35:41.000000 devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/example/cloud_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/example/local_bucketing_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/api/test_bucketing_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/api/test_config_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/api/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15156 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/api/test_local_bucketing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/fixture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/fixture/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/managers/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/models/test_bucketed_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/test_cloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/test_local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:42.000000 devcycle-python-server-sdk-3.3.5/test/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/util/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-08 14:35:21.000000 devcycle-python-server-sdk-3.3.5/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-3.3.4/README.md` & `devcycle-python-server-sdk-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/config_client.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/event_client.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/api/local_bucketing.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/api/local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/cloud_client.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/local_client.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/config_manager.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/managers/event_queue_manager.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/managers/event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/bucketed_config.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/platform_data.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/platform_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/options.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/options.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/utils.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/utils.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py` & `devcycle-python-server-sdk-3.3.5/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.3.5/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/example/cloud_client_example.py` & `devcycle-python-server-sdk-3.3.5/example/cloud_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/example/local_bucketing_client_example.py` & `devcycle-python-server-sdk-3.3.5/example/local_bucketing_client_example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/pyproject.toml` & `devcycle-python-server-sdk-3.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/setup.py` & `devcycle-python-server-sdk-3.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.3.5/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/api/test_config_client.py` & `devcycle-python-server-sdk-3.3.5/test/api/test_config_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/api/test_event_client.py` & `devcycle-python-server-sdk-3.3.5/test/api/test_event_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/api/test_local_bucketing.py` & `devcycle-python-server-sdk-3.3.5/test/api/test_local_bucketing.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/fixture/data.py` & `devcycle-python-server-sdk-3.3.5/test/fixture/data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/managers/test_config_manager.py` & `devcycle-python-server-sdk-3.3.5/test/managers/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/managers/test_event_queue_manager.py` & `devcycle-python-server-sdk-3.3.5/test/managers/test_event_queue_manager.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/models/test_bucketed_config.py` & `devcycle-python-server-sdk-3.3.5/test/models/test_bucketed_config.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/test_cloud_client.py` & `devcycle-python-server-sdk-3.3.5/test/test_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/test_local_client.py` & `devcycle-python-server-sdk-3.3.5/test/test_local_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-3.3.4/test/util/test_utils.py` & `devcycle-python-server-sdk-3.3.5/test/util/test_utils.py`

 * *Files identical despite different names*

