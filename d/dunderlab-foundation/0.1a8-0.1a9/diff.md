# Comparing `tmp/dunderlab-foundation-0.1a8.tar.gz` & `tmp/dunderlab-foundation-0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dunderlab-foundation-0.1a8.tar", last modified: Tue Aug  8 01:09:35 2023, max compression
+gzip compressed data, was "dunderlab-foundation-0.1a9.tar", last modified: Tue Aug  8 15:03:37 2023, max compression
```

## Comparing `dunderlab-foundation-0.1a8.tar` & `dunderlab-foundation-0.1a9.tar`

### file list

```diff
@@ -1,21 +1,756 @@
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 01:09:35.243928 dunderlab-foundation-0.1a8/
--rw-r--r--   0 yeison    (1000) users      (984)     1298 2023-08-08 00:47:48.000000 dunderlab-foundation-0.1a8/LICENSE
--rw-r--r--   0 yeison    (1000) users      (984)     1312 2023-08-08 01:09:35.243928 dunderlab-foundation-0.1a8/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)       16 2023-07-16 01:07:26.000000 dunderlab-foundation-0.1a8/README.md
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 01:09:35.240594 dunderlab-foundation-0.1a8/cmd/
--rw-r--r--   0 yeison    (1000) users      (984)     2815 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a8/cmd/foundation_logs
--rw-r--r--   0 yeison    (1000) users      (984)     1432 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a8/cmd/foundation_start
--rw-r--r--   0 yeison    (1000) users      (984)     6006 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a8/cmd/foundation_status
--rw-r--r--   0 yeison    (1000) users      (984)      881 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a8/cmd/foundation_worker
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 01:09:35.240594 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/
--rw-r--r--   0 yeison    (1000) users      (984)     1312 2023-08-08 01:09:35.000000 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (984)      374 2023-08-08 01:09:35.000000 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-08-08 01:09:35.000000 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (984)       25 2023-08-08 01:09:35.000000 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) users      (984)       11 2023-08-08 01:09:35.000000 dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/top_level.txt
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 01:09:35.240594 dunderlab-foundation-0.1a8/foundation/
--rw-r--r--   0 yeison    (1000) users      (984)        1 2023-07-16 00:31:29.000000 dunderlab-foundation-0.1a8/foundation/__init__.py
--rw-r--r--   0 yeison    (1000) users      (984)       38 2023-08-08 01:09:35.243928 dunderlab-foundation-0.1a8/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (984)     2079 2023-08-08 01:06:00.000000 dunderlab-foundation-0.1a8/setup.py
-drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 01:09:35.243928 dunderlab-foundation-0.1a8/test/
--rw-r--r--   0 yeison    (1000) users      (984)      532 2023-08-07 01:55:54.000000 dunderlab-foundation-0.1a8/test/tests_worker.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.267476 dunderlab-foundation-0.1a9/
+-rw-r--r--   0 yeison    (1000) users      (984)     1298 2023-08-08 00:47:48.000000 dunderlab-foundation-0.1a9/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)      207 2023-08-08 15:01:21.000000 dunderlab-foundation-0.1a9/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) users      (984)     1428 2023-08-08 15:03:37.267476 dunderlab-foundation-0.1a9/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)      132 2023-08-08 02:13:19.000000 dunderlab-foundation-0.1a9/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/cmd/
+-rw-r--r--   0 yeison    (1000) users      (984)     2815 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a9/cmd/foundation_logs
+-rw-r--r--   0 yeison    (1000) users      (984)      840 2023-08-08 13:26:11.000000 dunderlab-foundation-0.1a9/cmd/foundation_start
+-rw-r--r--   0 yeison    (1000) users      (984)     6006 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a9/cmd/foundation_status
+-rw-r--r--   0 yeison    (1000) users      (984)      881 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a9/cmd/foundation_worker
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)     1428 2023-08-08 15:03:37.000000 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)    57796 2023-08-08 15:03:37.000000 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-08-08 15:03:37.000000 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       25 2023-08-08 15:03:37.000000 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       11 2023-08-08 15:03:37.000000 dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/top_level.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-07-16 00:31:29.000000 dunderlab-foundation-0.1a9/foundation/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.200809 dunderlab-foundation-0.1a9/foundation/django/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/django/foundation/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/asgi.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3242 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/settings.py
+-rw-r--r--   0 yeison    (1000) users      (984)      755 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/urls.py
+-rw-r--r--   0 yeison    (1000) users      (984)      403 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/hci_framework/wsgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      669 2023-06-22 22:07:41.000000 dunderlab-foundation-0.1a9/foundation/django/foundation/manage.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/radiant/
+-rw-r--r--   0 yeison    (1000) users      (984)        2 2023-07-09 21:08:21.000000 dunderlab-foundation-0.1a9/foundation/radiant/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.200809 dunderlab-foundation-0.1a9/foundation/radiant/brython/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/radiant/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-09 21:05:07.000000 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/radiant/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1737 2023-07-10 00:34:54.000000 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/radiant/figurestream.py
+-rw-r--r--   0 yeison    (1000) users      (984)      254 2023-08-05 02:22:37.000000 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/radiant/server.py
+-rw-r--r--   0 yeison    (1000) users      (984)       57 2023-07-09 21:07:45.000000 dunderlab-foundation-0.1a9/foundation/radiant/brython/foundation/radiant/utils.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/radiant/python_tools/
+-rw-r--r--   0 yeison    (1000) users      (984)      804 2023-08-07 01:54:25.000000 dunderlab-foundation-0.1a9/foundation/radiant/python_tools/python_logger.py
+-rw-r--r--   0 yeison    (1000) users      (984)      853 2023-08-05 02:01:42.000000 dunderlab-foundation-0.1a9/foundation/radiant/python_tools/python_swarm.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3434 2023-08-06 22:24:54.000000 dunderlab-foundation-0.1a9/foundation/radiant/server.py
+-rw-r--r--   0 yeison    (1000) users      (984)      306 2023-08-01 02:26:57.000000 dunderlab-foundation-0.1a9/foundation/radiant/template.html
+-rw-r--r--   0 yeison    (1000) users      (984)       56 2023-07-09 21:07:01.000000 dunderlab-foundation-0.1a9/foundation/radiant/utils.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/utils/
+-rw-r--r--   0 yeison    (1000) users      (984)       67 2023-08-02 23:40:21.000000 dunderlab-foundation-0.1a9/foundation/utils/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1542 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a9/foundation/utils/kafkalogs.py
+-rw-r--r--   0 yeison    (1000) users      (984)    10660 2023-08-08 14:35:41.000000 dunderlab-foundation-0.1a9/foundation/utils/swarm.py
+-rw-r--r--   0 yeison    (1000) users      (984)     9962 2023-08-08 01:06:04.000000 dunderlab-foundation-0.1a9/foundation/utils/workers.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/
+-rw-r--r--   0 yeison    (1000) users      (984)      535 2023-08-02 21:50:34.000000 dunderlab-foundation-0.1a9/foundation/workers/__init__.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/django_worker/
+-rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-22 00:12:49.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/db.sqlite3
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangoship/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangoship/access.log
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-27 02:19:26.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangoship/error.log
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/
+-rwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-07-21 23:08:17.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/__init__.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      397 2023-07-21 23:08:17.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/asgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)     3233 2023-07-21 23:08:17.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/settings.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      766 2023-07-21 23:08:17.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/urls.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      485 2023-07-22 00:19:20.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/djangotest/wsgi.py
+-rwxr-xr-x   0 yeison    (1000) users      (984)      666 2023-07-21 23:08:17.000000 dunderlab-foundation-0.1a9/foundation/workers/django_worker/manage.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/figurestream_worker/
+-rwxr-xr-x   0 yeison    (1000) users      (984)     1191 2023-08-08 01:01:26.000000 dunderlab-foundation-0.1a9/foundation/workers/figurestream_worker/main.py
+-rw-r--r--   0 yeison    (1000) users      (984)       54 2023-08-08 01:07:01.000000 dunderlab-foundation-0.1a9/foundation/workers/figurestream_worker/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/main_app/
+-rw-r--r--   0 yeison    (1000) users      (984)     1654 2023-08-08 01:01:39.000000 dunderlab-foundation-0.1a9/foundation/workers/main_app/main.py
+-rw-r--r--   0 yeison    (1000) users      (984)       54 2023-08-08 13:29:02.000000 dunderlab-foundation-0.1a9/foundation/workers/main_app/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/main_app/styles/
+-rw-r--r--   0 yeison    (1000) users      (984)      402 2023-08-05 02:47:40.000000 dunderlab-foundation-0.1a9/foundation/workers/main_app/styles/styles.css
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/main_app/templates/
+-rw-r--r--   0 yeison    (1000) users      (984)      125 2023-08-05 02:31:01.000000 dunderlab-foundation-0.1a9/foundation/workers/main_app/templates/main_area.html
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/
+-rw-r--r--   0 yeison    (1000) users      (984)   131072 2023-08-08 13:27:52.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/db.sqlite3
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.207475 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/djangoship/
+-rw-r--r--   0 yeison    (1000) users      (984)     6507 2023-08-08 14:46:48.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/djangoship/access.log
+-rw-r--r--   0 yeison    (1000) users      (984)     2813 2023-08-08 14:46:47.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/djangoship/error.log
+-rwxr-xr-x   0 yeison    (1000) users      (984)      671 2023-07-22 20:40:50.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/manage.py
+-rw-r--r--   0 yeison    (1000) users      (984)      182 2023-07-22 22:50:08.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/requirements.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.210809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.214142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/
+-rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/autocomplete.4a81fc4242d0.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9114 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/autocomplete.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1147 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/autocomplete.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21357 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4847 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/base.64976e0f7339.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21207 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/base.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4737 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/base.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/changelists.9237a1ac391b.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6566 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/changelists.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1564 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/changelists.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dark_mode.css
+-rw-r--r--   0 yeison    (1000) users      (984)      849 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dark_mode.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2929 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css
+-rw-r--r--   0 yeison    (1000) users      (984)      849 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dark_mode.ef27a31af300.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dashboard.css
+-rw-r--r--   0 yeison    (1000) users      (984)      267 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dashboard.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css
+-rw-r--r--   0 yeison    (1000) users      (984)      267 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/dashboard.e90f2068217b.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9090 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2236 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/forms.3b181cba6653.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     9047 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/forms.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2199 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/forms.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      958 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css
+-rw-r--r--   0 yeison    (1000) users      (984)      417 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/login.586129c60a93.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      958 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/login.css
+-rw-r--r--   0 yeison    (1000) users      (984)      417 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/login.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css
+-rw-r--r--   0 yeison    (1000) users      (984)      779 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/nav_sidebar.269a1bd44627.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2694 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/nav_sidebar.css
+-rw-r--r--   0 yeison    (1000) users      (984)      779 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/nav_sidebar.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css
+-rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive.107cd2690311.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18533 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive.css
+-rw-r--r--   0 yeison    (1000) users      (984)     3432 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css
+-rw-r--r--   0 yeison    (1000) users      (984)      527 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive_rtl.97b066429fd8.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1785 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive_rtl.css
+-rw-r--r--   0 yeison    (1000) users      (984)      527 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/responsive_rtl.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4878 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/rtl.4685390ad96d.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4788 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/rtl.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1229 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/rtl.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.214142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.f94142512c91.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/LICENSE-SELECT2.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.a2194c262648.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    17358 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2232 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.9f54e6414f87.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14966 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1978 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/vendor/select2/select2.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    12110 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2561 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/widgets.0a3765e806b3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    11900 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/widgets.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2468 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/css/widgets.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.220809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)     1081 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/LICENSE.2c54f4e1ca1c.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/LICENSE.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/README.a70711a38d87.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      319 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/README.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      214 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/README.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/calendar-icons.39b290681a8b.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1094 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/calendar-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      385 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/calendar-icons.svg.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.220809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.7a23bf31ef8a.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_off.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.0047eba25b67.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1129 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      472 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/gis/move_vertex_on.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-addlink.d519b3bab011.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-addlink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      206 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-addlink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-alert.034cc7d8a67f.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      504 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-alert.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      329 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-alert.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-calendar.ac7aea671bea.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1086 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-calendar.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      438 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-calendar.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-changelink.18d2fd706348.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      380 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-changelink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      269 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-changelink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-clock.e1d4dfac3f2b.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      677 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-clock.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      357 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-clock.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-deletelink.564ef9dc3854.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      392 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      221 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-deletelink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-no.439e821418cd.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-no.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      297 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-no.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.81536e128bb6.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown-alt.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown.a18cb4398978.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      655 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      377 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-unknown.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-viewlink.41eb31f7826e.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      581 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      346 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-viewlink.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-yes.d2f9f035226a.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-yes.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      266 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/icon-yes.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/inline-delete.fec1b761f254.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      560 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/inline-delete.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      293 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/inline-delete.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/search.7cf54ff789c6.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/search.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      264 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/search.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/selector-icons.b4555096cea2.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3291 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/selector-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      770 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/selector-icons.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/sorting-icons.3a097b59f104.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/sorting-icons.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      366 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/sorting-icons.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-add.e59d620a9742.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      331 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-add.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      203 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-add.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.bbfb788a849e.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      280 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg
+-rw-r--r--   0 yeison    (1000) users      (984)      194 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/img/tooltag-arrowright.svg.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.227476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectBox.7d3ce5a98007.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     4530 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectBox.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1025 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectBox.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectFilter2.bdb8d0cc579e.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15292 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectFilter2.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2914 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/SelectFilter2.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/actions.eac7e3441574.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7872 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/actions.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1874 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/actions.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.227476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/
+-rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.9f6e209cebca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    19319 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3645 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/DateTimeShortcuts.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.8609f99b9ab2.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8943 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2301 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/admin/RelatedObjectLookups.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js
+-rw-r--r--   0 yeison    (1000) users      (984)      425 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/autocomplete.01591ab27be7.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1060 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/autocomplete.js
+-rw-r--r--   0 yeison    (1000) users      (984)      425 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/autocomplete.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/calendar.f8a5d055eb33.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     8466 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/calendar.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2193 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/calendar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      884 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js
+-rw-r--r--   0 yeison    (1000) users      (984)      430 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/cancel.ecc4c5ca7b32.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      884 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/cancel.js
+-rw-r--r--   0 yeison    (1000) users      (984)      430 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/cancel.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      606 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js
+-rw-r--r--   0 yeison    (1000) users      (984)      322 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/change_form.9d8ca4f96b75.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      606 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/change_form.js
+-rw-r--r--   0 yeison    (1000) users      (984)      322 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/change_form.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      614 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/collapse.f84e7410290f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1803 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/collapse.js
+-rw-r--r--   0 yeison    (1000) users      (984)      614 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/collapse.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/core.cf103cd04ebf.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5682 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/core.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1505 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/core.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      978 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js
+-rw-r--r--   0 yeison    (1000) users      (984)      502 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/filters.0e360b7a9f80.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      978 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/filters.js
+-rw-r--r--   0 yeison    (1000) users      (984)      502 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/filters.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/inlines.22d4d93c00b4.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    15526 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/inlines.js
+-rw-r--r--   0 yeison    (1000) users      (984)     3744 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/inlines.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      347 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js
+-rw-r--r--   0 yeison    (1000) users      (984)      236 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/jquery.init.b7781a0897fc.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      347 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/jquery.init.js
+-rw-r--r--   0 yeison    (1000) users      (984)      236 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/jquery.init.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      845 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/nav_sidebar.3b9190d420b1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3063 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/nav_sidebar.js
+-rw-r--r--   0 yeison    (1000) users      (984)      845 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/nav_sidebar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js
+-rw-r--r--   0 yeison    (1000) users      (984)      270 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/popup_response.c6cc78ea5551.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/popup_response.js
+-rw-r--r--   0 yeison    (1000) users      (984)      270 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/popup_response.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      536 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate.bd2361dfd64d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1531 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate.js
+-rw-r--r--   0 yeison    (1000) users      (984)      536 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      586 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js
+-rw-r--r--   0 yeison    (1000) users      (984)      277 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate_init.6cac7f3105b8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      586 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate_init.js
+-rw-r--r--   0 yeison    (1000) users      (984)      277 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/prepopulate_init.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      605 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/theme.ab270f56bb9c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1943 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/theme.js
+-rw-r--r--   0 yeison    (1000) users      (984)      605 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/theme.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/urlify.ae970a820212.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     7887 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/urlify.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2578 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/urlify.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.227476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.de877aa6d744.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1097 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      656 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/LICENSE.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js
+-rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.0208b96062ba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   292458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js
+-rw-r--r--   0 yeison    (1000) users      (984)    86002 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js
+-rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.641dd1437010.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89795 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    31011 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/jquery/jquery.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.230809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.f94142512c91.md.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1124 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md
+-rw-r--r--   0 yeison    (1000) users      (984)      685 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/LICENSE.md.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.250809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      460 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.4f6fcd73488c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js
+-rw-r--r--   0 yeison    (1000) users      (984)      460 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/af.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      905 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      498 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.65aa8e36bf5d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      905 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js
+-rw-r--r--   0 yeison    (1000) users      (984)      498 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ar.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      721 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.270c257daf81.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      721 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/az.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      968 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      541 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.39b8be30d4f0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      968 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js
+-rw-r--r--   0 yeison    (1000) users      (984)      541 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bg.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js
+-rw-r--r--   0 yeison    (1000) users      (984)      553 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.6d42b4dd5665.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1291 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js
+-rw-r--r--   0 yeison    (1000) users      (984)      553 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bn.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      965 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js
+-rw-r--r--   0 yeison    (1000) users      (984)      523 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.91624382358e.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      965 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js
+-rw-r--r--   0 yeison    (1000) users      (984)      523 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/bs.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.a166b745933a.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js
+-rw-r--r--   0 yeison    (1000) users      (984)      623 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.4f43e8e7d33a.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1292 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js
+-rw-r--r--   0 yeison    (1000) users      (984)      623 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/cs.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      828 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.766346afe4dd.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      828 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js
+-rw-r--r--   0 yeison    (1000) users      (984)      441 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/da.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.8a1c222b0204.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      866 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/de.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.56372c92d2f1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1017 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      551 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/dsb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js
+-rw-r--r--   0 yeison    (1000) users      (984)      644 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.27097f071856.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1182 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js
+-rw-r--r--   0 yeison    (1000) users      (984)      644 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/el.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      844 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js
+-rw-r--r--   0 yeison    (1000) users      (984)      447 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.cf932ba09a98.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      844 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js
+-rw-r--r--   0 yeison    (1000) users      (984)      447 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/en.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      922 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      474 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.66dbc2652fb1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      922 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js
+-rw-r--r--   0 yeison    (1000) users      (984)      474 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/es.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      801 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      432 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.2b96fd98289d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      801 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js
+-rw-r--r--   0 yeison    (1000) users      (984)      432 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/et.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      868 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      450 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.adfe5c97b72c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      868 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js
+-rw-r--r--   0 yeison    (1000) users      (984)      450 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/eu.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js
+-rw-r--r--   0 yeison    (1000) users      (984)      538 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.3b5bd1961cfd.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1023 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js
+-rw-r--r--   0 yeison    (1000) users      (984)      538 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fa.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      803 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.614ec42aa9ba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      803 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js
+-rw-r--r--   0 yeison    (1000) users      (984)      484 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.05e0542fcfe6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      484 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/fr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.d99b1fedaa86.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      924 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/gl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      984 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js
+-rw-r--r--   0 yeison    (1000) users      (984)      518 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.e420ff6cd3ed.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      984 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js
+-rw-r--r--   0 yeison    (1000) users      (984)      518 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/he.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      572 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.70640d41628f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1175 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      572 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      852 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js
+-rw-r--r--   0 yeison    (1000) users      (984)      477 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.a2b092cc1147.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      852 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      477 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js
+-rw-r--r--   0 yeison    (1000) users      (984)      556 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.fa3b55265efe.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1018 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      556 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hsb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      831 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.6ec6039cb8a3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      831 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js
+-rw-r--r--   0 yeison    (1000) users      (984)      467 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hu.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js
+-rw-r--r--   0 yeison    (1000) users      (984)      530 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.c7babaeef5a6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1028 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js
+-rw-r--r--   0 yeison    (1000) users      (984)      530 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/hy.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js
+-rw-r--r--   0 yeison    (1000) users      (984)      416 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.04debded514d.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js
+-rw-r--r--   0 yeison    (1000) users      (984)      416 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/id.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      807 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.3ddd9a6a97e9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      807 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js
+-rw-r--r--   0 yeison    (1000) users      (984)      465 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/is.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      897 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js
+-rw-r--r--   0 yeison    (1000) users      (984)      488 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.be4fe8d365b5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      897 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js
+-rw-r--r--   0 yeison    (1000) users      (984)      488 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/it.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      862 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.170ae885d74f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      862 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ja.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      533 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.2083264a54f0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1195 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js
+-rw-r--r--   0 yeison    (1000) users      (984)      533 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ka.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js
+-rw-r--r--   0 yeison    (1000) users      (984)      540 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.c23089cb06ca.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1088 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js
+-rw-r--r--   0 yeison    (1000) users      (984)      540 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/km.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      855 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js
+-rw-r--r--   0 yeison    (1000) users      (984)      506 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.e7be6c20e673.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      855 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js
+-rw-r--r--   0 yeison    (1000) users      (984)      506 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ko.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      944 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js
+-rw-r--r--   0 yeison    (1000) users      (984)      521 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.23c7ce903300.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      944 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js
+-rw-r--r--   0 yeison    (1000) users      (984)      521 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lt.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      505 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.08e62128eac1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      900 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js
+-rw-r--r--   0 yeison    (1000) users      (984)      505 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/lv.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js
+-rw-r--r--   0 yeison    (1000) users      (984)      557 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.dabbb9087130.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1038 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      557 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/mk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      811 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.4ba82c9a51ce.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      811 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js
+-rw-r--r--   0 yeison    (1000) users      (984)      436 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ms.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      778 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.da2fce143f27.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      778 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js
+-rw-r--r--   0 yeison    (1000) users      (984)      413 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nb.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js
+-rw-r--r--   0 yeison    (1000) users      (984)      591 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.3d79fd3f08db.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1357 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js
+-rw-r--r--   0 yeison    (1000) users      (984)      591 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ne.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      904 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js
+-rw-r--r--   0 yeison    (1000) users      (984)      469 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.997868a37ed8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      904 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      469 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/nl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      947 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js
+-rw-r--r--   0 yeison    (1000) users      (984)      524 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.6031b4f16452.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      947 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      524 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js
+-rw-r--r--   0 yeison    (1000) users      (984)      587 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.38dfa47af9e0.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1049 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js
+-rw-r--r--   0 yeison    (1000) users      (984)      587 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ps.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      876 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      486 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.e1b294433e7f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      876 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js
+-rw-r--r--   0 yeison    (1000) users      (984)      486 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt-BR.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      878 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.33b4a3b44d43.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      878 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js
+-rw-r--r--   0 yeison    (1000) users      (984)      470 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/pt.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      938 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.f75cb460ec3b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      938 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js
+-rw-r--r--   0 yeison    (1000) users      (984)      511 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ro.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      632 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.934aa95f5b5f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1171 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js
+-rw-r--r--   0 yeison    (1000) users      (984)      632 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/ru.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js
+-rw-r--r--   0 yeison    (1000) users      (984)      617 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.33d02cef8d11.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1306 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      617 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      925 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js
+-rw-r--r--   0 yeison    (1000) users      (984)      487 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.131a78bc0752.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      925 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      487 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      903 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      490 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.5636b60d29c9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      903 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js
+-rw-r--r--   0 yeison    (1000) users      (984)      490 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sq.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      608 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.f254bb8c4c7c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1109 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rw-r--r--   0 yeison    (1000) users      (984)      608 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr-Cyrl.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      980 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js
+-rw-r--r--   0 yeison    (1000) users      (984)      552 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.5ed85a48f483.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      980 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      552 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      786 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.7a9c2f71e777.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      786 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js
+-rw-r--r--   0 yeison    (1000) users      (984)      429 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/sv.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      515 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.f38c20b0221b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1074 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js
+-rw-r--r--   0 yeison    (1000) users      (984)      515 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/th.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      771 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js
+-rw-r--r--   0 yeison    (1000) users      (984)      434 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.7c572a68c78f.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      771 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      434 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      775 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js
+-rw-r--r--   0 yeison    (1000) users      (984)      423 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.b5a0643d1545.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      775 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js
+-rw-r--r--   0 yeison    (1000) users      (984)      423 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/tr.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js
+-rw-r--r--   0 yeison    (1000) users      (984)      626 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.8cede7f4803c.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1156 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js
+-rw-r--r--   0 yeison    (1000) users      (984)      626 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/uk.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      796 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js
+-rw-r--r--   0 yeison    (1000) users      (984)      479 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.097a5b75b3e1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      796 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js
+-rw-r--r--   0 yeison    (1000) users      (984)      479 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/vi.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      468 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.2cff662ec5f9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      768 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js
+-rw-r--r--   0 yeison    (1000) users      (984)      468 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-CN.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      707 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js
+-rw-r--r--   0 yeison    (1000) users      (984)      451 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.04554a227c2b.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      707 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js
+-rw-r--r--   0 yeison    (1000) users      (984)      451 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/i18n/zh-TW.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.c2afdeda3058.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   173566 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37925 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js
+-rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.fcd7500d8e13.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    79212 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    21986 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/select2/select2.full.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.250809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/
+-rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.bf79e414957a.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1103 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      679 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/LICENSE.txt.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js
+-rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.efda034b9537.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   232381 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js
+-rw-r--r--   0 yeison    (1000) users      (984)    60899 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.b0439563a5d3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   125266 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    37609 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/admin/js/vendor/xregexp/xregexp.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.254142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/css/
+-rw-r--r--   0 yeison    (1000) users      (984)      753 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css
+-rw-r--r--   0 yeison    (1000) users      (984)      452 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.1a774d452e48.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      740 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css
+-rw-r--r--   0 yeison    (1000) users      (984)      440 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/css/jquery.autocomplete.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.254142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/img/indicator.03ce3dcc84af.gif
+-rw-r--r--   0 yeison    (1000) users      (984)     1553 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/img/indicator.gif
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.254142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js
+-rw-r--r--   0 yeison    (1000) users      (984)      960 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.5fc2188f8a16.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2800 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js
+-rw-r--r--   0 yeison    (1000) users      (984)      960 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.ajaxQueue.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js
+-rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.26e55daaf7c5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    36679 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js
+-rw-r--r--   0 yeison    (1000) users      (984)     7733 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.autocomplete.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js
+-rw-r--r--   0 yeison    (1000) users      (984)      814 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.68c9c05397e9.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1821 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js
+-rw-r--r--   0 yeison    (1000) users      (984)      814 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/django_extensions/js/jquery.bgiframe.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.257476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     2783 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.1d4b05b397c3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    23411 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map
+-rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.51806092cc05.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2772 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    75600 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 yeison    (1000) users      (984)     8032 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-theme.min.css.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3398 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.46ed116b0edd.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3385 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1256 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap-tweaks.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   121457 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map
+-rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.cafbda9c0e9e.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    19586 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   540434 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map
+-rw-r--r--   0 yeison    (1000) users      (984)    94401 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.css.map.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   121560 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css
+-rw-r--r--   0 yeison    (1000) users      (984)    19657 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/bootstrap.min.f17d4516b026.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css
+-rw-r--r--   0 yeison    (1000) users      (984)      612 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/default.789dfb5732d7.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1152 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/default.css
+-rw-r--r--   0 yeison    (1000) users      (984)      612 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/default.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21723 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4230 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.c1e1ea213abf.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    21658 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css
+-rw-r--r--   0 yeison    (1000) users      (984)     4186 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/font-awesome-4.0.3.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      817 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css
+-rw-r--r--   0 yeison    (1000) users      (984)      390 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/prettify.a987f72342ee.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)      817 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/prettify.css
+-rw-r--r--   0 yeison    (1000) users      (984)      390 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/css/prettify.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.204142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.257476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/
+-rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/base.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/base.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     6156 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css
+-rw-r--r--   0 yeison    (1000) users      (984)     1609 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/base.e630f8f4990e.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css
+-rw-r--r--   0 yeison    (1000) users      (984)      671 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1682 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css
+-rw-r--r--   0 yeison    (1000) users      (984)      671 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/highlight.e0e4d973c6d7.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css
+-rw-r--r--   0 yeison    (1000) users      (984)      640 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.a2e6beeb6710.css.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1307 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css
+-rw-r--r--   0 yeison    (1000) users      (984)      640 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/css/jquery.json-view.min.css.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.257476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico
+-rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.5195b4d0f3eb.ico.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     5430 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico
+-rw-r--r--   0 yeison    (1000) users      (984)      256 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/favicon.ico.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/grid.a4b938cf382b.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/img/grid.png
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.260809 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/
+-rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/api.18a5ba8a1bd8.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    10391 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/api.js
+-rw-r--r--   0 yeison    (1000) users      (984)     2584 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/api.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js
+-rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.479b5f21dcba.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   300764 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js
+-rw-r--r--   0 yeison    (1000) users      (984)   112518 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/highlight.pack.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.b7c2d6981377.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     2700 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1013 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/docs/js/jquery.json-view.min.js.gz
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.264142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/
+-rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.3293616ec0c6.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.83e37a11f9d7.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.8b27bc96115c.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.dcb26c7239d8.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    38205 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 yeison    (1000) users      (984)   202148 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    56103 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    80652 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    44333 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    44432 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.08eda92397ae.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.448c34a56d69.woff2
+-rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.e18bbf611f2a.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    20127 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.f4769f9bdb74.eot
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.fa2772327f55.woff
+-rw-r--r--   0 yeison    (1000) users      (984)   108738 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 yeison    (1000) users      (984)    26509 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.svg.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    45404 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 yeison    (1000) users      (984)    23360 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.ttf.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    23424 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 yeison    (1000) users      (984)    18028 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.264142 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/
+-rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.9bbc6e960299.png
+-rw-r--r--   0 yeison    (1000) users      (984)     8777 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings-white.png
+-rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.90233c9067e9.png
+-rw-r--r--   0 yeison    (1000) users      (984)    12762 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/glyphicons-halflings.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/grid.a4b938cf382b.png
+-rw-r--r--   0 yeison    (1000) users      (984)     1458 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/img/grid.png
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.267476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/
+-rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/ajax-form.0ea6e6052ab5.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     3597 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js
+-rw-r--r--   0 yeison    (1000) users      (984)     1540 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/ajax-form.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.2f34b630ffe3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    39680 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    10896 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/bootstrap.min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    63224 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js
+-rw-r--r--   0 yeison    (1000) users      (984)    14375 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.e580e3854595.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)   157600 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js
+-rw-r--r--   0 yeison    (1000) users      (984)    40759 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/coreapi-0.1.1.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js
+-rw-r--r--   0 yeison    (1000) users      (984)      787 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/csrf.969930007329.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1719 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/csrf.js
+-rw-r--r--   0 yeison    (1000) users      (984)      787 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/csrf.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js
+-rw-r--r--   0 yeison    (1000) users      (984)      571 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/default.5b08897dbdc3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)     1268 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/default.js
+-rw-r--r--   0 yeison    (1000) users      (984)      571 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/default.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js
+-rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.dc5e7f18c8d3.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    89476 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js
+-rw-r--r--   0 yeison    (1000) users      (984)    30879 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/jquery-3.5.1.min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js
+-rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/prettify-min.709bfcc456c6.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    13632 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js
+-rw-r--r--   0 yeison    (1000) users      (984)     6025 2023-07-22 23:45:33.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/rest_framework/js/prettify-min.js.gz
+-rw-r--r--   0 yeison    (1000) users      (984)    14226 2023-08-08 13:27:49.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/resources/staticfiles.json
+-rw-r--r--   0 yeison    (1000) users      (984)      336 2023-07-23 01:07:34.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/startup.sh
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-08-08 15:03:37.267476 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2023-07-22 20:40:50.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)      407 2023-07-22 20:40:50.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/asgi.py
+-rw-r--r--   0 yeison    (1000) users      (984)     5910 2023-07-23 00:02:18.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/settings.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1062 2023-07-22 20:56:12.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/urls.py
+-rw-r--r--   0 yeison    (1000) users      (984)      494 2023-07-22 20:41:41.000000 dunderlab-foundation-0.1a9/foundation/workers/timescaledb_api/timescaledb_api/wsgi.py
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-08-08 15:03:37.267476 dunderlab-foundation-0.1a9/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     2079 2023-08-08 15:01:30.000000 dunderlab-foundation-0.1a9/setup.py
```

### Comparing `dunderlab-foundation-0.1a8/LICENSE` & `dunderlab-foundation-0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `dunderlab-foundation-0.1a8/PKG-INFO` & `dunderlab-foundation-0.1a9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-foundation
-Version: 0.1a8
+Version: 0.1a9
 Download-URL: https://github.com/dunderlab/python-dunerlab.foundation
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
@@ -23,8 +23,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# HCI Framework
+# Foundation
+
+Documentation will be here...
+
+
+[python-dunerlab.foundation](https://github.com/dunderlab/python-dunerlab.foundation)
```

