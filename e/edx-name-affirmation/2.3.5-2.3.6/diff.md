# Comparing `tmp/edx-name-affirmation-2.3.5.tar.gz` & `tmp/edx-name-affirmation-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-name-affirmation-2.3.5.tar", last modified: Fri Sep  9 13:46:14 2022, max compression
+gzip compressed data, was "edx-name-affirmation-2.3.6.tar", last modified: Tue Aug  8 10:32:13 2023, max compression
```

## Comparing `edx-name-affirmation-2.3.5.tar` & `edx-name-affirmation-2.3.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14344 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.514957 edx-name-affirmation-2.3.5/edx_name_affirmation/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10886 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.514957 edx-name-affirmation-2.3.5/edx_name_affirmation/conf/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/edx_name_affirmation/conf/locale/
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/conf/locale/config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5906 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0002_verifiednameconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0003_verifiedname_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0004_auto_20210816_0958.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0005_remove_verifiedname_is_verified.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0006_auto_20210830_2029.py
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0007_historicalverifiedname.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/name_change_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/statuses.py
--rw-r--r--   0 runner    (1001) docker     (121)     8612 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13462 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    18769 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2335 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_name_change_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     5395 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)    19334 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    12208 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/edx_name_affirmation/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14344 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2192 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-09 13:46:14.000000 edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-09 13:46:14.518957 edx-name-affirmation-2.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/celery44.in
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/celery44.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/celery50.in
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/celery50.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (121)     7881 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/doc.in
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/pip-tools.txt
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-09 13:46:14.522957 edx-name-affirmation-2.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2022-09-09 13:46:06.000000 edx-name-affirmation-2.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.439544 edx-name-affirmation-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     5668 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14504 2023-08-08 10:32:13.439544 edx-name-affirmation-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5462 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.435544 edx-name-affirmation-2.3.6/edx_name_affirmation/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10886 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.431544 edx-name-affirmation-2.3.6/edx_name_affirmation/conf/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.435544 edx-name-affirmation-2.3.6/edx_name_affirmation/conf/locale/
+-rw-r--r--   0 runner    (1001) docker     (122)     2280 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/conf/locale/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5906 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.435544 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0002_verifiednameconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0003_verifiedname_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0004_auto_20210816_0958.py
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0005_remove_verifiedname_is_verified.py
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0006_auto_20210830_2029.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0007_historicalverifiedname.py
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0008_alter_historicalverifiedname_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2133 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/name_change_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8612 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.439544 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13460 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18726 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_name_change_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19334 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12208 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/edx_name_affirmation/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.435544 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14504 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-08 10:32:13.000000 edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:32:13.439544 edx-name-affirmation-2.3.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/celery53.in
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/celery53.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1310 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7152 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/doc.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5307 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/doc.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/pip-tools.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6303 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-08-08 10:32:13.439544 edx-name-affirmation-2.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2801 2023-08-08 10:32:09.000000 edx-name-affirmation-2.3.6/setup.py
```

### Comparing `edx-name-affirmation-2.3.5/CHANGELOG.rst` & `edx-name-affirmation-2.3.6/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[2.3.6] - 2023-07-28
+~~~~~~~~~~~~~~~~~~~~
+* Upgrade django-simple-history. Added new migration. Fixed packages upgrade issues.
+
 [2.3.5] - 2022-09-09
 ~~~~~~~~~~~~~~~~~~~~
 * Fix bug that prevents a verified name from being updated if the user already has an approved verified name associated with a proctored exam attempt
 
 [2.3.4] - 2022-05-17
 ~~~~~~~~~~~~~~~~~~~~
 * Fix bug that prevents new verified names from being created if the user is trying to verify the same name
```

### Comparing `edx-name-affirmation-2.3.5/LICENSE` & `edx-name-affirmation-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/PKG-INFO` & `edx-name-affirmation-2.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-name-affirmation
-Version: 2.3.5
+Version: 2.3.6
 Summary: Name affirmation app for Open edX
 Home-page: https://github.com/edx/edx-name-affirmation
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: ####################
         edx-name-affirmation
@@ -178,14 +178,18 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [2.3.6] - 2023-07-28
+        ~~~~~~~~~~~~~~~~~~~~
+        * Upgrade django-simple-history. Added new migration. Fixed packages upgrade issues.
+        
         [2.3.5] - 2022-09-09
         ~~~~~~~~~~~~~~~~~~~~
         * Fix bug that prevents a verified name from being updated if the user already has an approved verified name associated with a proctored exam attempt
         
         [2.3.4] - 2022-05-17
         ~~~~~~~~~~~~~~~~~~~~
         * Fix bug that prevents new verified names from being created if the user is trying to verify the same name
```

### Comparing `edx-name-affirmation-2.3.5/README.rst` & `edx-name-affirmation-2.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/admin.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/admin.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/api.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/api.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/apps.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/apps.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/conf/locale/config.yaml` & `edx-name-affirmation-2.3.6/edx_name_affirmation/conf/locale/config.yaml`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/exceptions.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/handlers.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/handlers.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0001_initial.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0002_verifiednameconfig.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0002_verifiednameconfig.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0003_verifiedname_status.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0003_verifiedname_status.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0006_auto_20210830_2029.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0006_auto_20210830_2029.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/migrations/0007_historicalverifiedname.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/migrations/0007_historicalverifiedname.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/models.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/models.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/name_change_validator.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/name_change_validator.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/serializers.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/services.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/services.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/statuses.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/statuses.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tasks.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_api.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
         if create_config:
             VerifiedNameConfig.objects.create(user=self.user, use_verified_name_for_certs=expected_value)
 
         # create config for other user, make sure it is the opposite of the expected value.
         # we want to add an additional config to make sure that caching by user works properly
         other_user = User(username='bobsmith', email='bobsmith@test.com')
         other_user.save()
-        VerifiedNameConfig.objects.create(user=other_user, use_verified_name_for_certs=(not expected_value))
+        VerifiedNameConfig.objects.create(user=other_user, use_verified_name_for_certs=not expected_value)
 
         should_use_for_certs = should_use_verified_name_for_certs(self.user)
         self.assertEqual(should_use_for_certs, expected_value)
 
     def test_create_verified_name_config(self):
         """
         Test that verified name config is created and updated successfully
```

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_handlers.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class SignalTestCase(TestCase):
     """
     Test case for signals.py
     """
 
