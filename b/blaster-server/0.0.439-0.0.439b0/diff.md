# Comparing `tmp/blaster-server-0.0.439.tar.gz` & `tmp/blaster-server-0.0.439b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.439.tar", last modified: Fri Jul 28 21:35:50 2023, max compression
+gzip compressed data, was "blaster-server-0.0.439b0.tar", last modified: Tue Aug  8 12:04:26 2023, max compression
```

## Comparing `blaster-server-0.0.439.tar` & `blaster-server-0.0.439b0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.439/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.439/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-28 21:35:50.748765 blaster-server-0.0.439/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.439/README.md
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1124 2023-06-02 13:04:11.000000 blaster-server-0.0.439/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/cloud/aws/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.439/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/connection_pool.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.439/blaster/env.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.439/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-07-19 07:59:01.000000 blaster-server-0.0.439/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15799 2023-07-27 00:06:27.000000 blaster-server-0.0.439/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38638 2023-07-27 00:05:21.000000 blaster-server-0.0.439/blaster/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/tools/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    44805 2023-07-28 20:32:15.000000 blaster-server-0.0.439/blaster/tools/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.439/blaster/tools/sanitize_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.744765 blaster-server-0.0.439/blaster/utils/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/data/mime_types.json
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.439/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/fork.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/lat_long_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.439/blaster/utils/phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/websocket/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_app.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_core.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_exceptions.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_handshake.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_http.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_logging.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_socket.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_ssl_compat.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_url.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/_utils.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster/websocket/tests/
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/tests/__init__.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.439/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/blaster_server.egg-info/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/PKG-INFO
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/SOURCES.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/dependency_links.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/requires.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-07-28 21:35:50.000000 blaster-server-0.0.439/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/examples/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/fast_api_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/gevent_wsgi_test.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/meinheld_flask.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.439/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/simple_examples.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/test_chat_room.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/tornado_hello_world.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439/examples/wheezy_hello.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-07-28 21:35:50.748765 blaster-server-0.0.439/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-07-28 20:32:45.000000 blaster-server-0.0.439/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-07-28 21:35:50.748765 blaster-server-0.0.439/test/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.439/test/test_command_line_parser.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.439/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.439/test/test_schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.439/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/test_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.439/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      823 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.811320 blaster-server-0.0.439b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1150 2023-08-08 11:29:22.000000 blaster-server-0.0.439b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.811320 blaster-server-0.0.439b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.811320 blaster-server-0.0.439b0/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3508 2023-06-05 09:35:21.000000 blaster-server-0.0.439b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-05 09:30:19.000000 blaster-server-0.0.439b0/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.439b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    61703 2023-07-19 07:59:01.000000 blaster-server-0.0.439b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15799 2023-07-27 00:06:27.000000 blaster-server-0.0.439b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38865 2023-08-08 11:40:58.000000 blaster-server-0.0.439b0/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.811320 blaster-server-0.0.439b0/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    44805 2023-07-28 20:32:15.000000 blaster-server-0.0.439b0/blaster/tools/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2884 2023-06-13 08:41:55.000000 blaster-server-0.0.439b0/blaster/tools/sanitize_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-08-08 11:25:12.000000 blaster-server-0.0.439b0/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3950 2023-06-13 13:22:35.000000 blaster-server-0.0.439b0/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      823 2023-08-08 12:04:26.000000 blaster-server-0.0.439b0/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1790 2023-08-08 12:04:26.000000 blaster-server-0.0.439b0/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-08-08 12:04:26.000000 blaster-server-0.0.439b0/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-08-08 12:04:26.000000 blaster-server-0.0.439b0/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-08-08 12:04:26.000000 blaster-server-0.0.439b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1741 2023-06-23 10:38:41.000000 blaster-server-0.0.439b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1564 2023-08-08 11:29:43.000000 blaster-server-0.0.439b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-08-08 12:04:26.815320 blaster-server-0.0.439b0/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      109 2023-06-13 08:39:00.000000 blaster-server-0.0.439b0/test/test_command_line_parser.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.439b0/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5991 2023-06-09 14:06:20.000000 blaster-server-0.0.439b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.439b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.439/LICENSE.txt` & `blaster-server-0.0.439b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/PKG-INFO` & `blaster-server-0.0.439b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.439
+Version: 0.0.439b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
+Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
-Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `blaster-server-0.0.439/README.md` & `blaster-server-0.0.439b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/__init__.py` & `blaster-server-0.0.439b0/blaster/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,7 +42,9 @@
 # load default config, scan the stack and load
 stack = inspect.stack()
 for i in range(1, len(stack)):
 	if(file := inspect.getfile(stack[i].frame)):
 		if(file.startswith("/")):
 			config.load(os.path.dirname(file))
 			break
+
+__version__ = "0.0.439b"
```

