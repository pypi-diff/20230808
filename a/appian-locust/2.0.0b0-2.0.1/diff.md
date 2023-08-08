# Comparing `tmp/appian-locust-2.0.0b0.tar.gz` & `tmp/appian-locust-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appian-locust-2.0.0b0.tar", last modified: Mon Jun 26 16:49:14 2023, max compression
+gzip compressed data, was "appian-locust-2.0.1.tar", last modified: Thu Jul 27 19:20:47 2023, max compression
```

## Comparing `appian-locust-2.0.0b0.tar` & `appian-locust-2.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4875 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.505967 appian-locust-2.0.0b0/appian_locust/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9592 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_design.py
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_feature_toggle_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7849 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_grid_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)    52958 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_interactor.py
--rw-rw-rw-   0 root         (0) root         (0)     5177 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_locust_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7747 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_news.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_portals.py
--rw-rw-rw-   0 root         (0) root         (0)    15240 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_records.py
--rw-rw-rw-   0 root         (0) root         (0)     7390 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_records_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7474 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3016 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_save_request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     9939 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_sites.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_task_opener.py
--rw-rw-rw-   0 root         (0) root         (0)     7653 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/_ui_reconciler.py
--rw-rw-rw-   0 root         (0) root         (0)     7334 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/appian_client.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/appian_task_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.506967 appian-locust-2.0.0b0/appian_locust/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/exceptions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/exceptions/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1792 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/feature_flag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.507967 appian-locust-2.0.0b0/appian_locust/info/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/actions_info.py
--rw-rw-rw-   0 root         (0) root         (0)     3172 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/news_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/records_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/reports_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1258 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/sites_info.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/info/tasks_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.508967 appian-locust-2.0.0b0/appian_locust/objects/
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/application.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/design_object.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/page.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/objects/site.py
--rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/system_operator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.509967 appian-locust-2.0.0b0/appian_locust/uiform/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3896 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/application_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/design_object_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     6234 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/design_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     4395 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/record_list_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/record_uiform.py
--rw-rw-rw-   0 root         (0) root         (0)    73472 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/uiform/uiform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.510967 appian-locust-2.0.0b0/appian_locust/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)    16347 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/helper.py
--rwxrwxrwx   0 root         (0) root         (0)     1393 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/loadDriverUtils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/utilities/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    14525 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/appian_locust/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 16:49:14.506967 appian-locust-2.0.0b0/appian_locust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5449 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-26 16:49:14.000000 appian-locust-2.0.0b0/appian_locust.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-26 16:49:14.511968 appian-locust-2.0.0b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-26 16:49:05.000000 appian-locust-2.0.0b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.296424 appian-locust-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-07-27 19:20:38.000000 appian-locust-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-07-27 19:20:47.296424 appian-locust-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4183 2023-07-27 19:20:38.000000 appian-locust-2.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.290425 appian-locust-2.0.1/appian_locust/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9592 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_design.py
+-rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_feature_toggle_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     8499 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_grid_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)    53083 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_interactor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5177 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_locust_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7747 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_news.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_portals.py
+-rw-rw-rw-   0 root         (0) root         (0)    15240 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_records.py
+-rw-rw-rw-   0 root         (0) root         (0)     7390 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_records_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3016 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_save_request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     9939 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_sites.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_task_opener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7653 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/_ui_reconciler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7334 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/appian_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/appian_task_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.291425 appian-locust-2.0.1/appian_locust/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/exceptions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/exceptions/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1792 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/feature_flag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.293425 appian-locust-2.0.1/appian_locust/info/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/actions_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/news_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/records_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/reports_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1258 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/sites_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/info/tasks_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.293425 appian-locust-2.0.1/appian_locust/objects/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/objects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/objects/application.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/objects/design_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      546 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/objects/page.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/objects/site.py
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/system_operator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.295425 appian-locust-2.0.1/appian_locust/uiform/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/application_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/design_object_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     6234 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/design_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/record_list_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/record_uiform.py
+-rw-rw-rw-   0 root         (0) root         (0)    81884 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/uiform/uiform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.296424 appian-locust-2.0.1/appian_locust/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/utilities/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)    16347 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/utilities/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/utilities/loadDriverUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/utilities/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    14895 2023-07-27 19:20:38.000000 appian-locust-2.0.1/appian_locust/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 19:20:47.291425 appian-locust-2.0.1/appian_locust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4755 2023-07-27 19:20:47.000000 appian-locust-2.0.1/appian_locust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-07-27 19:20:47.000000 appian-locust-2.0.1/appian_locust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 19:20:47.000000 appian-locust-2.0.1/appian_locust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 19:20:47.000000 appian-locust-2.0.1/appian_locust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-27 19:20:47.000000 appian-locust-2.0.1/appian_locust.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-07-27 19:20:47.296424 appian-locust-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-07-27 19:20:38.000000 appian-locust-2.0.1/setup.py
```

### Comparing `appian-locust-2.0.0b0/LICENSE` & `appian-locust-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/PKG-INFO` & `appian-locust-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0b0
+Version: 2.0.1
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,33 +28,33 @@
 - Form interactions (filling/submitting)
 - Finding and interacting with basic components on a SAIL interface
 - Navigating to records/reports/sites
 
 .. what_is_appian_locust-inclusion-end-do-not-remove
 
 