-    def setUp(self):  # pylint: disable=super-method-not-called
+    def setUp(self):
         self.user = User(username='tester', email='tester@test.com')
         self.user.save()
         self.verified_name = 'Jonathan Smith'
         self.profile_name = 'Jon Smith'
         self.idv_attempt_id = 1111111
         self.proctoring_attempt_id = 2222222
```

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_models.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_name_change_validator.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_name_change_validator.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_services.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_tasks.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 @ddt.ddt
 class TaskTests(TestCase):
     """
     Tests for tasks.py
     """
-    def setUp(self):  # pylint: disable=super-method-not-called
+    def setUp(self):
         self.user = User(username='tester', email='tester@test.com')
         self.user.save()
         self.verified_name_obj = VerifiedName(
           user=self.user, verified_name='Jonathan Doe', profile_name='Jon Doe',
         )
         self.verified_name_obj.save()
         self.idv_attempt_id = 1111111
```

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/test_views.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/tests/utils.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/urls.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/urls.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation/views.py` & `edx-name-affirmation-2.3.6/edx_name_affirmation/views.py`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/PKG-INFO` & `edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-name-affirmation
-Version: 2.3.5
+Version: 2.3.6
 Summary: Name affirmation app for Open edX
 Home-page: https://github.com/edx/edx-name-affirmation
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Description: ####################
         edx-name-affirmation
@@ -178,14 +178,18 @@
            This project adheres to Semantic Versioning (https://semver.org/).
         
         .. There should always be an "Unreleased" section for changes pending release.
         
         Unreleased
         ~~~~~~~~~~
         
+        [2.3.6] - 2023-07-28
+        ~~~~~~~~~~~~~~~~~~~~
+        * Upgrade django-simple-history. Added new migration. Fixed packages upgrade issues.
+        
         [2.3.5] - 2022-09-09
         ~~~~~~~~~~~~~~~~~~~~
         * Fix bug that prevents a verified name from being updated if the user already has an approved verified name associated with a proctored exam attempt
         
         [2.3.4] - 2022-05-17
         ~~~~~~~~~~~~~~~~~~~~
         * Fix bug that prevents new verified names from being created if the user is trying to verify the same name
```

### Comparing `edx-name-affirmation-2.3.5/edx_name_affirmation.egg-info/SOURCES.txt` & `edx-name-affirmation-2.3.6/edx_name_affirmation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,32 +30,32 @@
 edx_name_affirmation/migrations/0001_initial.py
 edx_name_affirmation/migrations/0002_verifiednameconfig.py
 edx_name_affirmation/migrations/0003_verifiedname_status.py
 edx_name_affirmation/migrations/0004_auto_20210816_0958.py
 edx_name_affirmation/migrations/0005_remove_verifiedname_is_verified.py
 edx_name_affirmation/migrations/0006_auto_20210830_2029.py
 edx_name_affirmation/migrations/0007_historicalverifiedname.py
+edx_name_affirmation/migrations/0008_alter_historicalverifiedname_options.py
 edx_name_affirmation/migrations/__init__.py
 edx_name_affirmation/tests/__init__.py
 edx_name_affirmation/tests/test_api.py
 edx_name_affirmation/tests/test_handlers.py
 edx_name_affirmation/tests/test_models.py
 edx_name_affirmation/tests/test_name_change_validator.py
 edx_name_affirmation/tests/test_services.py
 edx_name_affirmation/tests/test_tasks.py
 edx_name_affirmation/tests/test_views.py
 edx_name_affirmation/tests/utils.py
 requirements/base.in
 requirements/base.txt
-requirements/celery44.in
-requirements/celery44.txt
-requirements/celery50.in
-requirements/celery50.txt
+requirements/celery53.in
+requirements/celery53.txt
 requirements/ci.in
 requirements/ci.txt
+requirements/common_constraints.txt
 requirements/constraints.txt
 requirements/dev.in
 requirements/dev.txt
 requirements/doc.in
 requirements/doc.txt
 requirements/pip-tools.in
 requirements/pip-tools.txt
```

### Comparing `edx-name-affirmation-2.3.5/requirements/base.txt` & `edx-name-affirmation-2.3.6/requirements/base.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,208 +1,193 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==5.1.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.7.2
     # via django
-billiard==3.6.4.0
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   celery
+    #   kombu
+billiard==4.1.0
     # via celery
-celery==5.2.7
+celery==5.3.1
     # via
     #   -c requirements/constraints.txt
     #   edx-celeryutils
-certifi==2022.6.15
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==2.1.1
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
     #   edx-django-utils
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
-code-annotations==1.3.0
+code-annotations==1.5.0
     # via edx-toggles
-coreapi==2.3.3
-    # via drf-yasg
-coreschema==0.0.4
-    # via
-    #   coreapi
-    #   drf-yasg
-cryptography==37.0.4
+cryptography==41.0.2
     # via pyjwt
-django==3.2.15
+django==3.2.20
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-config-models
     #   django-crum
     #   django-model-utils
+    #   django-waffle
     #   djangorestframework
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-celeryutils
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
     #   jsonfield
-django-config-models==2.3.0
+django-config-models==2.4.0
     # via -r requirements/base.in
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-toggles
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   edx-celeryutils
-django-simple-history==3.0.0
+django-simple-history==3.1.1
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/constraints.txt
     #   -r requirements/base.in