### Comparing `dunderlab-foundation-0.1a8/cmd/foundation_logs` & `dunderlab-foundation-0.1a9/cmd/foundation_logs`

 * *Files identical despite different names*

### Comparing `dunderlab-foundation-0.1a8/cmd/foundation_status` & `dunderlab-foundation-0.1a9/cmd/foundation_status`

 * *Files identical despite different names*

### Comparing `dunderlab-foundation-0.1a8/cmd/foundation_worker` & `dunderlab-foundation-0.1a9/cmd/foundation_worker`

 * *Files identical despite different names*

### Comparing `dunderlab-foundation-0.1a8/dunderlab_foundation.egg-info/PKG-INFO` & `dunderlab-foundation-0.1a9/dunderlab_foundation.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dunderlab-foundation
-Version: 0.1a8
+Version: 0.1a9
 Download-URL: https://github.com/dunderlab/python-dunerlab.foundation
 Author: Yeison Cardona
 Author-email: yencardonaal@unal.edu.co
 Maintainer: Yeison Cardona
 Maintainer-email: yencardonaal@unal.edu.co
 License: BSD-2-Clause
 Classifier: Development Status :: 4 - Beta
@@ -23,8 +23,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# HCI Framework
+# Foundation
+
+Documentation will be here...
+
+
+[python-dunerlab.foundation](https://github.com/dunderlab/python-dunerlab.foundation)
```

### Comparing `dunderlab-foundation-0.1a8/setup.py` & `dunderlab-foundation-0.1a9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
-version_str = '0.1a8'
+version_str = '0.1a9'
 
 setup(
     name='dunderlab-foundation',
     version=version_str,
     packages=['foundation'],
 
     author='Yeison Cardona',
```

