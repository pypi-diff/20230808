# Comparing `tmp/edx-opaque-keys-2.3.0.tar.gz` & `tmp/edx-opaque-keys-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-opaque-keys-2.3.0.tar", last modified: Fri Jan 28 14:59:21 2022, max compression
+gzip compressed data, was "edx-opaque-keys-2.4.0.tar", last modified: Tue Aug  8 10:51:09 2023, max compression
```

## Comparing `edx-opaque-keys-2.3.0.tar` & `edx-opaque-keys-2.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.245876 edx-opaque-keys-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     4772 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)    34499 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-01-28 14:59:21.245876 edx-opaque-keys-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.237877 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-28 14:59:21.000000 edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/
--rw-r--r--   0 runner    (1001) docker     (121)    15200 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/edx/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11464 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/asides.py
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/block_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/edx/django/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8223 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/django/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9474 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     9889 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)    60884 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7905 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_aside_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_asset_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_block_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    14687 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_block_usage_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)    10459 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_course_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_default_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_deprecated_locations.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_is_course.py
--rw-r--r--   0 runner    (1001) docker     (121)    12532 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_library_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)    10307 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_library_usage_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4921 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_locators.py
--rw-r--r--   0 runner    (1001) docker     (121)     6429 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.241876 edx-opaque-keys-2.3.0/opaque_keys/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12776 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/opaque_keys/tests/test_opaque_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.245876 edx-opaque-keys-2.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/requirements/django.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:21.245876 edx-opaque-keys-2.3.0/settings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-28 14:59:21.245876 edx-opaque-keys-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6345 2022-01-28 14:59:18.000000 edx-opaque-keys-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.099074 edx-opaque-keys-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-08-08 10:51:09.099074 edx-opaque-keys-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-08 10:51:09.000000 edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/
+-rw-r--r--   0 runner    (1001) docker     (122)    15200 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/edx/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11464 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/asides.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3493 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/block_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/edx/django/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8256 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/django/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1862 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9474 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/keys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9889 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60884 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_aside_keys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4907 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_asset_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_block_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14989 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_block_usage_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10459 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_course_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_default_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_deprecated_locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_is_course.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12532 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_library_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10307 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_library_usage_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4921 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_locators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.095074 edx-opaque-keys-2.4.0/opaque_keys/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12777 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/opaque_keys/tests/test_opaque_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.099074 edx-opaque-keys-2.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      933 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/requirements/django.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:09.099074 edx-opaque-keys-2.4.0/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 10:51:09.099074 edx-opaque-keys-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6349 2023-08-08 10:51:02.000000 edx-opaque-keys-2.4.0/setup.py
```

### Comparing `edx-opaque-keys-2.3.0/CHANGELOG.rst` & `edx-opaque-keys-2.4.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# 2.4.0
+
+* Added Support for Django 4.2
+
 # 2.3.0
 
 * Added Support for Django40 and removed Django22, 30 and 31
 
 # 2.2.2
 
 * Moved django pin from django.in to constraint.txt. Upgraded dependencies
```

### Comparing `edx-opaque-keys-2.3.0/LICENSE` & `edx-opaque-keys-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/PKG-INFO` & `edx-opaque-keys-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-opaque-keys
-Version: 2.3.0
+Version: 2.4.0
 Summary: UNKNOWN
-Home-page: https://github.com/edx/opaque-keys
+Home-page: https://github.com/openedx/opaque-keys
 Author: edX
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edx-opaque-keys-2.3.0/README.rst` & `edx-opaque-keys-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 =================================================
 
 Opaque-keys provides the ability to create and introspect course and xblock identities through a
 clear and consistent API. See the code's docstrings for more information.
 
 See the `edx-platform wiki documentation`_ for more detail.
 
-.. |build-status| image:: https://github.com/edx/opaque-keys/workflows/Python%20CI/badge.svg?branch=master
-   :target: https://github.com/edx/opaque-keys/actions?query=workflow%3A%22Python+CI%22
+.. |build-status| image:: https://github.com/openedx/opaque-keys/workflows/Python%20CI/badge.svg?branch=master
+   :target: https://github.com/openedx/opaque-keys/actions?query=workflow%3A%22Python+CI%22
 .. |coverage-status| image:: https://coveralls.io/repos/edx/opaque-keys/badge.svg?branch=master
    :target: https://coveralls.io/r/edx/opaque-keys
-.. _`edx-platform wiki documentation`: https://github.com/edx/edx-platform/wiki/Opaque-Keys-(Locators)
+.. _`edx-platform wiki documentation`: https://github.com/openedx/edx-platform/wiki/Opaque-Keys-(Locators)
```

### Comparing `edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/PKG-INFO` & `edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-opaque-keys
-Version: 2.3.0
+Version: 2.4.0
 Summary: UNKNOWN
-Home-page: https://github.com/edx/opaque-keys
+Home-page: https://github.com/openedx/opaque-keys
 Author: edX
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/SOURCES.txt` & `edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/edx_opaque_keys.egg-info/entry_points.txt` & `edx-opaque-keys-2.4.0/edx_opaque_keys.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/__init__.py` & `edx-opaque-keys-2.4.0/opaque_keys/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from abc import ABCMeta, abstractmethod
 from functools import total_ordering
 
 # pylint: disable=wrong-import-order
 from _collections import defaultdict
 from stevedore.enabled import EnabledExtensionManager
 