-django-waffle==3.0.0
+django-waffle==4.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   -r requirements/base.in
     #   django-config-models
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-drf-extensions
 drf-jwt==1.19.2
     # via edx-drf-extensions
-drf-yasg==1.21.3
+drf-yasg==1.21.7
     # via edx-api-doc-tools
-edx-api-doc-tools==1.6.0
+edx-api-doc-tools==1.7.0
     # via -r requirements/base.in
-edx-celeryutils==1.2.1
+edx-celeryutils==1.2.3
     # via -r requirements/base.in
-edx-django-utils==5.0.0
+edx-django-utils==5.6.0
     # via
     #   -r requirements/base.in
     #   django-config-models
     #   edx-drf-extensions
     #   edx-toggles
-edx-drf-extensions==8.2.0
+edx-drf-extensions==8.8.0
     # via -r requirements/base.in
 edx-opaque-keys==2.3.0
     # via edx-drf-extensions
 edx-toggles==5.0.0
     # via -r requirements/base.in
-future==0.18.2
-    # via
-    #   edx-celeryutils
-    #   pyjwkest
-idna==3.3
+idna==3.4
     # via requests
 inflection==0.5.1
     # via drf-yasg
-itypes==1.2.0
-    # via coreapi
 jinja2==3.1.2
-    # via
-    #   code-annotations
-    #   coreschema
+    # via code-annotations
 jsonfield==3.1.0
     # via edx-celeryutils
-kombu==5.2.4
+kombu==5.3.1
     # via celery
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
-newrelic==8.0.0.179
+newrelic==8.9.0
     # via edx-django-utils
-packaging==21.3
+packaging==23.1
     # via drf-yasg
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-prompt-toolkit==3.0.31
+prompt-toolkit==3.0.39
     # via click-repl
-psutil==5.9.1
+psutil==5.9.5
     # via edx-django-utils
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
-    # via pyjwkest
-pyjwkest==1.4.2
-    # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.8.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via edx-django-utils
-pyparsing==3.0.9
-    # via packaging
 python-dateutil==2.8.2
-    # via edx-drf-extensions
-python-slugify==6.1.2
-    # via code-annotations
-pytz==2022.2.1
     # via
     #   celery
+    #   edx-drf-extensions
+python-slugify==8.0.1
+    # via code-annotations
+pytz==2023.3
+    # via
     #   django
     #   djangorestframework
     #   drf-yasg
-pyyaml==6.0
-    # via code-annotations
-requests==2.28.1
+pyyaml==6.0.1
     # via
-    #   coreapi
-    #   edx-drf-extensions
-    #   pyjwkest
-ruamel-yaml==0.17.21
-    # via drf-yasg
-ruamel-yaml-clib==0.2.6
-    # via ruamel-yaml
+    #   code-annotations
+    #   drf-yasg
+requests==2.31.0
+    # via edx-drf-extensions
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
-    #   click-repl
     #   edx-drf-extensions
-    #   pyjwkest
     #   python-dateutil
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
 text-unidecode==1.3
     # via python-slugify
-uritemplate==4.1.1
+typing-extensions==4.7.1
     # via
-    #   coreapi
-    #   drf-yasg
-urllib3==1.26.12
+    #   asgiref
+    #   kombu
+tzdata==2023.3
+    # via
+    #   backports-zoneinfo
+    #   celery
+uritemplate==4.1.1
+    # via drf-yasg
+urllib3==2.0.4
     # via requests
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
```

### Comparing `edx-name-affirmation-2.3.5/requirements/celery50.txt` & `edx-name-affirmation-2.3.6/requirements/celery53.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
 amqp==5.1.1
     # via kombu
-billiard==3.6.4.0
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   celery
+    #   kombu
+billiard==4.1.0
     # via celery
-celery==5.2.7
-    # via -r requirements/celery50.in
-click==8.1.3
+celery==5.3.1
+    # via -r requirements/celery53.in
+click==8.1.6
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
-kombu==5.2.4
+kombu==5.3.1
     # via celery
-prompt-toolkit==3.0.31
+prompt-toolkit==3.0.39
     # via click-repl
-pytz==2022.2.1
+python-dateutil==2.8.2
     # via celery
 six==1.16.0
-    # via click-repl
+    # via python-dateutil
+typing-extensions==4.7.1
+    # via kombu
+tzdata==2023.3
+    # via
+    #   backports-zoneinfo
+    #   celery
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
```

### Comparing `edx-name-affirmation-2.3.5/requirements/dev.txt` & `edx-name-affirmation-2.3.6/requirements/dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,380 +1,345 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-asgiref==3.5.2
+asgiref==3.7.2
     # via
     #   -r requirements/quality.txt
     #   django
-astroid==2.12.5
+astroid==2.15.6
     # via
     #   -r requirements/quality.txt
     #   pylint
     #   pylint-celery
-bleach==5.0.1
+bleach==6.0.0
     # via
     #   -r requirements/quality.txt
     #   readme-renderer
-build==0.8.0
+build==0.10.0
     # via
     #   -r requirements/pip-tools.txt
     #   pip-tools
-certifi==2022.6.15
+certifi==2023.7.22
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   requests
-cffi==1.15.1
-    # via
-    #   -r requirements/quality.txt
-    #   cryptography
-chardet==5.0.0
+chardet==5.1.0
     # via diff-cover
-charset-normalizer==2.1.1
+charset-normalizer==3.2.0
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   requests
-click==8.1.3
+click==8.1.6
     # via
     #   -r requirements/pip-tools.txt
     #   -r requirements/quality.txt
     #   click-log
     #   code-annotations
     #   edx-lint
     #   pip-tools
     #   typer
 click-log==0.4.0
     # via
     #   -r requirements/quality.txt
     #   edx-lint
