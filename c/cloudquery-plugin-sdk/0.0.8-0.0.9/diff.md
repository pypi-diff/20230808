# Comparing `tmp/cloudquery-plugin-sdk-0.0.8.tar.gz` & `tmp/cloudquery-plugin-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudquery-plugin-sdk-0.0.8.tar", last modified: Tue Aug  1 13:01:21 2023, max compression
+gzip compressed data, was "cloudquery-plugin-sdk-0.0.9.tar", last modified: Wed Aug  2 14:15:25 2023, max compression
```

## Comparing `cloudquery-plugin-sdk-0.0.8.tar` & `cloudquery-plugin-sdk-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.090550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/markdown_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/memdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.094550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/int.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/table_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/serve/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.098550 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 13:00:57.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 13:01:21.000000 cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 13:01:21.102550 cloudquery-plugin-sdk-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-01 13:00:53.000000 cloudquery-plugin-sdk-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/markdown_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/memdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/memdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/memdb/memdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/discovery_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/discovery_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/discovery_v1/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.309185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/plugin_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/plugin_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/plugin_v3/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.313185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/message/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/message/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/message/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.313185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.313185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/date32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/date64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/scalar_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.313185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/table_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.313185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/serve/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/transformers/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:14:55.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 14:15:25.000000 cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-02 14:15:25.317185 cloudquery-plugin-sdk-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-02 14:14:48.000000 cloudquery-plugin-sdk-0.0.9/setup.py
```

### Comparing `cloudquery-plugin-sdk-0.0.8/PKG-INFO` & `cloudquery-plugin-sdk-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/generator.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/generator.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/docs/markdown_templates.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/docs/markdown_templates.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/memdb/memdb.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/memdb/memdb.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/internal/servers/plugin_v3/plugin.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/internal/servers/plugin_v3/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/message/write.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/message/write.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/plugin/plugin.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/plugin/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     def __init__(self, name: str, version: str) -> None:
         self._name = name
         self._version = version
 
     def init(self, spec: bytes) -> None:
         pass
 
+    def set_logger(self, logger) -> None:
+        pass
+
     def name(self) -> str:
         return self._name
 
     def version(self) -> str:
         return self._version
 
     def get_tables(self, options: TableOptions) -> List[Table]:
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/binary.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/binary.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/bool.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/bool.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date32.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/date32.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/date64.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/date64.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/float.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/float.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/int.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/int.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/json.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/json.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/list.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/list.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/scalar.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/scalar_factory.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/scalar_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from cloudquery.sdk.types import UUIDType, JSONType
 from .binary import Binary
 from .bool import Bool
 from .date32 import Date32
 from .date64 import Date64
 from .float import Float
 from .int import Int
+from .json import JSON
 from .list import List
 from .scalar import ScalarInvalidTypeError
 from .string import String
 from .timestamp import Timestamp
 from .uint import Uint
 from .uuid import UUID
 
@@ -85,10 +86,10 @@
         # elif dt_id == pa.types.lib.Type_TIME64:
         #     return ()
         elif dt_id == pa.types.lib.Type_TIMESTAMP:
             return Timestamp()
         elif dt == UUIDType():
             return UUID()
         elif dt == JSONType():
-            return String()
+            return JSON()
         else:
             raise ScalarInvalidTypeError("Invalid type {} for scalar".format(dt))
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/string.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/string.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from cloudquery.sdk.scalar import Scalar, ScalarInvalidTypeError
-from .scalar import NULL_VALUE
 
 
 class String(Scalar):
     def __eq__(self, scalar: Scalar) -> bool:
         if scalar is None:
             return False
         if type(scalar) == String:
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/timestamp.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/timestamp.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uint.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/uint.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/uuid.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/uuid.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scalar/vector.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scalar/vector.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/scheduler.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 
 from cloudquery.sdk.message import (
     SyncMessage,
     SyncInsertMessage,
     SyncMigrateTableMessage,
 )
 from cloudquery.sdk.schema import Resource
-from .table_resolver import TableResolver
+from .table_resolver import TableResolver, Client
 
 QUEUE_PER_WORKER = 100
 
 
 class ThreadPoolExecutorWithQueueSizeLimit(futures.ThreadPoolExecutor):
     def __init__(self, maxsize, *args, **kwargs):
         super(ThreadPoolExecutorWithQueueSizeLimit, self).__init__(*args, **kwargs)
         self._work_queue = queue.Queue(maxsize=maxsize)
 
 
 class TableResolverStarted:
-    def __init__(self, count=1) -> None:
-        self._count = count
-
-    @property
-    def count(self):
-        return self._count
+    def __init__(self) -> None:
+        pass
 
 
 class TableResolverFinished:
     def __init__(self) -> None:
         pass
 
 
@@ -39,14 +35,16 @@
     def __init__(
         self, concurrency: int, queue_size: int = 0, max_depth: int = 3, logger=None
     ):
         self._queue = queue.Queue()
         self._max_depth = max_depth
         if logger is None:
             self._logger = structlog.get_logger()
