# Comparing `tmp/django-redis_metrics-2.1.0.tar.gz` & `tmp/django-redis_metrics-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-redis_metrics-2.1.0.tar", last modified: Thu Mar 23 18:26:22 2023, max compression
+gzip compressed data, was "django-redis_metrics-2.2.0.tar", last modified: Tue Aug  8 20:41:39 2023, max compression
```

## Comparing `django-redis_metrics-2.1.0.tar` & `django-redis_metrics-2.2.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/
--rw-r--r--   0 brad      (1000) brad      (1000)      761 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/AUTHORS.rst
--rw-r--r--   0 brad      (1000) brad      (1000)     1086 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/LICENSE.txt
--rw-r--r--   0 brad      (1000) brad      (1000)       92 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/MANIFEST.in
--rw-r--r--   0 brad      (1000) brad      (1000)     2956 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/PKG-INFO
--rw-r--r--   0 brad      (1000) brad      (1000)     1830 2023-03-23 18:24:37.000000 django-redis_metrics-2.1.0/README.rst
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/
--rw-r--r--   0 brad      (1000) brad      (1000)     2956 2023-03-23 18:26:22.000000 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/PKG-INFO
--rw-r--r--   0 brad      (1000) brad      (1000)     2747 2023-03-23 18:26:22.000000 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 brad      (1000) brad      (1000)        1 2023-03-23 18:26:22.000000 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 brad      (1000) brad      (1000)       13 2023-03-23 18:26:22.000000 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/requires.txt
--rw-r--r--   0 brad      (1000) brad      (1000)       14 2023-03-23 18:26:22.000000 django-redis_metrics-2.1.0/django_redis_metrics.egg-info/top_level.txt
--rw-r--r--   0 brad      (1000) brad      (1000)     1425 2023-03-23 18:12:25.000000 django-redis_metrics-2.1.0/pyproject.toml
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/
--rw-r--r--   0 brad      (1000) brad      (1000)      234 2023-03-23 18:12:25.000000 django-redis_metrics-2.1.0/redis_metrics/__init__.py
--rw-r--r--   0 brad      (1000) brad      (1000)      175 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/apps.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2082 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/forms.py
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/management/
--rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/__init__.py
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/management/commands/
--rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/__init__.py
--rw-r--r--   0 brad      (1000) brad      (1000)      429 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/delete_gauge.py
--rw-r--r--   0 brad      (1000) brad      (1000)      464 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/delete_metric.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2801 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0 brad      (1000) brad      (1000)     1928 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0 brad      (1000) brad      (1000)     1742 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0 brad      (1000) brad      (1000)     1874 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0 brad      (1000) brad      (1000)     4343 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/management/commands/system_metric.py
--rw-r--r--   0 brad      (1000) brad      (1000)    24958 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/models.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2902 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/settings.py
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.707481 django-redis_metrics-2.1.0/redis_metrics/static/
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.707481 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/css/
--rwxr-xr-x   0 brad      (1000) brad      (1000)    24410 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/css/bs-theme.min.css
--rwxr-xr-x   0 brad      (1000) brad      (1000)    89844 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/css/bs.min.css
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/
--rw-r--r--   0 brad      (1000) brad      (1000)   142791 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/chart.min.js
--rw-r--r--   0 brad      (1000) brad      (1000)     1102 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/colors.js
--rw-r--r--   0 brad      (1000) brad      (1000)    24636 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/zepto.min.js
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.707481 django-redis_metrics-2.1.0/redis_metrics/templates/
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/
--rw-r--r--   0 brad      (1000) brad      (1000)     2778 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_aggregate_detail.html
--rw-r--r--   0 brad      (1000) brad      (1000)     2565 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_aggregate_history.html
--rw-r--r--   0 brad      (1000) brad      (1000)     1126 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_gauge.html
--rw-r--r--   0 brad      (1000) brad      (1000)     2021 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_detail.html
--rw-r--r--   0 brad      (1000) brad      (1000)     1540 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_history.html
--rw-r--r--   0 brad      (1000) brad      (1000)     1245 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_list.html
--rw-r--r--   0 brad      (1000) brad      (1000)      621 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_since.html
--rw-r--r--   0 brad      (1000) brad      (1000)      483 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/aggregate.html
--rw-r--r--   0 brad      (1000) brad      (1000)      617 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/aggregate_detail.html
--rw-r--r--   0 brad      (1000) brad      (1000)      824 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/aggregate_history.html
--rw-r--r--   0 brad      (1000) brad      (1000)     2030 2023-03-23 18:12:25.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/base.html
--rw-r--r--   0 brad      (1000) brad      (1000)      472 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/categorize.html
--rw-r--r--   0 brad      (1000) brad      (1000)     3126 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/default.html
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/email/
--rw-r--r--   0 brad      (1000) brad      (1000)      814 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/email/report.html
--rw-r--r--   0 brad      (1000) brad      (1000)      344 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/email/report.txt
--rw-r--r--   0 brad      (1000) brad      (1000)      424 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/gauges.html
--rw-r--r--   0 brad      (1000) brad      (1000)      470 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/metric_detail.html
--rw-r--r--   0 brad      (1000) brad      (1000)      756 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/metric_history.html
--rw-r--r--   0 brad      (1000) brad      (1000)      882 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/metrics_list.html
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/templatetags/
--rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templatetags/__init__.py
--rw-r--r--   0 brad      (1000) brad      (1000)     8113 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templatetags/redis_metric_tags.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2349 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/templatetags/redis_metrics_filters.py
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/tests/
--rw-r--r--   0 brad      (1000) brad      (1000)      283 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/__init__.py
--rw-r--r--   0 brad      (1000) brad      (1000)     1583 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/settings.py
-drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/redis_metrics/tests/templates/
--rw-r--r--   0 brad      (1000) brad      (1000)       32 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/templates/404.html
--rw-r--r--   0 brad      (1000) brad      (1000)     4542 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_forms.py
--rw-r--r--   0 brad      (1000) brad      (1000)    42803 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_models.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2328 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_settings.py
--rw-r--r--   0 brad      (1000) brad      (1000)    17830 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_templatetags.py
--rw-r--r--   0 brad      (1000) brad      (1000)     8916 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_utils.py
--rw-r--r--   0 brad      (1000) brad      (1000)    16892 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/test_views.py
--rw-r--r--   0 brad      (1000) brad      (1000)      255 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/tests/urls.py
--rw-r--r--   0 brad      (1000) brad      (1000)     1728 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/urls.py
--rw-r--r--   0 brad      (1000) brad      (1000)     2657 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/utils.py
--rw-r--r--   0 brad      (1000) brad      (1000)     7293 2023-03-23 15:52:19.000000 django-redis_metrics-2.1.0/redis_metrics/views.py
--rw-r--r--   0 brad      (1000) brad      (1000)       38 2023-03-23 18:26:22.717481 django-redis_metrics-2.1.0/setup.cfg
--rw-r--r--   0 brad      (1000) brad      (1000)       37 2023-03-23 18:12:25.000000 django-redis_metrics-2.1.0/setup.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/
+-rw-r--r--   0 brad      (1000) brad      (1000)      813 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/AUTHORS.rst
+-rw-r--r--   0 brad      (1000) brad      (1000)     1086 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/LICENSE.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)       92 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/MANIFEST.in
+-rw-r--r--   0 brad      (1000) brad      (1000)     2956 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/PKG-INFO
+-rw-r--r--   0 brad      (1000) brad      (1000)     1830 2023-03-23 18:24:37.000000 django-redis_metrics-2.2.0/README.rst
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/
+-rw-r--r--   0 brad      (1000) brad      (1000)     2956 2023-08-08 20:41:39.000000 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 brad      (1000) brad      (1000)     2747 2023-08-08 20:41:39.000000 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)        1 2023-08-08 20:41:39.000000 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)       13 2023-08-08 20:41:39.000000 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/requires.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)       14 2023-08-08 20:41:39.000000 django-redis_metrics-2.2.0/django_redis_metrics.egg-info/top_level.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)     1425 2023-03-23 18:12:25.000000 django-redis_metrics-2.2.0/pyproject.toml
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/
+-rw-r--r--   0 brad      (1000) brad      (1000)      234 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/redis_metrics/__init__.py
+-rw-r--r--   0 brad      (1000) brad      (1000)      175 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/apps.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2082 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/forms.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/management/
+-rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/__init__.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/management/commands/
+-rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/__init__.py
+-rw-r--r--   0 brad      (1000) brad      (1000)      429 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/delete_gauge.py
+-rw-r--r--   0 brad      (1000) brad      (1000)      464 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/delete_metric.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2801 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     1928 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     1742 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     1874 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     4343 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/management/commands/system_metric.py
+-rw-r--r--   0 brad      (1000) brad      (1000)    25131 2023-08-08 19:36:28.000000 django-redis_metrics-2.2.0/redis_metrics/models.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2924 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/redis_metrics/settings.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/static/
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/css/
+-rwxr-xr-x   0 brad      (1000) brad      (1000)    24410 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/css/bs-theme.min.css
+-rwxr-xr-x   0 brad      (1000) brad      (1000)    89844 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/css/bs.min.css
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/
+-rw-r--r--   0 brad      (1000) brad      (1000)   142791 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/chart.min.js
+-rw-r--r--   0 brad      (1000) brad      (1000)     1102 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/colors.js
+-rw-r--r--   0 brad      (1000) brad      (1000)    24636 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/zepto.min.js
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.054546 django-redis_metrics-2.2.0/redis_metrics/templates/
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/
+-rw-r--r--   0 brad      (1000) brad      (1000)     2778 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_aggregate_detail.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     2565 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_aggregate_history.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     1126 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_gauge.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     2021 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_detail.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     1540 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_history.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     1245 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_list.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      621 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_since.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      483 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/aggregate.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      617 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/aggregate_detail.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      824 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/aggregate_history.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     2030 2023-03-23 18:12:25.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/base.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      472 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/categorize.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     3126 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/default.html
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/email/
+-rw-r--r--   0 brad      (1000) brad      (1000)      814 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/email/report.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      344 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/email/report.txt
+-rw-r--r--   0 brad      (1000) brad      (1000)      424 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/gauges.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      470 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/metric_detail.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      756 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/metric_history.html
+-rw-r--r--   0 brad      (1000) brad      (1000)      882 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/metrics_list.html
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/templatetags/
+-rw-r--r--   0 brad      (1000) brad      (1000)        0 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templatetags/__init__.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     8113 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templatetags/redis_metric_tags.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2349 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/templatetags/redis_metrics_filters.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/tests/
+-rw-r--r--   0 brad      (1000) brad      (1000)      283 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/__init__.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     1583 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/settings.py
+drwxr-xr-x   0 brad      (1000) brad      (1000)        0 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/redis_metrics/tests/templates/
+-rw-r--r--   0 brad      (1000) brad      (1000)       32 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/templates/404.html
+-rw-r--r--   0 brad      (1000) brad      (1000)     4542 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_forms.py
+-rw-r--r--   0 brad      (1000) brad      (1000)    43365 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_models.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2328 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_settings.py
+-rw-r--r--   0 brad      (1000) brad      (1000)    17830 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_templatetags.py
+-rw-r--r--   0 brad      (1000) brad      (1000)    10119 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_utils.py
+-rw-r--r--   0 brad      (1000) brad      (1000)    16942 2023-08-08 20:38:57.000000 django-redis_metrics-2.2.0/redis_metrics/tests/test_views.py
+-rw-r--r--   0 brad      (1000) brad      (1000)      255 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/tests/urls.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     1728 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/urls.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     2657 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/utils.py
+-rw-r--r--   0 brad      (1000) brad      (1000)     7293 2023-03-23 15:52:19.000000 django-redis_metrics-2.2.0/redis_metrics/views.py
+-rw-r--r--   0 brad      (1000) brad      (1000)       38 2023-08-08 20:41:39.064546 django-redis_metrics-2.2.0/setup.cfg
+-rw-r--r--   0 brad      (1000) brad      (1000)       37 2023-03-23 18:12:25.000000 django-redis_metrics-2.2.0/setup.py
```

### Comparing `django-redis_metrics-2.1.0/AUTHORS.rst` & `django-redis_metrics-2.2.0/AUTHORS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -12,7 +12,8 @@
 - vlinhart `<https://github.com/vlinhart>`_
 - Dr. Stefan Schimanski `<https://github.com/sttts>`_
 - Seamus Mac Conaonaigh `<https://github.com/smaccona>`_
 - Phoebe Bright `<https://github.com/phoebebright>`_
 - Stephan Pötschner `<https://github.com/stephanpoetschner>`_
 - Elias Laitinen `<https://github.com/eliasla>`_
 - Derek Marsh `<https://github.com/dmarsh19>`_