### Comparing `blaster-server-0.0.439/blaster/cloud/analytics.py` & `blaster-server-0.0.439b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.439b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/cloud/push_tasks.py` & `blaster-server-0.0.439b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/cloud/storage.py` & `blaster-server-0.0.439b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/config.py` & `blaster-server-0.0.439b0/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/connection_pool.py` & `blaster-server-0.0.439b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/env.py` & `blaster-server-0.0.439b0/blaster/env.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/logging.py` & `blaster-server-0.0.439b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/mongo_orm.py` & `blaster-server-0.0.439b0/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/schema.py` & `blaster-server-0.0.439b0/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/server.py` & `blaster-server-0.0.439b0/blaster/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import traceback
 import inspect
 import socket
 from gevent.socket import socket as GeventSocket
 from gevent.server import StreamServer
 from requests_toolbelt.multipart import decoder
 
-from . import req_ctx
+from . import req_ctx, __version__
 from .tools import set_socket_fast_close_options,\
 	BufferedSocket, ltrim, _OBJ_END_
 from .tools.sanitize_html import SanitizedDict
 from .utils import events
 from .utils.data_utils import FILE_EXTENSION_TO_MIME_TYPE
 from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN, LOG_DEBUG
 from .schema import Object, Required, schema as schema_func
@@ -139,15 +139,15 @@
 class MissingBlasterArgumentException(Exception):
 	def __init__(self, arg_name, arg_type, *args: object) -> None:
 		self.arg_name = arg_name
 		self.arg_type = arg_type
 		super().__init__(*args)
 
 	def __str__(self) -> str:
-		return super().__str__() + f" {self.arg_name}: {self.arg_type}"
+		return super().__str__() + f"missing argument: {self.arg_name}"
 
 
 def raise_ex(ex):
 	raise ex
 
 
 class Request:
@@ -413,15 +413,15 @@
 	def __init__(self, server_exception_handlers=None, **kwargs):
 		self.info = {
 			k: kwargs.get(k, "-") for k in {"title", "description", "version"}
 		}
 		self.route_handlers = []
 		self.request_handlers = []
 		# error
-		self.server_exception_handlers = server_exception_handlers or []
+		self.server_exception_handlers = server_exception_handlers or [App.default_server_exception_handler]
 
 	def route(
 		self,
 		regex,
 		methods=None,
 		title='',
 		description='',
@@ -450,14 +450,19 @@
 				"before": [before] if callable(before) else list(before or [])
 			})
 			# return func as if nothing's decorated! (so you can call function as is)
 			return func
 
 		return wrapper
 
+	@staticmethod
+	def default_server_exception_handler(req: Request, ex: Exception):
+		if(isinstance(ex, MissingBlasterArgumentException)):
+			return 502, [], str(ex)
+
 	def start(self, port=80, handlers=[], **ssl_args):
 		# sort descending order of the path lengths
 		self.route_handlers.sort(
 			key=functools.cmp_to_key(lambda x, y: len(y["regex"]) - len(x["regex"]))
 		)  # reverse sort by length
 
 		# all additional handlers go the bottom of the current list
@@ -621,15 +626,15 @@
 		_all_apps.add(self)
 
 	def generate_openapi_doc(self, handler):
 		regex_path = handler["regex"]
 		regex_path = regex_path\
 			.replace("\\.", ".")\
 			.replace("{+", "{")\
-			.replace("{*", "{")  # openapi doesn't support yet
+			.replace("{*", "{")  # openapi doesn't support regex yet
 
 		self.openapi["paths"][regex_path] = _api = {}
 		func = handler["func"]
 		args = handler["args"]
 		kwargs = handler["kwargs"]
 		return_type = handler.get("return", None)
 
@@ -1119,15 +1124,18 @@
 	_is_server_running = False
 
 	for app in list(_all_apps):
 		app.stop()  # should handle all connections gracefully
 
 
 # create a global app for generic single server use
-DefaultApp = App(title="Blaster", description="Built for speed and rapid prototyping..", version="0.0.368")
+DefaultApp = App(
+	title="Blaster", description="Built for speed and rapid prototyping..",
+	version=__version__
+)
 
 # generic global route handler
 route = DefaultApp.route
 
 
 # generic glonal route handler
 def start_server(*args, **kwargs):