+        else:
+            self._logger = logger
         if concurrency <= 0:
             raise ValueError("concurrency must be greater than 0")
         if max_depth <= 0:
             raise ValueError("max_depth must be greater than 0")
         self._queue_size = (
             queue_size if queue_size > 0 else concurrency * QUEUE_PER_WORKER
         )
@@ -68,126 +66,141 @@
             )
 
     def shutdown(self):
         for pool in self._pools:
             pool.shutdown()
 
     def resolve_resource(
-        self, resolver: TableResolver, client, parent: Resource, item: Any
+        self, resolver: TableResolver, client: Client, parent: Resource, item: Any
     ) -> Resource:
         resource = Resource(resolver.table, parent, item)
         resolver.pre_resource_resolve(client, resource)
         for column in resolver.table.columns:
             resolver.resolve_column(client, resource, column.name)
         resolver.post_resource_resolve(client, resource)
         return resource
 
     def resolve_table(
         self,
         resolver: TableResolver,
         depth: int,
-        client,
+        client: Client,
         parent_item: Resource,
         res: queue.Queue,
     ):
-        table_resolvers_started = 0
         try:
             if depth == 0:
                 self._logger.info(
-                    "table resolver started", table=resolver.table.name, depth=depth
+                    "table resolver started",
+                    client_id=client.id(),
+                    table=resolver.table.name,
+                    depth=depth,
                 )
             else:
                 self._logger.debug(
-                    "table resolver started", table=resolver.table.name, depth=depth
+                    "table resolver started",
+                    client_id=client.id(),
+                    table=resolver.table.name,
+                    depth=depth,
                 )
             total_resources = 0
             for item in resolver.resolve(client, parent_item):
                 try:
                     resource = self.resolve_resource(
                         resolver, client, parent_item, item
                     )
                 except Exception as e:
                     self._logger.error(
                         "failed to resolve resource",
+                        client_id=client.id(),
                         table=resolver.table.name,
                         depth=depth,
-                        exception=e,
+                        exc_info=True,
                     )
                     continue
                 res.put(SyncInsertMessage(resource.to_arrow_record()))
                 for child_resolvers in resolver.child_resolvers:
+                    res.put(TableResolverStarted())
                     self._pools[depth + 1].submit(
                         self.resolve_table,
                         child_resolvers,
                         depth + 1,
                         client,
                         resource,
                         res,
                     )
-                    table_resolvers_started += 1
                 total_resources += 1
             if depth == 0:
                 self._logger.info(
                     "table resolver finished successfully",
+                    client_id=client.id(),
                     table=resolver.table.name,
+                    resources=total_resources,
                     depth=depth,
                 )
             else:
                 self._logger.debug(
                     "table resolver finished successfully",
+                    client_id=client.id(),
                     table=resolver.table.name,
+                    resources=total_resources,
                     depth=depth,
                 )
         except Exception as e:
             self._logger.error(
                 "table resolver finished with error",
+                client_id=client.id(),
                 table=resolver.table.name,
+                resources=total_resources,
                 depth=depth,
-                exception=e,
+                exc_info=True,
             )
         finally:
-            res.put(TableResolverStarted(count=table_resolvers_started))
             res.put(TableResolverFinished())
 
     def _sync(
         self,
         client,
         resolvers: List[TableResolver],
         res: queue.Queue,
         deterministic_cq_id=False,
     ):
-        total_table_resolvers = 0
-        try:
-            for resolver in resolvers:
-                clients = resolver.multiplex(client)
-                for client in clients:
-                    self._pools[0].submit(
-                        self.resolve_table, resolver, 0, client, None, res
-                    )
-                    total_table_resolvers += 1
-        finally:
-            res.put(TableResolverStarted(total_table_resolvers))
+        for resolver in resolvers:
+            clients = resolver.multiplex(client)
+            for client in clients:
+                res.put(TableResolverStarted())
+                self._pools[0].submit(
+                    self.resolve_table, resolver, 0, client, None, res
+                )
 
     def sync(
         self, client, resolvers: List[TableResolver], deterministic_cq_id=False
     ) -> Generator[SyncMessage, None, None]:
         res = queue.Queue()
-        for resolver in resolvers:
-            yield SyncMigrateTableMessage(table=resolver.table.to_arrow_schema())
+        yield from self._send_migrate_table_messages(resolvers)
+
         thread = futures.ThreadPoolExecutor()
         thread.submit(self._sync, client, resolvers, res, deterministic_cq_id)
         total_table_resolvers = 0
         finished_table_resolvers = 0
         while True:
             message = res.get()
             if type(message) == TableResolverStarted:
-                total_table_resolvers += message.count
+                total_table_resolvers += 1
                 if total_table_resolvers == finished_table_resolvers:
                     break
                 continue
             elif type(message) == TableResolverFinished:
                 finished_table_resolvers += 1
                 if total_table_resolvers == finished_table_resolvers:
                     break
                 continue
             yield message
         thread.shutdown(wait=True)