-For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__
+For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__.
 
 .. disclaimer-inclusion-begin-do-not-remove
 
 **Disclaimer:**
 This library is continuously evolving.
 Currently the main focus is supporting essential use-cases.
 We are happy to accept contributions to further extend functionality, address bug fixes and improve usability.
 Please see the `Contributing <contributing.html>`__ section and feel free to reach out.
 
 .. disclaimer-inclusion-end-do-not-remove
 
 .. quick_start-inclusion-begin-do-not-remove
 
-********************
-Quick Start Guide
-********************
+************************
+Quick Installation Guide
+************************
 
-This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.7+ installed on your machine before proceeding.
+This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.10+ installed on your machine before proceeding.
 
 Setup
 ------------
 
 1. Install appian-locust using `pip`, for more comprehensive projects we recommend using `pipenv`.
 
 .. code-block:: bash
@@ -71,40 +71,24 @@
 
     [requires]
     python_version = "3.10"
 
     [pipenv]
     allow_prereleases = true
 
-2. Configure your test to point at the Appian instance you will be using.
-You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
-
-- Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
-
-.. code-block:: json
-
-    {
-        "host_address": "site-name.appiancloud.com",
-        "auth": [
-            "user.name",
-            "password"
-        ]
-    }
-
-3. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_locustfile.py>`_.
+2. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/main/examples/example_locustfile.py>`_.
 
 .. code-block:: bash
 
-    locust -f example_locustfile.py -u 1 -t 60 --headless
+    locust -f example_locustfile.py
 
-If everything is set up correctly, you should start to see output from the load test reporting results. This should run for 60 seconds and end with a summary report of the results.
+If everything is set up correctly, you should see a link to the `Locust web interface <https://docs.locust.io/en/stable/quickstart.html#locust-s-web-interface>`_, which you can use to start test runs and view results.
 
-* For more examples of different site interactions, see the ``example_*.py`` files included in this repository.
-* For more in-depth information about the test library, see the rest of this documentation.
+* For more information about how to build the workflow for your locust test, see the `How to Write a Locust Test <how_to_write_locust_tests.html>`__ section.
+* For more information on running locust tests, see the `How to Run Locust <how_to_run_locust.html>`__ section.
 
 Build from source
 ----------------------
 Clone the repository:
 
 .. code-block:: bash
 
@@ -125,18 +109,18 @@
 If you have issues installing, make sure you have the proper prerequisites installed for Locust and its dependencies.
 If you're having trouble on Windows, check `here <https://github.com/locustio/locust/issues/1208#issuecomment-569693439>`__
 
 Troubleshooting
 ----------------
 * **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
 
-  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that ``host_address`` is specified correctly in your locust test file.
 
 * **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
 
-  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that `auth` specifies a valid username and password combination for the site you're testing on in your locust test file.
 
 * **"General request and response debugging"**
 
-  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
+  * Add ``self.client.record_mode = True`` to your ``HttpUser`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
 .. quick_start-inclusion-end-do-not-remove
```

### Comparing `appian-locust-2.0.0b0/README.rst` & `appian-locust-2.0.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 - Form interactions (filling/submitting)
 - Finding and interacting with basic components on a SAIL interface
 - Navigating to records/reports/sites
 
 .. what_is_appian_locust-inclusion-end-do-not-remove
 
 
-For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__
+For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__.
 
 .. disclaimer-inclusion-begin-do-not-remove
 
 **Disclaimer:**
 This library is continuously evolving.
 Currently the main focus is supporting essential use-cases.
 We are happy to accept contributions to further extend functionality, address bug fixes and improve usability.
 Please see the `Contributing <contributing.html>`__ section and feel free to reach out.
 
 .. disclaimer-inclusion-end-do-not-remove
 
 .. quick_start-inclusion-begin-do-not-remove
 