-code-annotations==1.3.0
+code-annotations==1.5.0
     # via
     #   -r requirements/quality.txt
     #   edx-lint
-codecov==2.1.12
-    # via -r requirements/ci.txt
-colorama==0.4.5
+colorama==0.4.6
     # via
     #   -r requirements/quality.txt
     #   typer
 commonmark==0.9.1
     # via
     #   -r requirements/quality.txt
     #   rich
-coverage==6.4.4
-    # via
-    #   -r requirements/ci.txt
-    #   codecov
-cryptography==37.0.4
-    # via
-    #   -r requirements/quality.txt
-    #   secretstorage
-diff-cover==6.5.1
+diff-cover==7.7.0
     # via -r requirements/dev.in
-dill==0.3.5.1
+dill==0.3.7
     # via
     #   -r requirements/quality.txt
     #   pylint
-distlib==0.3.6
+distlib==0.3.7
     # via
     #   -r requirements/ci.txt
     #   virtualenv
-django==3.2.15
+django==3.2.20
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/common_constraints.txt
     #   -r requirements/quality.txt
     #   edx-i18n-tools
-docutils==0.18.1
+docutils==0.19
     # via
     #   -r requirements/quality.txt
     #   readme-renderer
-    #   rstcheck
     #   rstcheck-core
-edx-i18n-tools==0.9.1
+edx-i18n-tools==1.0.0
     # via -r requirements/dev.in
-edx-lint==5.2.4
+edx-lint==5.3.4
     # via -r requirements/quality.txt
-filelock==3.8.0
+filelock==3.12.2
     # via
     #   -r requirements/ci.txt
     #   tox
     #   virtualenv
-idna==3.3
+idna==3.4
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   requests
-importlib-metadata==4.12.0
+importlib-metadata==6.8.0
     # via
     #   -r requirements/quality.txt
     #   keyring
     #   twine
-isort==5.10.1
+importlib-resources==6.0.0
     # via
     #   -r requirements/quality.txt
-    #   pylint
-jaraco-classes==3.2.2
+    #   keyring
+isort==5.12.0
     # via
     #   -r requirements/quality.txt
-    #   keyring
-jeepney==0.8.0
+    #   pylint
+jaraco-classes==3.3.0
     # via
     #   -r requirements/quality.txt
     #   keyring
-    #   secretstorage
 jinja2==3.1.2
     # via
     #   -r requirements/quality.txt
     #   code-annotations
     #   diff-cover
-keyring==23.9.0
+keyring==24.2.0
     # via
     #   -r requirements/quality.txt
     #   twine
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via
     #   -r requirements/quality.txt
     #   astroid
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via
     #   -r requirements/quality.txt
     #   jinja2
 mccabe==0.7.0
     # via
     #   -r requirements/quality.txt
     #   pylint
-more-itertools==8.14.0
+more-itertools==10.0.0
     # via
     #   -r requirements/quality.txt
     #   jaraco-classes
-packaging==21.3
+packaging==23.1
     # via
     #   -r requirements/ci.txt
     #   -r requirements/pip-tools.txt
     #   build
     #   tox
-path==16.4.0
+path==16.7.1
     # via edx-i18n-tools
-pbr==5.10.0
+pbr==5.11.1
     # via
     #   -r requirements/quality.txt
     #   stevedore
-pep517==0.13.0
-    # via
-    #   -r requirements/pip-tools.txt
-    #   build
-pip-tools==6.8.0
+pip-tools==7.1.0
     # via -r requirements/pip-tools.txt
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via
     #   -r requirements/quality.txt
     #   twine
-platformdirs==2.5.2
+platformdirs==3.10.0
     # via
     #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   pylint
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -r requirements/ci.txt
     #   diff-cover
     #   tox
-polib==1.1.1
+polib==1.2.0
     # via edx-i18n-tools
 py==1.11.0
     # via
     #   -r requirements/ci.txt
     #   tox
-pycodestyle==2.9.1
+pycodestyle==2.11.0
     # via -r requirements/quality.txt
-pycparser==2.21
+pydantic==1.10.12
     # via
     #   -r requirements/quality.txt
-    #   cffi
-pydantic==1.10.1
-    # via
-    #   -r requirements/quality.txt
-    #   rstcheck
     #   rstcheck-core
-pydocstyle==6.1.1
+pydocstyle==6.3.0
     # via -r requirements/quality.txt
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   -r requirements/quality.txt
     #   diff-cover
     #   readme-renderer
     #   rich
-pylint==2.15.0
+pylint==2.17.5
     # via
     #   -r requirements/quality.txt
     #   edx-lint
     #   pylint-celery
     #   pylint-django
     #   pylint-plugin-utils
 pylint-celery==0.3
     # via
     #   -r requirements/quality.txt
     #   edx-lint
 pylint-django==2.5.3
     # via
     #   -r requirements/quality.txt
     #   edx-lint
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.2
     # via
     #   -r requirements/quality.txt
     #   pylint-celery
     #   pylint-django
-pyparsing==3.0.9
+pyproject-hooks==1.0.0
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/pip-tools.txt
-    #   packaging
-python-slugify==6.1.2
+    #   build
+python-slugify==8.0.1
     # via
     #   -r requirements/quality.txt
     #   code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   -r requirements/quality.txt
     #   django
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   -r requirements/quality.txt
     #   code-annotations
     #   edx-i18n-tools
-readme-renderer==37.0
+readme-renderer==40.0
     # via
     #   -r requirements/quality.txt
     #   twine
-requests==2.28.1
+requests==2.31.0
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/quality.txt
-    #   codecov
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via
     #   -r requirements/quality.txt
     #   twine
 rfc3986==2.0.0
     # via
     #   -r requirements/quality.txt
     #   twine
-rich==12.5.1
+rich==12.6.0
     # via
     #   -r requirements/quality.txt
     #   twine
     #   typer