+
+    def _send_migrate_table_messages(
+        self, resolvers: List[TableResolver]
+    ) -> Generator[SyncMessage, None, None]:
+        for resolver in resolvers:
+            yield SyncMigrateTableMessage(table=resolver.table.to_arrow_schema())
+            if resolver.child_resolvers:
+                yield from self._send_migrate_table_messages(resolver.child_resolvers)
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/scheduler/table_resolver.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/scheduler/table_resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from cloudquery.sdk.schema.table import Table
 from cloudquery.sdk.schema import Resource
-from typing import Any, Generator
+from typing import Any, Generator, List
+
+
+class Client:
+    def id(self) -> str:
+        raise NotImplementedError()
+
+
+from cloudquery.sdk.schema import Resource
+from cloudquery.sdk.schema.table import Table
 
 
 class TableResolver:
     def __init__(self, table: Table, child_resolvers=[]) -> None:
         self._table = table
         self._child_resolvers = child_resolvers
 
@@ -12,26 +21,26 @@
     def table(self) -> Table:
         return self._table
 
     @property
     def child_resolvers(self):
         return self._child_resolvers
 
-    def multiplex(self, client):
+    def multiplex(self, client: Client) -> List[Client]:
         return [client]
 
     def resolve(self, client, parent_resource) -> Generator[Any, None, None]:
         raise NotImplementedError()
 
-    def pre_resource_resolve(self, client, resource):
+    def pre_resource_resolve(self, client: Client, resource):
         return
 
-    def resolve_column(self, client, resource: Resource, column_name: str):
+    def resolve_column(self, client: Client, resource: Resource, column_name: str):
         if type(resource.item) is dict:
             if column_name in resource.item:
                 resource.set(column_name, resource.item[column_name])
         else:
             if hasattr(resource.item, column_name):
-                resource.set(column_name, resource.item[column_name])
+                resource.set(column_name, getattr(resource.item, column_name))
 
-    def post_resource_resolve(self, client, resource):
+    def post_resource_resolve(self, client: Client, resource):
         return
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/column.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/column.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/resource.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/resource.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/schema/table.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/schema/table.py`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/json.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/uuid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import pyarrow as pa
 
 
-class JSONType(pa.PyExtensionType):
+class UUIDType(pa.ExtensionType):
     def __init__(self):
-        pa.PyExtensionType.__init__(self, pa.binary())
+        pa.ExtensionType.__init__(
+            self, extension_name="uuid", storage_type=pa.binary(16)
+        )
 
     def __reduce__(self):
-        return JSONType, ()
+        return UUIDType, ()
 
     def __arrow_ext_serialize__(self):
         # since we don't have a parameterized type, we don't need extra
         # metadata to be deserialized
-        return b"json-serialized"
+        return b"uuid-serialized"
 
     @classmethod
     def __arrow_ext_deserialize__(self, storage_type, serialized):
         # return an instance of this subclass given the serialized
         # metadata.
-        return JSONType()
+        return UUIDType()
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery/sdk/types/uuid.py` & `cloudquery-plugin-sdk-0.0.9/cloudquery/sdk/types/json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import pyarrow as pa
 
 
-class UUIDType(pa.PyExtensionType):
+class JSONType(pa.ExtensionType):
     def __init__(self):
-        pa.PyExtensionType.__init__(self, pa.binary(16))
+        pa.ExtensionType.__init__(self, extension_name="json", storage_type=pa.binary())
 
     def __reduce__(self):
-        return UUIDType, ()
+        return JSONType, ()
 
     def __arrow_ext_serialize__(self):
         # since we don't have a parameterized type, we don't need extra
         # metadata to be deserialized
-        return b"uuid-serialized"
+        return b"json-serialized"
 
     @classmethod
     def __arrow_ext_deserialize__(self, storage_type, serialized):
         # return an instance of this subclass given the serialized
         # metadata.
-        return UUIDType()
+        return JSONType()
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/PKG-INFO` & `cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudquery-plugin-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: CloudQuery Plugin SDK for Python
 Home-page: https://github.com/cloudquery/plugin-sdk-python
 Author: CloudQuery LTD
 Author-email: pypi-packages@cloudquery.io
 License: MPL-2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `cloudquery-plugin-sdk-0.0.8/cloudquery_plugin_sdk.egg-info/SOURCES.txt` & `cloudquery-plugin-sdk-0.0.9/cloudquery_plugin_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudquery-plugin-sdk-0.0.8/setup.py` & `cloudquery-plugin-sdk-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 packages = [
     package
     for package in setuptools.PEP420PackageFinder.find()
     if package.startswith("cloudquery")
 ]
 setuptools.setup(
     name=name,
-    version="0.0.8",
+    version="0.0.9",
     description=description,
     long_description=long_description,
     author="CloudQuery LTD",
     author_email="pypi-packages@cloudquery.io",
     license="MPL-2.0",
     url=url,
     classifiers=[
```