-********************
-Quick Start Guide
-********************
+************************
+Quick Installation Guide
+************************
 
-This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.7+ installed on your machine before proceeding.
+This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.10+ installed on your machine before proceeding.
 
 Setup
 ------------
 
 1. Install appian-locust using `pip`, for more comprehensive projects we recommend using `pipenv`.
 
 .. code-block:: bash
@@ -56,40 +56,24 @@
 
     [requires]
     python_version = "3.10"
 
     [pipenv]
     allow_prereleases = true
 
-2. Configure your test to point at the Appian instance you will be using.
-You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
-
-- Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
-
-.. code-block:: json
-
-    {
-        "host_address": "site-name.appiancloud.com",
-        "auth": [
-            "user.name",
-            "password"
-        ]
-    }
-
-3. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_locustfile.py>`_.
+2. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/main/examples/example_locustfile.py>`_.
 
 .. code-block:: bash
 
-    locust -f example_locustfile.py -u 1 -t 60 --headless
+    locust -f example_locustfile.py
 
-If everything is set up correctly, you should start to see output from the load test reporting results. This should run for 60 seconds and end with a summary report of the results.
+If everything is set up correctly, you should see a link to the `Locust web interface <https://docs.locust.io/en/stable/quickstart.html#locust-s-web-interface>`_, which you can use to start test runs and view results.
 
-* For more examples of different site interactions, see the ``example_*.py`` files included in this repository.
-* For more in-depth information about the test library, see the rest of this documentation.
+* For more information about how to build the workflow for your locust test, see the `How to Write a Locust Test <how_to_write_locust_tests.html>`__ section.
+* For more information on running locust tests, see the `How to Run Locust <how_to_run_locust.html>`__ section.
 
 Build from source
 ----------------------
 Clone the repository:
 
 .. code-block:: bash
 
@@ -110,18 +94,18 @@
 If you have issues installing, make sure you have the proper prerequisites installed for Locust and its dependencies.
 If you're having trouble on Windows, check `here <https://github.com/locustio/locust/issues/1208#issuecomment-569693439>`__
 
 Troubleshooting
 ----------------
 * **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
 
-  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that ``host_address`` is specified correctly in your locust test file.
 
 * **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
 
-  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that `auth` specifies a valid username and password combination for the site you're testing on in your locust test file.
 
 * **"General request and response debugging"**
 
-  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
+  * Add ``self.client.record_mode = True`` to your ``HttpUser`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
 .. quick_start-inclusion-end-do-not-remove
```

### Comparing `appian-locust-2.0.0b0/appian_locust/_actions.py` & `appian-locust-2.0.1/appian_locust/_actions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_admin.py` & `appian-locust-2.0.1/appian_locust/_admin.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_base.py` & `appian-locust-2.0.1/appian_locust/_base.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_design.py` & `appian-locust-2.0.1/appian_locust/_design.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_feature_toggle_helper.py` & `appian-locust-2.0.1/appian_locust/_feature_toggle_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_grid_interactor.py` & `appian-locust-2.0.1/appian_locust/_grid_interactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,7 +165,20 @@
                 }
             }
             if sort_info:
                 save_data['pagingInfo']['sort'] = sort_info
             if selected:
                 save_data['selected'] = selected
         return save_data
+
+    def find_rich_text_grid_link_component(self, grid: Dict[str, Any], column_name: str, row_index: int) -> Optional[Dict[str, Any]]:
+        for column in grid["columns"]:
+            if column["label"] == column_name:
+                row = column["data"][row_index]
+                return row["value"]["values"][0]["values"][0]["link"]
+        return None
+
+    def find_plaintext_grid_link_component(self, grid: Dict[str, Any], column_name: str, row_index: int) -> Optional[Dict[str, Any]]:
+        for column in grid["columns"]:
+            if column["label"] == column_name:
+                return column["links"][row_index]
+        return None
```

### Comparing `appian-locust-2.0.0b0/appian_locust/_interactor.py` & `appian-locust-2.0.1/appian_locust/_interactor.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 log = logger.getLogger(__name__)
 
 # TODO: Consider breaking this class up into smaller pieces
 
 
 RECORD_PATH = "recorded_responses"