-rstcheck==6.1.0
+rstcheck==6.1.2
     # via -r requirements/quality.txt
-rstcheck-core==1.0.2
+rstcheck-core==1.0.3
     # via
     #   -r requirements/quality.txt
     #   rstcheck
-secretstorage==3.3.3
-    # via
-    #   -r requirements/quality.txt
-    #   keyring
-shellingham==1.5.0
+shellingham==1.5.0.post1
     # via
     #   -r requirements/quality.txt
     #   typer
 six==1.16.0
     # via
     #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   bleach
     #   edx-lint
     #   tox
 snowballstemmer==2.2.0
     # via
     #   -r requirements/quality.txt
     #   pydocstyle
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via
     #   -r requirements/quality.txt
     #   django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   -r requirements/quality.txt
     #   code-annotations
 text-unidecode==1.3
     # via
     #   -r requirements/quality.txt
     #   python-slugify
-toml==0.10.2
-    # via
-    #   -r requirements/ci.txt
-    #   tox
 tomli==2.0.1
     # via
+    #   -r requirements/ci.txt
     #   -r requirements/pip-tools.txt
     #   -r requirements/quality.txt
     #   build
-    #   pep517
+    #   pip-tools
     #   pylint
-tomlkit==0.11.4
+    #   pyproject-hooks
+    #   tox
+tomlkit==0.12.1
     # via
     #   -r requirements/quality.txt
     #   pylint
-tox==3.25.1
+tox==3.28.0
     # via
+    #   -c requirements/common_constraints.txt
     #   -r requirements/ci.txt
     #   tox-battery
 tox-battery==0.6.1
     # via
     #   -r requirements/ci.txt
     #   -r requirements/dev.in
-twine==4.0.1
+twine==4.0.2
     # via -r requirements/quality.txt
-typer[all]==0.6.1
+typer[all]==0.7.0
     # via
     #   -r requirements/quality.txt
     #   rstcheck
-types-docutils==0.18.3
+types-docutils==0.19.1.9
     # via
     #   -r requirements/quality.txt
-    #   rstcheck
     #   rstcheck-core
-typing-extensions==4.3.0
+typing-extensions==4.7.1
     # via
     #   -r requirements/quality.txt
+    #   asgiref
     #   astroid
     #   pydantic
     #   pylint
     #   rich
-urllib3==1.26.12
+urllib3==2.0.4
     # via
-    #   -r requirements/ci.txt
     #   -r requirements/quality.txt
     #   requests
     #   twine
-virtualenv==20.16.4
+virtualenv==20.24.2
     # via
     #   -r requirements/ci.txt
     #   tox
 webencodings==0.5.1
     # via
     #   -r requirements/quality.txt
     #   bleach
-wheel==0.37.1
+wheel==0.41.0
     # via
     #   -r requirements/pip-tools.txt
     #   pip-tools
-wrapt==1.14.1
+wrapt==1.15.0
     # via
     #   -r requirements/quality.txt
     #   astroid
-zipp==3.8.1
+zipp==3.16.2
     # via
     #   -r requirements/quality.txt
     #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-name-affirmation-2.3.5/requirements/doc.txt` & `edx-name-affirmation-2.3.6/requirements/doc.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,275 +1,262 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
 amqp==5.1.1
     # via kombu
-asgiref==3.5.2
+asgiref==3.7.2
     # via django
-babel==2.10.3
+babel==2.12.1
     # via sphinx
-billiard==3.6.4.0
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   celery
+    #   kombu
+billiard==4.1.0
     # via celery
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-celery==5.2.7
+celery==5.3.1
     # via
     #   -c requirements/constraints.txt
     #   edx-celeryutils
-certifi==2022.6.15
+certifi==2023.7.22
     # via requests
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-charset-normalizer==2.1.1
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
     #   edx-django-utils
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
-code-annotations==1.3.0
+code-annotations==1.5.0
     # via edx-toggles
-coreapi==2.3.3
-    # via drf-yasg
-coreschema==0.0.4
-    # via
-    #   coreapi
-    #   drf-yasg
-cryptography==37.0.4
+cryptography==41.0.2
     # via pyjwt
-django==3.2.15
+django==3.2.20
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-config-models
     #   django-crum
     #   django-model-utils
+    #   django-waffle
     #   djangorestframework
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-celeryutils
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
     #   jsonfield
-django-config-models==2.3.0
+django-config-models==2.4.0
     # via -r requirements/base.in
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-toggles
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.in
     #   edx-celeryutils
-django-simple-history==3.0.0
+django-simple-history==3.1.1
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/constraints.txt
     #   -r requirements/base.in
-django-waffle==3.0.0
+django-waffle==4.0.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   -r requirements/base.in
     #   django-config-models
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-drf-extensions
-doc8==1.0.0
+doc8==1.1.1
     # via -r requirements/doc.in
 docutils==0.19
     # via
     #   doc8
     #   readme-renderer
     #   restructuredtext-lint
     #   sphinx
 drf-jwt==1.19.2
     # via edx-drf-extensions
-drf-yasg==1.21.3
+drf-yasg==1.21.7
     # via edx-api-doc-tools
-edx-api-doc-tools==1.6.0
+edx-api-doc-tools==1.7.0
     # via -r requirements/base.in
-edx-celeryutils==1.2.1
+edx-celeryutils==1.2.3
     # via -r requirements/base.in
-edx-django-utils==5.0.0
+edx-django-utils==5.6.0
     # via
     #   -r requirements/base.in
     #   django-config-models
     #   edx-drf-extensions
     #   edx-toggles
-edx-drf-extensions==8.2.0
+edx-drf-extensions==8.8.0
     # via -r requirements/base.in
 edx-opaque-keys==2.3.0
     # via edx-drf-extensions
