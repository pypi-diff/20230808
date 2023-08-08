# Comparing `tmp/statefun-tasks-0.9.93.tar.gz` & `tmp/statefun-tasks-1.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statefun-tasks-0.9.93.tar", last modified: Fri May 12 11:20:13 2023, max compression
+gzip compressed data, was "statefun-tasks-1.0.0rc0.tar", last modified: Tue Aug  8 09:23:47 2023, max compression
```

## Comparing `statefun-tasks-0.9.93.tar` & `statefun-tasks-1.0.0rc0.tar`

### file list

```diff
@@ -1,67 +1,47 @@
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/LICENSE
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/PKG-INFO
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      869 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/README.md
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-05-12 11:20:13.612605 statefun-tasks-0.9.93/setup.cfg
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      944 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/setup.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.468606 statefun-tasks-0.9.93/statefun_tasks/
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      934 2023-04-30 22:00:09.000000 statefun-tasks-0.9.93/statefun_tasks/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/builtin.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1004 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/builtin_tasks.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.504606 statefun-tasks-0.9.93/statefun_tasks/client/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/__init__.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    17395 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/tasks_client.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/client/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)    10552 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/context.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.520605 statefun-tasks-0.9.93/statefun_tasks/effects/
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/effect.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/effects/pause_pipeline_effect.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.532605 statefun-tasks-0.9.93/statefun_tasks/events/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/events/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6622 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/events/event_handlers.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.536605 statefun-tasks-0.9.93/statefun_tasks/extensions/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.540605 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     5596 2023-04-13 15:25:59.000000 statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   115734 2023-04-30 22:00:09.000000 statefun-tasks-0.9.93/statefun_tasks/messages_pb2.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9212 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17896 2023-03-03 19:15:45.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.544605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.568605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      298 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6795 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1926 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     6799 2023-04-30 23:05:05.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2969 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1658 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.588605 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      186 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/__init__.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    11000 2023-05-12 10:53:19.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     6410 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_aggregator.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1995 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/result_emitter.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    12023 2022-11-29 16:51:28.000000 statefun-tasks-0.9.93/statefun_tasks/pipeline_impl/helpers/task_submitter.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     7003 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/protobuf.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     9345 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/serialisation.py
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    16690 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/statefun_tasks/task_builder.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.592605 statefun-tasks-0.9.93/statefun_tasks/task_impl/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/__init__.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.608605 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      265 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/__init__.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      858 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/child_pipeline_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      537 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/message_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     3983 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_action_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     4724 2023-05-12 11:20:04.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_request_handler.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     1134 2022-11-27 19:05:41.000000 statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_response_handler.py
--rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7655 2023-04-10 17:01:43.000000 statefun-tasks-0.9.93/statefun_tasks/tasks.py
--rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/type_helpers.py
--rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    11331 2023-04-30 23:05:05.000000 statefun-tasks-0.9.93/statefun_tasks/types.py
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1793 2022-11-27 19:05:40.000000 statefun-tasks-0.9.93/statefun_tasks/utils.py
-drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-05-12 11:20:13.492606 statefun-tasks-0.9.93/statefun_tasks.egg-info/
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     1386 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/PKG-INFO
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)     2111 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)        1 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       42 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/requires.txt
--rw-r--r--   0 kingfra   (1000) kingfra   (1000)       15 2023-05-12 11:20:13.000000 statefun-tasks-0.9.93/statefun_tasks.egg-info/top_level.txt
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.887640 statefun-tasks-1.0.0rc0/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)    11357 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/LICENSE
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1496 2023-08-08 09:23:47.887640 statefun-tasks-1.0.0rc0/PKG-INFO
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      977 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/README.md
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       38 2023-08-08 09:23:47.887640 statefun-tasks-1.0.0rc0/setup.cfg
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      947 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/setup.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.811641 statefun-tasks-1.0.0rc0/statefun_tasks/
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1096 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/__init__.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)      585 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/statefun_tasks/builtin.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      194 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/builtin_tasks.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.843640 statefun-tasks-1.0.0rc0/statefun_tasks/client/
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      151 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/statefun_tasks/client/__init__.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    17420 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/client/tasks_client.py
+-rw-r--r--   0 kingfra   (1000) kingfra   (1000)      864 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/statefun_tasks/client/types.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    10944 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/context.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.855640 statefun-tasks-1.0.0rc0/statefun_tasks/effects/
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)       84 2023-04-10 17:01:43.000000 statefun-tasks-1.0.0rc0/statefun_tasks/effects/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      339 2023-04-10 17:01:43.000000 statefun-tasks-1.0.0rc0/statefun_tasks/effects/effect.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)      370 2023-04-10 17:01:43.000000 statefun-tasks-1.0.0rc0/statefun_tasks/effects/pause_pipeline_effect.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.863640 statefun-tasks-1.0.0rc0/statefun_tasks/events/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       43 2022-11-27 19:05:41.000000 statefun-tasks-1.0.0rc0/statefun_tasks/events/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     3423 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/events/event_handlers.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.863640 statefun-tasks-1.0.0rc0/statefun_tasks/extensions/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)        0 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/statefun_tasks/extensions/__init__.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.871640 statefun-tasks-1.0.0rc0/statefun_tasks/extensions/inline_tasks/
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)       65 2022-11-27 19:05:40.000000 statefun-tasks-1.0.0rc0/statefun_tasks/extensions/inline_tasks/__init__.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     5596 2023-04-13 15:25:59.000000 statefun-tasks-1.0.0rc0/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.883640 statefun-tasks-1.0.0rc0/statefun_tasks/handlers/
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      151 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/handlers/__init__.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)      537 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/handlers/message_handler.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     2673 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/handlers/task_action_handler.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     6403 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/handlers/task_request_handler.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)   104378 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/messages_pb2.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)    17707 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/pipeline_builder.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     6899 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/protobuf.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     6154 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/serialisation.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    15100 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/task_builder.py
+-rwxrwxr-x   0 kingfra   (1000) kingfra   (1000)     7293 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/tasks.py
+-rwxr-xr-x   0 kingfra   (1000) kingfra   (1000)     2483 2023-07-24 14:11:45.000000 statefun-tasks-1.0.0rc0/statefun_tasks/type_helpers.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)    11149 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/types.py
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1495 2023-08-08 09:23:12.000000 statefun-tasks-1.0.0rc0/statefun_tasks/utils.py
+drwxrwxr-x   0 kingfra   (1000) kingfra   (1000)        0 2023-08-08 09:23:47.835640 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1496 2023-08-08 09:23:47.000000 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/PKG-INFO
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)     1201 2023-08-08 09:23:47.000000 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)        1 2023-08-08 09:23:47.000000 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       42 2023-08-08 09:23:47.000000 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/requires.txt
+-rw-rw-r--   0 kingfra   (1000) kingfra   (1000)       15 2023-08-08 09:23:47.000000 statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/top_level.txt
```

### Comparing `statefun-tasks-0.9.93/LICENSE` & `statefun-tasks-1.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/PKG-INFO` & `statefun-tasks-1.0.0rc0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.93
+Version: 1.0.0rc0
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,8 +37,9 @@
     return f'{greeting}.  So now I will say goodbye'
 ```
 
 Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
 
+The pipeline function can be downloaded [here](https://github.com/fransking/flink-statefun-tasks-embedded).
```

### Comparing `statefun-tasks-0.9.93/README.md` & `statefun-tasks-1.0.0rc0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -21,7 +21,9 @@
 def say_goodbye(greeting):
     return f'{greeting}.  So now I will say goodbye'
 ```
 
 Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
+
+The pipeline function can be downloaded [here](https://github.com/fransking/flink-statefun-tasks-embedded).
```

