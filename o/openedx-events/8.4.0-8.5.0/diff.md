# Comparing `tmp/openedx-events-8.4.0.tar.gz` & `tmp/openedx-events-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-8.4.0.tar", last modified: Wed Aug  2 16:33:46 2023, max compression
+gzip compressed data, was "openedx-events-8.5.0.tar", last modified: Tue Aug  8 14:54:44 2023, max compression
```

## Comparing `openedx-events-8.4.0.tar` & `openedx-events-8.5.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)     9936 2023-08-02 16:33:40.000000 openedx-events-8.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-02 16:33:40.000000 openedx-events-8.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-08-02 16:33:40.000000 openedx-events-8.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-08-02 16:33:46.035698 openedx-events-8.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-08-02 16:33:40.000000 openedx-events-8.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7081 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3084 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11516 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (122)    12453 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10470 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7091 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.031698 openedx-events-8.4.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-08-02 16:33:40.000000 openedx-events-8.4.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.027698 openedx-events-8.4.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1789 2023-08-02 16:33:46.000000 openedx-events-8.4.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-02 16:33:45.000000 openedx-events-8.4.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-02 16:33:40.000000 openedx-events-8.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-02 16:33:46.035698 openedx-events-8.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-08-02 16:33:40.000000 openedx-events-8.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:33:46.035698 openedx-events-8.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-02 16:33:40.000000 openedx-events-8.4.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.184674 openedx-events-8.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10044 2023-08-08 14:54:39.000000 openedx-events-8.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-08-08 14:54:39.000000 openedx-events-8.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-08-08 14:54:39.000000 openedx-events-8.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    16072 2023-08-08 14:54:44.184674 openedx-events-8.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-08-08 14:54:39.000000 openedx-events-8.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.176674 openedx-events-8.5.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.176674 openedx-events-8.5.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7081 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4368 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (122)     7236 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5772 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5353 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5277 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11516 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12453 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11536 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9923 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2014 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10470 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7091 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.180674 openedx-events-8.5.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2451 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4845 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14277 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10393 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3206 2023-08-08 14:54:39.000000 openedx-events-8.5.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.176674 openedx-events-8.5.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16072 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-08 14:54:44.000000 openedx-events-8.5.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.184674 openedx-events-8.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-08 14:54:39.000000 openedx-events-8.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-08-08 14:54:44.184674 openedx-events-8.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2831 2023-08-08 14:54:39.000000 openedx-events-8.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 14:54:44.184674 openedx-events-8.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-08 14:54:39.000000 openedx-events-8.5.0/tests/test_openedx_events.py
```

### Comparing `openedx-events-8.4.0/CHANGELOG.rst` & `openedx-events-8.5.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.5.0] - 2023-08-08
+--------------------
+Changed
+~~~~~~~
+* Added json de/serialization for EventsMetadata
+
 [8.4.0] - 2023-07-20
 --------------------
 Added
 ~~~~~
 * Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
 * Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
```

### Comparing `openedx-events-8.4.0/LICENSE.txt` & `openedx-events-8.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/PKG-INFO` & `openedx-events-8.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.4.0
+Version: 8.5.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.5.0] - 2023-08-08
+--------------------
+Changed
+~~~~~~~
+* Added json de/serialization for EventsMetadata
+
 [8.4.0] - 2023-07-20
 --------------------
 Added
 ~~~~~
 * Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
 * Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
```

### Comparing `openedx-events-8.4.0/README.rst` & `openedx-events-8.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/content_authoring/data.py` & `openedx-events-8.5.0/openedx_events/content_authoring/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/content_authoring/signals.py` & `openedx-events-8.5.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/__init__.py` & `openedx-events-8.5.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-8.5.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-8.5.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/exceptions.py` & `openedx-events-8.5.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/learning/data.py` & `openedx-events-8.5.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/learning/signals.py` & `openedx-events-8.5.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/management/commands/consume_events.py` & `openedx-events-8.5.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-8.5.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-8.5.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-8.5.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/tests/test_tooling.py` & `openedx-events-8.5.0/openedx_events/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/tests/utils.py` & `openedx-events-8.5.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/tooling.py` & `openedx-events-8.5.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events/utils.py` & `openedx-events-8.5.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-8.4.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-8.5.0/openedx_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 8.4.0
+Version: 8.5.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -206,14 +206,20 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[8.5.0] - 2023-08-08
+--------------------
+Changed
+~~~~~~~
+* Added json de/serialization for EventsMetadata
+
 [8.4.0] - 2023-07-20
 --------------------
 Added
 ~~~~~
 * Added new ``PROGRAM_CERTIFICATE_AWARDED`` and ``PROGRAM_CERTIFICATE_REVOKED`` events in learning subdomain
 * Added new ``ProgramCertificateData`` and ``ProgramData`` data classes supporting the new program certificate events
```

### Comparing `openedx-events-8.4.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-8.5.0/openedx_events.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,12 +38,13 @@
 openedx_events/learning/signals.py
 openedx_events/management/__init__.py
 openedx_events/management/commands/__init__.py
 openedx_events/management/commands/consume_events.py
 openedx_events/management/commands/generate_avro_schemas.py
 openedx_events/tests/__init__.py
 openedx_events/tests/test_consume_events_command.py
+openedx_events/tests/test_data.py
 openedx_events/tests/test_generate_avro_schemas.py
 openedx_events/tests/test_tooling.py
 openedx_events/tests/utils.py
 requirements/base.in
 tests/test_openedx_events.py
```

### Comparing `openedx-events-8.4.0/setup.py` & `openedx-events-8.5.0/setup.py`

 * *Files identical despite different names*