-edx-sphinx-theme==3.0.0
+edx-sphinx-theme==3.1.0
     # via -r requirements/doc.in
 edx-toggles==5.0.0
     # via -r requirements/base.in
-future==0.18.2
-    # via
-    #   edx-celeryutils
-    #   pyjwkest
-idna==3.3
+idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==4.12.0
+importlib-metadata==6.8.0
     # via sphinx
 inflection==0.5.1
     # via drf-yasg
-itypes==1.2.0
-    # via coreapi
 jinja2==3.1.2
     # via
     #   code-annotations
-    #   coreschema
     #   sphinx
 jsonfield==3.1.0
     # via edx-celeryutils
-kombu==5.2.4
+kombu==5.3.1
     # via celery
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
-newrelic==8.0.0.179
+newrelic==8.9.0
     # via edx-django-utils
-packaging==21.3
+packaging==23.1
     # via
     #   drf-yasg
     #   sphinx
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
 pockets==0.9.1
     # via sphinxcontrib-napoleon
-prompt-toolkit==3.0.31
+prompt-toolkit==3.0.39
     # via click-repl
-psutil==5.9.1
+psutil==5.9.5
     # via edx-django-utils
 pycparser==2.21
     # via cffi
-pycryptodomex==3.15.0
-    # via pyjwkest
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   doc8
     #   readme-renderer
     #   sphinx
-pyjwkest==1.4.2
-    # via edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.8.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
-pymongo==3.12.3
+pymongo==3.13.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via edx-django-utils
-pyparsing==3.0.9
-    # via packaging
 python-dateutil==2.8.2
-    # via edx-drf-extensions
-python-slugify==6.1.2
+    # via
+    #   celery
+    #   edx-drf-extensions
+python-slugify==8.0.1
     # via code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   babel
-    #   celery
     #   django
     #   djangorestframework
     #   drf-yasg
-pyyaml==6.0
-    # via code-annotations
-readme-renderer==37.0
+pyyaml==6.0.1
+    # via
+    #   code-annotations
+    #   drf-yasg
+readme-renderer==40.0
     # via -r requirements/doc.in
-requests==2.28.1
+requests==2.31.0
     # via
-    #   coreapi
     #   edx-drf-extensions
-    #   pyjwkest
     #   sphinx
 restructuredtext-lint==1.4.0
     # via doc8
-ruamel-yaml==0.17.21
-    # via drf-yasg
-ruamel-yaml-clib==0.2.6
-    # via ruamel-yaml
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   bleach
-    #   click-repl
     #   edx-drf-extensions
     #   edx-sphinx-theme
     #   pockets
-    #   pyjwkest
     #   python-dateutil
     #   sphinxcontrib-napoleon
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==5.1.1
+sphinx==5.3.0
     # via
     #   -r requirements/doc.in
     #   edx-sphinx-theme
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-napoleon==0.7
     # via -r requirements/doc.in
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   code-annotations
     #   doc8
     #   edx-django-utils
     #   edx-opaque-keys
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via doc8
-uritemplate==4.1.1
+typing-extensions==4.7.1
     # via
-    #   coreapi
-    #   drf-yasg
-urllib3==1.26.12
+    #   asgiref
+    #   kombu
+tzdata==2023.3
+    # via
+    #   backports-zoneinfo
+    #   celery
+uritemplate==4.1.1
+    # via drf-yasg
+urllib3==2.0.4
     # via requests
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
-zipp==3.8.1
+zipp==3.16.2
     # via importlib-metadata
```

### Comparing `edx-name-affirmation-2.3.5/requirements/quality.txt` & `edx-name-affirmation-2.3.6/requirements/quality.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,179 +1,167 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
-asgiref==3.5.2
+asgiref==3.7.2
     # via django
-astroid==2.12.5
+astroid==2.15.6
     # via
     #   pylint
     #   pylint-celery
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-certifi==2022.6.15
+certifi==2023.7.22
     # via requests
-cffi==1.15.1
-    # via cryptography
-charset-normalizer==2.1.1
+charset-normalizer==3.2.0
     # via requests
-click==8.1.3
+click==8.1.6
     # via
     #   click-log
     #   code-annotations
     #   edx-lint
     #   typer
 click-log==0.4.0
     # via edx-lint
-code-annotations==1.3.0
+code-annotations==1.5.0
     # via edx-lint
-colorama==0.4.5
+colorama==0.4.6
     # via typer
 commonmark==0.9.1
     # via rich
-cryptography==37.0.4
-    # via secretstorage
-dill==0.3.5.1
+dill==0.3.7
     # via pylint
-django==3.2.15
+django==3.2.20
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/common_constraints.txt
     #   -r requirements/quality.in
-docutils==0.18.1
+docutils==0.19
     # via
     #   readme-renderer
-    #   rstcheck
     #   rstcheck-core
-edx-lint==5.2.4
+edx-lint==5.3.4
     # via -r requirements/quality.in
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.12.0
+importlib-metadata==6.8.0
     # via
     #   keyring
     #   twine
-isort==5.10.1
+importlib-resources==6.0.0
+    # via keyring
+isort==5.12.0
     # via
     #   -r requirements/quality.in
     #   pylint
-jaraco-classes==3.2.2
+jaraco-classes==3.3.0
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
 jinja2==3.1.2
     # via code-annotations
-keyring==23.9.0
+keyring==24.2.0
     # via twine
-lazy-object-proxy==1.7.1
+lazy-object-proxy==1.9.0
     # via astroid
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via jinja2
 mccabe==0.7.0
     # via pylint
-more-itertools==8.14.0
+more-itertools==10.0.0
     # via jaraco-classes
-pbr==5.10.0
+pbr==5.11.1
     # via stevedore
-pkginfo==1.8.3
+pkginfo==1.9.6
     # via twine
-platformdirs==2.5.2
+platformdirs==3.10.0
     # via pylint
