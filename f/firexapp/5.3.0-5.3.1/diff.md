# Comparing `tmp/firexapp-5.3.0.tar.gz` & `tmp/firexapp-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firexapp-5.3.0.tar", last modified: Mon Aug  7 19:31:29 2023, max compression
+gzip compressed data, was "firexapp-5.3.1.tar", last modified: Mon Aug  7 22:54:28 2023, max compression
```

## Comparing `firexapp-5.3.0.tar` & `firexapp-5.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.508924 firexapp-5.3.0/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-07 19:31:14.000000 firexapp-5.3.0/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-08-07 19:31:14.000000 firexapp-5.3.0/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 19:31:29.509925 firexapp-5.3.0/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-08-07 19:31:14.000000 firexapp-5.3.0/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-08-07 19:31:14.000000 firexapp-5.3.0/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.509925 firexapp-5.3.0/firexapp/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-07 19:31:29.509925 firexapp-5.3.0/firexapp/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7352 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/application.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.500924 firexapp-5.3.0/firexapp/broker_manager/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/broker_factory.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13497 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/broker_manager/redis_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/celery_manager.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/common.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/discovery.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.501924 firexapp-5.3.0/firexapp/engine/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/celery.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/default_celery_config.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6851 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/engine/logging.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.502925 firexapp-5.3.0/firexapp/events/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/broker_event_consumer.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/event_aggregator.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/events/model.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/fileregistry.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    15762 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/firex_subprocess.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/info.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/plugins.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.503924 firexapp-5.3.0/firexapp/reporters/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/reporters/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/reporters/json_reporter.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.505924 firexapp-5.3.0/firexapp/submit/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/arguments.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/console.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/install_configs.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/report_trigger.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/reporting.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/shutdown.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    32000 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/submit.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/tracking_service.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4647 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/submit/uid.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.507924 firexapp-5.3.0/firexapp/tasks/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/core_tasks.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/example.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/tasks/root_tasks.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.508924 firexapp-5.3.0/firexapp/testing/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/config_base.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    12807 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/config_interpreter.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/coverage_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/pydev_debug_plugin.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7451 2023-08-07 19:31:14.000000 firexapp-5.3.0/firexapp/testing/test_infra.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 19:31:29.499925 firexapp-5.3.0/firexapp.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      196 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 19:31:29.000000 firexapp-5.3.0/firexapp.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      267 2023-08-07 19:31:29.509925 firexapp-5.3.0/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1713 2023-08-07 19:31:14.000000 firexapp-5.3.0/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-07 19:31:14.000000 firexapp-5.3.0/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.316801 firexapp-5.3.1/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1513 2023-08-07 22:54:13.000000 firexapp-5.3.1/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      155 2023-08-07 22:54:13.000000 firexapp-5.3.1/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 22:54:28.316801 firexapp-5.3.1/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       17 2023-08-07 22:54:13.000000 firexapp-5.3.1/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2023-08-07 22:54:13.000000 firexapp-5.3.1/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.317801 firexapp-5.3.1/firexapp/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       93 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       45 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      497 2023-08-07 22:54:28.317801 firexapp-5.3.1/firexapp/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7352 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/application.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.308801 firexapp-5.3.1/firexapp/broker_manager/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      699 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3100 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/broker_factory.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13497 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/broker_manager/redis_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    13246 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/celery_manager.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6680 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/common.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6676 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/discovery.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.309801 firexapp-5.3.1/firexapp/engine/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1599 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/celery.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4667 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/default_celery_config.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6851 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/engine/logging.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.310801 firexapp-5.3.1/firexapp/events/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4726 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/broker_event_consumer.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    14847 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/event_aggregator.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3571 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/events/model.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1827 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/fileregistry.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15762 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/firex_subprocess.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11065 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/info.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    11513 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/plugins.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.310801 firexapp-5.3.1/firexapp/reporters/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/reporters/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6049 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/reporters/json_reporter.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.313801 firexapp-5.3.1/firexapp/submit/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    10084 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/arguments.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5627 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/console.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7692 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/install_configs.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      907 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/report_trigger.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     5423 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/reporting.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9662 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/shutdown.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    32000 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/submit.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1576 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/tracking_service.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4612 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/submit/uid.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.314801 firexapp-5.3.1/firexapp/tasks/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3226 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/core_tasks.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6445 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/example.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3687 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/tasks/root_tasks.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.316801 firexapp-5.3.1/firexapp/testing/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4360 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/config_base.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    12807 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/config_interpreter.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1099 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/coverage_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3365 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/pydev_debug_plugin.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7451 2023-08-07 22:54:13.000000 firexapp-5.3.1/firexapp/testing/test_infra.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2023-08-07 22:54:28.307801 firexapp-5.3.1/firexapp.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      435 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)     1598 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      190 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      201 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        9 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2023-08-07 22:54:28.000000 firexapp-5.3.1/firexapp.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      268 2023-08-07 22:54:28.317801 firexapp-5.3.1/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1731 2023-08-07 22:54:13.000000 firexapp-5.3.1/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2023-08-07 22:54:13.000000 firexapp-5.3.1/versioneer.py
```

### Comparing `firexapp-5.3.0/LICENSE` & `firexapp-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/fastentrypoints.py` & `firexapp-5.3.1/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/application.py` & `firexapp-5.3.1/firexapp/application.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/broker_manager/__init__.py` & `firexapp-5.3.1/firexapp/broker_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/broker_manager/broker_factory.py` & `firexapp-5.3.1/firexapp/broker_manager/broker_factory.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/broker_manager/redis_manager.py` & `firexapp-5.3.1/firexapp/broker_manager/redis_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/celery_manager.py` & `firexapp-5.3.1/firexapp/celery_manager.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/common.py` & `firexapp-5.3.1/firexapp/common.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/discovery.py` & `firexapp-5.3.1/firexapp/discovery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/engine/celery.py` & `firexapp-5.3.1/firexapp/engine/celery.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/engine/default_celery_config.py` & `firexapp-5.3.1/firexapp/engine/default_celery_config.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/engine/logging.py` & `firexapp-5.3.1/firexapp/engine/logging.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/events/broker_event_consumer.py` & `firexapp-5.3.1/firexapp/events/broker_event_consumer.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/events/event_aggregator.py` & `firexapp-5.3.1/firexapp/events/event_aggregator.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/events/model.py` & `firexapp-5.3.1/firexapp/events/model.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/fileregistry.py` & `firexapp-5.3.1/firexapp/fileregistry.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/firex_subprocess.py` & `firexapp-5.3.1/firexapp/firex_subprocess.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/info.py` & `firexapp-5.3.1/firexapp/info.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/plugins.py` & `firexapp-5.3.1/firexapp/plugins.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/reporters/json_reporter.py` & `firexapp-5.3.1/firexapp/reporters/json_reporter.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/arguments.py` & `firexapp-5.3.1/firexapp/submit/arguments.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/console.py` & `firexapp-5.3.1/firexapp/submit/console.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/install_configs.py` & `firexapp-5.3.1/firexapp/submit/install_configs.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/report_trigger.py` & `firexapp-5.3.1/firexapp/submit/report_trigger.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/reporting.py` & `firexapp-5.3.1/firexapp/submit/reporting.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/shutdown.py` & `firexapp-5.3.1/firexapp/submit/shutdown.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/submit.py` & `firexapp-5.3.1/firexapp/submit/submit.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/tracking_service.py` & `firexapp-5.3.1/firexapp/submit/tracking_service.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/submit/uid.py` & `firexapp-5.3.1/firexapp/submit/uid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import tempfile
 from getpass import getuser
 import random
 import firexkit
 import shutil
 import re
 from typing import Optional