+TEMPO_SITE_STUB = "D6JMim"
 
 
 class _Interactor:
     def __init__(self, session: HttpSession, host: str, portals_mode: bool = False, request_timeout: int = 300) -> None:
         """
         Class that represents interactions with the UI and Appian system
         If you want to record all requests made, you can set the record_mode attribute
@@ -373,16 +374,19 @@
         elif "sites" in get_url and "/pages/" in get_url:
             page_search = search(r'(?<=\/pages\/)([\w-]+)', get_url)
             if page_search:
                 page_name = page_search.group()
             else:
                 e = Exception("Unexpected record link URL - couldn't find page name after /pages/")
                 log_locust_error(e, raise_error=True)
-            page_type = get_url.split('/')[-1]
-            parse_pattern = page_name + "/" + page_type
+
+            parse_pattern = page_name
+            if TEMPO_SITE_STUB not in get_url:
+                page_type = get_url.split('/')[-1]
+                parse_pattern = parse_pattern + "/" + page_type
             url_prefix_index = get_url.index(parse_pattern) + len(page_name)
             # record_link_url = get_url[:get_url.index(parse_pattern) + len(page_name)].replace("/pages/",
             record_link_url = get_url[:url_prefix_index].replace("/pages/",
                                                                  "/page/") + "/record/" + record_link_url_suffix
         # Support record view links from a record within a site
         # Also supports record links on a task form (ex: /suite/rest/a/task/latest/JaUHEhaQ1jI7OMif0L/form)
         # Most urls will get caught here
```

### Comparing `appian-locust-2.0.0b0/appian_locust/_locust_error_handler.py` & `appian-locust-2.0.1/appian_locust/_locust_error_handler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_news.py` & `appian-locust-2.0.1/appian_locust/_news.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_portals.py` & `appian-locust-2.0.1/appian_locust/_portals.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_records.py` & `appian-locust-2.0.1/appian_locust/_records.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_records_helper.py` & `appian-locust-2.0.1/appian_locust/_records_helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_reports.py` & `appian-locust-2.0.1/appian_locust/_reports.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_save_request_builder.py` & `appian-locust-2.0.1/appian_locust/_save_request_builder.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_sites.py` & `appian-locust-2.0.1/appian_locust/_sites.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_task_opener.py` & `appian-locust-2.0.1/appian_locust/_task_opener.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_tasks.py` & `appian-locust-2.0.1/appian_locust/_tasks.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/_ui_reconciler.py` & `appian-locust-2.0.1/appian_locust/_ui_reconciler.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/appian_client.py` & `appian-locust-2.0.1/appian_locust/appian_client.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/appian_task_set.py` & `appian-locust-2.0.1/appian_locust/appian_task_set.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/exceptions/exceptions.py` & `appian-locust-2.0.1/appian_locust/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/feature_flag.py` & `appian-locust-2.0.1/appian_locust/feature_flag.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/actions_info.py` & `appian-locust-2.0.1/appian_locust/info/actions_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/news_info.py` & `appian-locust-2.0.1/appian_locust/info/news_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/records_info.py` & `appian-locust-2.0.1/appian_locust/info/records_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/reports_info.py` & `appian-locust-2.0.1/appian_locust/info/reports_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/sites_info.py` & `appian-locust-2.0.1/appian_locust/info/sites_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/info/tasks_info.py` & `appian-locust-2.0.1/appian_locust/info/tasks_info.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/objects/design_object.py` & `appian-locust-2.0.1/appian_locust/objects/design_object.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/objects/page.py` & `appian-locust-2.0.1/appian_locust/objects/page.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/system_operator.py` & `appian-locust-2.0.1/appian_locust/system_operator.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/application_uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/application_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/design_object_uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/design_object_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/design_uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/design_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/record_list_uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/record_list_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/record_uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/record_uiform.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/uiform/uiform.py` & `appian-locust-2.0.1/appian_locust/uiform/uiform.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import warnings
 from typing import Any, Dict, List, Union, Optional, TYPE_CHECKING
 from urllib.parse import quote, urlparse
 from copy import deepcopy
 
 from ..utilities import logger
 from .._grid_interactor import GridInteractor
-from .._interactor import _Interactor
+from .._interactor import _Interactor, TEMPO_SITE_STUB
 from .._locust_error_handler import raises_locust_error
 from .._task_opener import _TaskOpener
 from .._ui_reconciler import UiReconciler
 from ..exceptions import InvalidComponentException, ChoiceNotFoundException
 from ..utilities.helper import (extract_all_by_label, find_component_by_attribute_and_index_in_dict,
                                 find_component_by_attribute_in_dict, find_component_by_index_in_dict,
                                 find_component_by_label_and_type_dict, find_component_by_type_and_attribute_and_index_in_dict)
@@ -25,15 +25,14 @@
     from ..uiform import RecordInstanceUiForm
 
 KEY_UUID = "uuid"
 KEY_CONTEXT = "context"
 START_PROCESS_LINK_TYPE = 'StartProcessLink'
 PROCESS_TASK_LINK_TYPE = 'ProcessTaskLink'
 COMPONENTS_THAT_CAN_BE_FILLED = ["ParagraphField", "TextField", "SearchBoxWidget"]
-TEMPO_SITE_STUB = "D6JMim"
 
 log = logger.getLogger(__name__)
 
 
 class SailUiForm:
     def __init__(self, interactor: _Interactor, state: Dict[str, Any], breadcrumb: str = "SailUi"):
         """