-pycodestyle==2.9.1
+pycodestyle==2.11.0
     # via -r requirements/quality.in
-pycparser==2.21
-    # via cffi
-pydantic==1.10.1
-    # via
-    #   rstcheck
-    #   rstcheck-core
-pydocstyle==6.1.1
+pydantic==1.10.12
+    # via rstcheck-core
+pydocstyle==6.3.0
     # via -r requirements/quality.in
-pygments==2.13.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pylint==2.15.0
+pylint==2.17.5
     # via
     #   edx-lint
     #   pylint-celery
     #   pylint-django
     #   pylint-plugin-utils
 pylint-celery==0.3
     # via edx-lint
 pylint-django==2.5.3
     # via edx-lint
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.2
     # via
     #   pylint-celery
     #   pylint-django
-python-slugify==6.1.2
+python-slugify==8.0.1
     # via code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via django
-pyyaml==6.0
+pyyaml==6.0.1
     # via code-annotations
-readme-renderer==37.0
+readme-renderer==40.0
     # via twine
-requests==2.28.1
+requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.5.1
+rich==12.6.0
     # via
     #   twine
     #   typer
-rstcheck==6.1.0
+rstcheck==6.1.2
     # via -r requirements/quality.in
-rstcheck-core==1.0.2
+rstcheck-core==1.0.3
     # via rstcheck
-secretstorage==3.3.3
-    # via keyring
-shellingham==1.5.0
+shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   bleach
     #   edx-lint
 snowballstemmer==2.2.0
     # via pydocstyle
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via django
-stevedore==4.0.0
+stevedore==5.1.0
     # via code-annotations
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via pylint
-tomlkit==0.11.4
+tomlkit==0.12.1
     # via pylint
-twine==4.0.1
+twine==4.0.2
     # via -r requirements/quality.in
-typer[all]==0.6.1
+typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.18.3
-    # via
-    #   rstcheck
-    #   rstcheck-core
-typing-extensions==4.3.0
+types-docutils==0.19.1.9
+    # via rstcheck-core
+typing-extensions==4.7.1
     # via
+    #   asgiref
     #   astroid
     #   pydantic
     #   pylint
     #   rich
-urllib3==1.26.12
+urllib3==2.0.4
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-wrapt==1.14.1
+wrapt==1.15.0
     # via astroid
-zipp==3.8.1
-    # via importlib-metadata
+zipp==3.16.2
+    # via
+    #   importlib-metadata
+    #   importlib-resources
```

### Comparing `edx-name-affirmation-2.3.5/requirements/test.txt` & `edx-name-affirmation-2.3.6/requirements/test.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    make upgrade
 #
     # via
     #   -r requirements/base.txt
     #   kombu
-asgiref==3.5.2
+asgiref==3.7.2
     # via
     #   -r requirements/base.txt
     #   django
-attrs==22.1.0
-    # via pytest
+backports-zoneinfo[tzdata]==0.2.1
+    # via
+    #   -r requirements/base.txt
+    #   celery
+    #   kombu
     # via
     #   -r requirements/base.txt
     #   celery
     # via
     #   -c requirements/constraints.txt
     #   -r requirements/base.txt
     #   edx-celeryutils
-certifi==2022.6.15
+certifi==2023.7.22
     # via
     #   -r requirements/base.txt
     #   requests
 cffi==1.15.1
     # via
     #   -r requirements/base.txt
     #   cryptography
     #   pynacl
-charset-normalizer==2.1.1
+charset-normalizer==3.2.0
     # via
     #   -r requirements/base.txt
     #   requests
-click==8.1.3
+click==8.1.6
     # via
     #   -r requirements/base.txt
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   code-annotations
@@ -46,282 +49,250 @@
     # via
     #   -r requirements/base.txt
     #   celery
 click-plugins==1.1.1
     # via
     #   -r requirements/base.txt
     #   celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via
     #   -r requirements/base.txt
     #   celery
-code-annotations==1.3.0
+code-annotations==1.5.0
     # via
     #   -r requirements/base.txt
     #   -r requirements/test.in
     #   edx-toggles
-coreapi==2.3.3
-    # via
-    #   -r requirements/base.txt
-    #   drf-yasg
-coreschema==0.0.4
-    # via
-    #   -r requirements/base.txt
-    #   coreapi
-    #   drf-yasg
-coverage[toml]==6.4.4
+coverage[toml]==7.2.7
     # via pytest-cov
-cryptography==37.0.4
+cryptography==41.0.2
     # via
     #   -r requirements/base.txt
     #   pyjwt
 ddt==1.6.0
     # via -r requirements/test.in
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/common_constraints.txt
     #   -r requirements/base.txt
     #   django-config-models
     #   django-crum
     #   django-model-utils
+    #   django-waffle
     #   djangorestframework
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-celeryutils
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
     #   jsonfield
-django-config-models==2.3.0
+django-config-models==2.4.0
     # via -r requirements/base.txt
 django-crum==0.7.9
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
     #   edx-toggles
-django-model-utils==4.2.0
+django-model-utils==4.3.1
     # via
     #   -r requirements/base.txt
     #   edx-celeryutils
-django-simple-history==3.0.0
+django-simple-history==3.1.1
     # via
-    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+    #   -c requirements/constraints.txt
     #   -r requirements/base.txt
-django-waffle==3.0.0
+django-waffle==4.0.0
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
     #   edx-drf-extensions
     #   edx-toggles
-djangorestframework==3.13.1
+djangorestframework==3.14.0
     # via
     #   -r requirements/base.txt
     #   django-config-models
     #   drf-jwt
     #   drf-yasg
     #   edx-api-doc-tools
     #   edx-drf-extensions
 drf-jwt==1.19.2
     # via
     #   -r requirements/base.txt
     #   edx-drf-extensions
-drf-yasg==1.21.3
+drf-yasg==1.21.7
     # via
     #   -r requirements/base.txt
     #   edx-api-doc-tools