+- Joe Ferguson `<https://github.com/svpernova09/>`_
```

### Comparing `django-redis_metrics-2.1.0/LICENSE.txt` & `django-redis_metrics-2.2.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019, Brad Montgomery <brad@bradmontgomery.net>
+Copyright (c) 2023, Brad Montgomery <brad@bradmontgomery.net>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `django-redis_metrics-2.1.0/PKG-INFO` & `django-redis_metrics-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis_metrics
-Version: 2.1.0
+Version: 2.2.0
 Summary: django-redis-metrics is a Django application for tracking application metrics backed by Redis.
 Author-email: Brad Montgomery <brad@bradmontgomery.net>
 License: MIT
 Project-URL: Homepage, https://github.com/bradmontgomery/django-redis_metrics
 Project-URL: Bug Tracker, https://github.com/bradmontgomery/django-redis_metrics/issues
 Keywords: django,redis_metrics,redis,metrics,performance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-redis_metrics-2.1.0/README.rst` & `django-redis_metrics-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/django_redis_metrics.egg-info/PKG-INFO` & `django-redis_metrics-2.2.0/django_redis_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-redis-metrics
-Version: 2.1.0
+Version: 2.2.0
 Summary: django-redis-metrics is a Django application for tracking application metrics backed by Redis.
 Author-email: Brad Montgomery <brad@bradmontgomery.net>
 License: MIT
 Project-URL: Homepage, https://github.com/bradmontgomery/django-redis_metrics
 Project-URL: Bug Tracker, https://github.com/bradmontgomery/django-redis_metrics/issues
 Keywords: django,redis_metrics,redis,metrics,performance
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-redis_metrics-2.1.0/django_redis_metrics.egg-info/SOURCES.txt` & `django-redis_metrics-2.2.0/django_redis_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/pyproject.toml` & `django-redis_metrics-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/forms.py` & `django-redis_metrics-2.2.0/redis_metrics/forms.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/management/commands/fix_redis_metrics_keys.py` & `django-redis_metrics-2.2.0/redis_metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/management/commands/generate_test_metrics.py` & `django-redis_metrics-2.2.0/redis_metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/management/commands/redis_metrics_send_mail.py` & `django-redis_metrics-2.2.0/redis_metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/management/commands/reset_weekly_metrics.py` & `django-redis_metrics-2.2.0/redis_metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/management/commands/system_metric.py` & `django-redis_metrics-2.2.0/redis_metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/models.py` & `django-redis_metrics-2.2.0/redis_metrics/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         * ``gauge_slugs_key`` -- The key storing a set of all slugs for gauges
           (default is "gauge-slugs")
         * ``connection_class`` -- class to use to obtain a Redis connection (set in settings.REDIS_METRICS['CONNECTION_CLASS'])
         * ``host`` -- Redis host (set in settings.REDIS_METRICS['HOST'])
         * ``port`` -- Redis port (set in settings.REDIS_METRICS['PORT'])
         * ``db`` -- Redis DB (set in settings.REDIS_METRICS['DB'])
         * ``password`` -- Redis password (set in settings.REDIS_METRICS['PASSWORD'])
+        * ``ssl`` -- Use SSL when connecting (set in settings.REDIS_METRICS['SSL'])
         * ``socket_timeout``   -- Redis password (set in
           settings.REDIS_METRICS['SOCKET_TIMEOUT'])
         * ``connection_pool`` -- Redis connection pool info. (set in
           settings.REDIS_METRICS['SOCKET_CONNECTION_POOL'])
 
         """
         self._categories_key = kwargs.get('categories_key', 'categories')
@@ -64,14 +65,15 @@
             package, module = self.connection_class.rsplit('.', 1)
             self.r = getattr(import_module(package), module)()
         else:
             self.host = kwargs.pop('host', app_settings.HOST)
             self.port = kwargs.pop('port', app_settings.PORT)
             self.db = kwargs.pop('db', app_settings.DB)
             self.password = kwargs.pop('password', app_settings.PASSWORD)
+            self.ssl = kwargs.pop('ssl', app_settings.SSL)
             self.socket_timeout = kwargs.pop(
                 'socket_timeout',
                 app_settings.SOCKET_TIMEOUT
             )
             self.connection_pool = kwargs.pop(
                 'connection_pool',
                 app_settings.SOCKET_CONNECTION_POOL
@@ -79,14 +81,15 @@
 
             # Create the connection to Redis
             self.r = redis.StrictRedis(
                 host=self.host,
                 port=self.port,
                 db=self.db,
                 password=self.password,
+                ssl=self.ssl,
                 socket_timeout=self.socket_timeout,
                 connection_pool=self.connection_pool,
                 decode_responses=True
             )
 
     def _date_range(self, granularity, since, to=None):
         """Returns a generator that yields ``datetime.datetime`` objects from
```

### Comparing `django-redis_metrics-2.1.0/redis_metrics/settings.py` & `django-redis_metrics-2.2.0/redis_metrics/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,40 +20,41 @@
 
     On access, we'll first try to look up values in Django's settings, and
     if the setting is not found there, we'll provide a default value.
     """
 
     # list of (setting name, default value)
     _default_settings = {
-        'CONNECTION_CLASS': None,
-        'HOST': 'localhost',
-        'PORT': 6379,
-        'DB': 0,
-        'PASSWORD': None,
-        'SOCKET_TIMEOUT': None,
-        'SOCKET_CONNECTION_POOL': None,
-        'MIN_GRANULARITY': 'daily',
-        'MAX_GRANULARITY': 'yearly',
-        'MONDAY_FIRST_DAY_OF_WEEK': False,
-        'USE_ISO_WEEK_NUMBER': False,
+        "CONNECTION_CLASS": None,
+        "HOST": "localhost",
+        "PORT": 6379,
+        "DB": 0,
+        "PASSWORD": None,
+        "SSL": False,
+        "SOCKET_TIMEOUT": None,
+        "SOCKET_CONNECTION_POOL": None,
+        "MIN_GRANULARITY": "daily",
+        "MAX_GRANULARITY": "yearly",
+        "MONDAY_FIRST_DAY_OF_WEEK": False,
+        "USE_ISO_WEEK_NUMBER": False,
     }
 
     # A mapping of our old settings names to the new name
     _old_settings = {
-        'CONNECTION_CLASS': 'REDIS_METRICS_CONNECTION_CLASS',
-        'HOST': 'REDIS_METRICS_HOST',
-        'PORT': 'REDIS_METRICS_PORT',
-        'DB': 'REDIS_METRICS_DB',
-        'PASSWORD': 'REDIS_METRICS_PASSWORD',
-        'SOCKET_TIMEOUT': 'REDIS_METRICS_SOCKET_TIMEOUT',
-        'SOCKET_CONNECTION_POOL': 'REDIS_METRICS_SOCKET_CONNECTION_POOL',
-        'MIN_GRANULARITY': 'REDIS_METRICS_MIN_GRANULARITY',
-        'MAX_GRANULARITY': 'REDIS_METRICS_MAX_GRANULARITY',
-        'MONDAY_FIRST_DAY_OF_WEEK': 'REDIS_METRICS_MONDAY_FIRST_DAY_OF_WEEK',
-        'USE_ISO_WEEK_NUMBER': 'USE_ISO_WEEK_NUMBER',
+        "CONNECTION_CLASS": "REDIS_METRICS_CONNECTION_CLASS",
+        "HOST": "REDIS_METRICS_HOST",
+        "PORT": "REDIS_METRICS_PORT",
+        "DB": "REDIS_METRICS_DB",
+        "PASSWORD": "REDIS_METRICS_PASSWORD",
+        "SOCKET_TIMEOUT": "REDIS_METRICS_SOCKET_TIMEOUT",
+        "SOCKET_CONNECTION_POOL": "REDIS_METRICS_SOCKET_CONNECTION_POOL",
+        "MIN_GRANULARITY": "REDIS_METRICS_MIN_GRANULARITY",
+        "MAX_GRANULARITY": "REDIS_METRICS_MAX_GRANULARITY",
+        "MONDAY_FIRST_DAY_OF_WEEK": "REDIS_METRICS_MONDAY_FIRST_DAY_OF_WEEK",
+        "USE_ISO_WEEK_NUMBER": "USE_ISO_WEEK_NUMBER",
     }
 
     def __getattr__(self, name):
         """Access settings as an attribute."""
         try:
             return self[name]
         except KeyError as e:
@@ -82,8 +83,8 @@
         return getattr(settings, key, self._default_settings[key])
 
 
 app_settings = AppSettings()
 
 
 # All possible granularity values.
-GRANULARITIES = ['seconds', 'minutes', 'hourly', 'daily', 'weekly', 'monthly', 'yearly']
+GRANULARITIES = ["seconds", "minutes", "hourly", "daily", "weekly", "monthly", "yearly"]
```

### Comparing `django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/css/bs-theme.min.css` & `django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/css/bs-theme.min.css`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/css/bs.min.css` & `django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/css/bs.min.css`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/chart.min.js` & `django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/colors.js` & `django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/colors.js`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/static/redis_metrics/js/zepto.min.js` & `django-redis_metrics-2.2.0/redis_metrics/static/redis_metrics/js/zepto.min.js`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_aggregate_detail.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_aggregate_detail.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_aggregate_history.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_aggregate_history.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_gauge.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_gauge.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_detail.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_detail.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_history.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_history.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_metric_list.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_metric_list.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/_since.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/_since.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/aggregate_detail.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/aggregate_detail.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/aggregate_history.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/aggregate_history.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/base.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/base.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/default.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/default.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/email/report.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/email/report.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/metric_history.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/metric_history.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templates/redis_metrics/metrics_list.html` & `django-redis_metrics-2.2.0/redis_metrics/templates/redis_metrics/metrics_list.html`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templatetags/redis_metric_tags.py` & `django-redis_metrics-2.2.0/redis_metrics/templatetags/redis_metric_tags.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/templatetags/redis_metrics_filters.py` & `django-redis_metrics-2.2.0/redis_metrics/templatetags/redis_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/settings.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_forms.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_models.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,635 +2,643 @@
 This file demonstrates writing tests using the unittest module. These will pass
 when you run "manage.py test".
 
 Replace this with more appropriate tests for your application.
 """
 from __future__ import unicode_literals
 from datetime import datetime, timedelta
+
 try:
     from unittest.mock import call, patch, Mock
 except ImportError:
     from mock import call, patch, Mock
 
 from django.test import TestCase
 from django.test.utils import override_settings
 
 from ..models import R, dedupe
 
 
 TEST_SETTINGS = {
-    'HOST': 'localhost',
-    'PORT': 6379,
-    'DB': 0,
-    'PASSWORD': None,
-    'SOCKET_TIMEOUT': None,
-    'SOCKET_CONNECTION_POOL': None,
-    'MIN_GRANULARITY': 'seconds',
-    'MAX_GRANULARITY': 'yearly',
-    'MONDAY_FIRST_DAY_OF_WEEK': False,
-    'USE_ISO_WEEK_NUMBER': False,
+    "HOST": "localhost",
+    "PORT": 6379,
+    "DB": 0,
+    "PASSWORD": None,
+    "SSL": None,
+    "SOCKET_TIMEOUT": None,
+    "SOCKET_CONNECTION_POOL": None,
+    "MIN_GRANULARITY": "seconds",
+    "MAX_GRANULARITY": "yearly",
+    "MONDAY_FIRST_DAY_OF_WEEK": False,
+    "USE_ISO_WEEK_NUMBER": False,
 }
 
 
 @override_settings(REDIS_METRICS=TEST_SETTINGS)
 class TestR(TestCase):
     """Tests for the ``R`` class."""
 
     def setUp(self):
         # Patch the connection to redis, but keep a reference to the
         # created StrictRedis instance, so we can make assertions about how
         # it's called.
-        self.redis_patcher = patch('redis_metrics.models.redis.StrictRedis')
+        self.redis_patcher = patch("redis_metrics.models.redis.StrictRedis")
         mock_StrictRedis = self.redis_patcher.start()
         self.redis = mock_StrictRedis.return_value
         self.r = R()
 
     def tearDown(self):
         self.redis = self.redis_patcher.stop()
         super(TestR, self).tearDown()
 
     def test_dedupe(self):
         """Test the redis_metrics.models.dedupe function."""
         self.assertEqual(
-            list(dedupe(['a', 'a', 'b', 'c', 'b', 'c', 'c', 'c'])),
-            ['a', 'b', 'c']
+            list(dedupe(["a", "a", "b", "c", "b", "c", "c", "c"])), ["a", "b", "c"]
         )
 
     def test__init__(self):
         """Test creation of an R object with parameters."""
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             kwargs = {
-                'decode_responses': True,
-                'categories_key': 'CAT',
-                'metric_slugs_key': 'MSK',
-                'gauge_slugs_key': 'GSK',
-                'host': 'HOST',
-                'port': 'PORT',
-                'db': 'DB',
-                'password': 'PASSWORD',
-                'socket_timeout': 1,
-                'connection_pool': 1
+                "decode_responses": True,
+                "categories_key": "CAT",
+                "metric_slugs_key": "MSK",
+                "gauge_slugs_key": "GSK",
+                "host": "HOST",
+                "port": "PORT",
+                "db": "DB",
+                "password": "PASSWORD",
+                "ssl": "SSL",
+                "socket_timeout": 1,
+                "connection_pool": 1,
             }
             inst = R(**kwargs)
             self.assertEqual(inst.host, "HOST")
             self.assertEqual(inst.port, "PORT")
             self.assertEqual(inst.db, "DB")
-            self.assertEqual(inst.password, 'PASSWORD')
+            self.assertEqual(inst.password, "PASSWORD")
+            self.assertEqual(inst.ssl, "SSL")
             self.assertEqual(inst.socket_timeout, 1)
             self.assertEqual(inst.connection_pool, 1)
             self.assertEqual(inst._categories_key, "CAT")
             self.assertEqual(inst._metric_slugs_key, "MSK")
             self.assertEqual(inst._gauge_slugs_key, "GSK")
             mock_redis.assert_called_once_with(
                 decode_responses=True,
-                host='HOST',
-                port='PORT',
-                db='DB',
+                host="HOST",
+                port="PORT",
+                db="DB",
                 password="PASSWORD",
+                ssl="SSL",
                 socket_timeout=1,
-                connection_pool=1
+                connection_pool=1,
             )
 
     def test__init__with_default_kwargs(self):
         """Test creation of an R object without parameters."""
         r_kwargs = {
-            'decode_responses': True,
-            'host': 'localhost',
-            'db': 0,
-            'port': 6379,
-            'password': None,
-            'connection_pool': None,
-            'socket_timeout': None
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "password": None,
+            "ssl": None,
+            "socket_timeout": None,
+            "connection_pool": None,
+            "decode_responses": True,
         }
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             inst = R()
-            self.assertEqual(inst.host, 'localhost')
+            self.assertEqual(inst.host, "localhost")
             self.assertEqual(inst.port, 6379)
             self.assertEqual(inst.db, 0)
             self.assertEqual(inst.password, None)
             self.assertEqual(inst.socket_timeout, None)
             self.assertEqual(inst.connection_pool, None)
-            self.assertEqual(inst._categories_key, 'categories')
+            self.assertEqual(inst._categories_key, "categories")
             self.assertEqual(inst._metric_slugs_key, "metric-slugs")
             self.assertEqual(inst._gauge_slugs_key, "gauge-slugs")
             mock_redis.assert_called_once_with(**r_kwargs)
 
     def test__date_range(self):
         """Tests ``R._date_range`` at various granularities *without* a
         ``since`` date."""
         # minutes, seconds and hours should be capped at 300, 480, and 720
         d = datetime(2014, 1, 1)