-__version__ = '2.3.0'
+__version__ = '2.4.0'
 
 
 class InvalidKeyError(Exception):
     """
     Raised to indicated that a serialized key isn't valid (wasn't able to be parsed
     by any available providers).
     """
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/asides.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/asides.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/block_types.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/block_types.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/django/models.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/django/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         super().__init__(*args, **kwargs)
 
     def to_python(self, value):
         if value is self.Empty or value is None:
             return None
 
         error_message = f"{value} is not an instance of str or {self.KEY_CLASS}"
-        assert isinstance(value, (str,) + (self.KEY_CLASS,)), error_message
+        assert isinstance(value, (str,) if self.KEY_CLASS is None else (str, self.KEY_CLASS)), error_message
         if value == '':
             # handle empty string for models being created w/o fields populated
             return None
 
         if isinstance(value, str):
             if value.endswith('\n'):
                 # An opaque key with a trailing newline has leaked into the DB.
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/models.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/django/tests/test_models.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/keys.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/keys.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/locations.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/locations.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/locator.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/locator.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/__init__.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     """Base class (with utility methods) for deprecated Location tests"""
     def setUp(self):
         super().setUp()
 
         # Manually invoke the catch_warnings context manager so we can capture DeprecationWarnings
         # during this test run
         self.cws = warnings.catch_warnings()
+        # pylint: disable-next=unnecessary-dunder-call
         self.cws.__enter__()
         # Python 2.7 by default suppresses DeprecationWarnings. Make sure we show these, always, during tests.
         warnings.simplefilter('always', DeprecationWarning)
 
         # Manually exit the catch_warnings context manager when the test is done
+        # pylint: disable-next=unnecessary-dunder-call
         self.addCleanup(self.cws.__exit__)
 
     @contextmanager
     def assertDeprecationWarning(self, count=1):
         """Asserts that the contained code raises `count` deprecation warnings"""
         with warnings.catch_warnings(record=True) as caught:
             yield
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_aside_keys.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_aside_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,21 @@
     def test_join_v1_roundtrip(self, left, right):
         assume(not left.endswith(':'))
         assume('::' not in left)
         joined = _join_keys_v1(left, right)
         (_left, _right) = _split_keys_v1(joined)
         self.assertEqual((left, right), (_left, _right))
 
+    @given(left=ENCODING_TEXT, right=ENCODING_TEXT)
+    @settings(suppress_health_check=[HealthCheck.too_slow, HealthCheck.filter_too_much])
+    def test_join_v1_error(self, left, right):
+        assume(left.endswith(':'))
+        assume('::' in left)
+        self.assertRaises(ValueError, _join_keys_v1, left, right)
+
     @given(text=ENCODING_TEXT)
     @settings(suppress_health_check=[HealthCheck.too_slow])
     def test_decode_v1_roundtrip(self, text):
         """
         Test all combinations that include characters we're trying to encode, or using in the encoding.
         """
         try:
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_asset_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_asset_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_block_types.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_block_types.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_block_usage_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_block_usage_locators.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,7 +376,19 @@
             BlockUsageLocator(
                 CourseLocator('org', 'course', 'run'),
                 'problem',
                 local_id
             ).block_id,
             local_id
         )
+
+    def test_local_id_str(self):
+        local_id = LocalId()
+        test_id = BlockUsageLocator(
+            CourseLocator('org', 'course', 'run'),
+            'problem',
+            local_id
+        ).block_id
+        self.assertEqual(
+            f"{test_id}",
+            str(local_id)
+        )
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_course_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_course_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_default_deprecated.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_default_deprecated.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_deprecated_locations.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_deprecated_locations.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_is_course.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_is_course.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_library_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_library_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_library_usage_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_library_usage_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_locators.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/edx/tests/test_properties.py` & `edx-opaque-keys-2.4.0/opaque_keys/edx/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/tests/strategies.py` & `edx-opaque-keys-2.4.0/opaque_keys/tests/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,9 +378,9 @@
     This is only used for property-based testing.
     """
     if blacklist is None:
         blacklist = ()
     return strategies.one_of(*[
         instances_of_key(extension.plugin)
         for extension in cls._drivers()  # pylint: disable=protected-access
-        if not(issubclass(extension.plugin, blacklist))
+        if not (issubclass(extension.plugin, blacklist))
     ])
```

### Comparing `edx-opaque-keys-2.3.0/opaque_keys/tests/test_opaque_keys.py` & `edx-opaque-keys-2.4.0/opaque_keys/tests/test_opaque_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,16 @@
     def _from_string(cls, serialized):
         try:
             return cls(json.loads(serialized))
         except (ValueError, TypeError) as error:
             raise InvalidKeyError(cls, serialized) from error
 
     def __hash__(self):
-        return hash(type(self)) + sum([hash(elt) for elt in self.value.keys()])  # pylint: disable=no-member
+        # pylint: disable-next=consider-using-generator, no-member
+        return hash(type(self)) + sum([hash(elt) for elt in self.value.keys()])
 # pylint: enable=abstract-method
 
 
 class KeyTests(TestCase):
     """Basic namespace, from_string, and to_string tests."""
     def test_namespace_from_string(self):
         hex_key = DummyKey.from_string('hex:0x10')
```

### Comparing `edx-opaque-keys-2.3.0/requirements/constraints.txt` & `edx-opaque-keys-2.4.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/settings/base.py` & `edx-opaque-keys-2.4.0/settings/base.py`

 * *Files identical despite different names*

### Comparing `edx-opaque-keys-2.3.0/setup.py` & `edx-opaque-keys-2.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 VERSION = get_version("opaque_keys", "__init__.py")
 
 
 setup(
     name='edx-opaque-keys',
     version=VERSION,
     author='edX',
-    url='https://github.com/edx/opaque-keys',
+    url='https://github.com/openedx/opaque-keys',
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Framework :: Django",
```