-edx-api-doc-tools==1.6.0
+edx-api-doc-tools==1.7.0
     # via -r requirements/base.txt
-edx-celeryutils==1.2.1
+edx-celeryutils==1.2.3
     # via -r requirements/base.txt
-edx-django-utils==5.0.0
+edx-django-utils==5.6.0
     # via
     #   -r requirements/base.txt
     #   django-config-models
     #   edx-drf-extensions
     #   edx-toggles
-edx-drf-extensions==8.2.0
+edx-drf-extensions==8.8.0
     # via -r requirements/base.txt
 edx-opaque-keys==2.3.0
     # via
     #   -r requirements/base.txt
     #   edx-drf-extensions
 edx-toggles==5.0.0
     # via -r requirements/base.txt
-future==0.18.2
-    # via
-    #   -r requirements/base.txt
-    #   edx-celeryutils
-    #   pyjwkest
-idna==3.3
+exceptiongroup==1.1.2
+    # via pytest
+idna==3.4
     # via
     #   -r requirements/base.txt
     #   requests
 inflection==0.5.1
     # via
     #   -r requirements/base.txt
     #   drf-yasg
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
-itypes==1.2.0
-    # via
-    #   -r requirements/base.txt
-    #   coreapi
 jinja2==3.1.2
     # via
     #   -r requirements/base.txt
     #   code-annotations
-    #   coreschema
 jsonfield==3.1.0
     # via
     #   -r requirements/base.txt
     #   edx-celeryutils
     # via
     #   -r requirements/base.txt
     #   celery
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via
     #   -r requirements/base.txt
     #   jinja2
-mock==4.0.3
+mock==5.1.0
     # via -r requirements/test.in
-newrelic==8.0.0.179
+newrelic==8.9.0
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-packaging==21.3
+packaging==23.1
     # via
     #   -r requirements/base.txt
     #   drf-yasg
     #   pytest
-pbr==5.10.0
+pbr==5.11.1
     # via
     #   -r requirements/base.txt
     #   stevedore
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-prompt-toolkit==3.0.31
+prompt-toolkit==3.0.39
     # via
     #   -r requirements/base.txt
     #   click-repl
-psutil==5.9.1
+psutil==5.9.5
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-py==1.11.0
-    # via pytest
 pycparser==2.21
     # via
     #   -r requirements/base.txt
     #   cffi
-pycryptodomex==3.15.0
-    # via
-    #   -r requirements/base.txt
-    #   pyjwkest
-pyjwkest==1.4.2
-    # via
-    #   -r requirements/base.txt
-    #   edx-drf-extensions
-pyjwt[crypto]==2.4.0
+pyjwt[crypto]==2.8.0
     # via
     #   -r requirements/base.txt
     #   drf-jwt
     #   edx-drf-extensions
-pymongo==3.12.3
+pymongo==3.13.0
     # via
     #   -r requirements/base.txt
     #   edx-opaque-keys
 pynacl==1.5.0
     # via
     #   -r requirements/base.txt
     #   edx-django-utils
-pyparsing==3.0.9
-    # via
-    #   -r requirements/base.txt
-    #   packaging
-pytest==7.1.3
+pytest==7.4.0
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==3.0.0
+pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.5.2
     # via -r requirements/test.in
 python-dateutil==2.8.2
     # via
     #   -r requirements/base.txt
+    #   celery
     #   edx-drf-extensions
-python-slugify==6.1.2
+python-slugify==8.0.1
     # via
     #   -r requirements/base.txt
     #   code-annotations
-pytz==2022.2.1
+pytz==2023.3
     # via
     #   -r requirements/base.txt
-    #   celery
     #   django
     #   djangorestframework
     #   drf-yasg
-pyyaml==6.0
+pyyaml==6.0.1
     # via
     #   -r requirements/base.txt
     #   code-annotations
-requests==2.28.1
-    # via
-    #   -r requirements/base.txt
-    #   coreapi
-    #   edx-drf-extensions
-    #   pyjwkest
-ruamel-yaml==0.17.21
-    # via
-    #   -r requirements/base.txt
     #   drf-yasg
-ruamel-yaml-clib==0.2.6
+requests==2.31.0
     # via
     #   -r requirements/base.txt
-    #   ruamel-yaml
+    #   edx-drf-extensions
 semantic-version==2.10.0
     # via
     #   -r requirements/base.txt
     #   edx-drf-extensions
 six==1.16.0
     # via
     #   -r requirements/base.txt
-    #   click-repl
     #   edx-drf-extensions
-    #   pyjwkest
     #   python-dateutil
-sqlparse==0.4.2
+sqlparse==0.4.4
     # via
     #   -r requirements/base.txt
     #   django
-stevedore==4.0.0
+stevedore==5.1.0
     # via
     #   -r requirements/base.txt
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
 text-unidecode==1.3
     # via
     #   -r requirements/base.txt
     #   python-slugify
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
+typing-extensions==4.7.1
+    # via
+    #   -r requirements/base.txt
+    #   asgiref
+    #   kombu
+tzdata==2023.3
+    # via
+    #   -r requirements/base.txt
+    #   backports-zoneinfo
+    #   celery
 uritemplate==4.1.1
     # via
     #   -r requirements/base.txt
-    #   coreapi
     #   drf-yasg
-urllib3==1.26.12
+urllib3==2.0.4
     # via
     #   -r requirements/base.txt
     #   requests
     # via
     #   -r requirements/base.txt
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via
     #   -r requirements/base.txt
     #   prompt-toolkit
```

### Comparing `edx-name-affirmation-2.3.5/setup.cfg` & `edx-name-affirmation-2.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `edx-name-affirmation-2.3.5/setup.py` & `edx-name-affirmation-2.3.6/setup.py`

 * *Files identical despite different names*