@@ -429,14 +428,18 @@
     @raises_locust_error
     def click_record_link_by_attribute_and_index(self, attribute: str = "", attribute_value: str = "", index: int = 1, locust_request_label: str = "") -> 'RecordInstanceUiForm':
         """
         Click the index'th record link on the form if there is one present with an attribute matching attribute_value
         If no attribute is provided, the index'th record link is selected from all record links in the form
         Otherwise throws a ComponentNotFoundException
 
+        NOTE: This method returns a NEW RecordInstanceUiForm object, so you must save its return value into a new variable, like so:
+
+            >>> record_uiform = other_uiform.click_record_link_by_attribute_and_index(...)
+
         Keyword Args:
             attribute(str): Attribute to check for 'attribute_value' (default: "")
             attribute_value(str): Attribute value of record link to click (default: "")
             index(int): Index of record link to click (default: 1)
             locust_request_label(str): Label used to identify the request for locust statistics
 
         Returns (SailUiForm): The record form (feed) for the linked record.
@@ -460,14 +463,18 @@
         Args:
             label(str): Label of the record link to click
             is_test_label(bool): If you are clicking a record link via a test label instead of a label, set this boolean to true
 
         Keyword Args:
             locust_request_label(str): Label used to identify the request for locust statistics
 
+        NOTE: This method returns a NEW RecordInstanceUiForm object, so you must save its return value into a new variable, like so:
+
+            >>> record_uiform = other_uiform.click_record_link(...)
+
         Returns (RecordUiForm): The record form (feed) for the linked record.
 
         """
         attribute_to_find = 'testLabel' if is_test_label else 'label'
         return self.click_record_link_by_attribute_and_index(attribute=attribute_to_find, attribute_value=label, locust_request_label=locust_request_label)
 
     @raises_locust_error
@@ -495,14 +502,18 @@
 
         Args:
             label(str): Label of the record link to click
 
         Keyword Args:
             locust_request_label(str): Label used to identify the request for locust statistics
 