### Comparing `statefun-tasks-0.9.93/setup.py` & `statefun-tasks-1.0.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 install_requires = [
     'apache-flink-statefun>=3.2.0',
     'kafka-python'
 ]
 
 setuptools.setup(
     name="statefun-tasks",
-    version="0.9.93",
+    version="1.0.0-rc0",
     author="Frans King & Luke Ashworth",
     author_email="frans.king@sbbsystems.com",
     description="Tasks API for Stateful Functions on Flink",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://fransking.github.io/flink-statefun-tasks",
     packages=['statefun_tasks'] + [f'statefun_tasks.{package}' for package in setuptools.find_packages('statefun_tasks')],
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/__init__.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,23 @@
 
 # serialisation
 from statefun_tasks.protobuf import pack_any, unpack_any
 from statefun_tasks.serialisation import DefaultSerialiser
 
 
 # types
-from statefun_tasks.types import Task, Group, RetryPolicy, TaskAlreadyExistsException, TaskCancelledException, TasksException, \
-    PipelineInProgress, YieldTaskInvocation, MessageSizeExceeded
-    
+from statefun_tasks.types import (Task, Group, RetryPolicy, TaskAlreadyExistsException, TaskCancelledException, TasksException,
+                                  YieldTaskInvocation, MessageSizeExceeded)
+
+
+# type helpers
 from statefun_tasks.type_helpers import flink_value_type_for, add_flink_value_type_for
 
 
 # protobuf message types
-from statefun_tasks.messages_pb2 import TaskRequest, TaskResult, TaskException, TaskActionRequest, TaskActionResult, \
-    TaskActionException, TaskAction, TaskStatus, TaskDeferral, PausedTask, Pipeline, ChildPipeline, Address, TaskInfo, DeferredTask
+from statefun_tasks.messages_pb2 import (TaskRequest, TaskResult, TaskException, TaskActionRequest, TaskActionResult,
+                                         TaskActionException, TaskAction, TaskStatus, PausedTask, Pipeline, ChildPipeline, 
+                                         Address, TaskInfo)
+
+
+# builtin tasks
+from statefun_tasks.builtin_tasks import run_pipeline, flatten_results
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/builtin.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/builtin.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/statefun_tasks/client/tasks_client.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/client/tasks_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from statefun_tasks import DefaultSerialiser, PipelineBuilder, TaskRequest, TaskResult, TaskException, TaskAction, \
-    TaskActionRequest, TaskActionResult, TaskActionException, TaskStatus as TaskStatusProto, Task
+from statefun_tasks import (DefaultSerialiser, PipelineBuilder, TaskRequest, TaskResult, TaskException, TaskAction, 
+                            TaskActionRequest, TaskActionResult, TaskActionException, TaskStatus as TaskStatusProto, Task)
 from statefun_tasks.client.types import TaskError, TaskStatus
 
 from google.protobuf.any_pb2 import Any
 from kafka import KafkaProducer, KafkaConsumer
 
 import logging
 from uuid import uuid4
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/client/types.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/client/types.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/statefun_tasks/context.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,31 +24,27 @@
     __slots__ = (
         '_context', 
         '_egress_type_name', 
         '_serialiser', 
         '_egress_message_max_size',
         'storage', 
         'task_state', 
-        'pipeline_state', 
-        'pipeline_state_size', 
         '_task_meta', 
         '_task_name', 
         '_task_uid'
         )
 
     def __init__(self, context: Context, egress_type_name: str, egress_message_max_size=None, serialiser=None):
         self._context = context
         self._egress_type_name = egress_type_name
         self._serialiser = serialiser if serialiser is not None else DefaultSerialiser()
         self._egress_message_max_size = egress_message_max_size
 
         self.storage = context.storage
         self.task_state = self.storage.task_state or TaskState()
-        self.pipeline_state = self.storage.pipeline_state
-        self.pipeline_state_size = self.pipeline_state.ByteSize() if self.pipeline_state is not None else 0
 
         self._task_meta = {}
         self._task_name = None
         self._task_uid = None
 
     @property
     def task_uid(self):
@@ -195,14 +191,32 @@
         """
         Caller task Id in the form of context.caller.id
 
         :return: task Id
         """
         return None if self._context.caller.id == "" else self._context.caller.id
 
+    def get_original_caller_address(self):
+        """
+        Original caller address irrespective of whether this task is a retry (caller is self) or not
+
+        :return: address
+        """
+        task_state = self.task_state.by_uid[self.task_uid]
+        return task_state.original_caller_address if task_state.original_caller_address != '' else self.get_caller_address()
+
+    def get_original_caller_id(self):
+        """
+        Original caller id irrespective of whether this task is a retry (caller is self) or not
+
+        :return: address
+        """
+        task_state = self.task_state.by_uid[self.task_uid]
+        return task_state.original_caller_id if task_state.original_caller_id != '' else self.get_caller_id()
+
     def set_state(self, obj):
         self.task_state.internal_state.CopyFrom(pack_any(self._serialiser.to_proto(obj)))
 
     def get_state(self, default=None):
         if self.task_state.HasField('internal_state'):
             return self._serialiser.from_proto(self.task_state.internal_state, default)
         
@@ -292,12 +306,9 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self._context.storage.task_state = self.task_state
 
-        if self.pipeline_state is not None:
-            self._context.storage.pipeline_state = self.pipeline_state
-
     def __str__(self):
         return f'task_name: {self.task_name}, task_id: {self.get_task_id()}, caller: {self.get_caller_id()}'
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/statefun_tasks/messages_pb2.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/messages_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='messages.proto',
   package='statefun_tasks',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0emessages.proto\x12\x0estatefun_tasks\x1a\x19google/protobuf/any.proto\"\x0b\n\tNoneValue\"6\n\x07\x41\x64\x64ress\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\"\x92\x01\n\x10MapOfStringToAny\x12:\n\x05items\x18\x01 \x03(\x0b\x32+.statefun_tasks.MapOfStringToAny.ItemsEntry\x1a\x42\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"1\n\nArrayOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"1\n\nTupleOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"\xd4\x02\n\tTaskEntry\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12%\n\x07request\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x10\n\x08\x63omplete\x18\x04 \x01(\x08\x12\x12\n\nis_finally\x18\x05 \x01(\x08\x12\x11\n\tnamespace\x18\x06 \x01(\t\x12\x13\n\x0bworker_name\x18\x07 \x01(\t\x12\x13\n\x0bis_fruitful\x18\x08 \x01(\x08\x12\x35\n\x0cretry_policy\x18\t \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x19\n\x0c\x64isplay_name\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x12\x0b\n\x03uid\x18\x0c \x01(\t\x12\x18\n\x10is_exceptionally\x18\r \x01(\x08\x42\x0f\n\r_display_name\"\x8c\x01\n\nGroupEntry\x12\x10\n\x08group_id\x18\x01 \x01(\t\x12\'\n\x05group\x18\x02 \x03(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x17\n\x0fmax_parallelism\x18\x03 \x01(\x05\x12\x0f\n\x07is_wait\x18\x04 \x01(\x08\x12\x19\n\x11return_exceptions\x18\x05 \x01(\x08\"|\n\rPipelineEntry\x12/\n\ntask_entry\x18\x01 \x01(\x0b\x32\x19.statefun_tasks.TaskEntryH\x00\x12\x31\n\x0bgroup_entry\x18\x02 \x01(\x0b\x32\x1a.statefun_tasks.GroupEntryH\x00\x42\x07\n\x05\x65ntry\"\xa2\x02\n\x08Pipeline\x12.\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1d.statefun_tasks.PipelineEntry\x12\x0e\n\x06inline\x18\x02 \x01(\x08\x12/\n\x0cinitial_args\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x12=\n\x0einitial_kwargs\x18\x04 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAnyH\x01\x88\x01\x01\x12\x30\n\rinitial_state\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x02\x88\x01\x01\x42\x0f\n\r_initial_argsB\x11\n\x0f_initial_kwargsB\x10\n\x0e_initial_state\"i\n\x0fTaskRetryPolicy\x12\x11\n\tretry_for\x18\x01 \x03(\t\x12\x13\n\x0bmax_retries\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x65lay_ms\x18\x03 \x01(\x02\x12\x1c\n\x14\x65xponential_back_off\x18\x04 \x01(\x08\"k\n\rArgsAndKwargs\x12(\n\x04\x61rgs\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TupleOfAny\x12\x30\n\x06kwargs\x18\x02 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAny\"\xc3\x03\n\x0bTaskRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x15\n\x0breply_topic\x18\x03 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x04 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12%\n\x07request\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x35\n\x0cretry_policy\x18\x07 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x33\n\x04meta\x18\x08 \x03(\x0b\x32%.statefun_tasks.TaskRequest.MetaEntry\x12\x18\n\x0bis_fruitful\x18\t \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rinvocation_id\x18\n \x01(\tH\x02\x88\x01\x01\x12\x0b\n\x03uid\x18\x0b \x01(\t\x1a+\n\tMetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05replyB\x0e\n\x0c_is_fruitfulB\x10\n\x0e_invocation_id\"\xbd\x01\n\nTaskResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1a\n\rinvocation_id\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\x06 \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\xad\x02\n\rTaskException\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x13\n\x0bmaybe_retry\x18\x07 \x01(\x08\x12\x35\n\x0cretry_policy\x18\x08 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x1a\n\rinvocation_id\x18\t \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\n \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\x9f\x01\n\x15TaskResultOrException\x12\x31\n\x0btask_result\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x37\n\x0etask_exception\x18\x02 \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x42\x1a\n\x18task_result_or_exception\"e\n\x11TaskSpecificState\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x1f\n\x17original_caller_address\x18\x02 \x01(\t\x12\x1a\n\x12original_caller_id\x18\x03 \x01(\t\"\xd8\x01\n\tTaskState\x12\x34\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32$.statefun_tasks.TaskState.ByUidEntry\x12\x31\n\x0einternal_state\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x1aO\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.statefun_tasks.TaskSpecificState:\x02\x38\x01\x42\x11\n\x0f_internal_state\"\x90\x02\n\x0cTaskDeferral\x12+\n\x05tasks\x18\x01 \x03(\x0b\x32\x1c.statefun_tasks.DeferredTask\x12 \n\x13parent_task_address\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x1b\n\x0eparent_task_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x12L\n\x18task_result_or_exception\x18\x04 \x01(\x0b\x32%.statefun_tasks.TaskResultOrExceptionH\x02\x88\x01\x01\x42\x16\n\x14_parent_task_addressB\x11\n\x0f_parent_task_idB\x1b\n\x19_task_result_or_exception\":\n\x0c\x44\x65\x66\x65rredTask\x12\x10\n\x08task_uid\x18\x01 \x01(\t\x12\x18\n\x10has_initial_args\x18\x02 \x01(\x08\"T\n\nPausedTask\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\x31\n\x0ctask_request\x18\x02 \x01(\x0b\x32\x1b.statefun_tasks.TaskRequest\"\xdb\x07\n\rPipelineState\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12*\n\x08pipeline\x18\x07 \x01(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x31\n\x0ctask_results\x18\x08 \x01(\x0b\x32\x1b.statefun_tasks.TaskResults\x12;\n\x15result_before_finally\x18\t \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x41\n\x18\x65xception_before_finally\x18\n \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x12\x13\n\x0bis_fruitful\x18\x0b \x01(\x08\x12(\n\ntask_state\x18\x0c \x01(\x0b\x32\x14.google.protobuf.Any\x12R\n\x14task_deferrals_by_id\x18\r \x03(\x0b\x32\x34.statefun_tasks.PipelineState.TaskDeferralsByIdEntry\x12\x62\n\x1dtask_deferral_ids_by_task_uid\x18\x0e \x03(\x0b\x32;.statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry\x12*\n\x06status\x18\x0f \x01(\x0b\x32\x1a.statefun_tasks.TaskStatus\x12\x30\n\x0cpaused_tasks\x18\x10 \x03(\x0b\x32\x1a.statefun_tasks.PausedTask\x12\x36\n\x0f\x63hild_pipelines\x18\x11 \x03(\x0b\x32\x1d.statefun_tasks.ChildPipeline\x12-\n\x0flast_task_state\x18\x12 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x15\n\rinvocation_id\x18\x13 \x01(\t\x1aV\n\x16TaskDeferralsByIdEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.statefun_tasks.TaskDeferral:\x02\x38\x01\x1a?\n\x1dTaskDeferralIdsByTaskUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0e\x62\x65\x66ore_finally\"\xbe\x01\n\rChildPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12\'\n\x05tasks\x18\x07 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\x12\x15\n\rinvocation_id\x18\x08 \x01(\t\"h\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x13\n\x0bworker_name\x18\x04 \x01(\t\x12\x10\n\x08task_uid\x18\x05 \x01(\t\"\x89\x01\n\x0bTaskResults\x12\x36\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32&.statefun_tasks.TaskResults.ByUidEntry\x1a\x42\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\xaa\x01\n\x11TaskActionRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x0breply_topic\x18\x02 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x03 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12*\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x0b\n\x03uid\x18\x05 \x01(\tB\x07\n\x05reply\"}\n\x10TaskActionResult\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0b\n\x03uid\x18\x04 \x01(\t\"\xa1\x01\n\x13TaskActionException\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12\x0b\n\x03uid\x18\x06 \x01(\t\"\xa8\x01\n\nTaskStatus\x12\x30\n\x05value\x18\x01 \x01(\x0e\x32!.statefun_tasks.TaskStatus.Status\"h\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\r\n\tCOMPLETED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\n\n\x06PAUSED\x10\x04\x12\x0e\n\nCANCELLING\x10\x05\x12\r\n\tCANCELLED\x10\x06*|\n\nTaskAction\x12\x0e\n\nGET_STATUS\x10\x00\x12\x0f\n\x0bGET_REQUEST\x10\x01\x12\x0e\n\nGET_RESULT\x10\x02\x12\x12\n\x0ePAUSE_PIPELINE\x10\x03\x12\x14\n\x10UNPAUSE_PIPELINE\x10\x04\x12\x13\n\x0f\x43\x41NCEL_PIPELINE\x10\x05\x62\x06proto3'
+  serialized_pb=b'\n\x0emessages.proto\x12\x0estatefun_tasks\x1a\x19google/protobuf/any.proto\"\x0b\n\tNoneValue\"6\n\x07\x41\x64\x64ress\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\"\x92\x01\n\x10MapOfStringToAny\x12:\n\x05items\x18\x01 \x03(\x0b\x32+.statefun_tasks.MapOfStringToAny.ItemsEntry\x1a\x42\n\nItemsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"1\n\nArrayOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"1\n\nTupleOfAny\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.google.protobuf.Any\"\xd4\x02\n\tTaskEntry\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12%\n\x07request\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x10\n\x08\x63omplete\x18\x04 \x01(\x08\x12\x12\n\nis_finally\x18\x05 \x01(\x08\x12\x11\n\tnamespace\x18\x06 \x01(\t\x12\x13\n\x0bworker_name\x18\x07 \x01(\t\x12\x13\n\x0bis_fruitful\x18\x08 \x01(\x08\x12\x35\n\x0cretry_policy\x18\t \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x19\n\x0c\x64isplay_name\x18\n \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x12\x0b\n\x03uid\x18\x0c \x01(\t\x12\x18\n\x10is_exceptionally\x18\r \x01(\x08\x42\x0f\n\r_display_name\"\x8c\x01\n\nGroupEntry\x12\x10\n\x08group_id\x18\x01 \x01(\t\x12\'\n\x05group\x18\x02 \x03(\x0b\x32\x18.statefun_tasks.Pipeline\x12\x17\n\x0fmax_parallelism\x18\x03 \x01(\x05\x12\x0f\n\x07is_wait\x18\x04 \x01(\x08\x12\x19\n\x11return_exceptions\x18\x05 \x01(\x08\"|\n\rPipelineEntry\x12/\n\ntask_entry\x18\x01 \x01(\x0b\x32\x19.statefun_tasks.TaskEntryH\x00\x12\x31\n\x0bgroup_entry\x18\x02 \x01(\x0b\x32\x1a.statefun_tasks.GroupEntryH\x00\x42\x07\n\x05\x65ntry\"\xa2\x02\n\x08Pipeline\x12.\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1d.statefun_tasks.PipelineEntry\x12\x0e\n\x06inline\x18\x02 \x01(\x08\x12/\n\x0cinitial_args\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x12=\n\x0einitial_kwargs\x18\x04 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAnyH\x01\x88\x01\x01\x12\x30\n\rinitial_state\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x02\x88\x01\x01\x42\x0f\n\r_initial_argsB\x11\n\x0f_initial_kwargsB\x10\n\x0e_initial_state\"i\n\x0fTaskRetryPolicy\x12\x11\n\tretry_for\x18\x01 \x03(\t\x12\x13\n\x0bmax_retries\x18\x02 \x01(\x05\x12\x10\n\x08\x64\x65lay_ms\x18\x03 \x01(\x02\x12\x1c\n\x14\x65xponential_back_off\x18\x04 \x01(\x08\"k\n\rArgsAndKwargs\x12(\n\x04\x61rgs\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TupleOfAny\x12\x30\n\x06kwargs\x18\x02 \x01(\x0b\x32 .statefun_tasks.MapOfStringToAny\"\xc3\x03\n\x0bTaskRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x15\n\x0breply_topic\x18\x03 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x04 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12%\n\x07request\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x35\n\x0cretry_policy\x18\x07 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x33\n\x04meta\x18\x08 \x03(\x0b\x32%.statefun_tasks.TaskRequest.MetaEntry\x12\x18\n\x0bis_fruitful\x18\t \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rinvocation_id\x18\n \x01(\tH\x02\x88\x01\x01\x12\x0b\n\x03uid\x18\x0b \x01(\t\x1a+\n\tMetaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x07\n\x05replyB\x0e\n\x0c_is_fruitfulB\x10\n\x0e_invocation_id\"\xbd\x01\n\nTaskResult\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12#\n\x05state\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1a\n\rinvocation_id\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\x06 \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\xad\x02\n\rTaskException\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12#\n\x05state\x18\x06 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x13\n\x0bmaybe_retry\x18\x07 \x01(\x08\x12\x35\n\x0cretry_policy\x18\x08 \x01(\x0b\x32\x1f.statefun_tasks.TaskRetryPolicy\x12\x1a\n\rinvocation_id\x18\t \x01(\tH\x00\x88\x01\x01\x12\x0b\n\x03uid\x18\n \x01(\t\x12\x0f\n\x07is_wait\x18\x0b \x01(\x08\x42\x10\n\x0e_invocation_id\"\x9f\x01\n\x15TaskResultOrException\x12\x31\n\x0btask_result\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TaskResultH\x00\x12\x37\n\x0etask_exception\x18\x02 \x01(\x0b\x32\x1d.statefun_tasks.TaskExceptionH\x00\x42\x1a\n\x18task_result_or_exception\"e\n\x11TaskSpecificState\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x1f\n\x17original_caller_address\x18\x02 \x01(\t\x12\x1a\n\x12original_caller_id\x18\x03 \x01(\t\"\xd8\x01\n\tTaskState\x12\x34\n\x06\x62y_uid\x18\x01 \x03(\x0b\x32$.statefun_tasks.TaskState.ByUidEntry\x12\x31\n\x0einternal_state\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x88\x01\x01\x1aO\n\nByUidEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32!.statefun_tasks.TaskSpecificState:\x02\x38\x01\x42\x11\n\x0f_internal_state\"T\n\nPausedTask\x12\x13\n\x0b\x64\x65stination\x18\x01 \x01(\t\x12\x31\n\x0ctask_request\x18\x02 \x01(\x0b\x32\x1b.statefun_tasks.TaskRequest\"\xbe\x01\n\rChildPipeline\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0f\n\x07root_id\x18\x03 \x01(\t\x12\x14\n\x0croot_address\x18\x04 \x01(\t\x12\x11\n\tcaller_id\x18\x05 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x06 \x01(\t\x12\'\n\x05tasks\x18\x07 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\x12\x15\n\rinvocation_id\x18\x08 \x01(\t\"~\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x13\n\x0bworker_name\x18\x04 \x01(\t\x12\x10\n\x08task_uid\x18\x05 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x06 \x01(\t\"\xaa\x01\n\x11TaskActionRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\x0breply_topic\x18\x02 \x01(\tH\x00\x12\x30\n\rreply_address\x18\x03 \x01(\x0b\x32\x17.statefun_tasks.AddressH\x00\x12*\n\x06\x61\x63tion\x18\x04 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x0b\n\x03uid\x18\x05 \x01(\tB\x07\n\x05reply\"}\n\x10TaskActionResult\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12$\n\x06result\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x0b\n\x03uid\x18\x04 \x01(\t\"\xa1\x01\n\x13TaskActionException\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32\x1a.statefun_tasks.TaskAction\x12\x16\n\x0e\x65xception_type\x18\x03 \x01(\t\x12\x19\n\x11\x65xception_message\x18\x04 \x01(\t\x12\x12\n\nstacktrace\x18\x05 \x01(\t\x12\x0b\n\x03uid\x18\x06 \x01(\t\"\xa8\x01\n\nTaskStatus\x12\x30\n\x05value\x18\x01 \x01(\x0e\x32!.statefun_tasks.TaskStatus.Status\"h\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\r\n\tCOMPLETED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\n\n\x06PAUSED\x10\x04\x12\x0e\n\nCANCELLING\x10\x05\x12\r\n\tCANCELLED\x10\x06\"e\n\x0fPipelineCreated\x12\x11\n\tcaller_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63\x61ller_address\x18\x02 \x01(\t\x12\'\n\x05tasks\x18\x03 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\"C\n\x15PipelineStatusChanged\x12*\n\x06status\x18\x01 \x01(\x0b\x32\x1a.statefun_tasks.TaskStatus\"?\n\x14PipelineTasksSkipped\x12\'\n\x05tasks\x18\x01 \x03(\x0b\x32\x18.statefun_tasks.TaskInfo\"r\n\x14PipelineTaskFinished\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03uid\x18\x02 \x01(\t\x12*\n\x06status\x18\x03 \x01(\x0b\x32\x1a.statefun_tasks.TaskStatus\x12\x15\n\rsize_in_bytes\x18\x04 \x01(\r\"\x8f\x03\n\x05\x45vent\x12\x13\n\x0bpipeline_id\x18\x01 \x01(\t\x12\x18\n\x10pipeline_address\x18\x02 \x01(\t\x12\x18\n\x10root_pipeline_id\x18\x03 \x01(\t\x12\x1d\n\x15root_pipeline_address\x18\x04 \x01(\t\x12;\n\x10pipeline_created\x18\x05 \x01(\x0b\x32\x1f.statefun_tasks.PipelineCreatedH\x00\x12H\n\x17pipeline_status_changed\x18\x06 \x01(\x0b\x32%.statefun_tasks.PipelineStatusChangedH\x00\x12\x46\n\x16pipeline_tasks_skipped\x18\x07 \x01(\x0b\x32$.statefun_tasks.PipelineTasksSkippedH\x00\x12\x46\n\x16pipeline_task_finished\x18\x08 \x01(\x0b\x32$.statefun_tasks.PipelineTaskFinishedH\x00\x42\x07\n\x05\x65vent*|\n\nTaskAction\x12\x0e\n\nGET_STATUS\x10\x00\x12\x0f\n\x0bGET_REQUEST\x10\x01\x12\x0e\n\nGET_RESULT\x10\x02\x12\x12\n\x0ePAUSE_PIPELINE\x10\x03\x12\x14\n\x10UNPAUSE_PIPELINE\x10\x04\x12\x13\n\x0f\x43\x41NCEL_PIPELINE\x10\x05\x62\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_any__pb2.DESCRIPTOR,])
 
 _TASKACTION = _descriptor.EnumDescriptor(
   name='TaskAction',
   full_name='statefun_tasks.TaskAction',
   filename=None,
@@ -61,16 +61,16 @@
       name='CANCEL_PIPELINE', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5421,
-  serialized_end=5545,
+  serialized_start=4733,
+  serialized_end=4857,
 )
 _sym_db.RegisterEnumDescriptor(_TASKACTION)
 
 TaskAction = enum_type_wrapper.EnumTypeWrapper(_TASKACTION)
 GET_STATUS = 0
 GET_REQUEST = 1
 GET_RESULT = 2
@@ -120,16 +120,16 @@
       name='CANCELLED', index=6, number=6,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5315,
-  serialized_end=5419,
+  serialized_start=3872,
+  serialized_end=3976,
 )
 _sym_db.RegisterEnumDescriptor(_TASKSTATUS_STATUS)
 
 
 _NONEVALUE = _descriptor.Descriptor(
   name='NoneValue',
   full_name='statefun_tasks.NoneValue',
@@ -1236,46 +1236,32 @@
     fields=[]),
   ],
   serialized_start=2718,
   serialized_end=2934,
 )
 
 
-_TASKDEFERRAL = _descriptor.Descriptor(
-  name='TaskDeferral',
-  full_name='statefun_tasks.TaskDeferral',
+_PAUSEDTASK = _descriptor.Descriptor(
+  name='PausedTask',
+  full_name='statefun_tasks.PausedTask',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='tasks', full_name='statefun_tasks.TaskDeferral.tasks', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='parent_task_address', full_name='statefun_tasks.TaskDeferral.parent_task_address', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='parent_task_id', full_name='statefun_tasks.TaskDeferral.parent_task_id', index=2,
-      number=3, type=9, cpp_type=9, label=1,
+      name='destination', full_name='statefun_tasks.PausedTask.destination', index=0,
+      number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='task_result_or_exception', full_name='statefun_tasks.TaskDeferral.task_result_or_exception', index=3,
-      number=4, type=11, cpp_type=10, label=1,
+      name='task_request', full_name='statefun_tasks.PausedTask.task_request', index=1,
+      number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
@@ -1283,661 +1269,529 @@
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='_parent_task_address', full_name='statefun_tasks.TaskDeferral._parent_task_address',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_parent_task_id', full_name='statefun_tasks.TaskDeferral._parent_task_id',
-      index=1, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-    _descriptor.OneofDescriptor(
-      name='_task_result_or_exception', full_name='statefun_tasks.TaskDeferral._task_result_or_exception',
-      index=2, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
-  serialized_start=2937,
-  serialized_end=3209,
+  serialized_start=2936,
+  serialized_end=3020,
 )
 
 
-_DEFERREDTASK = _descriptor.Descriptor(
-  name='DeferredTask',
-  full_name='statefun_tasks.DeferredTask',
+_CHILDPIPELINE = _descriptor.Descriptor(
+  name='ChildPipeline',
+  full_name='statefun_tasks.ChildPipeline',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='task_uid', full_name='statefun_tasks.DeferredTask.task_uid', index=0,
+      name='id', full_name='statefun_tasks.ChildPipeline.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='has_initial_args', full_name='statefun_tasks.DeferredTask.has_initial_args', index=1,
-      number=2, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      name='address', full_name='statefun_tasks.ChildPipeline.address', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=3211,
-  serialized_end=3269,
-)
-
-
-_PAUSEDTASK = _descriptor.Descriptor(
-  name='PausedTask',
-  full_name='statefun_tasks.PausedTask',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='destination', full_name='statefun_tasks.PausedTask.destination', index=0,
-      number=1, type=9, cpp_type=9, label=1,
+      name='root_id', full_name='statefun_tasks.ChildPipeline.root_id', index=2,
+      number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='task_request', full_name='statefun_tasks.PausedTask.task_request', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='root_address', full_name='statefun_tasks.ChildPipeline.root_address', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=3271,
-  serialized_end=3355,
-)
-
-
-_PIPELINESTATE_TASKDEFERRALSBYIDENTRY = _descriptor.Descriptor(
-  name='TaskDeferralsByIdEntry',
-  full_name='statefun_tasks.PipelineState.TaskDeferralsByIdEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='statefun_tasks.PipelineState.TaskDeferralsByIdEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
+      name='caller_id', full_name='statefun_tasks.ChildPipeline.caller_id', index=4,
+      number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='statefun_tasks.PipelineState.TaskDeferralsByIdEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='caller_address', full_name='statefun_tasks.ChildPipeline.caller_address', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=b'8\001',
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=4176,
-  serialized_end=4262,
-)
-
-_PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY = _descriptor.Descriptor(
-  name='TaskDeferralIdsByTaskUidEntry',
-  full_name='statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry.key', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='tasks', full_name='statefun_tasks.ChildPipeline.tasks', index=6,
+      number=7, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry.value', index=1,
-      number=2, type=9, cpp_type=9, label=1,
+      name='invocation_id', full_name='statefun_tasks.ChildPipeline.invocation_id', index=7,
+      number=8, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=b'8\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4264,
-  serialized_end=4327,
+  serialized_start=3023,
+  serialized_end=3213,
 )
 
-_PIPELINESTATE = _descriptor.Descriptor(
-  name='PipelineState',
-  full_name='statefun_tasks.PipelineState',
+
+_TASKINFO = _descriptor.Descriptor(
+  name='TaskInfo',
+  full_name='statefun_tasks.TaskInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='statefun_tasks.PipelineState.id', index=0,
+      name='task_id', full_name='statefun_tasks.TaskInfo.task_id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='address', full_name='statefun_tasks.PipelineState.address', index=1,
+      name='task_type', full_name='statefun_tasks.TaskInfo.task_type', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='root_id', full_name='statefun_tasks.PipelineState.root_id', index=2,
+      name='namespace', full_name='statefun_tasks.TaskInfo.namespace', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='root_address', full_name='statefun_tasks.PipelineState.root_address', index=3,
+      name='worker_name', full_name='statefun_tasks.TaskInfo.worker_name', index=3,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='caller_id', full_name='statefun_tasks.PipelineState.caller_id', index=4,
+      name='task_uid', full_name='statefun_tasks.TaskInfo.task_uid', index=4,
       number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='caller_address', full_name='statefun_tasks.PipelineState.caller_address', index=5,
+      name='display_name', full_name='statefun_tasks.TaskInfo.display_name', index=5,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3215,
+  serialized_end=3341,
+)
+
+
+_TASKACTIONREQUEST = _descriptor.Descriptor(
+  name='TaskActionRequest',
+  full_name='statefun_tasks.TaskActionRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='pipeline', full_name='statefun_tasks.PipelineState.pipeline', index=6,
-      number=7, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_results', full_name='statefun_tasks.PipelineState.task_results', index=7,
-      number=8, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='result_before_finally', full_name='statefun_tasks.PipelineState.result_before_finally', index=8,
-      number=9, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='exception_before_finally', full_name='statefun_tasks.PipelineState.exception_before_finally', index=9,
-      number=10, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='id', full_name='statefun_tasks.TaskActionRequest.id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='is_fruitful', full_name='statefun_tasks.PipelineState.is_fruitful', index=10,
-      number=11, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
+      name='reply_topic', full_name='statefun_tasks.TaskActionRequest.reply_topic', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='task_state', full_name='statefun_tasks.PipelineState.task_state', index=11,
-      number=12, type=11, cpp_type=10, label=1,
+      name='reply_address', full_name='statefun_tasks.TaskActionRequest.reply_address', index=2,
+      number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='task_deferrals_by_id', full_name='statefun_tasks.PipelineState.task_deferrals_by_id', index=12,
-      number=13, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_deferral_ids_by_task_uid', full_name='statefun_tasks.PipelineState.task_deferral_ids_by_task_uid', index=13,
-      number=14, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='action', full_name='statefun_tasks.TaskActionRequest.action', index=3,
+      number=4, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='status', full_name='statefun_tasks.PipelineState.status', index=14,
-      number=15, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='uid', full_name='statefun_tasks.TaskActionRequest.uid', index=4,
+      number=5, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='reply', full_name='statefun_tasks.TaskActionRequest.reply',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=3344,
+  serialized_end=3514,
+)
+
+
+_TASKACTIONRESULT = _descriptor.Descriptor(
+  name='TaskActionResult',
+  full_name='statefun_tasks.TaskActionResult',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
     _descriptor.FieldDescriptor(
-      name='paused_tasks', full_name='statefun_tasks.PipelineState.paused_tasks', index=15,
-      number=16, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='id', full_name='statefun_tasks.TaskActionResult.id', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='child_pipelines', full_name='statefun_tasks.PipelineState.child_pipelines', index=16,
-      number=17, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='action', full_name='statefun_tasks.TaskActionResult.action', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='last_task_state', full_name='statefun_tasks.PipelineState.last_task_state', index=17,
-      number=18, type=11, cpp_type=10, label=1,
+      name='result', full_name='statefun_tasks.TaskActionResult.result', index=2,
+      number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='invocation_id', full_name='statefun_tasks.PipelineState.invocation_id', index=18,
-      number=19, type=9, cpp_type=9, label=1,
+      name='uid', full_name='statefun_tasks.TaskActionResult.uid', index=3,
+      number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_PIPELINESTATE_TASKDEFERRALSBYIDENTRY, _PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY, ],
+  nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='before_finally', full_name='statefun_tasks.PipelineState.before_finally',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
-  serialized_start=3358,
-  serialized_end=4345,
+  serialized_start=3516,
+  serialized_end=3641,
 )
 
 
-_CHILDPIPELINE = _descriptor.Descriptor(
-  name='ChildPipeline',
-  full_name='statefun_tasks.ChildPipeline',
+_TASKACTIONEXCEPTION = _descriptor.Descriptor(
+  name='TaskActionException',
+  full_name='statefun_tasks.TaskActionException',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='statefun_tasks.ChildPipeline.id', index=0,
+      name='id', full_name='statefun_tasks.TaskActionException.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='address', full_name='statefun_tasks.ChildPipeline.address', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='action', full_name='statefun_tasks.TaskActionException.action', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='root_id', full_name='statefun_tasks.ChildPipeline.root_id', index=2,
+      name='exception_type', full_name='statefun_tasks.TaskActionException.exception_type', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='root_address', full_name='statefun_tasks.ChildPipeline.root_address', index=3,
+      name='exception_message', full_name='statefun_tasks.TaskActionException.exception_message', index=3,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='caller_id', full_name='statefun_tasks.ChildPipeline.caller_id', index=4,
+      name='stacktrace', full_name='statefun_tasks.TaskActionException.stacktrace', index=4,
       number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='caller_address', full_name='statefun_tasks.ChildPipeline.caller_address', index=5,
+      name='uid', full_name='statefun_tasks.TaskActionException.uid', index=5,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='tasks', full_name='statefun_tasks.ChildPipeline.tasks', index=6,
-      number=7, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='invocation_id', full_name='statefun_tasks.ChildPipeline.invocation_id', index=7,
-      number=8, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4348,
-  serialized_end=4538,
+  serialized_start=3644,
+  serialized_end=3805,
 )
 
 
-_TASKINFO = _descriptor.Descriptor(
-  name='TaskInfo',
-  full_name='statefun_tasks.TaskInfo',
+_TASKSTATUS = _descriptor.Descriptor(
+  name='TaskStatus',
+  full_name='statefun_tasks.TaskStatus',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='task_id', full_name='statefun_tasks.TaskInfo.task_id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_type', full_name='statefun_tasks.TaskInfo.task_type', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='namespace', full_name='statefun_tasks.TaskInfo.namespace', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='worker_name', full_name='statefun_tasks.TaskInfo.worker_name', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_uid', full_name='statefun_tasks.TaskInfo.task_uid', index=4,
-      number=5, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='value', full_name='statefun_tasks.TaskStatus.value', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _TASKSTATUS_STATUS,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4540,
-  serialized_end=4644,
+  serialized_start=3808,
+  serialized_end=3976,
 )
 
 
-_TASKRESULTS_BYUIDENTRY = _descriptor.Descriptor(
-  name='ByUidEntry',
-  full_name='statefun_tasks.TaskResults.ByUidEntry',
+_PIPELINECREATED = _descriptor.Descriptor(
+  name='PipelineCreated',
+  full_name='statefun_tasks.PipelineCreated',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='key', full_name='statefun_tasks.TaskResults.ByUidEntry.key', index=0,
+      name='caller_id', full_name='statefun_tasks.PipelineCreated.caller_id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='value', full_name='statefun_tasks.TaskResults.ByUidEntry.value', index=1,
-      number=2, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
+      name='caller_address', full_name='statefun_tasks.PipelineCreated.caller_address', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='tasks', full_name='statefun_tasks.PipelineCreated.tasks', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
-  serialized_options=b'8\001',
+  serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4718,
-  serialized_end=4784,
+  serialized_start=3978,
+  serialized_end=4079,
 )
 
-_TASKRESULTS = _descriptor.Descriptor(
-  name='TaskResults',
-  full_name='statefun_tasks.TaskResults',
+
+_PIPELINESTATUSCHANGED = _descriptor.Descriptor(
+  name='PipelineStatusChanged',
+  full_name='statefun_tasks.PipelineStatusChanged',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='by_uid', full_name='statefun_tasks.TaskResults.by_uid', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
+      name='status', full_name='statefun_tasks.PipelineStatusChanged.status', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_TASKRESULTS_BYUIDENTRY, ],
+  nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4647,
-  serialized_end=4784,
+  serialized_start=4081,
+  serialized_end=4148,
 )
 
 
-_TASKACTIONREQUEST = _descriptor.Descriptor(
-  name='TaskActionRequest',
-  full_name='statefun_tasks.TaskActionRequest',
+_PIPELINETASKSSKIPPED = _descriptor.Descriptor(
+  name='PipelineTasksSkipped',
+  full_name='statefun_tasks.PipelineTasksSkipped',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='statefun_tasks.TaskActionRequest.id', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='reply_topic', full_name='statefun_tasks.TaskActionRequest.reply_topic', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='reply_address', full_name='statefun_tasks.TaskActionRequest.reply_address', index=2,
-      number=3, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='action', full_name='statefun_tasks.TaskActionRequest.action', index=3,
-      number=4, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='uid', full_name='statefun_tasks.TaskActionRequest.uid', index=4,
-      number=5, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='tasks', full_name='statefun_tasks.PipelineTasksSkipped.tasks', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
-    _descriptor.OneofDescriptor(
-      name='reply', full_name='statefun_tasks.TaskActionRequest.reply',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
   ],
-  serialized_start=4787,
-  serialized_end=4957,
+  serialized_start=4150,
+  serialized_end=4213,
 )
 
 
-_TASKACTIONRESULT = _descriptor.Descriptor(
-  name='TaskActionResult',
-  full_name='statefun_tasks.TaskActionResult',
+_PIPELINETASKFINISHED = _descriptor.Descriptor(
+  name='PipelineTaskFinished',
+  full_name='statefun_tasks.PipelineTaskFinished',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='statefun_tasks.TaskActionResult.id', index=0,
+      name='id', full_name='statefun_tasks.PipelineTaskFinished.id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='action', full_name='statefun_tasks.TaskActionResult.action', index=1,
-      number=2, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
+      name='uid', full_name='statefun_tasks.PipelineTaskFinished.uid', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='result', full_name='statefun_tasks.TaskActionResult.result', index=2,
+      name='status', full_name='statefun_tasks.PipelineTaskFinished.status', index=2,
       number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='uid', full_name='statefun_tasks.TaskActionResult.uid', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='size_in_bytes', full_name='statefun_tasks.PipelineTaskFinished.size_in_bytes', index=3,
+      number=4, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
@@ -1945,116 +1799,102 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4959,
-  serialized_end=5084,
+  serialized_start=4215,
+  serialized_end=4329,
 )
 
 
-_TASKACTIONEXCEPTION = _descriptor.Descriptor(
-  name='TaskActionException',
-  full_name='statefun_tasks.TaskActionException',
+_EVENT = _descriptor.Descriptor(
+  name='Event',
+  full_name='statefun_tasks.Event',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='id', full_name='statefun_tasks.TaskActionException.id', index=0,
+      name='pipeline_id', full_name='statefun_tasks.Event.pipeline_id', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='action', full_name='statefun_tasks.TaskActionException.action', index=1,
-      number=2, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
+      name='pipeline_address', full_name='statefun_tasks.Event.pipeline_address', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='exception_type', full_name='statefun_tasks.TaskActionException.exception_type', index=2,
+      name='root_pipeline_id', full_name='statefun_tasks.Event.root_pipeline_id', index=2,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='exception_message', full_name='statefun_tasks.TaskActionException.exception_message', index=3,
+      name='root_pipeline_address', full_name='statefun_tasks.Event.root_pipeline_address', index=3,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='stacktrace', full_name='statefun_tasks.TaskActionException.stacktrace', index=4,
-      number=5, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='pipeline_created', full_name='statefun_tasks.Event.pipeline_created', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='uid', full_name='statefun_tasks.TaskActionException.uid', index=5,
-      number=6, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
+      name='pipeline_status_changed', full_name='statefun_tasks.Event.pipeline_status_changed', index=5,
+      number=6, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=5087,
-  serialized_end=5248,
-)
-
-
-_TASKSTATUS = _descriptor.Descriptor(
-  name='TaskStatus',
-  full_name='statefun_tasks.TaskStatus',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
     _descriptor.FieldDescriptor(
-      name='value', full_name='statefun_tasks.TaskStatus.value', index=0,
-      number=1, type=14, cpp_type=8, label=1,
-      has_default_value=False, default_value=0,
+      name='pipeline_tasks_skipped', full_name='statefun_tasks.Event.pipeline_tasks_skipped', index=6,
+      number=7, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='pipeline_task_finished', full_name='statefun_tasks.Event.pipeline_task_finished', index=7,
+      number=8, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
-    _TASKSTATUS_STATUS,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
+    _descriptor.OneofDescriptor(
+      name='event', full_name='statefun_tasks.Event.event',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
   ],
-  serialized_start=5251,
-  serialized_end=5419,
+  serialized_start=4332,
+  serialized_end=4731,
 )
 
 _MAPOFSTRINGTOANY_ITEMSENTRY.fields_by_name['value'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _MAPOFSTRINGTOANY_ITEMSENTRY.containing_type = _MAPOFSTRINGTOANY
 _MAPOFSTRINGTOANY.fields_by_name['items'].message_type = _MAPOFSTRINGTOANY_ITEMSENTRY
 _ARRAYOFANY.fields_by_name['items'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _TUPLEOFANY.fields_by_name['items'].message_type = google_dot_protobuf_dot_any__pb2._ANY
@@ -2126,63 +1966,49 @@
 _TASKSTATE_BYUIDENTRY.fields_by_name['value'].message_type = _TASKSPECIFICSTATE
 _TASKSTATE_BYUIDENTRY.containing_type = _TASKSTATE
 _TASKSTATE.fields_by_name['by_uid'].message_type = _TASKSTATE_BYUIDENTRY
 _TASKSTATE.fields_by_name['internal_state'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _TASKSTATE.oneofs_by_name['_internal_state'].fields.append(
   _TASKSTATE.fields_by_name['internal_state'])
 _TASKSTATE.fields_by_name['internal_state'].containing_oneof = _TASKSTATE.oneofs_by_name['_internal_state']
-_TASKDEFERRAL.fields_by_name['tasks'].message_type = _DEFERREDTASK
-_TASKDEFERRAL.fields_by_name['task_result_or_exception'].message_type = _TASKRESULTOREXCEPTION
-_TASKDEFERRAL.oneofs_by_name['_parent_task_address'].fields.append(
-  _TASKDEFERRAL.fields_by_name['parent_task_address'])
-_TASKDEFERRAL.fields_by_name['parent_task_address'].containing_oneof = _TASKDEFERRAL.oneofs_by_name['_parent_task_address']
-_TASKDEFERRAL.oneofs_by_name['_parent_task_id'].fields.append(
-  _TASKDEFERRAL.fields_by_name['parent_task_id'])
-_TASKDEFERRAL.fields_by_name['parent_task_id'].containing_oneof = _TASKDEFERRAL.oneofs_by_name['_parent_task_id']
-_TASKDEFERRAL.oneofs_by_name['_task_result_or_exception'].fields.append(
-  _TASKDEFERRAL.fields_by_name['task_result_or_exception'])
-_TASKDEFERRAL.fields_by_name['task_result_or_exception'].containing_oneof = _TASKDEFERRAL.oneofs_by_name['_task_result_or_exception']
 _PAUSEDTASK.fields_by_name['task_request'].message_type = _TASKREQUEST
-_PIPELINESTATE_TASKDEFERRALSBYIDENTRY.fields_by_name['value'].message_type = _TASKDEFERRAL
-_PIPELINESTATE_TASKDEFERRALSBYIDENTRY.containing_type = _PIPELINESTATE
-_PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY.containing_type = _PIPELINESTATE
-_PIPELINESTATE.fields_by_name['pipeline'].message_type = _PIPELINE
-_PIPELINESTATE.fields_by_name['task_results'].message_type = _TASKRESULTS
-_PIPELINESTATE.fields_by_name['result_before_finally'].message_type = _TASKRESULT
-_PIPELINESTATE.fields_by_name['exception_before_finally'].message_type = _TASKEXCEPTION
-_PIPELINESTATE.fields_by_name['task_state'].message_type = google_dot_protobuf_dot_any__pb2._ANY
-_PIPELINESTATE.fields_by_name['task_deferrals_by_id'].message_type = _PIPELINESTATE_TASKDEFERRALSBYIDENTRY
-_PIPELINESTATE.fields_by_name['task_deferral_ids_by_task_uid'].message_type = _PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY
-_PIPELINESTATE.fields_by_name['status'].message_type = _TASKSTATUS
-_PIPELINESTATE.fields_by_name['paused_tasks'].message_type = _PAUSEDTASK
-_PIPELINESTATE.fields_by_name['child_pipelines'].message_type = _CHILDPIPELINE
-_PIPELINESTATE.fields_by_name['last_task_state'].message_type = google_dot_protobuf_dot_any__pb2._ANY
-_PIPELINESTATE.oneofs_by_name['before_finally'].fields.append(
-  _PIPELINESTATE.fields_by_name['result_before_finally'])
-_PIPELINESTATE.fields_by_name['result_before_finally'].containing_oneof = _PIPELINESTATE.oneofs_by_name['before_finally']
-_PIPELINESTATE.oneofs_by_name['before_finally'].fields.append(
-  _PIPELINESTATE.fields_by_name['exception_before_finally'])
-_PIPELINESTATE.fields_by_name['exception_before_finally'].containing_oneof = _PIPELINESTATE.oneofs_by_name['before_finally']
 _CHILDPIPELINE.fields_by_name['tasks'].message_type = _TASKINFO
-_TASKRESULTS_BYUIDENTRY.fields_by_name['value'].message_type = google_dot_protobuf_dot_any__pb2._ANY
-_TASKRESULTS_BYUIDENTRY.containing_type = _TASKRESULTS
-_TASKRESULTS.fields_by_name['by_uid'].message_type = _TASKRESULTS_BYUIDENTRY
 _TASKACTIONREQUEST.fields_by_name['reply_address'].message_type = _ADDRESS
 _TASKACTIONREQUEST.fields_by_name['action'].enum_type = _TASKACTION
 _TASKACTIONREQUEST.oneofs_by_name['reply'].fields.append(
   _TASKACTIONREQUEST.fields_by_name['reply_topic'])
 _TASKACTIONREQUEST.fields_by_name['reply_topic'].containing_oneof = _TASKACTIONREQUEST.oneofs_by_name['reply']
 _TASKACTIONREQUEST.oneofs_by_name['reply'].fields.append(
   _TASKACTIONREQUEST.fields_by_name['reply_address'])
 _TASKACTIONREQUEST.fields_by_name['reply_address'].containing_oneof = _TASKACTIONREQUEST.oneofs_by_name['reply']
 _TASKACTIONRESULT.fields_by_name['action'].enum_type = _TASKACTION
 _TASKACTIONRESULT.fields_by_name['result'].message_type = google_dot_protobuf_dot_any__pb2._ANY
 _TASKACTIONEXCEPTION.fields_by_name['action'].enum_type = _TASKACTION
 _TASKSTATUS.fields_by_name['value'].enum_type = _TASKSTATUS_STATUS
 _TASKSTATUS_STATUS.containing_type = _TASKSTATUS
+_PIPELINECREATED.fields_by_name['tasks'].message_type = _TASKINFO
+_PIPELINESTATUSCHANGED.fields_by_name['status'].message_type = _TASKSTATUS
+_PIPELINETASKSSKIPPED.fields_by_name['tasks'].message_type = _TASKINFO
+_PIPELINETASKFINISHED.fields_by_name['status'].message_type = _TASKSTATUS
+_EVENT.fields_by_name['pipeline_created'].message_type = _PIPELINECREATED
+_EVENT.fields_by_name['pipeline_status_changed'].message_type = _PIPELINESTATUSCHANGED
+_EVENT.fields_by_name['pipeline_tasks_skipped'].message_type = _PIPELINETASKSSKIPPED
+_EVENT.fields_by_name['pipeline_task_finished'].message_type = _PIPELINETASKFINISHED
+_EVENT.oneofs_by_name['event'].fields.append(
+  _EVENT.fields_by_name['pipeline_created'])
+_EVENT.fields_by_name['pipeline_created'].containing_oneof = _EVENT.oneofs_by_name['event']
+_EVENT.oneofs_by_name['event'].fields.append(
+  _EVENT.fields_by_name['pipeline_status_changed'])
+_EVENT.fields_by_name['pipeline_status_changed'].containing_oneof = _EVENT.oneofs_by_name['event']
+_EVENT.oneofs_by_name['event'].fields.append(
+  _EVENT.fields_by_name['pipeline_tasks_skipped'])
+_EVENT.fields_by_name['pipeline_tasks_skipped'].containing_oneof = _EVENT.oneofs_by_name['event']
+_EVENT.oneofs_by_name['event'].fields.append(
+  _EVENT.fields_by_name['pipeline_task_finished'])
+_EVENT.fields_by_name['pipeline_task_finished'].containing_oneof = _EVENT.oneofs_by_name['event']
 DESCRIPTOR.message_types_by_name['NoneValue'] = _NONEVALUE
 DESCRIPTOR.message_types_by_name['Address'] = _ADDRESS
 DESCRIPTOR.message_types_by_name['MapOfStringToAny'] = _MAPOFSTRINGTOANY
 DESCRIPTOR.message_types_by_name['ArrayOfAny'] = _ARRAYOFANY
 DESCRIPTOR.message_types_by_name['TupleOfAny'] = _TUPLEOFANY
 DESCRIPTOR.message_types_by_name['TaskEntry'] = _TASKENTRY
 DESCRIPTOR.message_types_by_name['GroupEntry'] = _GROUPENTRY
@@ -2192,25 +2018,26 @@
 DESCRIPTOR.message_types_by_name['ArgsAndKwargs'] = _ARGSANDKWARGS
 DESCRIPTOR.message_types_by_name['TaskRequest'] = _TASKREQUEST
 DESCRIPTOR.message_types_by_name['TaskResult'] = _TASKRESULT
 DESCRIPTOR.message_types_by_name['TaskException'] = _TASKEXCEPTION
 DESCRIPTOR.message_types_by_name['TaskResultOrException'] = _TASKRESULTOREXCEPTION
 DESCRIPTOR.message_types_by_name['TaskSpecificState'] = _TASKSPECIFICSTATE
 DESCRIPTOR.message_types_by_name['TaskState'] = _TASKSTATE
-DESCRIPTOR.message_types_by_name['TaskDeferral'] = _TASKDEFERRAL
-DESCRIPTOR.message_types_by_name['DeferredTask'] = _DEFERREDTASK
 DESCRIPTOR.message_types_by_name['PausedTask'] = _PAUSEDTASK
-DESCRIPTOR.message_types_by_name['PipelineState'] = _PIPELINESTATE
 DESCRIPTOR.message_types_by_name['ChildPipeline'] = _CHILDPIPELINE
 DESCRIPTOR.message_types_by_name['TaskInfo'] = _TASKINFO
-DESCRIPTOR.message_types_by_name['TaskResults'] = _TASKRESULTS
 DESCRIPTOR.message_types_by_name['TaskActionRequest'] = _TASKACTIONREQUEST
 DESCRIPTOR.message_types_by_name['TaskActionResult'] = _TASKACTIONRESULT
 DESCRIPTOR.message_types_by_name['TaskActionException'] = _TASKACTIONEXCEPTION
 DESCRIPTOR.message_types_by_name['TaskStatus'] = _TASKSTATUS
+DESCRIPTOR.message_types_by_name['PipelineCreated'] = _PIPELINECREATED
+DESCRIPTOR.message_types_by_name['PipelineStatusChanged'] = _PIPELINESTATUSCHANGED
+DESCRIPTOR.message_types_by_name['PipelineTasksSkipped'] = _PIPELINETASKSSKIPPED
+DESCRIPTOR.message_types_by_name['PipelineTaskFinished'] = _PIPELINETASKFINISHED
+DESCRIPTOR.message_types_by_name['Event'] = _EVENT
 DESCRIPTOR.enum_types_by_name['TaskAction'] = _TASKACTION
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 NoneValue = _reflection.GeneratedProtocolMessageType('NoneValue', (_message.Message,), {
   'DESCRIPTOR' : _NONEVALUE,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.NoneValue)
@@ -2349,87 +2176,35 @@
   'DESCRIPTOR' : _TASKSTATE,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.TaskState)
   })
 _sym_db.RegisterMessage(TaskState)
 _sym_db.RegisterMessage(TaskState.ByUidEntry)
 
-TaskDeferral = _reflection.GeneratedProtocolMessageType('TaskDeferral', (_message.Message,), {
-  'DESCRIPTOR' : _TASKDEFERRAL,
-  '__module__' : 'messages_pb2'
-  # @@protoc_insertion_point(class_scope:statefun_tasks.TaskDeferral)
-  })
-_sym_db.RegisterMessage(TaskDeferral)
-
-DeferredTask = _reflection.GeneratedProtocolMessageType('DeferredTask', (_message.Message,), {
-  'DESCRIPTOR' : _DEFERREDTASK,
-  '__module__' : 'messages_pb2'
-  # @@protoc_insertion_point(class_scope:statefun_tasks.DeferredTask)
-  })
-_sym_db.RegisterMessage(DeferredTask)
-
 PausedTask = _reflection.GeneratedProtocolMessageType('PausedTask', (_message.Message,), {
   'DESCRIPTOR' : _PAUSEDTASK,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.PausedTask)
   })
 _sym_db.RegisterMessage(PausedTask)
 
-PipelineState = _reflection.GeneratedProtocolMessageType('PipelineState', (_message.Message,), {
-
-  'TaskDeferralsByIdEntry' : _reflection.GeneratedProtocolMessageType('TaskDeferralsByIdEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PIPELINESTATE_TASKDEFERRALSBYIDENTRY,
-    '__module__' : 'messages_pb2'
-    # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineState.TaskDeferralsByIdEntry)
-    })
-  ,
-
-  'TaskDeferralIdsByTaskUidEntry' : _reflection.GeneratedProtocolMessageType('TaskDeferralIdsByTaskUidEntry', (_message.Message,), {
-    'DESCRIPTOR' : _PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY,
-    '__module__' : 'messages_pb2'
-    # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineState.TaskDeferralIdsByTaskUidEntry)
-    })
-  ,
-  'DESCRIPTOR' : _PIPELINESTATE,
-  '__module__' : 'messages_pb2'
-  # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineState)
-  })
-_sym_db.RegisterMessage(PipelineState)
-_sym_db.RegisterMessage(PipelineState.TaskDeferralsByIdEntry)
-_sym_db.RegisterMessage(PipelineState.TaskDeferralIdsByTaskUidEntry)
-
 ChildPipeline = _reflection.GeneratedProtocolMessageType('ChildPipeline', (_message.Message,), {
   'DESCRIPTOR' : _CHILDPIPELINE,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.ChildPipeline)
   })
 _sym_db.RegisterMessage(ChildPipeline)
 
 TaskInfo = _reflection.GeneratedProtocolMessageType('TaskInfo', (_message.Message,), {
   'DESCRIPTOR' : _TASKINFO,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.TaskInfo)
   })
 _sym_db.RegisterMessage(TaskInfo)
 
-TaskResults = _reflection.GeneratedProtocolMessageType('TaskResults', (_message.Message,), {
-
-  'ByUidEntry' : _reflection.GeneratedProtocolMessageType('ByUidEntry', (_message.Message,), {
-    'DESCRIPTOR' : _TASKRESULTS_BYUIDENTRY,
-    '__module__' : 'messages_pb2'
-    # @@protoc_insertion_point(class_scope:statefun_tasks.TaskResults.ByUidEntry)
-    })
-  ,
-  'DESCRIPTOR' : _TASKRESULTS,
-  '__module__' : 'messages_pb2'
-  # @@protoc_insertion_point(class_scope:statefun_tasks.TaskResults)
-  })
-_sym_db.RegisterMessage(TaskResults)
-_sym_db.RegisterMessage(TaskResults.ByUidEntry)
-
 TaskActionRequest = _reflection.GeneratedProtocolMessageType('TaskActionRequest', (_message.Message,), {
   'DESCRIPTOR' : _TASKACTIONREQUEST,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.TaskActionRequest)
   })
 _sym_db.RegisterMessage(TaskActionRequest)
 
@@ -2450,15 +2225,47 @@
 TaskStatus = _reflection.GeneratedProtocolMessageType('TaskStatus', (_message.Message,), {
   'DESCRIPTOR' : _TASKSTATUS,
   '__module__' : 'messages_pb2'
   # @@protoc_insertion_point(class_scope:statefun_tasks.TaskStatus)
   })
 _sym_db.RegisterMessage(TaskStatus)
 
+PipelineCreated = _reflection.GeneratedProtocolMessageType('PipelineCreated', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINECREATED,
+  '__module__' : 'messages_pb2'
+  # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineCreated)
+  })
+_sym_db.RegisterMessage(PipelineCreated)
+
+PipelineStatusChanged = _reflection.GeneratedProtocolMessageType('PipelineStatusChanged', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINESTATUSCHANGED,
+  '__module__' : 'messages_pb2'
+  # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineStatusChanged)
+  })
+_sym_db.RegisterMessage(PipelineStatusChanged)
+
+PipelineTasksSkipped = _reflection.GeneratedProtocolMessageType('PipelineTasksSkipped', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINETASKSSKIPPED,
+  '__module__' : 'messages_pb2'
+  # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineTasksSkipped)
+  })
+_sym_db.RegisterMessage(PipelineTasksSkipped)
+
+PipelineTaskFinished = _reflection.GeneratedProtocolMessageType('PipelineTaskFinished', (_message.Message,), {
+  'DESCRIPTOR' : _PIPELINETASKFINISHED,
+  '__module__' : 'messages_pb2'
+  # @@protoc_insertion_point(class_scope:statefun_tasks.PipelineTaskFinished)
+  })
+_sym_db.RegisterMessage(PipelineTaskFinished)
+
+Event = _reflection.GeneratedProtocolMessageType('Event', (_message.Message,), {
+  'DESCRIPTOR' : _EVENT,
+  '__module__' : 'messages_pb2'
+  # @@protoc_insertion_point(class_scope:statefun_tasks.Event)
+  })
+_sym_db.RegisterMessage(Event)
+
 
 _MAPOFSTRINGTOANY_ITEMSENTRY._options = None
 _TASKREQUEST_METAENTRY._options = None
 _TASKSTATE_BYUIDENTRY._options = None
-_PIPELINESTATE_TASKDEFERRALSBYIDENTRY._options = None
-_PIPELINESTATE_TASKDEFERRALIDSBYTASKUIDENTRY._options = None
-_TASKRESULTS_BYUIDENTRY._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/pipeline_builder.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/pipeline_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from re import L
 from statefun_tasks.types import Task, Group, RetryPolicy, ProtobufSerialisable
 from statefun_tasks.utils import _gen_id
-from statefun_tasks.pipeline import _Pipeline
 from statefun_tasks.messages_pb2 import TaskRequest, Pipeline
 from statefun_tasks.builtin import builtin
+from statefun_tasks.serialisation import pack_any, DefaultSerialiser
 from typing import Iterable
 import math
 
 
 def in_parallel(entries: list, max_parallelism=None, num_stages:int = 1, return_exceptions=False):
     """
     Creates a parallism of tasks to be run concurrently
@@ -274,35 +274,14 @@
         try:
             task = finally_action.to_task(args, kwargs, is_finally=True)
             self._pipeline.append(task)
         except AttributeError:
             raise AttributeError(f'Function {finally_action.__module__}.{finally_action.__name__} should be decorated with tasks.bind')
         return self
 
-    def to_pipeline(self, serialiser=None, is_fruitful=True, events=None):
-        """
-        Concretises the builder into a pipeline
-
-        :param option serialiser: the serialiser to use such as DefaultSerialiser
-        :param option is_fruitful: whether this pipeline is fruitful (i.e. returns a result). Default is True
-        :param option events: event handler instance if this pipeline should fire events
-
-        :return: a Flink Tasks pipeline
-        """
-        self.validate()
-
-        return _Pipeline(self._pipeline, 
-            inline=self._inline, 
-            initial_args=self._initial_args,
-            initial_kwargs=self._initial_kwargs,
-            initial_state=self._initial_state,
-            is_fruitful=is_fruitful,
-            serialiser=serialiser,
-            events=events)
-
     def set_task_defaults(self, default_namespace, default_worker_name) ->  'PipelineBuilder':
         """
         Sets defaults on task entries if they are not set
         :return: the builder
         """
         for task in self._get_tasks():
             if task.namespace == '':
@@ -378,15 +357,33 @@
     def to_proto(self, serialiser=None) -> Pipeline:
         """
         Serialises the pipeline to protobuf
 
         :param serialiser: the serialiser to use such as DefaultSerialiser
         :return: Pipeline protobuf message
         """
-        return self.to_pipeline(serialiser=serialiser).to_proto()
+        self.validate()
+
+        serialiser = serialiser or DefaultSerialiser()
+
+        pipeline = Pipeline(
+            entries=[p.to_proto(serialiser) for p in self._pipeline], 
+            inline=self._inline)
+
+        if self._initial_args is not None:
+            pipeline.initial_args.CopyFrom(pack_any(serialiser.to_proto(self._initial_args)))
+        
+        if self._initial_kwargs is not None:
+            pipeline.initial_kwargs.CopyFrom(serialiser.to_proto(self._initial_kwargs))
+
+        if self._initial_state is not None:
+            pipeline.initial_state.CopyFrom(pack_any(serialiser.to_proto(self._initial_state)))
+        
+        return pipeline
+
 
     @staticmethod
     def from_proto(pipeline_proto: Pipeline) -> 'PipelineBuilder':
         """
         Deserialises the pipeline from protobuf
 
         :param pipeline_proto: the pipeline as protobuf
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/protobuf.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import itertools
 from abc import ABC, abstractmethod
 from statefun_tasks.utils import _is_tuple
-from statefun_tasks.messages_pb2 import MapOfStringToAny, ArrayOfAny, TupleOfAny, TaskEntry, GroupEntry, NoneValue, \
-    TaskRetryPolicy, TaskRequest, TaskResult, TaskException, TaskState, TaskResults, Pipeline, PipelineEntry, Address, \
-    ArgsAndKwargs, PipelineState, TaskResultOrException
-
+from statefun_tasks.messages_pb2 import (MapOfStringToAny, ArrayOfAny, TupleOfAny, TaskEntry, GroupEntry, NoneValue,
+                                         TaskRetryPolicy, TaskRequest, TaskResult, TaskException, TaskState, 
+                                         Pipeline, PipelineEntry, Address,ArgsAndKwargs, TaskResultOrException)
 from google.protobuf.wrappers_pb2 import DoubleValue, Int64Value, BoolValue, StringValue, BytesValue
 from google.protobuf.any_pb2 import Any
 from google.protobuf.message import Message
 
 from typing import Union, TypeVar, Generic, Iterable, List
 
 
@@ -28,20 +27,18 @@
     TaskEntry,
     GroupEntry,
     TaskRetryPolicy,
     TaskRequest,
     TaskResult,
     TaskException,
     TaskState,
-    TaskResults,
     Pipeline,
     PipelineEntry,
     Address,
     ArgsAndKwargs,
-    PipelineState,
     TaskResultOrException
 ]
 
 TProtoType = TypeVar('TProtoType', bound=Message)
 
 
 class ObjectProtobufConverter(ABC, Generic[TProtoType]):
@@ -148,20 +145,14 @@
     compatible_converter = next((c for c in converters if c.can_convert_from_proto(v)), None)
     if compatible_converter is None:
         # task args can be protobuf messages, so not everything needs to be converted
         return v
     return compatible_converter.convert_from_proto(v)
 
 
-def _parse_any_from_bytes(bytes) -> Any:
-    proto = Any()
-    proto.ParseFromString(bytes)
-    return proto
-
-
 def _is_wrapped_known_proto_type(value, known_proto_types):
     return isinstance(value, Any) and any(
         (value.Is(proto_type.DESCRIPTOR) for proto_type in itertools.chain(_FRAMEWORK_KNOWN_PROTO_TYPES, known_proto_types)))
 
 
 def _convert_to_proto(data, protobuf_converters: Iterable[ObjectProtobufConverter]) \
         -> Union[MapOfStringToAny, ArrayOfAny, TupleOfAny, Message]:
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/task_builder.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/task_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from statefun_tasks.serialisation import DefaultSerialiser
 from statefun_tasks.pipeline_builder import PipelineBuilder
-
-from statefun_tasks.types import Task, RetryPolicy, \
-    TASK_STATE_TYPE, TASK_REQUEST_TYPE, TASK_RESULT_TYPE, TASK_EXCEPTION_TYPE, PIPELINE_STATE_TYPE
-
+from statefun_tasks.types import (Task, RetryPolicy, TASK_STATE_TYPE, TASK_REQUEST_TYPE, 
+                                  TASK_RESULT_TYPE, TASK_EXCEPTION_TYPE)
 from statefun_tasks.messages_pb2 import TaskResult, TaskException, TaskRequest, Address
 from statefun_tasks.type_helpers import _create_task_result, _create_task_exception
 from statefun_tasks.context import TaskContext
 from statefun_tasks.utils import _task_type_for, _unpack_single_tuple_args, _gen_id
-from statefun_tasks.pipeline import _Pipeline
 from statefun_tasks.tasks import FlinkTask
-from statefun_tasks.task_impl.handlers import TaskRequestHandler, TaskResponseHandler, TaskActionHandler, ChildPipelineHandler
+from statefun_tasks.handlers import TaskRequestHandler, TaskActionHandler
 from statefun_tasks.events import EventHandlers
-from statefun_tasks.builtin_tasks import run_pipeline, flatten_results
 
 from statefun import ValueSpec, Context, Message
 from datetime import timedelta
 from functools import partial
-from typing import Callable, Any, Tuple
 import logging
 
 _log = logging.getLogger('FlinkTasks')
 
 
 class FlinkTasks(object):
     """
@@ -33,48 +28,47 @@
     :param default_namespace: namespace to expose functions under. Maps to Flink Statefun function namespace in module.yaml
     :param default_worker_name: worker name to expose.  Maps to Flink Statefun function type in module.yaml
     :param egress_type_name: egress type name.  Maps to Flink Statefun egress in module.yaml
     :param optional egress_message_max_size: maximum size of an egress message in bytes. If specified attempts to send messages over this size will raise a MessageSizeExceeded exception
     :param optional serialiser: serialiser to use (will use DefaultSerialiser if not set)
     :param optional state_expiration: duration after which state will be expired by Flink (expire_after_call)
     :param optional keep_task_state: whether to keep state (request, result) associated with tasks as well as pipelines (defaults to false)
+    :param optional embedded_pipeline_namespace: namespace of the embedded function that pipelines will be forwarded to
+    :param optional embedded_pipeline_type: type name of the embedded function that pipelines will be forwarded to
     """
     def __init__(self, 
                  default_namespace: str = None, 
                  default_worker_name: str = None, 
                  egress_type_name: str = None, 
                  egress_message_max_size: int = None, 
                  serialiser = None, 
                  state_expiration: timedelta = None,
-                 keep_task_state = False):
+                 keep_task_state = False,
+                 embedded_pipeline_namespace: str = None,
+                 embedded_pipeline_type: str = None):
+    
         self._default_namespace = default_namespace
         self._default_worker_name = default_worker_name
         self._egress_type_name = egress_type_name
         self._egress_message_max_size = egress_message_max_size
         self._serialiser = serialiser if serialiser is not None else DefaultSerialiser()
         self._bindings = {}
         self._events = EventHandlers()
         
         # to register in Flink's @functions.bind() attribute
         self._value_specs = [
             ValueSpec(name="task_request", type=TASK_REQUEST_TYPE, expire_after_call=state_expiration),
             ValueSpec(name="task_result", type=TASK_RESULT_TYPE, expire_after_call=state_expiration),
             ValueSpec(name="task_exception", type=TASK_EXCEPTION_TYPE, expire_after_call=state_expiration),
-            ValueSpec(name="task_state", type=TASK_STATE_TYPE, expire_after_call=state_expiration),
-            ValueSpec(name="pipeline_state", type=PIPELINE_STATE_TYPE, expire_after_call=state_expiration)
+            ValueSpec(name="task_state", type=TASK_STATE_TYPE, expire_after_call=state_expiration)
         ]
 
-        self.register_builtin(run_pipeline, with_context=True, with_state=True)
-        self.register_builtin(flatten_results)
-
         self._handlers = [
-            TaskRequestHandler(keep_task_state),
-            TaskResponseHandler(),
-            TaskActionHandler(),
-            ChildPipelineHandler()
+            TaskRequestHandler(embedded_pipeline_namespace, embedded_pipeline_type, keep_task_state),
+            TaskActionHandler()
         ]
 
     @staticmethod
     def extend(function, retry_policy: RetryPolicy = None, **params):
         """
         Adds the extensions to make a function unsable by a PipelineBuilder -> fn.send(), fn.to_task() and fn.defaults()
 
@@ -162,24 +156,14 @@
         EventHandler for this FlinkTasks instance
         """
         return self._events
 
     def value_specs(self):
         return self._value_specs
 
-    def register_builtin(self, fun, **params):
-        """
-        Registers a built in Flink Task e.g. __builtins.run_pipeline
-        This should only be used if you want to provide your own built in (pre-defined) tasks
-
-        :param fun: a function, partial or lambda representing the built in
-        :param params: any additional parameters to the Flink Task (such as a retry policy)
-        """
-        self._bindings[fun.task_name] = FlinkTask(fun, self._serialiser, self.events, **params)
-
     def register(self, fun, wrapper=None, module_name=None, **params):
         """
         Registers a Python function as a Flink Task.
         Normally you would attribute the function with @tasks.bind() instead
 
         :param fun: the python function
         :param optional wrapper: if wrapping a task function with e.g. functools.wraps then pass the wrapper here
@@ -309,28 +293,14 @@
         :param ex: the exception to return
         :param optional delay: the delay before Flink sends the result
         :param optional cancellation_token: a cancellation token to associate with this message
         """
         task_exception = _create_task_exception(task_input, ex)
         await self.emit_result(context, task_input, task_exception, delay, cancellation_token)
 
-    def get_pipeline(self, context):
-        pipeline_protos = context.pipeline_state.pipeline
-
-        if pipeline_protos is not None:
-            return _Pipeline.from_proto(pipeline_protos, self._serialiser, self._events)
-        else:
-            raise ValueError(f'Missing pipeline for task_id - {context.get_task_id()}')
-
-    def try_get_pipeline(self, context):
-        try:
-            return self.get_pipeline(context)
-        except:
-            return None
-
     async def emit_result(self, context, task_input, task_result, delay: timedelta=None, cancellation_token: str = None):
         # copy over invocation id and notify we are about to emit a result
         if isinstance(task_result, (TaskResult, TaskException)):
             task_result.invocation_id = task_input.invocation_id
             await self.events.notify_emit_result(context, task_result)
             
         # send a message to egress if reply_topic was specified
@@ -340,24 +310,16 @@
         # or call back to a particular flink function if reply_address was specified
         elif task_input.HasField('reply_address'):
             address, identifer = context.to_address_and_id(task_input.reply_address)
             context.send_message(address, identifer, task_result, delay, cancellation_token)
 
         # otherwise call back to the caller (if there is one)
         elif isinstance(task_input, TaskRequest):
-            address, caller_id = self._get_caller_address_and_id(context, task_input)
+            address = context.get_original_caller_address()
+            caller_id = context.get_original_caller_id()
+
             if address is not None and caller_id is not None:
                 context.send_message(address, caller_id, task_result, delay, cancellation_token)
 
         # clean up
         if task_input.uid in context.task_state.by_uid:
             del context.task_state.by_uid[task_input.uid]
-
-    @staticmethod
-    def _get_caller_address_and_id(context, task_request):
-        task_state = context.task_state.by_uid[task_request.uid]
-        
-        # either as original caller (e.g. if this is a result of a retry) or context.get_caller_...() otherwise
-        address = task_state.original_caller_address if task_state.original_caller_address != '' else context.get_caller_address()
-        caller_id = task_state.original_caller_id if task_state.original_caller_id != '' else context.get_caller_id()
-
-        return address, caller_id
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/message_handler.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/statefun_tasks/task_impl/handlers/task_request_handler.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/handlers/task_request_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from statefun_tasks.context import TaskContext
-from statefun_tasks.task_impl.handlers import MessageHandler
-from statefun_tasks.types import TASK_REQUEST_TYPE, PipelineInProgress
-from statefun_tasks.type_helpers import _create_task_exception
-from statefun_tasks.messages_pb2 import TaskRequest
+from statefun_tasks.handlers import MessageHandler
+from statefun_tasks.types import TASK_REQUEST_TYPE
+from statefun_tasks.messages_pb2 import TaskRequest, Address
 from statefun import Message
 from datetime import timedelta
 
 
 class TaskRequestHandler(MessageHandler):
-    def __init__(self, keep_task_state=True):
+    def __init__(self, embedded_pipeline_namespace: str=None, embedded_pipeline_type: str=None, keep_task_state=True):
+        self._embedded_pipeline_namespace = embedded_pipeline_namespace
+        self._embedded_pipeline_type = embedded_pipeline_type
         self._keep_task_state = keep_task_state
         pass
 
     def unpack(self, context: TaskContext, message: Message):
         if message.is_type(TASK_REQUEST_TYPE):
             task_input = message.as_type(TASK_REQUEST_TYPE)
             
@@ -34,52 +35,46 @@
 
         flink_task = tasks.get_task(task_request.type)
 
         # notify started
         await tasks.events.notify_task_started(context, task_request)
         
         # run task code
-        task_result, task_exception, pipeline, state = await flink_task.run(context, task_request)
-
-        # if a pipeline is returned then try to reset its state in case it already exists
-        if pipeline is not None:
-            try:
-                pipeline.reset(context)
-            except PipelineInProgress as ex:  # can't re-run a running pipeline.  Must wait for it to finish
-                task_exception, pipeline = _create_task_exception(task_request, ex), None
+        task_result, task_exception, pipeline, is_fruitful = await flink_task.run(context, task_request)
 
         # notify finished
         await tasks.events.notify_task_finished(context, task_result, task_exception, is_pipeline=pipeline is not None)
 
-        # if task returns a pipeline then start it if we can
-        if pipeline is not None and await pipeline.handle_message(context, task_request, state):
-            ()
+        # if task returns a pipeline then forward to pipeline function
+        if pipeline is not None:
+            self._send_pipeline_request(context, task_request, task_result, is_fruitful)
 
-        # else if we have an task exception, attempt retry or return the error
-        elif task_exception is not None:
+        # if we have an task exception, attempt retry or return the error
+        if task_exception is not None:
             if await self._attempt_retry(context, tasks, task_request, task_exception):
                 return  # we have triggered a retry so ignore the result of this invocation
 
             context.storage.task_exception = task_exception
             await tasks.emit_result(context, task_request, task_exception)
 
-        # else if we have a task result return it
+        # else if we have a task result return it unless the result is a pipeline
         elif task_result is not None:
             context.storage.task_result = task_result
-            await tasks.emit_result(context, task_request, task_result)
 
-        if not self._keep_task_state:
-            # clear state from intermediate tasks
             if pipeline is None:
-                del context.storage.task_request
+                await tasks.emit_result(context, task_request, task_result)
 
+        if not self._keep_task_state:
+            # clear state from intermediate tasks
+            del context.storage.task_request
             del context.storage.task_result
             del context.storage.task_exception
 
-    async def _attempt_retry(self, context, tasks, task_request, task_exception):
+    @staticmethod
+    async def _attempt_retry(context, tasks, task_request, task_exception):
         task_state = context.task_state.by_uid[task_request.uid]
 
         if task_exception.maybe_retry and task_exception.retry_policy is not None:           
             if task_state.retry_count >= task_exception.retry_policy.max_retries:
                 return False
 
             # increment retry count
@@ -104,7 +99,43 @@
 
             # notify retry
             await tasks.events.notify_task_retry(context, task_request, task_state.retry_count)
 
             return True
 
         return False
+    
+    def _send_pipeline_request(self, context, task_request, task_result, is_fruitful):
+        if self._embedded_pipeline_namespace is None or self._embedded_pipeline_type is None:
+            raise ValueError('Unable to forward pipeline to embedded pipeline function. \
+                             Missing configuration in FlinkTasks(embedded_pipeline_namespace=..., embedded_pipeline_type=...)')
+
+        pipeline_request = TaskRequest(
+                id=task_request.id,
+                uid=task_request.uid,
+                invocation_id=task_request.invocation_id,
+                type="__builtins.run_pipeline",
+                is_fruitful=is_fruitful
+        )
+
+        pipeline_request.request.CopyFrom(task_result.result)
+        pipeline_request.state.CopyFrom(task_result.state)
+
+        # send the result of the pipeline to egress if reply_topic was specified
+        if task_request.HasField('reply_topic'):
+            pipeline_request.reply_topic = task_request.reply_topic
+
+        # or call back to a particular flink function if reply_address was specified
+        elif task_request.HasField('reply_address'):
+            pipeline_request.reply_address.CopyFrom(task_request.reply_address)
+
+        # otherwise call back to the caller (if there is one)
+        else:
+            address = context.get_original_caller_address()
+            caller_id = context.get_original_caller_id()
+
+            if address is not None and '/' in address and caller_id is not None:
+                namespace, type = address.split('/')
+                address = Address(namespace=namespace, type=type, id=caller_id)
+                pipeline_request.reply_address.CopyFrom(address)
+            
+        context.send_message(f'{self._embedded_pipeline_namespace}/{self._embedded_pipeline_type}', pipeline_request.uid, pipeline_request)
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/tasks.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def function(self):
         """
         The Python function that this FlinkTask wraps
         """
         return self._fun
 
     async def run(self, task_context: TaskContext, task_request: TaskRequest):
-        task_result, task_exception, pipeline, effect = None, None, None, None
+        task_result, task_exception, pipeline, effect, is_fruitful = None, None, None, None, self._is_fruitful
 
         task_args, kwargs, fn_state = self._to_task_args_and_kwargs(task_context, task_request)
 
         # run the flink task
         try:
             fn_result = self._fun(*task_args, **kwargs)
             
@@ -62,31 +62,31 @@
                 fn_result = await fn_result               
 
             # result of a task might be wrapped in an effect
             if isinstance(fn_result, Effect):
                 effect = fn_result
                 fn_result = effect.fn_result
                 
-            pipeline, task_result, fn_state = self._to_pipeline_or_task_result(task_context, task_request, fn_result, fn_state)
+            pipeline, task_result, is_fruitful = self._to_pipeline_or_task_result(task_request, fn_result, fn_state)
 
             # apply effects if we have them
             if effect is not None:
                 effect.apply(task_result)
 
         except YieldTaskInvocation as e:
             # task yielded so we don't output anything
             ()
 
         except Exception as e:
             # we errored so return a task_exception instead
             task_exception = self._to_task_exception(task_request, e)
 
-        return task_result, task_exception, pipeline, fn_state
+        return task_result, task_exception, pipeline, is_fruitful
 
-    def _to_pipeline_or_task_result(self, task_context, task_request, fn_result, fn_state):
+    def _to_pipeline_or_task_result(self, task_request, fn_result, fn_state):
         pipeline, is_fruitful = None, self._is_fruitful
 
         if is_fruitful and task_request.HasField('is_fruitful'):
             is_fruitful = task_request.is_fruitful
 
         # if single result then wrap in tuple as this is the maximal case
         if not _is_tuple(fn_result):
@@ -104,31 +104,26 @@
 
         # if a single element tuple remains then unpack back to single value
         # so (8,) becomes 8 but (8,9) remains a tuple
         fn_result = fn_result[0] if len(fn_result) == 1 else fn_result
 
         # result of the task might be a Flink pipeline
         if isinstance(fn_result, PipelineBuilder):
-            # this new pipeline which once complete will yield the result of the whole pipeline
-            # back to the caller as if it were a simple task
-            pipeline = fn_result.set_task_defaults(
-                default_namespace=task_context.get_namespace(), 
-                default_worker_name=task_context.get_worker_name()).\
-            to_pipeline(serialiser=self._serialiser, is_fruitful=is_fruitful, events=self._events)
-            fn_result = ()
+            pipeline = fn_result.to_proto(self._serialiser)
+            fn_result = pipeline
 
-        # drop the result if the task is marked as not fruitful or caller has asked for the result to be dropped
-        if not is_fruitful:
+        # else drop the result if the task is marked as not fruitful or caller has asked for the result to be dropped
+        elif not is_fruitful:
             fn_result = ()
             
         task_result = _create_task_result(task_request)
 
         self._serialiser.serialise_result(task_result, fn_result, fn_state)
 
-        return pipeline, task_result, fn_state
+        return pipeline, task_result, is_fruitful
 
     def _to_task_exception(self, task_request, ex):
         # use retry policy on task request first then fallback to task definition
         task_retry_policy = task_request.retry_policy
         if not task_request.HasField('retry_policy'):
             task_retry_policy = self._retry_policy
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/type_helpers.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/type_helpers.py`

 * *Files identical despite different names*

### Comparing `statefun-tasks-0.9.93/statefun_tasks/types.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from statefun_tasks.utils import _type_name, _gen_id
-from statefun_tasks.messages_pb2 import PipelineState, TaskState, TaskRequest, TaskResult, TaskException, \
-    TaskActionRequest, TaskActionResult, TaskActionException, TaskEntry, GroupEntry, PipelineEntry, TaskRetryPolicy, \
-    Pipeline, ChildPipeline
-
+from statefun_tasks.messages_pb2 import (TaskState, TaskRequest, TaskResult, TaskException, TaskActionRequest, 
+                                         TaskActionResult, TaskActionException, TaskEntry, GroupEntry, PipelineEntry, TaskRetryPolicy, 
+                                         Pipeline, ChildPipeline)
 from statefun import make_protobuf_type
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from datetime import timedelta
 from collections import deque
 
 # Protobuf type registrations required by Flink Statefun API
-PIPELINE_STATE_TYPE = make_protobuf_type(PipelineState, namespace='io.statefun_tasks.types')
 TASK_STATE_TYPE = make_protobuf_type(TaskState, namespace='io.statefun_tasks.types')
 TASK_REQUEST_TYPE = make_protobuf_type(TaskRequest, namespace='io.statefun_tasks.types')
 TASK_RESULT_TYPE = make_protobuf_type(TaskResult, namespace='io.statefun_tasks.types')
 TASK_EXCEPTION_TYPE = make_protobuf_type(TaskException, namespace='io.statefun_tasks.types')
 TASK_ACTION_REQUEST_TYPE = make_protobuf_type(TaskActionRequest, namespace='io.statefun_tasks.types')
 TASK_ACTION_RESULT_TYPE = make_protobuf_type(TaskActionResult, namespace='io.statefun_tasks.types')
 TASK_ACTION_EXCEPTION_TYPE = make_protobuf_type(TaskActionException, namespace='io.statefun_tasks.types')
 CHILD_PIPELINE_TYPE = make_protobuf_type(ChildPipeline, namespace='io.statefun_tasks.types')
 
 
 _VALUE_TYPE_MAP = {
-    TaskState: PIPELINE_STATE_TYPE,
     TaskState: TASK_STATE_TYPE,
     TaskRequest: TASK_REQUEST_TYPE,
     TaskResult: TASK_RESULT_TYPE,
     TaskException: TASK_EXCEPTION_TYPE,
     TaskActionRequest: TASK_ACTION_REQUEST_TYPE,
     TaskActionResult: TASK_ACTION_RESULT_TYPE,
     TaskActionException: TASK_ACTION_EXCEPTION_TYPE,
@@ -348,19 +345,14 @@
 
 
 class TaskCancelledException(TasksException):
     def __init__(self, message):
         super().__init__(message)
 
 
-class PipelineInProgress(TasksException):
-    def __init__(self, message):
-        super().__init__(message)
-
-
 class YieldTaskInvocation(Exception):
     def __init__(self):
         super().__init__()
 
 
 class ProtobufSerialisable(ABC):
     @abstractmethod
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks/utils.py` & `statefun-tasks-1.0.0rc0/statefun_tasks/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from google.protobuf.message import Message
 from google.protobuf.any_pb2 import Any
 
 import inspect
 from uuid import uuid4
 from typing import get_type_hints
-from itertools import chain
 
 
 def _gen_id():
     return str(uuid4())
 
 
 def _type_name(thing):
@@ -19,29 +18,14 @@
 
 
 def _task_type_for(fun, module_name=None):
     module = fun.__module__ if module_name is None else module_name
     return ".".join([module, fun.__name__])
 
 
-def _try_next(iterator):
-    try:
-        return next(iterator)
-    except StopIteration:
-        return None
-
-
-def _try_peek(iterator):
-    try:
-        n = next(iterator)
-        return n, chain([n], iterator)
-    except StopIteration:
-        return None, iterator
-
-
 def _is_named_tuple(value):
     # duck test to see if a value is a NamedTuple and not just a tuple
     if not isinstance(value, tuple):
         return False
 
     return hasattr(type(value), '_fields')
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks.egg-info/PKG-INFO` & `statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statefun-tasks
-Version: 0.9.93
+Version: 1.0.0rc0
 Summary: Tasks API for Stateful Functions on Flink
 Home-page: https://fransking.github.io/flink-statefun-tasks
 Author: Frans King & Luke Ashworth
 Author-email: frans.king@sbbsystems.com
 License: https://www.apache.org/licenses/LICENSE-2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -37,8 +37,9 @@
     return f'{greeting}.  So now I will say goodbye'
 ```
 
 Try the [demo](https://flink-demo-az.sbbsystems.co.uk).
 
 Additional documentation can be found [here](https://fransking.github.io/flink-statefun-tasks).
 
+The pipeline function can be downloaded [here](https://github.com/fransking/flink-statefun-tasks-embedded).
```

### Comparing `statefun-tasks-0.9.93/statefun_tasks.egg-info/SOURCES.txt` & `statefun-tasks-1.0.0rc0/statefun_tasks.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 setup.py
 statefun_tasks/__init__.py
 statefun_tasks/builtin.py
 statefun_tasks/builtin_tasks.py
 statefun_tasks/context.py
 statefun_tasks/messages_pb2.py
-statefun_tasks/pipeline.py
 statefun_tasks/pipeline_builder.py
 statefun_tasks/protobuf.py
 statefun_tasks/serialisation.py
 statefun_tasks/task_builder.py
 statefun_tasks/tasks.py
 statefun_tasks/type_helpers.py
 statefun_tasks/types.py
@@ -27,26 +26,11 @@
 statefun_tasks/effects/effect.py
 statefun_tasks/effects/pause_pipeline_effect.py
 statefun_tasks/events/__init__.py
 statefun_tasks/events/event_handlers.py
 statefun_tasks/extensions/__init__.py
 statefun_tasks/extensions/inline_tasks/__init__.py
 statefun_tasks/extensions/inline_tasks/inline_tasks_impl.py
-statefun_tasks/pipeline_impl/__init__.py
-statefun_tasks/pipeline_impl/handlers/__init__.py
-statefun_tasks/pipeline_impl/handlers/begin_pipeline_handler.py
-statefun_tasks/pipeline_impl/handlers/cancel_pipeline_handler.py
-statefun_tasks/pipeline_impl/handlers/continue_pipeline_handler.py
-statefun_tasks/pipeline_impl/handlers/end_pipeline_handler.py
-statefun_tasks/pipeline_impl/handlers/pipeline_message_handler.py
-statefun_tasks/pipeline_impl/helpers/__init__.py
-statefun_tasks/pipeline_impl/helpers/pipeline_graph.py
-statefun_tasks/pipeline_impl/helpers/result_aggregator.py
-statefun_tasks/pipeline_impl/helpers/result_emitter.py
-statefun_tasks/pipeline_impl/helpers/task_submitter.py
-statefun_tasks/task_impl/__init__.py
-statefun_tasks/task_impl/handlers/__init__.py
-statefun_tasks/task_impl/handlers/child_pipeline_handler.py
-statefun_tasks/task_impl/handlers/message_handler.py
-statefun_tasks/task_impl/handlers/task_action_handler.py
-statefun_tasks/task_impl/handlers/task_request_handler.py
-statefun_tasks/task_impl/handlers/task_response_handler.py
+statefun_tasks/handlers/__init__.py
+statefun_tasks/handlers/message_handler.py
+statefun_tasks/handlers/task_action_handler.py
+statefun_tasks/handlers/task_request_handler.py
```