-from collections import namedtuple
 
 from firexapp.submit.arguments import whitelist_arguments
 from firexkit.permissions import DEFAULT_CHMOD_MODE
 
 BASE_LOGGING_DIR_ENV_VAR_KEY = 'firex_base_logging_dir'
 
 FIREX_ID_DATE_FMT = "%y%m%d-%H%M%S"
```

### Comparing `firexapp-5.3.0/firexapp/tasks/core_tasks.py` & `firexapp-5.3.1/firexapp/tasks/core_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/tasks/example.py` & `firexapp-5.3.1/firexapp/tasks/example.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/tasks/root_tasks.py` & `firexapp-5.3.1/firexapp/tasks/root_tasks.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/testing/config_base.py` & `firexapp-5.3.1/firexapp/testing/config_base.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/testing/config_interpreter.py` & `firexapp-5.3.1/firexapp/testing/config_interpreter.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/testing/coverage_plugin.py` & `firexapp-5.3.1/firexapp/testing/coverage_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/testing/pydev_debug_plugin.py` & `firexapp-5.3.1/firexapp/testing/pydev_debug_plugin.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp/testing/test_infra.py` & `firexapp-5.3.1/firexapp/testing/test_infra.py`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/firexapp.egg-info/SOURCES.txt` & `firexapp-5.3.1/firexapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firexapp-5.3.0/setup.py` & `firexapp-5.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
           "celery[redis]==5.3.1",
           "psutil",
           "python-Levenshtein",
           "entrypoints",
           "colorlog==2.10.0",
           "beautifulsoup4",
           "detach3k",
+          "pytz",
       ],
       extras_require={
           'test': [
               'firex-keeper',
           ],
           'flame': [
               'firex-flame'
```

### Comparing `firexapp-5.3.0/versioneer.py` & `firexapp-5.3.1/versioneer.py`

 * *Files identical despite different names*