+        NOTE: This method returns a NEW RecordInstanceUiForm object, so you must save its return value into a new variable, like so:
+
+            >>> record_uiform = other_uiform.click_record_view_link(...)
+
         Returns (SailUiForm): The record form (feed) for the linked record.
 
         """
         view_tab_label = f"{label}_tab"
         outer_component = find_component_by_attribute_in_dict(attribute="testLabel", value=view_tab_label, component_tree=self._state)
         component = outer_component["link"]
         locust_label = locust_request_label or f"{self.breadcrumb}.ClickRecordLink"
@@ -607,15 +618,15 @@
             page_name = link_component["sitePageUrlStub"]
             new_state = self._click_start_process_link(site_name, page_name, False, link_component, locust_request_label=locust_label)
         elif link_type == PROCESS_TASK_LINK_TYPE:
             task_name = link_component.get('label') or 'Unnammed Task'
             task_id = link_component.get('opaqueTaskId')
             if not task_id:
                 raise Exception(f"No task id found for task with name '{task_name}'")
-            site_name = link_component.get("siteUrlStub") or "D6JMim"
+            site_name = link_component.get("siteUrlStub") or TEMPO_SITE_STUB
             page_name = link_component.get("sitePageUrlStub")
             headers = {
                 'X-Site-UrlStub': site_name,
                 'X-Page-UrlStub': page_name,
                 'X-Client-Mode': 'SITES'
             }
             new_state = self.task_opener.visit_by_task_id(task_name, task_id, extra_headers=headers)
@@ -1286,14 +1297,153 @@
 
         reeval_url = self._get_update_url_for_reeval(self._state)
         new_state = self._interactor.update_grid_from_sail_form(reeval_url, grid, new_grid_save,
                                                                 self.context, self.uuid, context_label=context_label)
         return self._reconcile_state(new_state)
 
     @raises_locust_error
+    def click_grid_rich_text_link(self, column_name: str, row_index: int, grid_label: Optional[str] = None, grid_index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+        """
+        Click on a link in a grid with RichText values
+
+        Either a label or an index is required, indices are useful if there is no title for the grid
+
+        Args:
+            column_name (str): The name of the column the link is in
+            row_index (int): The row in the column to click on, 0 indexed
+            grid_label (str): The label of the grid, if index is not supplied
+            grid_index (str): the index of the grid, if label is not supplied
+            locust_request_label (str, optional): The label locust should associate this request with
+
+        Returns (SailUiForm): The latest state of the UiForm
+
+        """
+        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=grid_label, index=grid_index)
+
+        if not grid_label:
+            grid_label = self.grid_interactor.format_grid_display_label(grid)
+        locust_request_label = locust_request_label or f"{self.breadcrumb}.Grid.Click.{grid_label}.{column_name}.{row_index}"
+
+        link_component = self.grid_interactor.find_rich_text_grid_link_component(grid=grid, column_name=column_name, row_index=row_index)
+        if not link_component:
+            raise Exception(f"Column with name {column_name} not found in grid with identifier {grid_label or grid_index}")
+
+        new_state = self._dispatch_click(component=link_component, locust_label=locust_request_label)
+        return self._reconcile_state(new_state)
+
+    @raises_locust_error
+    def click_grid_rich_text_record_link(self, column_name: str, row_index: int, grid_label: Optional[str] = None,
+                                         grid_index: Optional[int] = None, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+        """
+        Click on a Record link in a grid with RichText values
+
+        Either a label or an index is required, indices are useful if there is no title for the grid
+
+        NOTE: This method returns a NEW RecordInstanceUiForm object, so you must save its return value into a new variable, like so:
+
+            >>> record_uiform = other_uiform.click_grid_rich_text_record_link(...)
+
+        Args:
+            column_name (str): The name of the column the link is in
+            row_index (int): The row in the column to click on, 0 indexed
+            grid_label (str): The label of the grid, if index is not supplied
+            grid_index (str): the index of the grid, if label is not supplied
+            locust_request_label (str, optional): The label locust should associate this request with
+
+        Returns (SailUiForm): The latest state of the UiForm
+
+        """
+        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=grid_label, index=grid_index)
+
+        if not grid_label:
+            grid_label = self.grid_interactor.format_grid_display_label(grid)
+        locust_request_label = locust_request_label or f"{self.breadcrumb}.Grid.Click.{grid_label}.{column_name}.{row_index}"
+
+        link_component = self.grid_interactor.find_rich_text_grid_link_component(grid=grid, column_name=column_name,
+                                                                                 row_index=row_index)
+        if not link_component:
+            raise Exception(f"Column with name {column_name} not found in grid with identifier {grid_label or grid_index}")
+
+        new_state = self._interactor.click_record_link(self.form_url, link_component, self.context, self.uuid,
+                                                       locust_label=locust_request_label)
+
+        from .record_uiform import RecordInstanceUiForm
+        return RecordInstanceUiForm(self._interactor, new_state)
+
+    @raises_locust_error
+    def click_grid_plaintext_link(self, column_name: str, row_index: int, grid_label: Optional[str] = None,
+                                  grid_index: Optional[int] = None, locust_request_label: str = "") -> 'SailUiForm':
+        """
+        Click on a link in a grid with plaintext values
+
+        Either a label or an index is required, indices are useful if there is no title for the grid
+
+        Args:
+            column_name (str): The name of the column the link is in
+            row_index (int): The row in the column to click on, 0 indexed
+            grid_label (str): The label of the grid, if index is not supplied
+            grid_index (str): the index of the grid, if label is not supplied
+            locust_request_label (str, optional): The label locust should associate this request with
+
+        Returns (SailUiForm): The latest state of the UiForm
+
+        """
+        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=grid_label, index=grid_index)
+
+        if not grid_label:
+            grid_label = self.grid_interactor.format_grid_display_label(grid)
+        locust_request_label = locust_request_label or f"{self.breadcrumb}.Grid.Click.{grid_label}.{column_name}.{row_index}"
+
+        link_component = self.grid_interactor.find_plaintext_grid_link_component(grid=grid, column_name=column_name, row_index=row_index)
+        if not link_component:
+            raise Exception(f"Column with name {column_name} not found in grid with identifier {grid_label or grid_index}")
+
+        new_state = self._dispatch_click(component=link_component, locust_label=locust_request_label)
+        return self._reconcile_state(new_state)
+
+    @raises_locust_error
+    def click_grid_plaintext_record_link(self, column_name: str, row_index: int, grid_label: Optional[str] = None,
+                                         grid_index: Optional[int] = None, locust_request_label: str = "") -> 'RecordInstanceUiForm':
+        """
+        Click on a Record link in a grid with plaintext values
+
+        Either a label or an index is required, indices are useful if there is no title for the grid
+
+        NOTE: This method returns a NEW RecordInstanceUiForm object, so you must save its return value into a new variable, like so:
+
+            >>> record_uiform = other_uiform.click_grid_plaintext_record_link(...)
+
+        Args:
+            column_name (str): The name of the column the link is in
+            row_index (int): The row in the column to click on, 0 indexed
+            grid_label (str): The label of the grid, if index is not supplied
+            grid_index (str): the index of the grid, if label is not supplied
+            locust_request_label (str, optional): The label locust should associate this request with
+
+        Returns (SailUiForm): The latest state of the UiForm
+
+        """
+        grid = self.grid_interactor.find_grid_by_label_or_index(self._state, label=grid_label, index=grid_index)
+
+        if not grid_label:
+            grid_label = self.grid_interactor.format_grid_display_label(grid)
+        locust_request_label = locust_request_label or f"{self.breadcrumb}.Grid.Click.{grid_label}.{column_name}.{row_index}"
+
+        link_component = self.grid_interactor.find_plaintext_grid_link_component(grid=grid, column_name=column_name,
+                                                                                 row_index=row_index)
+        if not link_component:
+            raise Exception(f"Column with name {column_name} not found in grid with identifier {grid_label or grid_index}")
+
+        new_state = self._interactor.click_record_link(self.form_url, link_component, self.context, self.uuid,
+                                                       locust_label=locust_request_label)
+
+        from .record_uiform import RecordInstanceUiForm
+        return RecordInstanceUiForm(self._interactor, new_state)
+
+    @raises_locust_error
     def select_card_choice_field_by_label(self, label: str, index: int, locust_request_label: str = "") -> 'SailUiForm':
         """
         Select a card by it's lable
         Index is position to be selected
 
         Args:
             label(str): Label of the radio button field