```

### Comparing `blaster-server-0.0.439/blaster/tools/__init__.py` & `blaster-server-0.0.439b0/blaster/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/tools/sanitize_html.py` & `blaster-server-0.0.439b0/blaster/tools/sanitize_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/data/countries.json` & `blaster-server-0.0.439b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/data/mime_types.json` & `blaster-server-0.0.439b0/blaster/utils/data/mime_types.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -43,19 +43,19 @@
         "mime_type": "application/epub+zip",
         "description": ""
     },
     ".pfr": {
         "mime_type": "application/font-tdpfr",
         "description": ""
     },
-    ".gz": {
+    ".tgz": {
         "mime_type": "application/x-gzip",
         "description": ""
     },
-    ".tgz": {
+    ".gz": {
         "mime_type": "application/x-gzip",
         "description": ""
     },
     ".stk": {
         "mime_type": "application/hyperstudio",
         "description": ""
     },
@@ -87,23 +87,23 @@
         "mime_type": "application/mac-compactpro",
         "description": ""
     },
     ".mrc": {
         "mime_type": "application/marc",
         "description": ""
     },
-    ".ma": {
+    ".mb": {
         "mime_type": "application/mathematica",
         "description": ""
     },
-    ".mb": {
+    ".nb": {
         "mime_type": "application/mathematica",
         "description": ""
     },
-    ".nb": {
+    ".ma": {
         "mime_type": "application/mathematica",
         "description": ""
     },
     ".mathml": {
         "mime_type": "text/mathml",
         "description": ""
     },
@@ -119,38 +119,34 @@
         "mime_type": "application/mediaservercontrol+xml",
         "description": ""
     },
     ".mp4s": {
         "mime_type": "application/mp4",
         "description": ""
     },
-    ".doc": {
+    ".dot": {
         "mime_type": "application/msword",
         "description": "Microsoft Word is a popular word processor program which has existed in a number of versions for DOS, Windows, and the Macintosh. It is often distributed as part of the Microsoft Office suite. Various native file formats have been used, and some other non-Word-specific formats can also be opened and saved.Please note the more modern .docx file extension does not use this mime type."
     },
-    ".dot": {
+    ".wiz": {
         "mime_type": "application/msword",
         "description": "Microsoft Word is a popular word processor program which has existed in a number of versions for DOS, Windows, and the Macintosh. It is often distributed as part of the Microsoft Office suite. Various native file formats have been used, and some other non-Word-specific formats can also be opened and saved.Please note the more modern .docx file extension does not use this mime type."
     },
-    ".wiz": {
+    ".doc": {
         "mime_type": "application/msword",
         "description": "Microsoft Word is a popular word processor program which has existed in a number of versions for DOS, Windows, and the Macintosh. It is often distributed as part of the Microsoft Office suite. Various native file formats have been used, and some other non-Word-specific formats can also be opened and saved.Please note the more modern .docx file extension does not use this mime type."
     },
     ".mxf": {
         "mime_type": "application/mxf",
         "description": ""
     },
     ".a": {
         "mime_type": "application/octet-stream",
         "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
     },
-    ".bin": {
-        "mime_type": "application/octet-stream",
-        "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
-    },
     ".bpk": {
         "mime_type": "application/octet-stream",
         "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
     },
     ".deploy": {
         "mime_type": "application/octet-stream",
         "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
@@ -207,14 +203,18 @@
         "mime_type": "application/octet-stream",
         "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
     },
     ".so": {
         "mime_type": "application/octet-stream",
         "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
     },
+    ".bin": {
+        "mime_type": "application/octet-stream",
+        "description": "This MIME type is used for binary files, it's usuall a fallback for unknown/generic MIMEs with no specific designation."
+    },
     ".oda": {
         "mime_type": "application/oda",
         "description": ""
     },
     ".opf": {
         "mime_type": "application/oebps-package+xml",
         "description": ""
@@ -615,19 +615,19 @@
         "mime_type": "application/vnd.curl.pcurl",
         "description": ""
     },
     ".rdz": {
         "mime_type": "application/vnd.data-vision.rdz",
         "description": ""
     },
-    ".deb": {
+    ".udeb": {
         "mime_type": "application/x-debian-package",
         "description": ""
     },
-    ".udeb": {
+    ".deb": {
         "mime_type": "application/x-debian-package",
         "description": ""
     },
     ".fe_launch": {
         "mime_type": "application/vnd.denovo.fcselayout-link",
         "description": ""
     },
@@ -1199,23 +1199,23 @@
         "mime_type": "application/vnd.ms-excel",
         "description": ""
     },
     ".xlm": {
         "mime_type": "application/vnd.ms-excel",
         "description": ""
     },
-    ".xls": {
+    ".xlt": {
         "mime_type": "application/vnd.ms-excel",
         "description": ""
     },
-    ".xlt": {
+    ".xlw": {
         "mime_type": "application/vnd.ms-excel",
         "description": ""
     },
-    ".xlw": {
+    ".xls": {
         "mime_type": "application/vnd.ms-excel",
         "description": ""
     },
     ".xlam": {
         "mime_type": "application/vnd.ms-excel.addin.macroenabled.12",
         "description": ""
     },
@@ -1263,19 +1263,19 @@
         "mime_type": "application/vnd.ms-powerpoint",
         "description": ""
     },
     ".pps": {
         "mime_type": "application/vnd.ms-powerpoint",
         "description": ""
     },
-    ".ppt": {
+    ".pwz": {
         "mime_type": "application/vnd.ms-powerpoint",
         "description": ""
     },
-    ".pwz": {
+    ".ppt": {
         "mime_type": "application/vnd.ms-powerpoint",
         "description": ""
     },
     ".ppam": {
         "mime_type": "application/vnd.ms-powerpoint.addin.macroenabled.12",
         "description": ""
     },
@@ -1291,19 +1291,19 @@
         "mime_type": "application/vnd.ms-powerpoint.slideshow.macroenabled.12",
         "description": ""
     },
     ".potm": {
         "mime_type": "application/vnd.ms-powerpoint.template.macroenabled.12",
         "description": ""
     },
-    ".mpp": {
+    ".mpt": {
         "mime_type": "application/vnd.ms-project",
         "description": ""
     },
-    ".mpt": {
+    ".mpp": {
         "mime_type": "application/vnd.ms-project",
         "description": ""
     },
     ".docm": {
         "mime_type": "application/vnd.ms-word.document.macroenabled.12",
         "description": ""
     },
@@ -1663,18 +1663,14 @@
         "mime_type": "application/vnd.spotfire.sfs",
         "description": ""
     },
     ".db": {
         "mime_type": "application/vnd.sqlite3",
         "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
     },
-    ".sqlite": {
-        "mime_type": "application/vnd.sqlite3",
-        "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
-    },
     ".sqlite3": {
         "mime_type": "application/vnd.sqlite3",
         "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
     },
     ".db-wal": {
         "mime_type": "application/vnd.sqlite3",
         "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
@@ -1687,14 +1683,18 @@
         "mime_type": "application/vnd.sqlite3",
         "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
     },
     ".sqlite-shm": {
         "mime_type": "application/vnd.sqlite3",
         "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
     },
+    ".sqlite": {
+        "mime_type": "application/vnd.sqlite3",
+        "description": "SQLite is a self-contained, serverless, zero-configuration, transactional SQL database engine. The code for SQLite is in the public domain and is thus free for use for any purpose, commercial or private."
+    },
     ".sdc": {
         "mime_type": "application/vnd.stardivision.calc",
         "description": ""
     },
     ".sda": {
         "mime_type": "application/vnd.stardivision.draw",
         "description": ""
@@ -2307,19 +2307,19 @@
         "mime_type": "application/x-pkcs7-certificates",
         "description": ""
     },
     ".spc": {
         "mime_type": "application/x-pkcs7-certificates",
         "description": ""
     },
-    ".pyc": {
+    ".pyo": {
         "mime_type": "application/x-python-code",
         "description": ""
     },
-    ".pyo": {
+    ".pyc": {
         "mime_type": "application/x-python-code",
         "description": ""
     },
     ".rpa": {
         "mime_type": "application/x-redhat-package-manager",
         "description": ""
     },
@@ -2415,23 +2415,23 @@
         "mime_type": "application/xhtml+xml",
         "description": ""
     },
     ".xhtml": {
         "mime_type": "application/xhtml+xml",
         "description": ""
     },
-    ".xml": {
+    ".xpdl": {
         "mime_type": "application/xml",
         "description": ""
     },
-    ".xpdl": {
+    ".xsl": {
         "mime_type": "application/xml",
         "description": ""
     },
-    ".xsl": {
+    ".xml": {
         "mime_type": "application/xml",
         "description": ""
     },
     ".dtd": {
         "mime_type": "application/xml-dtd",
         "description": ""
     },
@@ -2535,31 +2535,31 @@
         "mime_type": "audio/mpeg",
         "description": "MP3 is the name commonly given to the audio formats specified by MPEG-1 Layer III and MPEG-2 Layer III, standardized as ISO/IEC 11172-3:1993, with some additions in ISO/IEC 13818-3:1995. It uses lossy compressed data.MP3 is based in part on work by the Fraunhofer Institute, which held patents in the format. Other companies may also have held patents encumbering its implementation. One of the relevant patents was U.S. Patent 5,812,672, which expired in September 2015; many other related patents in various countries expired earlier. The final expiration of all relevant patents took until 2017, however, due to some \"submarine patents\" which were kept in the application process for years, extending their expiration dates. A modified version of DCT compression (Discrete cosine transform) is used, a lossy compression method also used in JPEG images.ID3 tags are often used to provide metadata in MP3 files, though they aren't part of the MP3 specification."
     },
     ".mp2a": {
         "mime_type": "audio/mpeg",
         "description": "MP3 is the name commonly given to the audio formats specified by MPEG-1 Layer III and MPEG-2 Layer III, standardized as ISO/IEC 11172-3:1993, with some additions in ISO/IEC 13818-3:1995. It uses lossy compressed data.MP3 is based in part on work by the Fraunhofer Institute, which held patents in the format. Other companies may also have held patents encumbering its implementation. One of the relevant patents was U.S. Patent 5,812,672, which expired in September 2015; many other related patents in various countries expired earlier. The final expiration of all relevant patents took until 2017, however, due to some \"submarine patents\" which were kept in the application process for years, extending their expiration dates. A modified version of DCT compression (Discrete cosine transform) is used, a lossy compression method also used in JPEG images.ID3 tags are often used to provide metadata in MP3 files, though they aren't part of the MP3 specification."
     },
-    ".mp3": {
+    ".mpga": {
         "mime_type": "audio/mpeg",
         "description": "MP3 is the name commonly given to the audio formats specified by MPEG-1 Layer III and MPEG-2 Layer III, standardized as ISO/IEC 11172-3:1993, with some additions in ISO/IEC 13818-3:1995. It uses lossy compressed data.MP3 is based in part on work by the Fraunhofer Institute, which held patents in the format. Other companies may also have held patents encumbering its implementation. One of the relevant patents was U.S. Patent 5,812,672, which expired in September 2015; many other related patents in various countries expired earlier. The final expiration of all relevant patents took until 2017, however, due to some \"submarine patents\" which were kept in the application process for years, extending their expiration dates. A modified version of DCT compression (Discrete cosine transform) is used, a lossy compression method also used in JPEG images.ID3 tags are often used to provide metadata in MP3 files, though they aren't part of the MP3 specification."
     },
-    ".mpga": {
+    ".mp3": {
         "mime_type": "audio/mpeg",
         "description": "MP3 is the name commonly given to the audio formats specified by MPEG-1 Layer III and MPEG-2 Layer III, standardized as ISO/IEC 11172-3:1993, with some additions in ISO/IEC 13818-3:1995. It uses lossy compressed data.MP3 is based in part on work by the Fraunhofer Institute, which held patents in the format. Other companies may also have held patents encumbering its implementation. One of the relevant patents was U.S. Patent 5,812,672, which expired in September 2015; many other related patents in various countries expired earlier. The final expiration of all relevant patents took until 2017, however, due to some \"submarine patents\" which were kept in the application process for years, extending their expiration dates. A modified version of DCT compression (Discrete cosine transform) is used, a lossy compression method also used in JPEG images.ID3 tags are often used to provide metadata in MP3 files, though they aren't part of the MP3 specification."
     },
     ".oga": {
         "mime_type": "audio/ogg",
         "description": ""
     },
-    ".ogg": {
+    ".spx": {
         "mime_type": "audio/ogg",
         "description": ""
     },
-    ".spx": {
+    ".ogg": {
         "mime_type": "audio/ogg",
         "description": ""
     },
     ".opus": {
         "mime_type": "audio/opus",
         "description": "Opus audio"
     },
@@ -2671,19 +2671,19 @@
         "mime_type": "font/woff2",
         "description": "Web Open Font Format (WOFF)"
     },
     ".gcode": {
         "mime_type": "gcode",
         "description": "GCODE files are created by slicing programs, such as Simplify3D and Slic3r, that translate CAD drawings into G-Code, which a 3D printer can read.There's no official mimetype assigned as far as the author is aware, however these are the ones commonly reported."
     },
-    ".avif": {
+    ".avifs": {
         "mime_type": "image/avif",
         "description": "AVIF (AV1 Image File Format) is an image and animation file format, an extension of HEIF allowing images encoded with AV1. Most files will only have AV1-encoded images, but a mixture of different encodings is allowed. Early draft versions were named AV1 Still Image File Format."
     },
-    ".avifs": {
+    ".avif": {
         "mime_type": "image/avif",
         "description": "AVIF (AV1 Image File Format) is an image and animation file format, an extension of HEIF allowing images encoded with AV1. Most files will only have AV1-encoded images, but a mixture of different encodings is allowed. Early draft versions were named AV1 Still Image File Format."
     },
     ".bmp": {
         "mime_type": "image/bmp",
         "description": ""
     },
@@ -2747,19 +2747,19 @@
         "mime_type": "image/png",
         "description": "Portable Network Graphics (PNG) was devised starting in a discussion on newsgroup comp.graphics in 1995, with the first version of its specification released in 1996. The motivation for its creation was to create a free and unencumbered image format in the wake of the patent issue with GIF."
     },
     ".btif": {
         "mime_type": "image/prs.btif",
         "description": ""
     },
-    ".svg": {
+    ".svgz": {
         "mime_type": "image/svg+xml",
         "description": ""
     },
-    ".svgz": {
+    ".svg": {
         "mime_type": "image/svg+xml",
         "description": ""
     },
     ".tif": {
         "mime_type": "image/tiff",
         "description": "TIFF, formerly known as Tag(ged) Image File Format, is an image format capable of storing multiple high quality images in a single file. A TIFF image may be uncompressed or use a compression scheme internally. Two of the most widely used compression schemes in TIFF files are lossless, including LZW and, for bitonal images CCITT Group 4, as used for facsimile transmission [fax]. JPEG baseline DCT-based lossy compression is also used."
     },
@@ -3043,19 +3043,19 @@
         "mime_type": "model/vrml",
         "description": ""
     },
     ".wrl": {
         "mime_type": "model/vrml",
         "description": ""
     },
-    ".ics": {
+    ".ifb": {
         "mime_type": "text/calendar",
         "description": ""
     },
-    ".ifb": {
+    ".ics": {
         "mime_type": "text/calendar",
         "description": ""
     },
     ".css": {
         "mime_type": "text/css",
         "description": ""
     },
@@ -3071,30 +3071,30 @@
         "mime_type": "text/html",
         "description": ""
     },
     ".js": {
         "mime_type": "text/javascript",
         "description": "JavaScript (sometimes abbreviated JS) is a scripting language commonly implemented as part of a web browser in order to create enhanced user interfaces and dynamic websites, but also used in other contexts (such as server-side JavaScript).This is not the same as Java. People constantly get confused about that.JavaScript was originally developed at Netscape by Brendan Eich (who later became Mozilla CEO... very briefly), where it was originally called LiveScript while under development, but became JavaScript (with the name licensed from Sun) in order to capitalize on the popularity of Java, though the languages aren't really related (although there are some similarities in syntax). Later, a Microsoft implementation designed to be (more or less) compatible was called JScript, and an attempt at a formally standardized version of the language was published by ECMA as ECMAScript.The node.js runtime environment is (mostly) implemented in JavaScript, as are applications running within it.Due to its status as the only scripting language for browsers, JavaScript skyrocketed in popularity in the 2000's and 2010's and as of 2017 serves as a lingua franca of Web development. Arguably, it is currently the world's most popular programming language (it tops GitHub and StackOverflow currently)."
     },
-    ".md": {
-        "mime_type": "text/markdown",
-        "description": "Markdown is a lightweight and human readable markup format for text formatting created by John Gruber and Aaron Swartz. It is similar to various forms of wiki markup. There is no formal specification for the original Markdown, and it has ambiguities that are handled inconsistently by different implementations.An attempt to improve on this situation was done (released 2014-09) by a group unrelated to the originators of Markdown, and was originally dubbed Standard Markdown until John Gruber objected to this name, and it was first renamed \"Common Markdown\" and later CommonMark. Markdeep is an extended Markdown implemented in JavaScript for web use."
-    },
     ".markdown": {
         "mime_type": "text/markdown",
         "description": "Markdown is a lightweight and human readable markup format for text formatting created by John Gruber and Aaron Swartz. It is similar to various forms of wiki markup. There is no formal specification for the original Markdown, and it has ambiguities that are handled inconsistently by different implementations.An attempt to improve on this situation was done (released 2014-09) by a group unrelated to the originators of Markdown, and was originally dubbed Standard Markdown until John Gruber objected to this name, and it was first renamed \"Common Markdown\" and later CommonMark. Markdeep is an extended Markdown implemented in JavaScript for web use."
     },
     ".mdown": {
         "mime_type": "text/markdown",
         "description": "Markdown is a lightweight and human readable markup format for text formatting created by John Gruber and Aaron Swartz. It is similar to various forms of wiki markup. There is no formal specification for the original Markdown, and it has ambiguities that are handled inconsistently by different implementations.An attempt to improve on this situation was done (released 2014-09) by a group unrelated to the originators of Markdown, and was originally dubbed Standard Markdown until John Gruber objected to this name, and it was first renamed \"Common Markdown\" and later CommonMark. Markdeep is an extended Markdown implemented in JavaScript for web use."
     },
     ".markdn": {
         "mime_type": "text/markdown",
         "description": "Markdown is a lightweight and human readable markup format for text formatting created by John Gruber and Aaron Swartz. It is similar to various forms of wiki markup. There is no formal specification for the original Markdown, and it has ambiguities that are handled inconsistently by different implementations.An attempt to improve on this situation was done (released 2014-09) by a group unrelated to the originators of Markdown, and was originally dubbed Standard Markdown until John Gruber objected to this name, and it was first renamed \"Common Markdown\" and later CommonMark. Markdeep is an extended Markdown implemented in JavaScript for web use."
     },
+    ".md": {
+        "mime_type": "text/markdown",
+        "description": "Markdown is a lightweight and human readable markup format for text formatting created by John Gruber and Aaron Swartz. It is similar to various forms of wiki markup. There is no formal specification for the original Markdown, and it has ambiguities that are handled inconsistently by different implementations.An attempt to improve on this situation was done (released 2014-09) by a group unrelated to the originators of Markdown, and was originally dubbed Standard Markdown until John Gruber objected to this name, and it was first renamed \"Common Markdown\" and later CommonMark. Markdeep is an extended Markdown implemented in JavaScript for web use."
+    },
     ".conf": {
         "mime_type": "text/plain",
         "description": ""
     },
     ".def": {
         "mime_type": "text/plain",
         "description": ""
@@ -3243,18 +3243,14 @@
         "mime_type": "text/x-asm",
         "description": ""
     },
     ".s": {
         "mime_type": "text/x-asm",
         "description": ""
     },
-    ".c": {
-        "mime_type": "text/x-c",
-        "description": ""
-    },
     ".cc": {
         "mime_type": "text/x-c",
         "description": ""
     },
     ".cpp": {
         "mime_type": "text/x-c",
         "description": ""
@@ -3271,30 +3267,34 @@
         "mime_type": "text/x-c",
         "description": ""
     },
     ".hh": {
         "mime_type": "text/x-c",
         "description": ""
     },
-    ".f": {
-        "mime_type": "text/x-fortran",
+    ".c": {
+        "mime_type": "text/x-c",
         "description": ""
     },
     ".f77": {
         "mime_type": "text/x-fortran",
         "description": ""
     },
     ".f90": {
         "mime_type": "text/x-fortran",
         "description": ""
     },
     ".for": {
         "mime_type": "text/x-fortran",
         "description": ""
     },
+    ".f": {
+        "mime_type": "text/x-fortran",
+        "description": ""
+    },
     ".java": {
         "mime_type": "text/x-java-source",
         "description": ""
     },
     ".p": {
         "mime_type": "text/x-pascal",
         "description": "Pascal is an influential imperative and procedural programming language, designed in 1968\u20131969 and published in 1970. Borland's Turbo Pascal, and the later Borland Pascal, were popular in the 1980s and early 1990s on the PC/MS-DOS platform (CP/M versions were also released)."
@@ -3359,23 +3359,23 @@
         "mime_type": "video/mj2",
         "description": ""
     },
     ".mjp2": {
         "mime_type": "video/mj2",
         "description": ""
     },
-    ".mp4": {
+    ".mp4v": {
         "mime_type": "video/mp4",
         "description": "MP4 usually refers to the multimedia file format defined in Part 14 (and to a lesser extent Part 1) of the MPEG-4 standard. \"MP4\" could also mean the entire MPEG-4 standard, or some other subset of MPEG-4. MPEG-4 Part 14 is an application of Part 12. The recommended extension for it is \".mp4\", though \".m4a\" is often used for audio-only files. It is standardized by ISO/IEC 14496-14."
     },
-    ".mp4v": {
+    ".mpg4": {
         "mime_type": "video/mp4",
         "description": "MP4 usually refers to the multimedia file format defined in Part 14 (and to a lesser extent Part 1) of the MPEG-4 standard. \"MP4\" could also mean the entire MPEG-4 standard, or some other subset of MPEG-4. MPEG-4 Part 14 is an application of Part 12. The recommended extension for it is \".mp4\", though \".m4a\" is often used for audio-only files. It is standardized by ISO/IEC 14496-14."
     },
-    ".mpg4": {
+    ".mp4": {
         "mime_type": "video/mp4",
         "description": "MP4 usually refers to the multimedia file format defined in Part 14 (and to a lesser extent Part 1) of the MPEG-4 standard. \"MP4\" could also mean the entire MPEG-4 standard, or some other subset of MPEG-4. MPEG-4 Part 14 is an application of Part 12. The recommended extension for it is \".mp4\", though \".m4a\" is often used for audio-only files. It is standardized by ISO/IEC 14496-14."
     },
     ".m1v": {
         "mime_type": "video/mpeg",
         "description": ""
     },
@@ -3387,43 +3387,43 @@
         "mime_type": "video/mpeg",
         "description": ""
     },
     ".mpe": {
         "mime_type": "video/mpeg",
         "description": ""
     },
-    ".mpeg": {
+    ".mpg": {
         "mime_type": "video/mpeg",
         "description": ""
     },
-    ".mpg": {
+    ".mpeg": {
         "mime_type": "video/mpeg",
         "description": ""
     },
     ".ogv": {
         "mime_type": "video/ogg",
         "description": ""
     },
-    ".mov": {
+    ".qt": {
         "mime_type": "video/quicktime",
         "description": ""
     },
-    ".qt": {
+    ".mov": {
         "mime_type": "video/quicktime",
         "description": ""
     },
     ".fvt": {
         "mime_type": "video/vnd.fvt",
         "description": ""
     },
-    ".m4u": {
+    ".mxu": {
         "mime_type": "video/vnd.mpegurl",
         "description": ""
     },
-    ".mxu": {
+    ".m4u": {
         "mime_type": "video/vnd.mpegurl",
         "description": ""
     },
     ".pyv": {
         "mime_type": "video/vnd.ms-playready.media.pyv",
         "description": ""
     },
```

### Comparing `blaster-server-0.0.439/blaster/utils/data_utils.py` & `blaster-server-0.0.439b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/events.py` & `blaster-server-0.0.439b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/fork.py` & `blaster-server-0.0.439b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.439b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.439b0/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/utils/xss_html.py` & `blaster-server-0.0.439b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/__init__.py` & `blaster-server-0.0.439b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_abnf.py` & `blaster-server-0.0.439b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_app.py` & `blaster-server-0.0.439b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_core.py` & `blaster-server-0.0.439b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_exceptions.py` & `blaster-server-0.0.439b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_handshake.py` & `blaster-server-0.0.439b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_http.py` & `blaster-server-0.0.439b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_logging.py` & `blaster-server-0.0.439b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_socket.py` & `blaster-server-0.0.439b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.439b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_url.py` & `blaster-server-0.0.439b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/_utils.py` & `blaster-server-0.0.439b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/server.py` & `blaster-server-0.0.439b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.439b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.439b0/blaster_server.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.439
+Version: 0.0.439b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
+Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
-Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE.txt
-
-UNKNOWN
-
```

### Comparing `blaster-server-0.0.439/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.439b0/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/gevent_wsgi_test.py` & `blaster-server-0.0.439b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/mongo_ormexample.py` & `blaster-server-0.0.439b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/simple_examples.py` & `blaster-server-0.0.439b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/test_chat_room.py` & `blaster-server-0.0.439b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/tornado_hello_world.py` & `blaster-server-0.0.439b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/examples/wheezy_hello.py` & `blaster-server-0.0.439b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/setup.py` & `blaster-server-0.0.439b0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
+from blaster import __version__
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.439',
+	version=__version__,
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.439/test/test_mongo_orm.py` & `blaster-server-0.0.439b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/test/test_phone_number_utils.py` & `blaster-server-0.0.439b0/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/test/test_schema.py` & `blaster-server-0.0.439b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/test/test_tools.py` & `blaster-server-0.0.439b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/test/test_utils.py` & `blaster-server-0.0.439b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.439/test/timeit_snippets.py` & `blaster-server-0.0.439b0/test/timeit_snippets.py`

 * *Files identical despite different names*