-        self.assertEqual(len(list(self.r._date_range('seconds', d))), 300)
-        self.assertEqual(len(list(self.r._date_range('minutes', d))), 480)
-        self.assertEqual(len(list(self.r._date_range('hourly', d))), 720)
+        self.assertEqual(len(list(self.r._date_range("seconds", d))), 300)
+        self.assertEqual(len(list(self.r._date_range("minutes", d))), 480)
+        self.assertEqual(len(list(self.r._date_range("hourly", d))), 720)
 
         # Everything else should have a timedelta of 7 days
-        self.assertEqual(len(list(self.r._date_range('daily', None))), 8)
-        self.assertEqual(len(list(self.r._date_range('weekly', None))), 8)
-        self.assertEqual(len(list(self.r._date_range('monthly', None))), 8)
-        self.assertEqual(len(list(self.r._date_range('yearly', None))), 8)
+        self.assertEqual(len(list(self.r._date_range("daily", None))), 8)
+        self.assertEqual(len(list(self.r._date_range("weekly", None))), 8)
+        self.assertEqual(len(list(self.r._date_range("monthly", None))), 8)
+        self.assertEqual(len(list(self.r._date_range("yearly", None))), 8)
 
         # Test with a specified `to` argument.
         since = datetime(2014, 1, 1)
         to = datetime(2015, 1, 1)
-        self.assertEqual(len(list(self.r._date_range('daily', since, to))), 366)
-        self.assertEqual(len(list(self.r._date_range('weekly', since, to))), 366)
-        self.assertEqual(len(list(self.r._date_range('monthly', since, to))), 366)
-        self.assertEqual(len(list(self.r._date_range('yearly', since, to))), 366)
+        self.assertEqual(len(list(self.r._date_range("daily", since, to))), 366)
+        self.assertEqual(len(list(self.r._date_range("weekly", since, to))), 366)
+        self.assertEqual(len(list(self.r._date_range("monthly", since, to))), 366)
+        self.assertEqual(len(list(self.r._date_range("yearly", since, to))), 366)
 
     def test__date_range_seconds(self):
         """Tests ``R._date_range`` at the "seconds" granularity."""
         since = datetime.utcnow() - timedelta(seconds=5)
-        values = self.r._date_range('seconds', since)
+        values = self.r._date_range("seconds", since)
         self.assertEqual(len(list(values)), 5)
 
     def test__date_range_minutes(self):
         """Tests ``R._date_range`` at the "minutes" granularity."""
         since = datetime.utcnow() - timedelta(minutes=5)
-        values = self.r._date_range('minutes', since)
+        values = self.r._date_range("minutes", since)
         self.assertEqual(len(list(values)), 5)
 
     def test__date_range_hourly(self):
         """Tests ``R._date_range`` at the "hourly" granularity."""
         since = datetime.utcnow() - timedelta(hours=5)
-        values = self.r._date_range('hourly', since)
+        values = self.r._date_range("hourly", since)
         self.assertEqual(len(list(values)), 5)
 
     def test__date_range_daily(self):
         """Tests ``R._date_range`` at the "daily" granularity."""
         since = datetime.utcnow() - timedelta(days=5)
-        values = self.r._date_range('daily', since)
+        values = self.r._date_range("daily", since)
         self.assertEqual(len(list(values)), 6)  # 6 because we do days + 1
 
     def test__date_range_weekly(self):
         """Tests ``R._date_range`` at the "weekly" granularity."""
         since = datetime.utcnow() - timedelta(days=5)
-        values = self.r._date_range('weekly', since)
+        values = self.r._date_range("weekly", since)
         self.assertEqual(len(list(values)), 6)  # 6 because we do days + 1
 
     def test__date_range_monthly(self):
         """Tests ``R._date_range`` at the "monthly" granularity."""
         since = datetime.utcnow() - timedelta(days=5)
-        values = self.r._date_range('montly', since)
+        values = self.r._date_range("montly", since)
         self.assertEqual(len(list(values)), 6)  # 6 because we do days + 1
 
     def test__date_range_yearly(self):
         """Tests ``R._date_range`` at the "yearly" granularity."""
         since = datetime.utcnow() - timedelta(days=5)
-        values = self.r._date_range('yearly', since)
+        values = self.r._date_range("yearly", since)
         self.assertEqual(len(list(values)), 6)  # 6 because we do days + 1
 
     def test_categories(self):
         """Verify that ``R.categories()`` calls redis SMEMBERS command."""
         self.r.categories()
         self.redis.smembers.assert_called_once_with("categories")
 
     def test__category_key(self):
         """Creates a redis key for a given category string."""
-        self.assertEqual(
-            self.r._category_key("Sample Category"),
-            u"c:Sample Category"
-        )
+        self.assertEqual(self.r._category_key("Sample Category"), "c:Sample Category")
 
     def test__category_slugs(self):
         """Verify that this returns an empty list or a list of slugs."""
         # When there are no results from redis
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             mock_redis.return_value.smembers.return_value = set([])
             r = R()
             result = r._category_slugs("Sample Category")
             self.assertEqual(len(result), 0)
 
         # When there are no results from redis
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             mock_redis.return_value.smembers.return_value = set(["slug-a", "slug-b"])
             r = R()
             result = r._category_slugs("Sample Category")
-            self.assertEqual(set(result), set(['slug-a', 'slug-b']))
+            self.assertEqual(set(result), set(["slug-a", "slug-b"]))
 