```

### Comparing `appian-locust-2.0.0b0/appian_locust/utilities/credentials.py` & `appian-locust-2.0.1/appian_locust/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/utilities/helper.py` & `appian-locust-2.0.1/appian_locust/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/utilities/loadDriverUtils.py` & `appian-locust-2.0.1/appian_locust/utilities/loadDriverUtils.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/utilities/logger.py` & `appian-locust-2.0.1/appian_locust/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/appian_locust/visitor.py` & `appian-locust-2.0.1/appian_locust/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,17 @@
         """
         Get a RecordListUiForm for a record list page on a site
 
         Args:
             site_name(str): Site where the page exists
             page_name(str): Page to navigate to
 
+        NOTE: The actual Type of the Site Page MUST be "Record List", this will not work for sites that are of other page types,
+              such as an Interface with a record grid.
+
         Returns: SailUiForm
 
         Example:
             >>> self.appian.visitor.visit_site_recordlist("site_name","page_name")
 
         """
         page_type = self.__sites.get_site_page_type(site_name, page_name)
@@ -234,14 +237,17 @@
         """
         Navigates to a site page that is a recordlist then clicks on a random record instance on the first page
 
         Args:
             site_name: Site Url stub
             page_name: Page Url stub
 
+        NOTE: The actual Type of the Site Page MUST be "Record List", this will not work for sites that are of other page types,
+              such as an Interface with a record grid.
+
         Returns: RecordInstanceUiForm
         """
 
         site_page_json_response = self.__sites.fetch_site_tab_record_json(site_name, page_name)
         summary_view = site_page_json_response.get("feed") is not None
         breadcrumb = f"Sites.{site_name}.{page_name}.SailUi"
         return RecordInstanceUiForm(self.__interactor, site_page_json_response, summary_view=summary_view, breadcrumb=breadcrumb)
```

### Comparing `appian-locust-2.0.0b0/appian_locust.egg-info/PKG-INFO` & `appian-locust-2.0.1/appian_locust.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appian-locust
-Version: 2.0.0b0
+Version: 2.0.1
 Summary: Tools and functions to make testing Appian with Locust easier
 Home-page: https://gitlab.com/appian-oss/appian-locust
 Author: Appian Performance & Reliability Engineering Squad
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -28,33 +28,33 @@
 - Form interactions (filling/submitting)
 - Finding and interacting with basic components on a SAIL interface
 - Navigating to records/reports/sites
 
 .. what_is_appian_locust-inclusion-end-do-not-remove
 
 
-For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__
+For full documentation, visit the `docs page <https://appian-locust.readthedocs.io/en/latest/>`__.
 
 .. disclaimer-inclusion-begin-do-not-remove
 
 **Disclaimer:**
 This library is continuously evolving.
 Currently the main focus is supporting essential use-cases.
 We are happy to accept contributions to further extend functionality, address bug fixes and improve usability.
 Please see the `Contributing <contributing.html>`__ section and feel free to reach out.
 
 .. disclaimer-inclusion-end-do-not-remove
 
 .. quick_start-inclusion-begin-do-not-remove
 
-********************
-Quick Start Guide
-********************
+************************
+Quick Installation Guide
+************************
 
-This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.7+ installed on your machine before proceeding.
+This is a quick guide to getting up and running with the appian-locust library. You will need Python 3.10+ installed on your machine before proceeding.
 
 Setup
 ------------
 
 1. Install appian-locust using `pip`, for more comprehensive projects we recommend using `pipenv`.
 
 .. code-block:: bash
@@ -71,40 +71,24 @@
 
     [requires]
     python_version = "3.10"
 
     [pipenv]
     allow_prereleases = true
 
-2. Configure your test to point at the Appian instance you will be using.
-You can use example file provided in this repository `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_:
-
-- Set ``host_address`` to the address of your Appian instance.
-- In ``auth``, specify the username and password of the user account to use. Note: This user must be able to access Tempo.
-
-.. code-block:: json
-
-    {
-        "host_address": "site-name.appiancloud.com",
-        "auth": [
-            "user.name",
-            "password"
-        ]
-    }
-
-3. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_locustfile.py>`_.
+2. Run the sample test `example_locustfile.py <https://gitlab.com/appian-oss/appian-locust/-/blob/main/examples/example_locustfile.py>`_.
 
 .. code-block:: bash
 
-    locust -f example_locustfile.py -u 1 -t 60 --headless
+    locust -f example_locustfile.py
 
-If everything is set up correctly, you should start to see output from the load test reporting results. This should run for 60 seconds and end with a summary report of the results.
+If everything is set up correctly, you should see a link to the `Locust web interface <https://docs.locust.io/en/stable/quickstart.html#locust-s-web-interface>`_, which you can use to start test runs and view results.
 
-* For more examples of different site interactions, see the ``example_*.py`` files included in this repository.
-* For more in-depth information about the test library, see the rest of this documentation.
+* For more information about how to build the workflow for your locust test, see the `How to Write a Locust Test <how_to_write_locust_tests.html>`__ section.
+* For more information on running locust tests, see the `How to Run Locust <how_to_run_locust.html>`__ section.
 
 Build from source
 ----------------------
 Clone the repository:
 
 .. code-block:: bash
 
@@ -125,18 +109,18 @@
 If you have issues installing, make sure you have the proper prerequisites installed for Locust and its dependencies.
 If you're having trouble on Windows, check `here <https://github.com/locustio/locust/issues/1208#issuecomment-569693439>`__
 
 Troubleshooting
 ----------------
 * **"Failed to establish a new connection: [Errno 8] nodename nor servname provided, or not known"**
 
-  * check that ``host_address`` is specified correctly in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that ``host_address`` is specified correctly in your locust test file.
 
 * **"Login unsuccessful, no multipart cookie found...make sure credentials are correct"**
 
-  * check that `auth` specifies a valid username and password combination for the site you're testing on in `example_config.json <https://gitlab.com/appian-oss/appian-locust/-/blob/master/examples/example_config.json>`_.
+  * check that `auth` specifies a valid username and password combination for the site you're testing on in your locust test file.
 
 * **"General request and response debugging"**
 
-  * Add ``self.appian.interactor.record_mode = True`` to your ``AppianTaskSet`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
+  * Add ``self.client.record_mode = True`` to your ``HttpUser`` subclass.  Files will be placed in ``/record_responses`` where the runner is executed.
 
 .. quick_start-inclusion-end-do-not-remove
```

### Comparing `appian-locust-2.0.0b0/appian_locust.egg-info/SOURCES.txt` & `appian-locust-2.0.1/appian_locust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/setup.cfg` & `appian-locust-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `appian-locust-2.0.0b0/setup.py` & `appian-locust-2.0.1/setup.py`

 * *Files identical despite different names*