-    @patch.object(R, '_category_slugs')
+    @patch.object(R, "_category_slugs")
     def test__categorize(self, mock_category_slugs):
         """Categorizing a slug should add the correct key/values to Redis,
         and it should store the Category in a redis set."""
 
         # Sample category and metric slug
         cat = "Sample Category"
         cat_key = "c:Sample Category"
         slug = "sample-slug"
 
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             redis_instance = mock_redis.return_value
             r = R()
 
             r._categorize(slug, cat)
             calls = [call.sadd(cat_key, slug), call.sadd("categories", cat)]
             redis_instance.assert_has_calls(calls, any_order=True)
 
     def test__granularities(self):
         """Tests ``R._granularities with default test settings."""
         # With default settings, min/max granularity is "seconds" and "yearly"
         self.assertEqual(
             list(self.r._granularities()),
-            ['seconds', 'minutes', 'hourly', 'daily', 'weekly', 'monthly', 'yearly']
+            ["seconds", "minutes", "hourly", "daily", "weekly", "monthly", "yearly"],
         )
 
     def test__granularities_with_altered_min(self):
         """Tests ``R._granularities with an altered minimum value."""
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MIN_GRANULARITY'] = 'daily'
+        test_settings["MIN_GRANULARITY"] = "daily"
         with override_settings(REDIS_METRICS=test_settings):
             self.assertEqual(
-                list(self.r._granularities()),
-                ['daily', 'weekly', 'monthly', 'yearly']
+                list(self.r._granularities()), ["daily", "weekly", "monthly", "yearly"]
             )
 
     def test__granularities_with_altered_max(self):
         """Tests ``R._granularities with an altered maximum value."""
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MAX_GRANULARITY'] = 'daily'
+        test_settings["MAX_GRANULARITY"] = "daily"
         with override_settings(REDIS_METRICS=test_settings):
             self.assertEqual(
-                list(self.r._granularities()),
-                ['seconds', 'minutes', 'hourly', 'daily']
+                list(self.r._granularities()), ["seconds", "minutes", "hourly", "daily"]
             )
 
     def test_get_metric_key_pattern_seconds(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('seconds', slug, date),
-            "m:test-slug:s:2019-01-02-03-04-05"
+            self.r._get_metric_key_pattern("seconds", slug, date),
+            "m:test-slug:s:2019-01-02-03-04-05",
         )
 
     def test_get_metric_key_pattern_minutes(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('minutes', slug, date),
-            "m:test-slug:i:2019-01-02-03-04"
+            self.r._get_metric_key_pattern("minutes", slug, date),
+            "m:test-slug:i:2019-01-02-03-04",
         )
 
     def test_get_metric_key_pattern_hourly(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('hourly', slug, date),
-            "m:test-slug:h:2019-01-02-03"
+            self.r._get_metric_key_pattern("hourly", slug, date),
+            "m:test-slug:h:2019-01-02-03",
         )
 
     def test_get_metric_key_pattern_daily(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('daily', slug, date),
-            "m:test-slug:2019-01-02"
+            self.r._get_metric_key_pattern("daily", slug, date),
+            "m:test-slug:2019-01-02",
         )
 
     def test_get_metric_key_pattern_weekly_sunday_as_first(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MONDAY_FIRST_DAY_OF_WEEK'] = False
+        test_settings["MONDAY_FIRST_DAY_OF_WEEK"] = False
         with override_settings(REDIS_METRICS=test_settings):
             slug = "test-slug"
             date = datetime(2012, 4, 1, 3, 4, 5)
             self.assertEqual(
-                self.r._get_metric_key_pattern('weekly', slug, date),
-                "m:test-slug:w:2012-14"
+                self.r._get_metric_key_pattern("weekly", slug, date),
+                "m:test-slug:w:2012-14",
             )
 
     def test_get_metric_key_pattern_weekly_monday_at_first(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MONDAY_FIRST_DAY_OF_WEEK'] = True
+        test_settings["MONDAY_FIRST_DAY_OF_WEEK"] = True
         with override_settings(REDIS_METRICS=test_settings):
             slug = "test-slug"
             date = datetime(2012, 4, 1, 3, 4, 5)
             self.assertEqual(
-                self.r._get_metric_key_pattern('weekly', slug, date),
-                "m:test-slug:w:2012-13"
+                self.r._get_metric_key_pattern("weekly", slug, date),
+                "m:test-slug:w:2012-13",
             )
 
     def test_get_metric_key_pattern_weekly_iso_week(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['USE_ISO_WEEK_NUMBER'] = True
+        test_settings["USE_ISO_WEEK_NUMBER"] = True
         with override_settings(REDIS_METRICS=test_settings):
             slug = "test-slug"
             date = datetime(2019, 1, 2, 3, 4, 5)
             self.assertEqual(
-                self.r._get_metric_key_pattern('weekly', slug, date),
-                "m:test-slug:w:2019-1"
+                self.r._get_metric_key_pattern("weekly", slug, date),
+                "m:test-slug:w:2019-1",
             )
 
     def test_get_metric_key_pattern_monthly(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('monthly', slug, date),
-            "m:test-slug:m:2019-01"
+            self.r._get_metric_key_pattern("monthly", slug, date),
+            "m:test-slug:m:2019-01",
         )
 
     def test_get_metric_key_pattern_yearly(self):
         slug = "test-slug"
         date = datetime(2019, 1, 2, 3, 4, 5)
         self.assertEqual(
-            self.r._get_metric_key_pattern('yearly', slug, date),
-            "m:test-slug:y:2019"
+            self.r._get_metric_key_pattern("yearly", slug, date), "m:test-slug:y:2019"
         )
 
     def test__build_keys(self):
         """Tests ``R._build_keys``. with default arguments."""
-        with patch('redis_metrics.models.datetime') as mock_datetime:
+        with patch("redis_metrics.models.datetime") as mock_datetime:
             mock_datetime.utcnow.return_value = datetime(2014, 7, 2, 12, 6, 34)
             expected_results = [
                 "m:test-slug:s:2014-07-02-12-06-34",
                 "m:test-slug:i:2014-07-02-12-06",
                 "m:test-slug:h:2014-07-02-12",
                 "m:test-slug:2014-07-02",
                 "m:test-slug:w:2014-26",
                 "m:test-slug:m:2014-07",
                 "m:test-slug:y:2014",
             ]
-            keys = self.r._build_keys('test-slug')
+            keys = self.r._build_keys("test-slug")
             self.assertEqual(keys, expected_results)
 
     def test__build_keys_seconds(self):
         """Tests ``R._build_keys``. with a *seconds* granularity."""
         d = datetime(2012, 4, 1, 11, 30, 59)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='seconds')
-        self.assertEqual(keys, ['m:test-slug:s:2012-04-01-11-30-59'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="seconds")
+        self.assertEqual(keys, ["m:test-slug:s:2012-04-01-11-30-59"])
 
     def test__build_keys_minutes(self):
         """Tests ``R._build_keys``. with a *minutes* granularity."""
         d = datetime(2012, 4, 1, 11, 30)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='minutes')
-        self.assertEqual(keys, ['m:test-slug:i:2012-04-01-11-30'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="minutes")
+        self.assertEqual(keys, ["m:test-slug:i:2012-04-01-11-30"])
 
     def test__build_keys_hourly(self):
         """Tests ``R._build_keys``. with a *hourly* granularity."""
         d = datetime(2012, 4, 1, 11, 30)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='hourly')
-        self.assertEqual(keys, ['m:test-slug:h:2012-04-01-11'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="hourly")
+        self.assertEqual(keys, ["m:test-slug:h:2012-04-01-11"])
 
     def test__build_keys_daily(self):
         """Tests ``R._build_keys``. with a *daily* granularity."""
         d = datetime(2012, 4, 1)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='daily')
-        self.assertEqual(keys, ['m:test-slug:2012-04-01'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="daily")
+        self.assertEqual(keys, ["m:test-slug:2012-04-01"])
 
     def test__build_keys_weekly(self):
         """Tests ``R._build_keys``. with a *weekly* granularity."""
         d = datetime(2012, 4, 1)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='weekly')
-        self.assertEqual(keys, ['m:test-slug:w:2012-14'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="weekly")
+        self.assertEqual(keys, ["m:test-slug:w:2012-14"])
 
     def test__build_keys_weekly_week_starts_monday(self):
         """Tests ``R._build_keys``. with a *weekly* granularity."""
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MONDAY_FIRST_DAY_OF_WEEK'] = True
+        test_settings["MONDAY_FIRST_DAY_OF_WEEK"] = True
         with override_settings(REDIS_METRICS=test_settings):
             d = datetime(2012, 4, 1)  # April Fools!
-            keys = self.r._build_keys('test-slug', date=d, granularity='weekly')
-            self.assertEqual(keys, ['m:test-slug:w:2012-13'])
+            keys = self.r._build_keys("test-slug", date=d, granularity="weekly")
+            self.assertEqual(keys, ["m:test-slug:w:2012-13"])
 
     def test__build_keys_weekly_iso_week(self):
         """Tests ``R._build_keys``. with a *weekly* granularity."""
         test_settings = TEST_SETTINGS.copy()
-        test_settings['USE_ISO_WEEK_NUMBER'] = True
+        test_settings["USE_ISO_WEEK_NUMBER"] = True
         with override_settings(REDIS_METRICS=test_settings):
             d1 = datetime(2018, 12, 30)
-            keys = self.r._build_keys('test-slug', date=d1, granularity='weekly')
-            self.assertEqual(keys, ['m:test-slug:w:2018-52'])
+            keys = self.r._build_keys("test-slug", date=d1, granularity="weekly")
+            self.assertEqual(keys, ["m:test-slug:w:2018-52"])
             d2 = datetime(2018, 12, 31)
-            keys = self.r._build_keys('test-slug', date=d2, granularity='weekly')
-            self.assertEqual(keys, ['m:test-slug:w:2019-1'])
+            keys = self.r._build_keys("test-slug", date=d2, granularity="weekly")
+            self.assertEqual(keys, ["m:test-slug:w:2019-1"])
             d3 = datetime(2019, 1, 1)
-            keys = self.r._build_keys('test-slug', date=d3, granularity='weekly')
-            self.assertEqual(keys, ['m:test-slug:w:2019-1'])
+            keys = self.r._build_keys("test-slug", date=d3, granularity="weekly")
+            self.assertEqual(keys, ["m:test-slug:w:2019-1"])
 
     def test__build_keys_monthly(self):
         """Tests ``R._build_keys``. with a *monthly* granularity."""
         d = datetime(2012, 4, 1)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='monthly')
-        self.assertEqual(keys, ['m:test-slug:m:2012-04'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="monthly")
+        self.assertEqual(keys, ["m:test-slug:m:2012-04"])
 
     def test__build_keys_yearly(self):
         """Tests ``R._build_keys``. with a *yearly* granularity."""
         d = datetime(2012, 4, 1)  # April Fools!
-        keys = self.r._build_keys('test-slug', date=d, granularity='yearly')
-        self.assertEqual(keys, ['m:test-slug:y:2012'])
+        keys = self.r._build_keys("test-slug", date=d, granularity="yearly")
+        self.assertEqual(keys, ["m:test-slug:y:2012"])
 
     def test_metric_slugs(self):
         """Test that ``R.metric_slugs`` makes a call to Redis SMEMBERS."""
         self.r.metric_slugs()
         self.redis.assert_has_calls([call.smembers(self.r._metric_slugs_key)])
 
-    @patch.object(R, '_category_slugs')
+    @patch.object(R, "_category_slugs")
     def test_metric_slugs_by_category(self, mock_category_slugs):
         """Test that we get metric slugs organized by category."""
         # set up a mock return value for the category's redis set
-        self.redis.smembers.return_value = ['Sample Category']
+        self.redis.smembers.return_value = ["Sample Category"]
         # set up return value for mock call to _category_slugs
-        mock_category_slugs.return_value = ['foo', 'bar']
+        mock_category_slugs.return_value = ["foo", "bar"]
 
         # Since this method all calls out to ``R.metric_slugs``, let's patch
         # that so it returns a list of all slugs, one of which will not be
         # categorized
-        self.r.metric_slugs = Mock(return_value=['foo', 'bar', 'baz'])
+        self.r.metric_slugs = Mock(return_value=["foo", "bar", "baz"])
 
         # Now, test the thing.
         result = self.r.metric_slugs_by_category()
-        expected_result = {
-            'Sample Category': ['foo', 'bar'],
-            'Uncategorized': ['baz']
-        }
+        expected_result = {"Sample Category": ["foo", "bar"], "Uncategorized": ["baz"]}
         self.assertEqual(result, expected_result)
         self.redis.smembers.assert_called_once_with("categories")
         mock_category_slugs.assert_called_once_with("Sample Category")
         self.r.metric_slugs.assert_called_once_with()
 
     def test_delete_metric(self):
         """Verify that ``R.delete_metric`` deletes all keys and removes keys
         from the set of metric slugs."""
 
         # Make sure KEYS returns some data
         self.redis.keys.return_value = ["m:slug:0", "m:slug:1"]
-        self.r.delete_metric('slug')  # call delete_metric
+        self.r.delete_metric("slug")  # call delete_metric
 
         # Verify that the metric data is removed as are the keys from the set
-        self.redis.assert_has_calls([
-            call.keys("m:slug:*"),
-            call.delete("m:slug:0", "m:slug:1"),
-            call.srem(self.r._metric_slugs_key, "slug")
-        ])
+        self.redis.assert_has_calls(
+            [
+                call.keys("m:slug:*"),
+                call.delete("m:slug:0", "m:slug:1"),
+                call.srem(self.r._metric_slugs_key, "slug"),
+            ]
+        )
 
-    @patch.object(R, '_build_keys')
+    @patch.object(R, "_build_keys")
     def test_set_metric(self, mock_build_keys):
         """Test setting metrics using ``R.set_metric``."""
         # Define redis keys
         mock_build_keys.return_value = [
-            'm:test-slug:s:2000-01-02-11-45-30',
-            'm:test-slug:i:2000-01-02-11-45',
-            'm:test-slug:h:2000-01-02-11',
-            'm:test-slug:2000-01-02',
-            'm:test-slug:m:2000-01',
-            'm:test-slug:w:2000-01',
-            'm:test-slug:y:2000'
+            "m:test-slug:s:2000-01-02-11-45-30",
+            "m:test-slug:i:2000-01-02-11-45",
+            "m:test-slug:h:2000-01-02-11",
+            "m:test-slug:2000-01-02",
+            "m:test-slug:m:2000-01",
+            "m:test-slug:w:2000-01",
+            "m:test-slug:y:2000",
         ]
-        slug = 'test-slug'
+        slug = "test-slug"
         value = 42
 
         # get the metric keys so we can check for the appropriate calls
         self.r.set_metric(slug, value)
 
         # Verify that setting a metric adds the appropriate slugs to the keys
         # set and then incrememts each key
-        self.redis.sadd.assert_called_once_with('metric-slugs', slug)
-        self.redis.mset.assert_called_once_with({
-            'm:test-slug:s:2000-01-02-11-45-30': 42,
-            'm:test-slug:i:2000-01-02-11-45': 42,
-            'm:test-slug:h:2000-01-02-11': 42,
-            'm:test-slug:2000-01-02': 42,
-            'm:test-slug:m:2000-01': 42,
-            'm:test-slug:w:2000-01': 42,
-            'm:test-slug:y:2000': 42,
-        })
+        self.redis.sadd.assert_called_once_with("metric-slugs", slug)
+        self.redis.mset.assert_called_once_with(
+            {
+                "m:test-slug:s:2000-01-02-11-45-30": 42,
+                "m:test-slug:i:2000-01-02-11-45": 42,
+                "m:test-slug:h:2000-01-02-11": 42,
+                "m:test-slug:2000-01-02": 42,
+                "m:test-slug:m:2000-01": 42,
+                "m:test-slug:w:2000-01": 42,
+                "m:test-slug:y:2000": 42,
+            }
+        )
 
         # Expiration should not have gotten called
         self.assertFalse(self.redis.expire.called)
 
-    @patch.object(R, '_build_keys')
+    @patch.object(R, "_build_keys")
     def test_set_metric_with_expiration(self, mock_build_keys):
         """Test setting metrics using ``R.set_metric`` with an expiration."""
         # Define redis keys
         mock_build_keys.return_value = [
-            'm:test-slug:s:2000-01-02-11-45-30',
-            'm:test-slug:i:2000-01-02-11-45',
-            'm:test-slug:h:2000-01-02-11',
-            'm:test-slug:2000-01-02',
-            'm:test-slug:m:2000-01',
-            'm:test-slug:w:2000-01',
-            'm:test-slug:y:2000'
+            "m:test-slug:s:2000-01-02-11-45-30",
+            "m:test-slug:i:2000-01-02-11-45",
+            "m:test-slug:h:2000-01-02-11",
+            "m:test-slug:2000-01-02",
+            "m:test-slug:m:2000-01",
+            "m:test-slug:w:2000-01",
+            "m:test-slug:y:2000",
         ]
-        slug = 'test-slug'
+        slug = "test-slug"
         value = 42
 
         # get the metric keys so we can check for the appropriate calls
         self.r.set_metric(slug, value, expire=500)
 
         # Verify that each key had an expiration set.
-        self.redis.expire.assert_has_calls([
-            call('m:test-slug:s:2000-01-02-11-45-30', 500),
-            call('m:test-slug:i:2000-01-02-11-45', 500),
-            call('m:test-slug:h:2000-01-02-11', 500),
-            call('m:test-slug:2000-01-02', 500),
-            call('m:test-slug:m:2000-01', 500),
-            call('m:test-slug:w:2000-01', 500),
-            call('m:test-slug:y:2000', 500),
-        ])
+        self.redis.expire.assert_has_calls(
+            [
+                call("m:test-slug:s:2000-01-02-11-45-30", 500),
+                call("m:test-slug:i:2000-01-02-11-45", 500),
+                call("m:test-slug:h:2000-01-02-11", 500),
+                call("m:test-slug:2000-01-02", 500),
+                call("m:test-slug:m:2000-01", 500),
+                call("m:test-slug:w:2000-01", 500),
+                call("m:test-slug:y:2000", 500),
+            ]
+        )
 
-    @patch.object(R, '_categorize')
+    @patch.object(R, "_categorize")
     def test_set_metric_with_category(self, mock_categorize):
         """Test setting metrics using ``R.set_metric`` when a category
         is provided."""
 
         # get the metric keys so we can check for the appropriate calls
-        self.r.set_metric('test-slug', 42, category='Test Category')
-        mock_categorize.assert_called_once_with('test-slug', "Test Category")
+        self.r.set_metric("test-slug", 42, category="Test Category")
+        mock_categorize.assert_called_once_with("test-slug", "Test Category")
 
     def test_metric(self):
         """Test setting metrics using ``R.metric``."""
 
-        slug = 'test-metric'
+        slug = "test-metric"
         n = 1
 
         # get the keys used for the metric, so we can check for the appropriate
         # calls
         keys = self.r._build_keys(slug)
         second, minute, hour, day, week, month, year = keys
         self.r.metric(slug, num=n)
 
         # Verify that setting a metric adds the appropriate slugs to the keys
         # set and then incrememts each key
-        self.redis.assert_has_calls([
-            call.sadd(self.r._metric_slugs_key, slug),
-            call.pipeline(),
-            call.pipeline().incr(second, n),
-            call.pipeline().incr(minute, n),
-            call.pipeline().incr(hour, n),
-            call.pipeline().incr(day, n),
-            call.pipeline().incr(week, n),
-            call.pipeline().incr(month, n),
-            call.pipeline().incr(year, n),
-        ])
+        self.redis.assert_has_calls(
+            [
+                call.sadd(self.r._metric_slugs_key, slug),
+                call.pipeline(),
+                call.pipeline().incr(second, n),
+                call.pipeline().incr(minute, n),
+                call.pipeline().incr(hour, n),
+                call.pipeline().incr(day, n),
+                call.pipeline().incr(week, n),
+                call.pipeline().incr(month, n),
+                call.pipeline().incr(year, n),
+            ]
+        )
 
         # Expiration should not have gotten called
         self.assertFalse(self.redis.expire.called)
 
     def test_metric_with_overridden_granularities(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MIN_GRANULARITY'] = 'daily'
-        test_settings['MAX_GRANULARITY'] = 'weekly'
+        test_settings["MIN_GRANULARITY"] = "daily"
+        test_settings["MAX_GRANULARITY"] = "weekly"
         with override_settings(REDIS_METRICS=test_settings):
-            slug = 'test-metric'
+            slug = "test-metric"
             n = 1
 
             # get the keys used for the metric, so we can check for the appropriate
             # calls
             daily, weekly = self.r._build_keys(slug)
             self.r.metric(slug, num=n)
 
             # Verify that setting a metric adds the appropriate slugs to the keys
             # set and then incrememts each key
-            self.redis.assert_has_calls([
-                call.sadd(self.r._metric_slugs_key, slug),
-                call.pipeline(),
-                call.pipeline().incr(daily, n),
-                call.pipeline().incr(weekly, n),
-            ])
+            self.redis.assert_has_calls(
+                [
+                    call.sadd(self.r._metric_slugs_key, slug),
+                    call.pipeline(),
+                    call.pipeline().incr(daily, n),
+                    call.pipeline().incr(weekly, n),
+                ]
+            )
 
             # Expiration should not have gotten called
             self.assertFalse(self.redis.expire.called)
 
-    @patch.object(R, '_categorize')
+    @patch.object(R, "_categorize")
     def test_metric_with_category(self, mock_categorize):
         """The ``metric`` method should call ``_categorize`` if passed a
         ``category`` argument."""
         category = "Some Category"
-        slug = 'categorized-metric'
+        slug = "categorized-metric"
         n = 1
 
         # get the keys used for the metric, so we can check for calls
         keys = self.r._build_keys(slug)
         second, minute, hour, day, week, month, year = keys
         self.r.metric(slug, num=n, category=category)
 
         # Verify that setting a metric adds the appropriate slugs to the keys
         # set and then incrememts each key
-        self.redis.assert_has_calls([
-            call.sadd(self.r._metric_slugs_key, slug),
-            call.pipeline(),
-            call.pipeline().incr(second, n),
-            call.pipeline().incr(minute, n),
-            call.pipeline().incr(hour, n),
-            call.pipeline().incr(day, n),
-            call.pipeline().incr(week, n),
-            call.pipeline().incr(month, n),
-            call.pipeline().incr(year, n),
-        ])
+        self.redis.assert_has_calls(
+            [
+                call.sadd(self.r._metric_slugs_key, slug),
+                call.pipeline(),
+                call.pipeline().incr(second, n),
+                call.pipeline().incr(minute, n),
+                call.pipeline().incr(hour, n),
+                call.pipeline().incr(day, n),
+                call.pipeline().incr(week, n),
+                call.pipeline().incr(month, n),
+                call.pipeline().incr(year, n),
+            ]
+        )
 
         # Make sure this gets categorized.
         mock_categorize.assert_called_once_with(slug, category)
 
         # Expiration should not have gotten called
         self.assertFalse(self.redis.expire.called)
 
-    @patch.object(R, '_categorize')
+    @patch.object(R, "_categorize")
     def test_metric_with_expiration(self, mock_categorize):
         """The ``metric`` method should call the redis ``expire`` method if
         passed an ``expire`` argument."""
 
-        slug = 'categorized-metric'
+        slug = "categorized-metric"
         n = 1
 
         # get the keys used for the metric, so we can check for calls
         keys = self.r._build_keys(slug)
         self.r.metric(slug, num=n, expire=3600)
 
         # Verify that setting a metric adds the appropriate slugs to the keys
@@ -643,51 +651,55 @@
         self.redis.assert_has_calls(call_list)
 
         # Make sure nothing was categorized.
         self.assertFalse(mock_categorize.called)
 
     def test_get_metric(self):
         """Tests getting a single metric; ``R.get_metric``."""
-        slug = 'test-metric'
+        slug = "test-metric"
         self.r.get_metric(slug)
 
         # Verify that we GET the keys from redis
         sec, min, hour, day, week, month, year = self.r._build_keys(slug)
-        self.redis.assert_has_calls([
-            call.get(sec),
-            call.get(min),
-            call.get(hour),
-            call.get(day),
-            call.get(week),
-            call.get(month),
-            call.get(year),
-        ])
+        self.redis.assert_has_calls(
+            [
+                call.get(sec),
+                call.get(min),
+                call.get(hour),
+                call.get(day),
+                call.get(week),
+                call.get(month),
+                call.get(year),
+            ]
+        )
 
     def test_get_metric_with_overridden_granularities(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MIN_GRANULARITY'] = 'daily'
-        test_settings['MAX_GRANULARITY'] = 'weekly'
+        test_settings["MIN_GRANULARITY"] = "daily"
+        test_settings["MAX_GRANULARITY"] = "weekly"
         with override_settings(REDIS_METRICS=test_settings):
-            slug = 'test-metric'
+            slug = "test-metric"
             self.r.get_metric(slug)
 
             # Verify that we GET the keys from redis
             day, week = self.r._build_keys(slug)
-            self.redis.assert_has_calls([
-                call.get(day),
-                call.get(week),
-            ])
+            self.redis.assert_has_calls(
+                [
+                    call.get(day),
+                    call.get(week),
+                ]
+            )
 
     def test_get_metrics(self):
         # Set a return value for mget, so all of the method gets exercised.
         prev_return = self.redis.mget.return_value
-        self.redis.mget.return_value = ['1', '2']
+        self.redis.mget.return_value = ["1", "2"]
 
         # Slugs for metrics we want
-        slugs = ['metric-1', 'metric-2']
+        slugs = ["metric-1", "metric-2"]
 
         # Build the various keys for each metric
         keys_list = []
         for s in slugs:
             keys_list.append(self.r._build_keys(s))
 
         # construct the calls to redis.mget
@@ -700,23 +712,23 @@
         self.assertEqual(self.redis.mget.call_count, 2)  # ...twice
 
         # Reset mget's previous return value
         self.redis.mget.return_value = prev_return
 
     def test_get_metrics_with_overridden_granularities(self):
         test_settings = TEST_SETTINGS.copy()
-        test_settings['MIN_GRANULARITY'] = 'daily'
-        test_settings['MAX_GRANULARITY'] = 'weekly'
+        test_settings["MIN_GRANULARITY"] = "daily"
+        test_settings["MAX_GRANULARITY"] = "weekly"
         with override_settings(REDIS_METRICS=test_settings):
             # Set a return value for mget, so all of the method gets exercised.
             prev_return = self.redis.mget.return_value
-            self.redis.mget.return_value = ['1', '2']
+            self.redis.mget.return_value = ["1", "2"]
 
             # Slugs for metrics we want
-            slugs = ['metric-1', 'metric-2']
+            slugs = ["metric-1", "metric-2"]
 
             # Build the various keys for each metric
             keys_list = []
             for s in slugs:
                 keys_list.append(self.r._build_keys(s))
 
             # construct the calls to redis.mget
@@ -731,258 +743,261 @@
             # Reset mget's previous return value
             self.redis.mget.return_value = prev_return
 
     def test_get_category_metrics(self):
         """returns metrics for a given category"""
         r = R()
         # Mock methods called by `get_category_metrics`
-        r._category_slugs = Mock(return_value=['some-slug'])
+        r._category_slugs = Mock(return_value=["some-slug"])
         r.get_metrics = Mock(return_value="RESULT")
         results = r.get_category_metrics("Sample Category")
-        self.assertEqual(results, 'RESULT')
+        self.assertEqual(results, "RESULT")
         r._category_slugs.assert_called_once_with("Sample Category")
-        r.get_metrics.assert_called_once_with(['some-slug'])
+        r.get_metrics.assert_called_once_with(["some-slug"])
 
     def test_delete_category(self):
         r_kwargs = {
-            'decode_responses': True,
-            'host': 'localhost',
-            'db': 0,
-            'port': 6379,
-            'password': None,
-            'connection_pool': None,
-            'socket_timeout': None
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "password": None,
+            "ssl": None,
+            "socket_timeout": None,
+            "connection_pool": None,
+            "decode_responses": True,
         }
         with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             r = R()
             r.delete_category("Foo")
-            mock_redis.assert_has_calls([
-                call(**r_kwargs),
-                call().delete('c:Foo'),
-                call().srem("categories", "Foo")
-            ])
+            mock_redis.assert_has_calls(
+                [
+                    call(**r_kwargs),
+                    call().delete("c:Foo"),
+                    call().srem("categories", "Foo"),
+                ]
+            )
 
     @patch.object(R, "delete_category")
     def test_reset_category_with_no_metrics(self, mock_delete_category):
         """Calling ``reset_category`` with an empty list of metrics should
         just delete the category."""
         with patch("redis_metrics.models.redis.StrictRedis"):
             r = R()
             r.reset_category("Stuff", [])
             mock_delete_category.assert_called_once_with("Stuff")
 
     def test_reset_category(self):
         r_kwargs = {
-            'decode_responses': True,
-            'host': 'localhost',
-            'db': 0,
-            'port': 6379,
-            'password': None,
-            'connection_pool': None,
-            'socket_timeout': None
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "password": None,
+            "ssl": None,
+            "socket_timeout": None,
+            "connection_pool": None,
+            "decode_responses": True,
         }
         with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             r = R()
-            r.reset_category("Stuff", ['foo', 'bar'])
-            mock_redis.assert_has_calls([
-                call(**r_kwargs),
-                call().sadd('c:Stuff', 'foo', 'bar'),
-                call().sadd('categories', 'Stuff'),
-            ])
+            r.reset_category("Stuff", ["foo", "bar"])
+            mock_redis.assert_has_calls(
+                [
+                    call(**r_kwargs),
+                    call().sadd("c:Stuff", "foo", "bar"),
+                    call().sadd("categories", "Stuff"),
+                ]
+            )
 
-    def _metric_history_keys(self, slugs, since=None, to=None,
-                             granularity='daily'):
+    def _metric_history_keys(self, slugs, since=None, to=None, granularity="daily"):
         """generates the same list of keys used in ``get_metric_history``.
         These can then be used to test for calls to redis. Note: This is
-        duplicate code from ``get_metric_history`` :-/ """
+        duplicate code from ``get_metric_history`` :-/"""
         if type(slugs) != list:
             slugs = [slugs]
         keys = []
         for slug in slugs:
             for date in self.r._date_range(granularity, since, to):
                 keys += self.r._build_keys(slug, date, granularity)
         keys = list(dedupe(keys))
         return keys
 
-    def _test_get_metric_history(self, slugs, since=None, to=None,
-                                 granularity=None):
+    def _test_get_metric_history(self, slugs, since=None, to=None, granularity=None):
         """actual test code for ``R.get_metric_history``."""
         keys = self._metric_history_keys(slugs, since, to, granularity)
-        self.r.get_metric_history(
-            slugs, since=since, to=to, granularity=granularity)
+        self.r.get_metric_history(slugs, since=since, to=to, granularity=granularity)
         self.redis.assert_has_calls([call.mget(keys)])
 
     def test_get_metric_history_hourly(self):
         """Tests ``R.get_metric_history`` with hourly granularity."""
-        self._test_get_metric_history('test-slug', granularity='hourly')
+        self._test_get_metric_history("test-slug", granularity="hourly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            'test-slug',
+            "test-slug",
             since=datetime(2014, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='hourly'
+            granularity="hourly",
         )
 
     def test_get_metric_history_daily(self):
         """Tests ``R.get_metric_history`` with daily granularity."""
-        self._test_get_metric_history('test-slug', granularity='daily')
+        self._test_get_metric_history("test-slug", granularity="daily")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            'test-slug',
+            "test-slug",
             since=datetime(2014, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='daily'
+            granularity="daily",
         )
 
     def test_get_metric_history_weekly(self):
         """Tests ``R.get_metric_history`` with weekly granularity."""
-        self._test_get_metric_history('test-slug', granularity='weekly')
+        self._test_get_metric_history("test-slug", granularity="weekly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            'test-slug',
+            "test-slug",
             since=datetime(2014, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='weekly'
+            granularity="weekly",
         )
 
     def test_get_metric_history_monthly(self):
         """Tests ``R.get_metric_history`` with monthly granularity."""
-        self._test_get_metric_history('test-slug', granularity='monthly')
+        self._test_get_metric_history("test-slug", granularity="monthly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            'test-slug',
+            "test-slug",
             since=datetime(2014, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='monthly'
+            granularity="monthly",
         )
 
     def test_get_metric_history_yearly(self):
         """Tests ``R.get_metric_history`` with yearly granularity."""
-        self._test_get_metric_history('test-slug', granularity='yearly')
+        self._test_get_metric_history("test-slug", granularity="yearly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            'test-slug',
+            "test-slug",
             since=datetime(2014, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='yearly'
+            granularity="yearly",
         )
 
     def test_get_metric_multiple_history_hourly(self):
-        self._test_get_metric_history(['foo', 'bar'], granularity='hourly')
+        self._test_get_metric_history(["foo", "bar"], granularity="hourly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            ['foo', 'bar'],
+            ["foo", "bar"],
             since=datetime(2015, 1, 1),
             to=datetime(2015, 2, 1),
-            granularity='hourly'
+            granularity="hourly",
         )
 
     def test_get_metric_multiple_history_daily(self):
-        self._test_get_metric_history(['foo', 'bar'], granularity='daily')
+        self._test_get_metric_history(["foo", "bar"], granularity="daily")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            ['foo', 'bar'],
+            ["foo", "bar"],
             since=datetime(2015, 1, 1),
             to=datetime(2015, 2, 1),
-            granularity='daily'
+            granularity="daily",
         )
 
     def test_get_metric_multiple_history_weekly(self):
-        self._test_get_metric_history(['foo', 'bar'], granularity='weekly')
+        self._test_get_metric_history(["foo", "bar"], granularity="weekly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            ['foo', 'bar'],
+            ["foo", "bar"],
             since=datetime(2015, 1, 1),
             to=datetime(2015, 2, 1),
-            granularity='weekly'
+            granularity="weekly",
         )
 
     def test_get_metric_multiple_history_monthly(self):
-        self._test_get_metric_history(['foo', 'bar'], granularity='monthly')
+        self._test_get_metric_history(["foo", "bar"], granularity="monthly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            ['foo', 'bar'],
+            ["foo", "bar"],
             since=datetime(2015, 1, 1),
             to=datetime(2015, 12, 1),
-            granularity='monthly'
+            granularity="monthly",
         )
 
     def test_get_metric_multiple_history_yearly(self):
-        self._test_get_metric_history(['foo', 'bar'], granularity='yearly')
+        self._test_get_metric_history(["foo", "bar"], granularity="yearly")
 
         # with specified to/since dates
         self._test_get_metric_history(
-            ['foo', 'bar'],
+            ["foo", "bar"],
             since=datetime(2015, 1, 1),
             to=datetime(2016, 1, 1),
-            granularity='yearly'
+            granularity="yearly",
         )
 
-    @patch.object(R, '_date_range')
+    @patch.object(R, "_date_range")
     def test_get_metric_history_replaces_none_with_zero(self, mock_date_range):
         """Ensure that None-values get replaced with Zeros in
         ``R.get_metric_history``."""
 
         # Mock the _date_range method so we can specify it's return values.
         mock_date_range.return_value = [
             datetime(2000, 1, 1),
             datetime(2000, 1, 2),
             datetime(2000, 1, 3),
             datetime(2000, 1, 4),
         ]
 
         # Temporarily change the return value for mget
         mget_return = self.redis.mget.return_value
-        self.redis.mget.return_value = ['1', '2', None, '3']
+        self.redis.mget.return_value = ["1", "2", None, "3"]
 
         # Note: we're not providing a since parameter here, since we've
         # mocked the R._date_range method.
         results = self.r.get_metric_history("foo", granularity="daily")
 
         # Format the range of dates that for which we should get results
         expected = [
-            ('m:foo:2000-01-01', '1'),
-            ('m:foo:2000-01-02', '2'),
-            ('m:foo:2000-01-03', 0),
-            ('m:foo:2000-01-04', '3'),
+            ("m:foo:2000-01-01", "1"),
+            ("m:foo:2000-01-02", "2"),
+            ("m:foo:2000-01-03", 0),
+            ("m:foo:2000-01-04", "3"),
         ]
         self.assertEqual(results, expected)
 
         # Reset mget's previous return value
         self.redis.mget.return_value = mget_return
 
-    @patch.object(R, 'get_metric_history')
+    @patch.object(R, "get_metric_history")
     def test_get_metric_history_as_columns(self, mock_metric_hist):
         # set up some sample (yearly) metrics
         mock_metric_hist.return_value = [
-            ("m:bar:y:2012", '1'),
-            ('m:bar:y:2013', '2'),
-            ('m:foo:y:2012', '3'),
-            ('m:foo:y:2013', '4'),
+            ("m:bar:y:2012", "1"),
+            ("m:bar:y:2013", "2"),
+            ("m:foo:y:2012", "3"),
+            ("m:foo:y:2013", "4"),
         ]
         expected_results = [
-            ('Period', 'foo', 'bar'),
-            ('y:2012', '3', '1'),
-            ('y:2013', '4', '2'),
+            ("Period", "foo", "bar"),
+            ("y:2012", "3", "1"),
+            ("y:2013", "4", "2"),
         ]
-        with patch('redis_metrics.models.redis.StrictRedis'):
+        with patch("redis_metrics.models.redis.StrictRedis"):
             r = R()
             kwargs = {
-                'slugs': ['foo', 'bar'],
-                'since': None,
-                'granularity': 'yearly',
+                "slugs": ["foo", "bar"],
+                "since": None,
+                "granularity": "yearly",
             }
             results = r.get_metric_history_as_columns(**kwargs)
             self.assertEqual(results, expected_results)
 
     def _test_get_metric_history_as_columns(self, slugs, granularity):
         """Test that R.get_metric_history_as_columns makes calls to the
         following functions:
@@ -996,89 +1011,91 @@
         keys = self._metric_history_keys(slugs, granularity=granularity)
         self.r.get_metric_history_as_columns(slugs, granularity=granularity)
 
         # Verifies the correct call to redis
         self.redis.assert_has_calls([call.mget(keys)])
 
         # Verify that the method gets called correctly
-        with patch('redis_metrics.models.R') as mock_r:
+        with patch("redis_metrics.models.R") as mock_r:
             r = mock_r.return_value  # Get an instance of our Mocked R class
             r.get_metric_history_as_columns(slugs, granularity=granularity)
-            mock_r.assert_has_calls([
-                call().get_metric_history_as_columns(
-                    slugs, granularity=granularity
-                )
-            ])
+            mock_r.assert_has_calls(
+                [call().get_metric_history_as_columns(slugs, granularity=granularity)]
+            )
 
     def test_get_metric_history_as_columns_hourly(self):
-        self._test_get_metric_history_as_columns(['foo', 'bar'], 'hourly')
+        self._test_get_metric_history_as_columns(["foo", "bar"], "hourly")
 
     def test_get_metric_history_as_columns_daily(self):
-        self._test_get_metric_history_as_columns(['foo', 'bar'], 'daily')
+        self._test_get_metric_history_as_columns(["foo", "bar"], "daily")
 
     def test_get_metric_history_as_columns_weekly(self):
-        self._test_get_metric_history_as_columns(['foo', 'bar'], 'weekly')
+        self._test_get_metric_history_as_columns(["foo", "bar"], "weekly")
 
     def test_get_metric_history_as_columns_monthly(self):
-        self._test_get_metric_history_as_columns(['foo', 'bar'], 'monthly')
+        self._test_get_metric_history_as_columns(["foo", "bar"], "monthly")
 
     def test_get_metric_history_as_columns_yearly(self):
-        self._test_get_metric_history_as_columns(['foo', 'bar'], 'yearly')
+        self._test_get_metric_history_as_columns(["foo", "bar"], "yearly")
 
-    @patch.object(R, 'get_metric_history')
+    @patch.object(R, "get_metric_history")
     def test_get_metric_history_chart_data(self, mock_metric_hist):
         # set up some sample (yearly) metrics
         mock_metric_hist.return_value = [
-            ("m:bar:y:2012", '1'),
-            ('m:bar:y:2013', '2'),
-            ('m:foo:y:2012', '3'),
-            ('m:foo:y:2013', '4'),
+            ("m:bar:y:2012", "1"),
+            ("m:bar:y:2013", "2"),
+            ("m:foo:y:2012", "3"),
+            ("m:foo:y:2013", "4"),
         ]
         expected_results = {
-            'periods': ['y:2012', 'y:2013'],
-            'data': [
-                {'slug': 'bar', 'values': ['1', '2']},
-                {'slug': 'foo', 'values': ['3', '4']},
-            ]
+            "periods": ["y:2012", "y:2013"],
+            "data": [
+                {"slug": "bar", "values": ["1", "2"]},
+                {"slug": "foo", "values": ["3", "4"]},
+            ],
         }
-        with patch('redis_metrics.models.redis.StrictRedis'):
+        with patch("redis_metrics.models.redis.StrictRedis"):
             r = R()
             kwargs = {
-                'slugs': ['foo', 'bar'],
-                'since': None,
-                'granularity': 'yearly',
+                "slugs": ["foo", "bar"],
+                "since": None,
+                "granularity": "yearly",
             }
             results = r.get_metric_history_chart_data(**kwargs)
             self.assertEqual(results, expected_results)
 
     def test_gauge_slugs(self):
         """Tests that ``R.gauge_slugs`` calls the SMEMBERS command."""
         self.r.gauge_slugs()
         self.redis.assert_has_calls([call.smembers(self.r._gauge_slugs_key)])
 
     def test__gauge_key(self):
         """Tests that ``R._gauge_key`` correctly generates gauge keys."""
-        key = self.r._gauge_key('test-gauge')
-        self.assertEqual(key, 'g:test-gauge')
+        key = self.r._gauge_key("test-gauge")
+        self.assertEqual(key, "g:test-gauge")
 
     def test_gauge(self):
         """Tests setting a gauge with ``R.gauge``. Verifies that the gauge slug
         is added to the set of gauge slugs and that the value gets set."""
-        self.r.gauge('test-gauge', 9000)
-        self.redis.assert_has_calls([
-            call.sadd(self.r._gauge_slugs_key, 'test-gauge'),
-            call.set('g:test-gauge', 9000),
-        ])
+        self.r.gauge("test-gauge", 9000)
+        self.redis.assert_has_calls(
+            [
+                call.sadd(self.r._gauge_slugs_key, "test-gauge"),
+                call.set("g:test-gauge", 9000),
+            ]
+        )
 
     def test_get_gauge(self):
         """Tests retrieving a gague with ``R.get_gauge``. Verifies that the
         Redis GET command is called with the correct key."""
-        self.r.get_gauge('test-gauge')
-        self.redis.assert_has_calls([call.get('g:test-gauge')])
+        self.r.get_gauge("test-gauge")
+        self.redis.assert_has_calls([call.get("g:test-gauge")])
 
     def test_delete_gauge(self):
         """Tests deltion of a gauge."""
         self.r.delete_gauge("test-gauge")
-        self.redis.assert_has_calls([
-            call.delete('g:test-gauge'),
-            call.srem(self.r._gauge_slugs_key, "test-gauge"),
-        ])
+        self.redis.assert_has_calls(
+            [
+                call.delete("g:test-gauge"),
+                call.srem(self.r._gauge_slugs_key, "test-gauge"),
+            ]
+        )
```

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_settings.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_templatetags.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_utils.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,230 +1,283 @@
 from __future__ import unicode_literals
 from datetime import datetime
+
 try:
     from unittest.mock import call, patch, Mock
 except ImportError:
     from mock import call, patch, Mock
 
 from django.test import TestCase
 from django.test.utils import override_settings
 
 from ..models import R
 from .. import utils
 
 
 TEST_SETTINGS = {
-    'HOST': 'localhost',
-    'PORT': 6379,
-    'DB': 0,
-    'PASSWORD': None,
-    'SOCKET_TIMEOUT': None,
-    'SOCKET_CONNECTION_POOL': None,
-    'MIN_GRANULARITY': 'seconds',
-    'MAX_GRANULARITY': 'yearly',
-    'MONDAY_FIRST_DAY_OF_WEEK': False,
-    'USE_ISO_WEEK_NUMBER': False,
+    "HOST": "localhost",
+    "PORT": 6379,
+    "DB": 0,
+    "PASSWORD": None,
+    "SOCKET_TIMEOUT": None,
+    "SOCKET_CONNECTION_POOL": None,
+    "MIN_GRANULARITY": "seconds",
+    "MAX_GRANULARITY": "yearly",
+    "MONDAY_FIRST_DAY_OF_WEEK": False,
+    "USE_ISO_WEEK_NUMBER": False,
+    "SSL": False,
 }
 
 
 @override_settings(REDIS_METRICS=TEST_SETTINGS)
 class TestUtils(TestCase):
     """Tests for functions in ``redis_metrics.utils``."""
 
     def setUp(self):
         utils._redis_model = None
 
     def test_get_r(self):
         # Global `_redis_model` is None by default
         r_kwargs = {
-            'decode_responses': True,
-            'host': 'localhost',
-            'db': 0,
-            'port': 6379,
-            'password': None,
-            'connection_pool': None,
-            'socket_timeout': None
+            "host": "localhost",
+            "port": 6379,
+            "db": 0,
+            "password": None,
+            "ssl": False,
+            "connection_pool": None,
+            "socket_timeout": None,
+            "decode_responses": True,
         }
-        with patch('redis_metrics.models.redis.StrictRedis') as mock_redis:
+        with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             inst = R()
-            self.assertEqual(inst.host, 'localhost')
+            self.assertEqual(inst.host, "localhost")
             self.assertEqual(inst.port, 6379)
             self.assertEqual(inst.db, 0)
             self.assertEqual(inst.password, None)
         self.assertEqual(utils._redis_model, None)
         with patch("redis_metrics.models.redis.StrictRedis") as mock_redis:
             r = utils.get_r()
             self.assertIsInstance(r, R)
             self.assertEqual(r, utils._redis_model)
             mock_redis.assert_called_once_with(**r_kwargs)
 
     def test_set_metric(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.set_metric("test-slug", 42)
-            mock_get_r.assert_has_calls([
-                call(),
-                call().set_metric("test-slug", 42, category=None, expire=None, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().set_metric(
+                        "test-slug", 42, category=None, expire=None, date=None
+                    ),
+                ]
+            )
 
     def test_set_metric_with_category(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.set_metric("test-slug", 42, category="Woo")
-            mock_get_r.assert_has_calls([
-                call(),
-                call().set_metric("test-slug", 42, category="Woo", expire=None, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().set_metric(
+                        "test-slug", 42, category="Woo", expire=None, date=None
+                    ),
+                ]
+            )
 
     def test_set_metric_with_expiration(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.set_metric("test-slug", 42, expire=300)
-            mock_get_r.assert_has_calls([
-                call(),
-                call().set_metric("test-slug", 42, category=None, expire=300, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().set_metric(
+                        "test-slug", 42, category=None, expire=300, date=None
+                    ),
+                ]
+            )
 
     def test_metric(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.metric("test-slug")
-            mock_get_r.assert_has_calls([
-                call(),
-                call().metric("test-slug", num=1, category=None, expire=None, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().metric(
+                        "test-slug", num=1, category=None, expire=None, date=None
+                    ),
+                ]
+            )
 
     def test_metric_with_category(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.metric("test-slug", category="Woo")
-            mock_get_r.assert_has_calls([
-                call(),
-                call().metric("test-slug", num=1, category="Woo", expire=None, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().metric(
+                        "test-slug", num=1, category="Woo", expire=None, date=None
+                    ),
+                ]
+            )
 
     def test_metric_with_expiration(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.metric("test-slug", expire=300)
-            mock_get_r.assert_has_calls([
-                call(),
-                call().metric("test-slug", num=1, category=None, expire=300, date=None),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().metric(
+                        "test-slug", num=1, category=None, expire=300, date=None
+                    ),
+                ]
+            )
 
     def test_metric_with_date(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.metric("test-slug", date=datetime(2000, 1, 2))
-            mock_get_r.assert_has_calls([
-                call(),
-                call().metric("test-slug", num=1, category=None, expire=None, date=datetime(2000, 1, 2)),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().metric(
+                        "test-slug",
+                        num=1,
+                        category=None,
+                        expire=None,
+                        date=datetime(2000, 1, 2),
+                    ),
+                ]
+            )
 
     def test_gauge(self):
         with patch("redis_metrics.utils.get_r") as mock_get_r:
             utils.gauge("test-slug", 9000)
-            mock_get_r.assert_has_calls([
-                call(),
-                call().gauge("test-slug", 9000),
-            ])
+            mock_get_r.assert_has_calls(
+                [
+                    call(),
+                    call().gauge("test-slug", 9000),
+                ]
+            )
 
     def test_generate_test_metrics(self):
         keys = [
-            'm:test-slug:s:2000-01-02-03-04-05',
-            'm:test-slug:i:2000-01-02-03-04',
-            'm:test-slug:h:2000-01-02-03',
-            'm:test-slug:2000-01-02',
-            'm:test-slug:w:2000-01',
-            'm:test-slug:m:2000-01',
-            'm:test-slug:y:2000',
+            "m:test-slug:s:2000-01-02-03-04-05",
+            "m:test-slug:i:2000-01-02-03-04",
+            "m:test-slug:h:2000-01-02-03",
+            "m:test-slug:2000-01-02",
+            "m:test-slug:w:2000-01",
+            "m:test-slug:m:2000-01",
+            "m:test-slug:y:2000",
         ]
         config = {
-            '_build_keys.return_value': keys,
-            '_metric_slugs_key': 'MSK',
-            '_date_range.return_value': [datetime.utcnow()],
+            "_build_keys.return_value": keys,
+            "_metric_slugs_key": "MSK",
+            "_date_range.return_value": [datetime.utcnow()],
         }
         mock_r = Mock(**config)
-        config = {'return_value': mock_r}
+        config = {"return_value": mock_r}
         with patch("redis_metrics.utils.get_r", **config) as mock_get_r:
             # When called with random = True
             with patch("redis_metrics.utils.random") as mock_random:
                 mock_random.randint.return_value = 9999
                 utils.generate_test_metrics(
                     slug="test-slug", num=1, randomize=True, increment_value=1
                 )
                 mock_get_r.assert_called_once_with()
-                mock_r.r.sadd.assert_called_once_with('MSK', 'test-slug')
+                mock_r.r.sadd.assert_called_once_with("MSK", "test-slug")
                 mock_random.seed.assert_called_once_with()
-                mock_random.randint.assert_has_calls([
-                    call(0, 1), call(0, 1), call(0, 1), call(0, 1),
-                ])
-                mock_r.r.incr.assert_has_calls([
-                    call('m:test-slug:2000-01-02', 9999),
-                    call('m:test-slug:w:2000-01', 9999),
-                    call('m:test-slug:m:2000-01', 9999),
-                    call('m:test-slug:y:2000', 9999),
-                ])
+                mock_random.randint.assert_has_calls(
+                    [
+                        call(0, 1),
+                        call(0, 1),
+                        call(0, 1),
+                        call(0, 1),
+                    ]
+                )
+                mock_r.r.incr.assert_has_calls(
+                    [
+                        call("m:test-slug:2000-01-02", 9999),
+                        call("m:test-slug:w:2000-01", 9999),
+                        call("m:test-slug:m:2000-01", 9999),
+                        call("m:test-slug:y:2000", 9999),
+                    ]
+                )
 
             mock_get_r.reset_mock()
             mock_r.reset_mock()
 
             # When called with random = False
             utils.generate_test_metrics(
                 slug="test-slug", num=1, randomize=False, increment_value=1
             )
             mock_get_r.assert_called_once_with()
-            mock_r.r.sadd.assert_called_once_with('MSK', 'test-slug')
-            mock_r.r.incr.assert_has_calls([
-                call('m:test-slug:2000-01-02', 0),
-                call('m:test-slug:w:2000-01', 0),
-                call('m:test-slug:m:2000-01', 0),
-                call('m:test-slug:y:2000', 0),
-            ])
+            mock_r.r.sadd.assert_called_once_with("MSK", "test-slug")
+            mock_r.r.incr.assert_has_calls(
+                [
+                    call("m:test-slug:2000-01-02", 0),
+                    call("m:test-slug:w:2000-01", 0),
+                    call("m:test-slug:m:2000-01", 0),
+                    call("m:test-slug:y:2000", 0),
+                ]
+            )
 
     def test_generate_test_metrics_with_cap(self):
         keys = [
-            'm:test-slug:s:2000-01-02-03-04-05',
-            'm:test-slug:i:2000-01-02-03-04',
-            'm:test-slug:h:2000-01-02-03',
-            'm:test-slug:2000-01-02',
-            'm:test-slug:w:2000-01',
-            'm:test-slug:m:2000-01',
-            'm:test-slug:y:2000',
+            "m:test-slug:s:2000-01-02-03-04-05",
+            "m:test-slug:i:2000-01-02-03-04",
+            "m:test-slug:h:2000-01-02-03",
+            "m:test-slug:2000-01-02",
+            "m:test-slug:w:2000-01",
+            "m:test-slug:m:2000-01",
+            "m:test-slug:y:2000",
         ]
         config = {
-            '_build_keys.return_value': keys,
-            '_metric_slugs_key': 'MSK',
-            'r.get.return_value': 100,
-            '_date_range.return_value': [datetime.utcnow()],
+            "_build_keys.return_value": keys,
+            "_metric_slugs_key": "MSK",
+            "r.get.return_value": 100,
+            "_date_range.return_value": [datetime.utcnow()],
         }
         mock_r = Mock(**config)
-        config = {'return_value': mock_r}
+        config = {"return_value": mock_r}
         with patch("redis_metrics.utils.get_r", **config) as mock_get_r:
             # When called with random = True
             with patch("redis_metrics.utils.random") as mock_random:
                 mock_random.randint.return_value = 9999
                 utils.generate_test_metrics(
                     slug="test-slug", num=1, randomize=True, cap=5, increment_value=1
                 )
                 mock_get_r.assert_called_once_with()
-                mock_r.r.sadd.assert_called_once_with('MSK', 'test-slug')
+                mock_r.r.sadd.assert_called_once_with("MSK", "test-slug")
                 mock_random.seed.assert_called_once_with()
-                mock_random.randint.assert_has_calls([
-                    call(0, 1), call(0, 1), call(0, 1), call(0, 1),
-                ])
+                mock_random.randint.assert_has_calls(
+                    [
+                        call(0, 1),
+                        call(0, 1),
+                        call(0, 1),
+                        call(0, 1),
+                    ]
+                )
                 # Should be no increment due to cap
-                mock_r.r.incr.assert_has_calls([
-                    call('m:test-slug:2000-01-02', 0),
-                    call('m:test-slug:w:2000-01', 0),
-                    call('m:test-slug:m:2000-01', 0),
-                    call('m:test-slug:y:2000', 0),
-                ])
+                mock_r.r.incr.assert_has_calls(
+                    [
+                        call("m:test-slug:2000-01-02", 0),
+                        call("m:test-slug:w:2000-01", 0),
+                        call("m:test-slug:m:2000-01", 0),
+                        call("m:test-slug:y:2000", 0),
+                    ]
+                )
 
             mock_get_r.reset_mock()
             mock_r.reset_mock()
 
     def test_delete_test_metrics(self):
         d = datetime.utcnow()
-        with patch('redis_metrics.utils.get_r') as mock_get_r:
+        with patch("redis_metrics.utils.get_r") as mock_get_r:
             mock_r = mock_get_r.return_value
-            mock_r._metric_slugs_key = 'MSK'
-            mock_r._build_keys.return_value = ['keys']
+            mock_r._metric_slugs_key = "MSK"
+            mock_r._build_keys.return_value = ["keys"]
             mock_r._date_range.return_value = [d]
 
             utils.delete_test_metrics(slug="test-metric", num=1)
             mock_r._build_keys.assert_called_once_with("test-metric", date=d)
-            mock_r.r.srem.assert_called_once_with('MSK', 'test-metric')
-            mock_r.r.delete.assert_called_once_with('keys')
+            mock_r.r.srem.assert_called_once_with("MSK", "test-metric")
+            mock_r.r.delete.assert_called_once_with("keys")
```

### Comparing `django-redis_metrics-2.1.0/redis_metrics/tests/test_views.py` & `django-redis_metrics-2.2.0/redis_metrics/tests/test_views.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,393 +2,393 @@
 This file demonstrates writing tests using the unittest module. These will pass
 when you run "manage.py test".
 
 Replace this with more appropriate tests for your application.
 """
 from __future__ import unicode_literals
 from datetime import datetime
+
 try:
     from unittest.mock import call, patch
 except ImportError:
     from mock import call, patch
 
 from django.urls import reverse
 from django.test import TestCase, Client
 from django.test.utils import override_settings
 
 
 TEST_SETTINGS = {
-    'HOST': 'localhost',
-    'PORT': 6379,
-    'DB': 0,
-    'PASSWORD': None,
-    'SOCKET_TIMEOUT': None,
-    'SOCKET_CONNECTION_POOL': None,
-    'MIN_GRANULARITY': 'seconds',
-    'MAX_GRANULARITY': 'yearly',
-    'MONDAY_FIRST_DAY_OF_WEEK': False,
-    'USE_ISO_WEEK_NUMBER': False,
+    "HOST": "localhost",
+    "PORT": 6379,
+    "DB": 0,
+    "PASSWORD": None,
+    "SOCKET_TIMEOUT": None,
+    "SOCKET_CONNECTION_POOL": None,
+    "MIN_GRANULARITY": "seconds",
+    "MAX_GRANULARITY": "yearly",
+    "MONDAY_FIRST_DAY_OF_WEEK": False,
+    "USE_ISO_WEEK_NUMBER": False,
+    "SSL": False,
 }
 
 
 @override_settings(REDIS_METRICS=TEST_SETTINGS)
 class TestViews(TestCase):
-    url = 'redis_metrics.urls'
+    url = "redis_metrics.urls"
 
     def _get_user_model(self):
         try:  # pragma: no cover
             # Django >= 1.5
             from django.contrib.auth import get_user_model  # pragma: no cover
+
             User = get_user_model()  # pragma: no cover
         except ImportError:  # pragma: no cover
             # Fallback for Django 1.4 (or lower)
             from django.contrib.auth.models import User  # pragma: no cover
         return User
 
     def setUp(self):
         # Patch the connection to redis, but keep a reference to the
         # created StrictRedis instance, so we can make assertions about how
         # it's called.
-        self.redis_patcher = patch('redis_metrics.models.redis.StrictRedis')
+        self.redis_patcher = patch("redis_metrics.models.redis.StrictRedis")
         mock_StrictRedis = self.redis_patcher.start()
         self.redis = mock_StrictRedis.return_value
 
         User = self._get_user_model()
         self.user = User.objects.create_superuser(
             username="redis_metrics_test_user",
             email="redis_metrics_test_user@example.com",
-            password="secret"
+            password="secret",
         )
-        assert self.client.login(
-            username="redis_metrics_test_user",
-            password="secret")
+        assert self.client.login(username="redis_metrics_test_user", password="secret")
         self.unauthed_client = Client()  # Keep an unauthenticated client
 
     def tearDown(self):
         self.redis_patcher.stop()
         self.user.delete()
 
     def assertUnauthedRequestRedirects(self, url):
         resp = self.unauthed_client.get(url)
         self.assertEqual(resp.status_code, 302)
         return resp
 
     def test_default_view(self):
-        url = reverse('redis_metrics_default')
+        url = reverse("redis_metrics_default")
         resp = self.client.get(url)
         self.assertEqual(resp.status_code, 200)
         self.assertTemplateUsed(resp, "redis_metrics/default.html")
 
     def test_gauges_view(self):
         """Test the ``GaugesView``."""
-        url = reverse('redis_metrics_gauges')
-        with patch('redis_metrics.views.get_r') as mock_r:
+        url = reverse("redis_metrics_gauges")
+        with patch("redis_metrics.views.get_r") as mock_r:
             # Set appropriate return values for methods that'll get called
             # in the MetricsListView.
             r = mock_r.return_value  # Get an instance of our Mocked R class
-            r.gauge_slugs.return_value = set(['gauge-a', 'gauge-b'])
+            r.gauge_slugs.return_value = set(["gauge-a", "gauge-b"])
 
             # Do the Request and test for content
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('Gauges', str(resp.content))
-            self.assertEqual(
-                resp.context['gauges'],
-                set(['gauge-a', 'gauge-b'])
-            )
+            self.assertIn("Gauges", str(resp.content))
+            self.assertEqual(resp.context["gauges"], set(["gauge-a", "gauge-b"]))
 
             # Make sure our Mock R object called the right methods.
             mock_r.assert_has_calls([call().gauge_slugs()])
 
     def test_metrics_list(self):
         """Test the ``MetricsListView``."""
-        url = reverse('redis_metrics_list')
-        with patch('redis_metrics.views.get_r') as mock_r:
+        url = reverse("redis_metrics_list")
+        with patch("redis_metrics.views.get_r") as mock_r:
             # Set appropriate return values for methods that'll get called
             # in the MetricsListView.
             r = mock_r.return_value  # Get an instance of our Mocked R class
             r.metric_slugs_by_category.return_value = {
-                "Sample Category": ['test-metric-a', 'test-metric-b'],
+                "Sample Category": ["test-metric-a", "test-metric-b"],
             }
-            r.gauge_slugs.return_value = set(['test-gauge'])
+            r.gauge_slugs.return_value = set(["test-gauge"])
 
             # Do the Request and test for content
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('Sample Category', resp.context['metrics'].keys())
+            self.assertIn("Sample Category", resp.context["metrics"].keys())
 
-            metrics_values = list(resp.context['metrics'].values())
-            self.assertIn('test-metric-a', metrics_values[0])
-            self.assertIn('test-metric-b', metrics_values[0])
+            metrics_values = list(resp.context["metrics"].values())
+            self.assertIn("test-metric-a", metrics_values[0])
+            self.assertIn("test-metric-b", metrics_values[0])
 
             # Make sure our Mock R object called the right methods.
-            mock_r.assert_has_calls([
-                call().metric_slugs_by_category(),
-            ])
+            mock_r.assert_has_calls(
+                [
+                    call().metric_slugs_by_category(),
+                ]
+            )
 
     def test_metric_detail(self):
-        with patch('redis_metrics.views.get_r') as mock_get_r:
+        with patch("redis_metrics.views.get_r") as mock_get_r:
             inst = mock_get_r.return_value
-            inst._granularities.return_value = ['daily', 'weekly']
+            inst._granularities.return_value = ["daily", "weekly"]
 
-            slug = 'test-metric'
-            url = reverse('redis_metric_detail', args=[slug])
+            slug = "test-metric"
+            url = reverse("redis_metric_detail", args=[slug])
 
             # Do the Request & test results
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertEqual(resp.context_data['slug'], slug)
-            self.assertEqual(resp.context_data['granularities'], ['daily', 'weekly'])
+            self.assertEqual(resp.context_data["slug"], slug)
+            self.assertEqual(resp.context_data["granularities"], ["daily", "weekly"])
 
     def test_metric_history(self):
-        with patch('redis_metrics.views.get_r') as mock_get_r:
+        with patch("redis_metrics.views.get_r") as mock_get_r:
             inst = mock_get_r.return_value
-            inst._granularities.return_value = ['daily', 'weekly']
+            inst._granularities.return_value = ["daily", "weekly"]
 
-            slug = 'test-metric'
-            granularity = 'daily'
-            url = reverse('redis_metric_history', args=[slug, granularity])
+            slug = "test-metric"
+            granularity = "daily"
+            url = reverse("redis_metric_history", args=[slug, granularity])
 
             # Do the Request & test results
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
             context = resp.context_data
-            self.assertEqual(context['slug'], slug)
-            self.assertEqual(context['since'], None)
-            self.assertEqual(context['granularity'], granularity)
-            self.assertEqual(context['granularities'], ['daily', 'weekly'])
+            self.assertEqual(context["slug"], slug)
+            self.assertEqual(context["since"], None)
+            self.assertEqual(context["granularity"], granularity)
+            self.assertEqual(context["granularities"], ["daily", "weekly"])
 
     def test_metric_history_since(self):
         """Tests the ``MetricHistoryView`` when there's a ``since`` variable"""
-        slug = 'test-metric'
-        granularity = 'daily'
-        url = reverse('redis_metric_history', args=[slug, granularity])
+        slug = "test-metric"
+        granularity = "daily"
+        url = reverse("redis_metric_history", args=[slug, granularity])
 
         # Do the Request & test results for a Date
-        resp = self.client.get(url, {'since': '2012-12-25'})
+        resp = self.client.get(url, {"since": "2012-12-25"})
         self.assertEqual(resp.status_code, 200)
         context = resp.context_data
-        self.assertEqual(context['since'], datetime(2012, 12, 25))
-        self.assertEqual(context['slug'], slug)
-        self.assertEqual(context['granularity'], granularity)
+        self.assertEqual(context["since"], datetime(2012, 12, 25))
+        self.assertEqual(context["slug"], slug)
+        self.assertEqual(context["granularity"], granularity)
 
         # Do the Request & test results for a Date & Time
-        resp = self.client.get(url, {'since': '2012-12-25 11:30:45'})
+        resp = self.client.get(url, {"since": "2012-12-25 11:30:45"})
         self.assertEqual(resp.status_code, 200)
         context = resp.context_data
-        self.assertEqual(context['since'], datetime(2012, 12, 25, 11, 30, 45))
-        self.assertEqual(context['slug'], slug)
-        self.assertEqual(context['granularity'], granularity)
+        self.assertEqual(context["since"], datetime(2012, 12, 25, 11, 30, 45))
+        self.assertEqual(context["slug"], slug)
+        self.assertEqual(context["granularity"], granularity)
 
     def test_metrics_list_requires_admin(self):
         """Verifies that ``MetricsListView`` requires authentication."""
-        self.assertUnauthedRequestRedirects(reverse('redis_metrics_list'))
+        self.assertUnauthedRequestRedirects(reverse("redis_metrics_list"))
 
     def test_metric_detail_requires_admin(self):
         """Verifies that ``MetricDetailView`` requires authentication."""
         self.assertUnauthedRequestRedirects(
-            reverse('redis_metric_detail', args=['whatever'])
+            reverse("redis_metric_detail", args=["whatever"])
         )
 
     def test_metric_history_requires_admin(self):
         """Verifies that ``MetricHistoryView`` requires authentication."""
         self.assertUnauthedRequestRedirects(
-            reverse('redis_metric_history', args=['whatever', 'daily'])
+            reverse("redis_metric_history", args=["whatever", "daily"])
         )
 
     def test_aggregate_form_view(self):
         """Verifies that GET requests to the ``AggregateFormView`` have the
         correct context info (i.e. a form)."""
-        url = reverse('redis_metric_aggregate')
+        url = reverse("redis_metric_aggregate")
         self.assertUnauthedRequestRedirects(url)
-        with patch('redis_metrics.views.get_r'):
+        with patch("redis_metrics.views.get_r"):
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('form', resp.context_data)
+            self.assertIn("form", resp.context_data)
 
     def test_aggregate_form_view_post(self):
         """Verifies that POST requests to the ``AggregateFormView`` work as
         expected."""
-        url = reverse('redis_metric_aggregate')
-        with patch('redis_metrics.views.get_r'):
-            with patch('redis_metrics.forms.R') as mock_r:
+        url = reverse("redis_metric_aggregate")
+        with patch("redis_metrics.views.get_r"):
+            with patch("redis_metrics.forms.R") as mock_r:
                 # Set up a return value for ``R.metric_slugs``, which is used
                 # in the ``AggregateMetricForm``
                 r = mock_r.return_value  # An instance of our Mocked R class
-                r.metric_slugs.return_value = set(['test', 'foo', 'bar'])
+                r.metric_slugs.return_value = set(["test", "foo", "bar"])
 
                 # Test with ONE metric selected
-                data = {'metrics': ['foo']}
+                data = {"metrics": ["foo"]}
                 resp = self.client.post(url, data)
                 self.assertEqual(resp.status_code, 302)
                 # make sure the metric slug shows up in the redirect URL
-                self.assertIn('foo', resp.get("Location", ''))
+                self.assertIn("foo", resp.get("Location", ""))
 
                 # Test with TWO metrics selected
-                data = {'metrics': ['foo', 'bar']}
+                data = {"metrics": ["foo", "bar"]}
                 resp = self.client.post(url, data)
                 self.assertEqual(resp.status_code, 302)
                 # make sure the metric slug shows up in the redirect URL
-                self.assertIn('foo+bar', resp.get("Location", ''))
+                self.assertIn("foo+bar", resp.get("Location", ""))
 
     def test_aggregate_detail_view(self):
         """Tests ``views.AggregateDetailView``."""
-        with patch('redis_metrics.views.get_r') as mock_get_r:
+        with patch("redis_metrics.views.get_r") as mock_get_r:
             inst = mock_get_r.return_value
-            inst._granularities.return_value = ['daily', 'weekly']
+            inst._granularities.return_value = ["daily", "weekly"]
 
-            slug_set = set(['foo', 'bar', 'test-metric', 'yippitty-poo-bah'])
-            slugs = '+'.join(slug_set)
-            url = reverse('redis_metric_aggregate_detail', args=[slugs])
+            slug_set = set(["foo", "bar", "test-metric", "yippitty-poo-bah"])
+            slugs = "+".join(slug_set)
+            url = reverse("redis_metric_aggregate_detail", args=[slugs])
 
             # Do the Request & test results
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('slugs', resp.context_data)
-            self.assertIn('granularities', resp.context_data)
-            self.assertEqual(resp.context_data['slugs'], slug_set)
-            self.assertEqual(resp.context_data['granularities'], ['daily', 'weekly'])
+            self.assertIn("slugs", resp.context_data)
+            self.assertIn("granularities", resp.context_data)
+            self.assertEqual(resp.context_data["slugs"], slug_set)
+            self.assertEqual(resp.context_data["granularities"], ["daily", "weekly"])
 
     def _test_aggregate_history_view(self, slugs, granularity):
         """Tests ``views.AggregateHistoryView`` with the given slugs,
         granularity, without a specified date verifying the values are
         correctly passed to the template."""
-        with patch('redis_metrics.views.get_r') as mock_get_r:
+        with patch("redis_metrics.views.get_r") as mock_get_r:
             inst = mock_get_r.return_value
-            inst._granularities.return_value = ['daily', 'weekly']
+            inst._granularities.return_value = ["daily", "weekly"]
 
             slug_set = set(slugs)
-            url = reverse('redis_metric_aggregate_history',
-                          args=['+'.join(slugs), granularity])
+            url = reverse(
+                "redis_metric_aggregate_history", args=["+".join(slugs), granularity]
+            )
 
             # Do the Request & test results
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('slugs', resp.context_data)
-            self.assertIn('granularity', resp.context_data)
-            self.assertIn('since', resp.context_data)
-            self.assertIn('granularities', resp.context_data)
-            self.assertEqual(resp.context_data['slugs'], slug_set)
-            self.assertEqual(resp.context_data['granularity'], granularity)
-            self.assertEqual(resp.context_data['granularities'], ['daily', 'weekly'])
-            self.assertIsNone(resp.context_data['since'])
+            self.assertIn("slugs", resp.context_data)
+            self.assertIn("granularity", resp.context_data)
+            self.assertIn("since", resp.context_data)
+            self.assertIn("granularities", resp.context_data)
+            self.assertEqual(resp.context_data["slugs"], slug_set)
+            self.assertEqual(resp.context_data["granularity"], granularity)
+            self.assertEqual(resp.context_data["granularities"], ["daily", "weekly"])
+            self.assertIsNone(resp.context_data["since"])
 
     def test_aggregate_history_view_hourly(self):
-        self._test_aggregate_history_view(['foo', 'bar'], 'hourly')
+        self._test_aggregate_history_view(["foo", "bar"], "hourly")
 
     def test_aggregate_history_view_daily(self):
-        self._test_aggregate_history_view(['foo', 'bar'], 'daily')
+        self._test_aggregate_history_view(["foo", "bar"], "daily")
 
     def test_aggregate_history_view_weekly(self):
-        self._test_aggregate_history_view(['foo', 'bar'], 'weekly')
+        self._test_aggregate_history_view(["foo", "bar"], "weekly")
 
     def test_aggregate_history_view_monthly(self):
-        self._test_aggregate_history_view(['foo', 'bar'], 'monthly')
+        self._test_aggregate_history_view(["foo", "bar"], "monthly")
 
     def test_aggregate_history_view_yearly(self):
-        self._test_aggregate_history_view(['foo', 'bar'], 'yearly')
+        self._test_aggregate_history_view(["foo", "bar"], "yearly")
 
     def test_aggregate_history_view_since(self):
         """Tests ``views.AggregateHistoryView`` with a ``since`` parameter."""
-        slugs = ['foo', 'bar']
-        granularity = 'yearly'
+        slugs = ["foo", "bar"]
+        granularity = "yearly"
         url = reverse(
-            'redis_metric_aggregate_history',
-            args=['+'.join(slugs), granularity]
+            "redis_metric_aggregate_history", args=["+".join(slugs), granularity]
         )
 
         # Do the Request & test results with a just a date
-        resp = self.client.get(url, {'since': "2012-12-25"})
+        resp = self.client.get(url, {"since": "2012-12-25"})
         self.assertEqual(resp.status_code, 200)
-        self.assertIsInstance(resp.context_data['since'], datetime)
-        self.assertEqual(resp.context_data['since'], datetime(2012, 12, 25))
+        self.assertIsInstance(resp.context_data["since"], datetime)
+        self.assertEqual(resp.context_data["since"], datetime(2012, 12, 25))
 
         # Do the Request & test results with a date & time
-        resp = self.client.get(url, {'since': "2012-12-25 11:30:45"})
+        resp = self.client.get(url, {"since": "2012-12-25 11:30:45"})
         self.assertEqual(resp.status_code, 200)
-        self.assertIsInstance(resp.context_data['since'], datetime)
-        self.assertEqual(
-            resp.context_data['since'],
-            datetime(2012, 12, 25, 11, 30, 45)
-        )
+        self.assertIsInstance(resp.context_data["since"], datetime)
+        self.assertEqual(resp.context_data["since"], datetime(2012, 12, 25, 11, 30, 45))
 
     def test_category_form_view(self):
         """Verifies that GET requests to the ``CategoryFormView`` have the
         correct context info (i.e. a form)."""
-        url = reverse('redis_metrics_categorize')
+        url = reverse("redis_metrics_categorize")
         self.assertUnauthedRequestRedirects(url)
 
         # NOTE: you can't mock the form in the views, because calls to the
         # form get dispatched somewhere else. That's why this is mocking the
         # R object in the form, instead of the form, itself.
         k = {
-            'return_value.metric_slugs.return_value': ['foo', 'bar', 'baz'],
-            'return_value._category_slugs.return_value': [],
+            "return_value.metric_slugs.return_value": ["foo", "bar", "baz"],
+            "return_value._category_slugs.return_value": [],
         }
-        with patch('redis_metrics.forms.R', **k):
+        with patch("redis_metrics.forms.R", **k):
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('form', resp.context_data)
+            self.assertIn("form", resp.context_data)
             self.assertIn("id_category_name", str(resp.content))
             self.assertIn("id_metrics", str(resp.content))
 
     def test_category_form_view_with_initial(self):
         """Verifies that GET requests to the ``CategoryFormView`` have the
         correct context info/initial data when called with a specified
         Category."""
-        url = reverse('redis_metrics_categorize', args=['Stuff'])
+        url = reverse("redis_metrics_categorize", args=["Stuff"])
         self.assertUnauthedRequestRedirects(url)
 
         # NOTE: you can't mock the form in the views, because calls to the
         # form get dispatched somewhere else. That's why this is mocking the
         # R object in the form, instead of the form, itself.
         k = {
-            'return_value.metric_slugs.return_value': ['foo', 'bar', 'baz'],
-            'return_value._category_slugs.return_value': ['foo', 'bar'],
+            "return_value.metric_slugs.return_value": ["foo", "bar", "baz"],
+            "return_value._category_slugs.return_value": ["foo", "bar"],
         }
-        with patch('redis_metrics.forms.R', **k) as mock_R:
+        with patch("redis_metrics.forms.R", **k) as mock_R:
             resp = self.client.get(url)
             self.assertEqual(resp.status_code, 200)
-            self.assertIn('form', resp.context_data)
+            self.assertIn("form", resp.context_data)
             self.assertIn("id_category_name", str(resp.content))
             self.assertIn("id_metrics", str(resp.content))
 
             # foo and bar should be pre-selected, but baz should not, since
             # it's not in the "Stuff" category
-            initial_metrics = resp.context['form'].fields['metrics'].initial
-            self.assertIn('foo', initial_metrics)
-            self.assertIn('bar', initial_metrics)
-            self.assertNotIn('baz', initial_metrics)
+            initial_metrics = resp.context["form"].fields["metrics"].initial
+            self.assertIn("foo", initial_metrics)
+            self.assertIn("bar", initial_metrics)
+            self.assertNotIn("baz", initial_metrics)
 
             # This is what should happen in the form
-            mock_R.assert_has_calls([
-                # happens in __init__
-                call(),
-                call().metric_slugs(),
-                call()._category_slugs('Stuff')
-            ])
+            mock_R.assert_has_calls(
+                [
+                    # happens in __init__
+                    call(),
+                    call().metric_slugs(),
+                    call()._category_slugs("Stuff"),
+                ]
+            )
 
     def test_category_form_view_post(self):
         """Verifies that POST requests to the ``CategoryFormView`` work as
         expected."""
-        url = reverse('redis_metrics_categorize')
+        url = reverse("redis_metrics_categorize")
 
         # NOTE: you can't mock the form in the views, because calls to the
         # form get dispatched somewhere else. That's why this is mocking the
         # R object in the form, instead of the form, itself.
         k = {
-            'return_value.metric_slugs.return_value': ['foo', 'bar', 'baz'],
-            'return_value._category_slugs.return_value': ['foo', 'bar'],
+            "return_value.metric_slugs.return_value": ["foo", "bar", "baz"],
+            "return_value._category_slugs.return_value": ["foo", "bar"],
         }
-        with patch('redis_metrics.forms.R', **k) as mock_R:
-            data = {'category_name': 'Foo', 'metrics': ['foo', 'bar']}
+        with patch("redis_metrics.forms.R", **k) as mock_R:
+            data = {"category_name": "Foo", "metrics": ["foo", "bar"]}
             resp = self.client.post(url, data)
             self.assertEqual(resp.status_code, 302)
             # This is what should happen in the form when POSTing
-            mock_R.assert_has_calls([
-                # happens in __init__
-                call(),
-                call().metric_slugs(),
-
-                # happens in categorize_metrics
-                call().reset_category('Foo', ['foo', 'bar']),
-            ])
+            mock_R.assert_has_calls(
+                [
+                    # happens in __init__
+                    call(),
+                    call().metric_slugs(),
+                    # happens in categorize_metrics
+                    call().reset_category("Foo", ["foo", "bar"]),
+                ]
+            )
```

### Comparing `django-redis_metrics-2.1.0/redis_metrics/urls.py` & `django-redis_metrics-2.2.0/redis_metrics/urls.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/utils.py` & `django-redis_metrics-2.2.0/redis_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django-redis_metrics-2.1.0/redis_metrics/views.py` & `django-redis_metrics-2.2.0/redis_metrics/views.py`

 * *Files identical despite different names*

