# Comparing `tmp/pyatlan-0.4.2.tar.gz` & `tmp/pyatlan-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-0.4.2.tar", last modified: Tue Jul 25 07:53:30 2023, max compression
+gzip compressed data, was "pyatlan-0.4.3.tar", last modified: Tue Aug  8 12:01:24 2023, max compression
```

## Comparing `pyatlan-0.4.2.tar` & `pyatlan-0.4.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-25 07:53:19.000000 pyatlan-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-25 07:53:19.000000 pyatlan-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-25 07:53:19.000000 pyatlan-0.4.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-25 07:53:30.216642 pyatlan-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-25 07:53:19.000000 pyatlan-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.204642 pyatlan-0.4.2/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52173 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/events/atlan_lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/generate_from_typdefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/generator/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    63856 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    60988 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 07:53:19.000000 pyatlan-0.4.2/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.208642 pyatlan-0.4.2/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:53:30.000000 pyatlan-0.4.2/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-25 07:53:19.000000 pyatlan-0.4.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 07:53:19.000000 pyatlan-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 07:53:30.216642 pyatlan-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-25 07:53:19.000000 pyatlan-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.212642 pyatlan-0.4.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    35979 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22401 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/integration/test_sql_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:30.216642 pyatlan-0.4.2/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/model/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    30532 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    36655 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-25 07:53:19.000000 pyatlan-0.4.2/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.988101 pyatlan-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-08-08 12:01:11.000000 pyatlan-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-08 12:01:11.000000 pyatlan-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 12:01:11.000000 pyatlan-0.4.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-08 12:01:24.988101 pyatlan-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-08 12:01:11.000000 pyatlan-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.972100 pyatlan-0.4.3/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.976100 pyatlan-0.4.3/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.976100 pyatlan-0.4.3/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56928 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.976100 pyatlan-0.4.3/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/events/atlan_lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.976100 pyatlan-0.4.3/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/generator/generate_from_typdefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.976100 pyatlan-0.4.3/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/generator/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.980100 pyatlan-0.4.3/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   982643 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63856 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60988 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 12:01:11.000000 pyatlan-0.4.3/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.972100 pyatlan-0.4.3/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-08 12:01:24.000000 pyatlan-0.4.3/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-08 12:01:11.000000 pyatlan-0.4.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 12:01:11.000000 pyatlan-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 12:01:24.988101 pyatlan-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-08 12:01:11.000000 pyatlan-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.980100 pyatlan-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.984101 pyatlan-0.4.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35976 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/integration/test_sql_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.984101 pyatlan-0.4.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:24.988101 pyatlan-0.4.3/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/model/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30512 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30268 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36690 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-08-08 12:01:11.000000 pyatlan-0.4.3/tests/unit/test_utils.py
```

### Comparing `pyatlan-0.4.2/LICENSE` & `pyatlan-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/PKG-INFO` & `pyatlan-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.2
+Version: 0.4.3
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.2/README.md` & `pyatlan-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-0.4.3/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-0.4.3/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/enum_cache.py` & `pyatlan-0.4.3/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/group_cache.py` & `pyatlan-0.4.3/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/role_cache.py` & `pyatlan-0.4.3/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/cache/user_cache.py` & `pyatlan-0.4.3/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/client/atlan.py` & `pyatlan-0.4.3/pyatlan/client/atlan.py`

 * *Files 6% similar despite different names*

```diff
@@ -850,14 +850,38 @@
     def upsert(
         self,
         entity: Union[Asset, list[Asset]],
         replace_atlan_tags: bool = False,
         replace_custom_metadata: bool = False,
         overwrite_custom_metadata: bool = False,
     ) -> AssetMutationResponse:
+        """Deprecated - use save() instead."""
+        return self.save(
+            entity=entity,
+            replace_atlan_tags=replace_atlan_tags,
+            replace_custom_metadata=replace_custom_metadata,
+            overwrite_custom_metadata=overwrite_custom_metadata,
+        )
+
+    def save(
+        self,
+        entity: Union[Asset, list[Asset]],
+        replace_atlan_tags: bool = False,
+        replace_custom_metadata: bool = False,
+        overwrite_custom_metadata: bool = False,
+    ) -> AssetMutationResponse:
+        """If an asset with the same qualified_name exists, updates the existing asset. Otherwise, creates the asset.
+        If an asset does exist, opertionally overwrites any Atlan tags. Custom metadata will either be
+        overwritten or merged depending on the options provided.
+
+        :param entity: one or more assets to save
+        :param replace_atlan_tags: whether to replace AtlanTags during an update (True) or not (False)
+        :param replace_custom_metadata: replaces any custom metadata with non-empty values provided
+        :param overwrite_custom_metadata: overwrites any custom metadata, even with empty values
+        """
         query_params = {
             "replaceClassifications": replace_atlan_tags,
             "replaceBusinessAttributes": replace_custom_metadata,
             "overwriteBusinessAttributes": overwrite_custom_metadata,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
@@ -869,49 +893,121 @@
         request = BulkRequest[Asset](entities=entities)
         raw_json = self._call_api(BULK_UPDATE, query_params, request)
         return AssetMutationResponse(**raw_json)
 
     def upsert_merging_cm(
         self, entity: Union[Asset, list[Asset]], replace_atlan_tags: bool = False
     ) -> AssetMutationResponse:
-        query_params = {
-            "replaceClassifications": replace_atlan_tags,
-            "replaceBusinessAttributes": True,
-            "overwriteBusinessAttributes": False,
-        }
-        entities: list[Asset] = []
-        if isinstance(entity, list):
-            entities.extend(entity)
-        else:
-            entities.append(entity)
-        for asset in entities:
-            asset.validate_required()
-        request = BulkRequest[Asset](entities=entities)
-        raw_json = self._call_api(BULK_UPDATE, query_params, request)
-        return AssetMutationResponse(**raw_json)
+        """Deprecated - use save_merging_cm() instead."""
+        return self.save_merging_cm(
+            entity=entity, replace_atlan_tags=replace_atlan_tags
+        )
+
+    def save_merging_cm(
+        self, entity: Union[Asset, list[Asset]], replace_atlan_tags: bool = False
+    ) -> AssetMutationResponse:
+        """If no asset exists, has the same behavior as the upsert() method, while also setting
+        any custom metadata provided. If an asset does exist, optionally overwrites any Atlan tags.
+        Will merge any provided custom metadata with any custom metadata that already exists on the asset.
+
+        :param entity: one or more assets to save
+        :param replace_atlan_tags: whether to replace AtlanTags during an update (True) or not (False)
+        :returns: details of the created or updated assets
+        """
+        return self.save(
+            entity=entity,
+            replace_atlan_tags=replace_atlan_tags,
+            replace_custom_metadata=True,
+            overwrite_custom_metadata=False,
+        )
+
+    def update_merging_cm(
+        self, entity: Asset, replace_atlan_tags: bool = False
+    ) -> AssetMutationResponse:
+        """If no asset exists, fails with a NotFoundError. Will merge any provided
+        custom metadata with any custom metadata that already exists on the asset.
+        If an asset does exist, optionally overwrites any Atlan tags.
+
+        :param entity: the asset to update
+        :param replace_atlan_tags: whether to replace AtlanTags during an update (True) or not (False)
+        :returns: details of the updated asset
+        :raises NotFoundError: if the asset does not exist (will not create it)
+        """
+        self.get_asset_by_qualified_name(
+            qualified_name=entity.qualified_name,
+            asset_type=type(entity),
+            min_ext_info=True,
+            ignore_relationships=True,
+        )  # Allow this to throw the NotFoundError if the entity does not exist
+        return self.save_merging_cm(
+            entity=entity, replace_atlan_tags=replace_atlan_tags
+        )
 
     def upsert_replacing_cm(
         self, entity: Union[Asset, list[Asset]], replace_atlan_tagss: bool = False
     ) -> AssetMutationResponse:
+        """Deprecated - use save_replacing_cm() instead."""
+        return self.save_replacing_cm(
+            entity=entity, replace_atlan_tags=replace_atlan_tagss
+        )
+
+    def save_replacing_cm(
+        self, entity: Union[Asset, list[Asset]], replace_atlan_tags: bool = False
+    ) -> AssetMutationResponse:
+        """If no asset exists, has the same behavior as the upsert() method, while also setting
+        any custom metadata provided.
+        If an asset does exist, optionally overwrites any Atlan tags.
+        Will overwrite all custom metadata on any existing asset with only the custom metadata provided
+        (wiping out any other custom metadata on an existing asset that is not provided in the request).
+
+        :param entity: one or more assets to save
+        :param replace_atlan_tags: whether to replace AtlanTags during an update (True) or not (False)
+        :returns: details of the created or updated assets
+        """
+
         query_params = {
-            "replaceClassifications": replace_atlan_tagss,
+            "replaceClassifications": replace_atlan_tags,
             "replaceBusinessAttributes": True,
             "overwriteBusinessAttributes": True,
         }
         entities: list[Asset] = []
         if isinstance(entity, list):
             entities.extend(entity)
         else:
             entities.append(entity)
         for asset in entities:
             asset.validate_required()
         request = BulkRequest[Asset](entities=entities)
         raw_json = self._call_api(BULK_UPDATE, query_params, request)
         return AssetMutationResponse(**raw_json)
 
+    def update_replacing_cm(
+        self, entity: Asset, replace_atlan_tags: bool = False
+    ) -> AssetMutationResponse:
+        """If no asset exists, fails with a NotFoundException.
+        Will overwrite all custom metadata on any existing asset with only the custom metadata provided
+        (wiping out any other custom metadata on an existing asset that is not provided in the request).
+        If an asset does exist, optionally overwrites any Atlan tags.
+
+        :param entity: the asset to update
+        :param replace_atlan_tags: whether to replace AtlanTags during an update (True) or not (False)
+        :returns: details of the updated asset
+        :raises NotFoundError: if the asset does not exist (will not create it)
+        """
+
+        self.get_asset_by_qualified_name(
+            qualified_name=entity.qualified_name,
+            asset_type=type(entity),
+            min_ext_info=True,
+            ignore_relationships=True,
+        )  # Allow this to throw the NotFoundError if the entity does not exist
+        return self.save_replacing_cm(
+            entity=entity, replace_atlan_tags=replace_atlan_tags
+        )
+
     def purge_entity_by_guid(self, guid) -> AssetMutationResponse:
         raw_json = self._call_api(
             DELETE_ENTITY_BY_GUID.format_path_with_params(guid),
             {"deleteType": AtlanDeleteType.HARD.value},
         )
         return AssetMutationResponse(**raw_json)
 
@@ -1206,15 +1302,15 @@
         replacement_terms: list[AtlasGlossaryTerm] = []
         if existing_terms := asset.assigned_terms:
             replacement_terms.extend(
                 term for term in existing_terms if term.relationship_status != "DELETED"
             )
         replacement_terms.extend(terms)
         asset.assigned_terms = replacement_terms
-        response = self.upsert(entity=asset)
+        response = self.save(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def replace_terms(
         self,
@@ -1232,15 +1328,15 @@
         elif qualified_name:
             asset = self.get_asset_by_qualified_name(
                 qualified_name=qualified_name, asset_type=asset_type
             )
         else:
             raise ValueError("Either guid or qualified name must be specified")
         asset.assigned_terms = terms
-        response = self.upsert(entity=asset)
+        response = self.save(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def remove_terms(
         self,
@@ -1269,15 +1365,15 @@
             replacement_terms.extend(
                 term
                 for term in existing_terms
                 if term.relationship_status != "DELETED"
                 and term.guid not in guids_to_be_removed
             )
         asset.assigned_terms = replacement_terms
-        response = self.upsert(entity=asset)
+        response = self.save(entity=asset)
         if assets := response.assets_updated(asset_type=asset_type):
             return assets[0]
         return asset
 
     @validate_arguments()
     def find_connections_by_name(
         self,
```

### Comparing `pyatlan-0.4.2/pyatlan/client/constants.py` & `pyatlan-0.4.3/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/error.py` & `pyatlan-0.4.3/pyatlan/error.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/events/atlan_event_handler.py` & `pyatlan-0.4.3/pyatlan/events/atlan_event_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,8 +148,8 @@
 
     def upsert_changes(self, changed_assets: List[Asset]):
         """
         Actually send the changed assets to Atlan so that they are persisted.
         """
         # TODO: Migrate to an AssetBatch once implemented
         for one in changed_assets:
-            self.client.upsert_merging_cm(one)
+            self.client.save_merging_cm(one)
```

### Comparing `pyatlan-0.4.2/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-0.4.3/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/exceptions.py` & `pyatlan-0.4.3/pyatlan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/generator/generate_from_typdefs.py` & `pyatlan-0.4.3/pyatlan/generator/generate_from_typdefs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/assets.py` & `pyatlan-0.4.3/pyatlan/model/assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/atlan_image.py` & `pyatlan-0.4.3/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/core.py` & `pyatlan-0.4.3/pyatlan/model/core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/custom_metadata.py` & `pyatlan-0.4.3/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/enums.py` & `pyatlan-0.4.3/pyatlan/model/enums.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/events.py` & `pyatlan-0.4.3/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/group.py` & `pyatlan-0.4.3/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/keycloak_events.py` & `pyatlan-0.4.3/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/lineage.py` & `pyatlan-0.4.3/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/query.py` & `pyatlan-0.4.3/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/response.py` & `pyatlan-0.4.3/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/role.py` & `pyatlan-0.4.3/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/search.py` & `pyatlan-0.4.3/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/structs.py` & `pyatlan-0.4.3/pyatlan/model/structs.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/typedef.py` & `pyatlan-0.4.3/pyatlan/model/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/model/user.py` & `pyatlan-0.4.3/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/multipart_data_generator.py` & `pyatlan-0.4.3/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan/utils.py` & `pyatlan-0.4.3/pyatlan/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/pyatlan.egg-info/PKG-INFO` & `pyatlan-0.4.3/pyatlan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 0.4.2
+Version: 0.4.3
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyatlan-0.4.2/pyatlan.egg-info/SOURCES.txt` & `pyatlan-0.4.3/pyatlan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/setup.py` & `pyatlan-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/integration/admin_test.py` & `pyatlan-0.4.3/tests/integration/admin_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
+from datetime import datetime, timedelta
 from typing import Generator, Optional
 
 import pytest
 from pydantic import StrictStr
 
 from pyatlan.cache.role_cache import RoleCache
 from pyatlan.client.atlan import AtlanClient
 from pyatlan.model.group import AtlanGroup, CreateGroupResponse
 from pyatlan.model.keycloak_events import AdminEventRequest, KeycloakEventRequest
 from pyatlan.model.user import AtlanUser
 from tests.integration.client import TestId
 
+TODAY = datetime.now().strftime("%Y-%m-%d")
+YESTERDAY = (datetime.now() - timedelta(days=1)).strftime("%Y-%m-%d")
 MODULE_NAME = TestId.make_unique("Admin")
 GROUP_NAME1 = f"{MODULE_NAME}1"
 GROUP_NAME2 = f"{MODULE_NAME}2"
 
 EMAIL_DOMAIN = f"@{TestId.make_unique('example').replace('_','')}.com"
 USER_EMAIL1 = GROUP_NAME1 + EMAIL_DOMAIN
 USER_EMAIL2 = GROUP_NAME2 + EMAIL_DOMAIN
@@ -282,28 +285,28 @@
 
 
 @pytest.mark.order(after="test_final_user_state")
 def test_retrieve_logs(
     client: AtlanClient,
     users: list[AtlanUser],
 ):
-    request = KeycloakEventRequest(date_from="2023-07-12", date_to="2023-07-13")
+    request = KeycloakEventRequest(date_from=YESTERDAY, date_to=TODAY)
     events = client.get_keycloak_events(request)
     assert events
     count = 0
     for _ in events:
         count += 1
     assert count > 0
 
 
 @pytest.mark.order(after="test_final_user_state")
 def test_retrieve_admin_logs(
     client: AtlanClient,
     users: list[AtlanUser],
 ):
-    request = AdminEventRequest(date_from="2023-07-12", date_to="2023-07-13")
+    request = AdminEventRequest(date_from=YESTERDAY, date_to=TODAY)
     events = client.get_admin_events(request)
     assert events
     count = 0
     for _ in events:
         count += 1
     assert count > 0
```

### Comparing `pyatlan-0.4.2/tests/integration/atlan_tag_test.py` & `pyatlan-0.4.3/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/integration/client.py` & `pyatlan-0.4.3/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/integration/connection_test.py` & `pyatlan-0.4.3/tests/integration/connection_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def create_connection(
     client: AtlanClient, name: str, connector_type: AtlanConnectorType
 ) -> Connection:
     admin_role_guid = str(RoleCache.get_id_for_name("$admin"))
     to_create = Connection.create(
         name=name, connector_type=connector_type, admin_roles=[admin_role_guid]
     )
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     result = response.assets_created(asset_type=Connection)[0]
     return client.get_asset_by_guid(result.guid, asset_type=Connection)
 
 
 def test_invalid_connection(client: AtlanClient):
     with pytest.raises(
         ValueError, match="One of admin_user, admin_groups or admin_roles is required"
```

### Comparing `pyatlan-0.4.2/tests/integration/custom_metadata_test.py` & `pyatlan-0.4.3/tests/integration/custom_metadata_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,15 +759,15 @@
     raci[CM_ATTR_RACI_CONSULTED] = [group1.name]
     raci[CM_ATTR_RACI_INFORMED] = [group1.name, group2.name]
     raci[CM_ATTR_RACI_EXTRA] = "something extra..."
     to_update = AtlasGlossaryTerm.create_for_modification(
         qualified_name=term.qualified_name, name=term.name, glossary_guid=glossary.guid
     )
     to_update.set_custom_metadata(custom_metadata=raci)
-    response = client.upsert_replacing_cm(to_update, replace_atlan_tagss=False)
+    response = client.update_replacing_cm(to_update, replace_atlan_tags=False)
     assert response
     assert len(response.assets_deleted(asset_type=AtlasGlossaryTerm)) == 0
     assert len(response.assets_created(asset_type=AtlasGlossaryTerm)) == 0
     assert len(response.assets_updated(asset_type=AtlasGlossaryTerm)) == 1
     t = response.assets_updated(asset_type=AtlasGlossaryTerm)[0]
     assert isinstance(t, AtlasGlossaryTerm)
     assert t.guid == term.guid
@@ -976,11 +976,11 @@
                 badge_condition_value="2",
                 badge_condition_colorhex=BadgeConditionColor.RED,
             ),
         ],
     )
     badge.user_description = "How many data quality checks ran against this asset."
     assert badge.status == EntityStatus.ACTIVE
-    response = client.upsert(badge)
+    response = client.save(badge)
     assert (badges := response.assets_created(asset_type=Badge))
     assert len(badges) == 1
     client.purge_entity_by_guid(badges[0].guid)
```

### Comparing `pyatlan-0.4.2/tests/integration/file_test.py` & `pyatlan-0.4.3/tests/integration/file_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 def file(client: AtlanClient, connection: Connection) -> Generator[File, None, None]:
     to_create = File.create(
         name=FILE_NAME,
         connection_qualified_name=connection.qualified_name,
         file_type=FileType.PDF,
     )
     to_create.file_path = "https://www.example.com"
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     result = response.assets_created(asset_type=File)[0]
     yield result
     delete_asset(client, guid=result.guid, asset_type=File)
 
 
 def test_file(
     client: AtlanClient,
```

### Comparing `pyatlan-0.4.2/tests/integration/glossary_test.py` & `pyatlan-0.4.3/tests/integration/glossary_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 
 TERM_NAME1 = f"{MODULE_NAME}1"
 TERM_NAME2 = f"{MODULE_NAME}2"
 
 
 def create_glossary(client: AtlanClient, name: str) -> AtlasGlossary:
     g = AtlasGlossary.create(name=StrictStr(name))
-    r = client.upsert(g)
+    r = client.save(g)
     return r.assets_created(AtlasGlossary)[0]
 
 
 def create_category(
     client: AtlanClient, name: str, glossary: AtlasGlossary
 ) -> AtlasGlossaryCategory:
     c = AtlasGlossaryCategory.create(name=name, anchor=glossary)
-    return client.upsert(c).assets_created(AtlasGlossaryCategory)[0]
+    return client.save(c).assets_created(AtlasGlossaryCategory)[0]
 
 
 def create_term(
     client: AtlanClient, name: str, glossary_guid: str
 ) -> AtlasGlossaryTerm:
     t = AtlasGlossaryTerm.create(
         name=StrictStr(name), glossary_guid=StrictStr(glossary_guid)
     )
-    r = client.upsert(t)
+    r = client.save(t)
     return r.assets_created(AtlasGlossaryTerm)[0]
 
 
 @pytest.fixture(scope="module")
 def glossary(
     client: AtlanClient,
 ) -> Generator[AtlasGlossary, None, None]:
@@ -88,14 +88,29 @@
     client: AtlanClient, glossary: AtlasGlossary
 ) -> Generator[AtlasGlossaryTerm, None, None]:
     t = create_term(client, name=TERM_NAME1, glossary_guid=glossary.guid)
     yield t
     delete_asset(client, guid=t.guid, asset_type=AtlasGlossaryTerm)
 
 
+def test_term_failure(
+    client: AtlanClient,
+    glossary: AtlasGlossary,
+):
+    with pytest.raises(
+        NotFoundError,
+        match="Instance AtlasGlossaryTerm with unique attribute .* does not exist",
+    ):
+        client.update_merging_cm(
+            AtlasGlossaryTerm.create(
+                name=f"{TERM_NAME1} X", glossary_guid=glossary.guid
+            )
+        )
+
+
 def test_term1(
     client: AtlanClient,
     term1: AtlasGlossaryTerm,
     glossary: AtlasGlossary,
 ):
     assert term1.guid
     assert term1.name == TERM_NAME1
@@ -152,26 +167,26 @@
 
 @pytest.mark.order(after="test_read_glossary")
 def test_trim_to_required_glossary(
     client: AtlanClient,
     glossary: AtlasGlossary,
 ):
     glossary = glossary.trim_to_required()
-    response = client.upsert(glossary)
+    response = client.save(glossary)
     assert response.mutated_entities is None
 
 
 @pytest.mark.order(after="test_term1")
 def test_term_trim_to_required(
     client: AtlanClient,
     term1: AtlasGlossaryTerm,
 ):
     term1 = client.get_asset_by_guid(guid=term1.guid, asset_type=AtlasGlossaryTerm)
     term1 = term1.trim_to_required()
-    response = client.upsert(term1)
+    response = client.save(term1)
     assert response.mutated_entities is None
 
 
 def test_find_glossary_by_name(client: AtlanClient, glossary: AtlasGlossary):
     assert glossary.guid == client.find_glossary_by_name(name=glossary.name).guid
```

### Comparing `pyatlan-0.4.2/tests/integration/lineage_test.py` & `pyatlan-0.4.3/tests/integration/lineage_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,28 +60,28 @@
     delete_asset(client, guid=db.guid, asset_type=Database)
 
 
 def create_database(client, connection, database_name: str):
     to_create = Database.create(
         name=database_name, connection_qualified_name=connection.qualified_name
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     return result.assets_created(asset_type=Database)[0]
 
 
 @pytest.fixture(scope="module")
 def schema(
     client: AtlanClient,
     connection: Connection,
     database: Database,
 ) -> Generator[Schema, None, None]:
     to_create = Schema.create(
         name=SCHEMA_NAME, database_qualified_name=database.qualified_name
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     sch = result.assets_created(asset_type=Schema)[0]
     yield sch
     delete_asset(client, guid=sch.guid, asset_type=Schema)
 
 
 @pytest.fixture(scope="module")
 def table(
@@ -89,15 +89,15 @@
     connection: Connection,
     database: Database,
     schema: Schema,
 ) -> Generator[Table, None, None]:
     to_create = Table.create(
         name=TABLE_NAME, schema_qualified_name=schema.qualified_name
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     tbl = result.assets_created(asset_type=Table)[0]
     yield tbl
     delete_asset(client, guid=tbl.guid, asset_type=Table)
 
 
 @pytest.fixture(scope="module")
 def mview(
@@ -105,29 +105,29 @@
     connection: Connection,
     database: Database,
     schema: Schema,
 ) -> Generator[MaterialisedView, None, None]:
     to_create = MaterialisedView.create(
         name=MVIEW_NAME, schema_qualified_name=schema.qualified_name
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     mv = result.assets_created(asset_type=MaterialisedView)[0]
     yield mv
     delete_asset(client, guid=mv.guid, asset_type=MaterialisedView)
 
 
 @pytest.fixture(scope="module")
 def view(
     client: AtlanClient,
     connection: Connection,
     database: Database,
     schema: Schema,
 ) -> Generator[View, None, None]:
     to_create = View.create(name=VIEW_NAME, schema_qualified_name=schema.qualified_name)
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     v = result.assets_created(asset_type=View)[0]
     yield v
     delete_asset(client, guid=v.guid, asset_type=View)
 
 
 @pytest.fixture(scope="module")
 def column1(
@@ -139,15 +139,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME1,
         parent_type=Table,
         parent_qualified_name=table.qualified_name,
         order=1,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def column2(
@@ -159,15 +159,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME2,
         parent_type=Table,
         parent_qualified_name=table.qualified_name,
         order=2,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def column3(
@@ -179,15 +179,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME3,
         parent_type=MaterialisedView,
         parent_qualified_name=mview.qualified_name,
         order=1,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def column4(
@@ -199,15 +199,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME4,
         parent_type=MaterialisedView,
         parent_qualified_name=mview.qualified_name,
         order=2,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def column5(
@@ -219,15 +219,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME5,
         parent_type=View,
         parent_qualified_name=view.qualified_name,
         order=1,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def column6(
@@ -239,15 +239,15 @@
 ) -> Generator[Column, None, None]:
     to_create = Column.create(
         name=COLUMN_NAME6,
         parent_type=View,
         parent_qualified_name=view.qualified_name,
         order=2,
     )
-    result = client.upsert(to_create)
+    result = client.save(to_create)
     c = result.assets_created(asset_type=Column)[0]
     yield c
     delete_asset(client, guid=c.guid, asset_type=Column)
 
 
 @pytest.fixture(scope="module")
 def lineage_start(
@@ -262,15 +262,15 @@
     process_name = f"{table.name} >> {mview.name}"
     to_create = Process.create(
         name=process_name,
         connection_qualified_name=connection.qualified_name,
         inputs=[Table.ref_by_guid(table.guid)],
         outputs=[MaterialisedView.ref_by_guid(mview.guid)],
     )
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     ls = response.assets_created(asset_type=Process)[0]
     yield ls
     delete_asset(client, guid=ls.guid, asset_type=Process)
 
 
 def test_lineage_start(
     client: AtlanClient,
@@ -311,15 +311,15 @@
     process_name = f"{mview.name} >> {view.name}"
     to_create = Process.create(
         name=process_name,
         connection_qualified_name=connection.qualified_name,
         inputs=[MaterialisedView.ref_by_guid(mview.guid)],
         outputs=[View.ref_by_guid(view.guid)],
     )
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     ls = response.assets_created(asset_type=Process)[0]
     yield ls
     delete_asset(client, guid=ls.guid, asset_type=Process)
 
 
 def test_lineage_end(
     client: AtlanClient,
@@ -682,15 +682,15 @@
     lineage_start: Process,
     lineage_end: Process,
 ):
     to_restore = Process.create_for_modification(
         lineage_start.qualified_name, lineage_start.name
     )
     to_restore.status = EntityStatus.ACTIVE
-    client.upsert(to_restore)
+    client.save(to_restore)
     restored = client.get_asset_by_guid(lineage_start.guid, asset_type=Process)
     assert restored
     count = 0
     # TODO: replace with exponential back-off and jitter
     while restored.status == EntityStatus.DELETED:
         time.sleep(2)
         restored = client.get_asset_by_guid(lineage_start.guid, asset_type=Process)
```

### Comparing `pyatlan-0.4.2/tests/integration/persona_test.py` & `pyatlan-0.4.3/tests/integration/persona_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 @pytest.fixture(scope="module")
 def persona(
     client: AtlanClient,
     connection: Connection,
     glossary: AtlasGlossary,
 ) -> Generator[Persona, None, None]:
     to_create = Persona.create(name=MODULE_NAME)
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     p = response.assets_created(asset_type=Persona)[0]
     yield p
     delete_asset(client, guid=p.guid, asset_type=Persona)
 
 
 def test_persona(
     client: AtlanClient,
@@ -82,15 +82,15 @@
     )
     to_update.description = "Now with a description!"
     to_update.deny_asset_tabs = {
         AssetSidebarTab.LINEAGE.value,
         AssetSidebarTab.RELATIONS.value,
         AssetSidebarTab.QUERIES.value,
     }
-    response = client.upsert(to_update)
+    response = client.save(to_update)
     assert response
     updated = response.assets_updated(asset_type=Persona)
     assert updated
     assert len(updated) == 1
     assert updated[0]
     assert updated[0].guid == persona.guid
     assert updated[0].description == "Now with a description!"
@@ -142,15 +142,15 @@
     glossary_policy = Persona.create_glossary_policy(
         name="All glossaries",
         persona_id=persona.guid,
         policy_type=AuthPolicyType.ALLOW,
         actions={PersonaGlossaryAction.CREATE, PersonaGlossaryAction.UPDATE},
         resources={f"entity:{glossary.qualified_name}"},
     )
-    response = client.upsert([metadata, data, glossary_policy])
+    response = client.save([metadata, data, glossary_policy])
     assert response
     personas = response.assets_updated(asset_type=Persona)
     assert personas
     assert len(personas) == 1
     assert personas[0].guid == persona.guid
     policies = response.assets_created(asset_type=AuthPolicy)
     assert policies
```

### Comparing `pyatlan-0.4.2/tests/integration/purpose_test.py` & `pyatlan-0.4.3/tests/integration/purpose_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 @pytest.fixture(scope="module")
 def purpose(
     client: AtlanClient,
     atlan_tag: AtlanTagDef,
 ) -> Generator[Purpose, None, None]:
     to_create = Purpose.create(name=MODULE_NAME, atlan_tags=[atlan_tag.display_name])
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     p = response.assets_created(asset_type=Purpose)[0]
     yield p
     delete_asset(client, guid=p.guid, asset_type=Purpose)
 
 
 def test_purpose(
     client: AtlanClient,
@@ -65,15 +65,15 @@
     )
     to_update.description = "Now with a description!"
     to_update.deny_asset_tabs = {
         AssetSidebarTab.LINEAGE.value,
         AssetSidebarTab.RELATIONS.value,
         AssetSidebarTab.QUERIES.value,
     }
-    response = client.upsert(to_update)
+    response = client.save(to_update)
     assert response
     updated = response.assets_updated(asset_type=Purpose)
     assert updated
     assert len(updated) == 1
     assert updated[0]
     assert updated[0].guid == purpose.guid
     assert updated[0].description == "Now with a description!"
@@ -113,15 +113,15 @@
     data = Purpose.create_data_policy(
         name="Mask the data",
         purpose_id=purpose.guid,
         policy_type=AuthPolicyType.DATAMASK,
         all_users=True,
     )
     data.policy_mask_type = DataMaskingType.HASH
-    response = client.upsert([metadata, data])
+    response = client.save([metadata, data])
     assert response
     purposes = response.assets_updated(asset_type=Purpose)
     assert purposes
     assert len(purposes) == 1
     assert purposes[0].guid == purpose.guid
     policies = response.assets_created(asset_type=AuthPolicy)
     assert policies
```

### Comparing `pyatlan-0.4.2/tests/integration/query_parser_test.py` & `pyatlan-0.4.3/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/integration/s3_asset_test.py` & `pyatlan-0.4.3/tests/integration/s3_asset_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     client: AtlanClient, connection: Connection
 ) -> Generator[S3Bucket, None, None]:
     to_create = S3Bucket.create(
         name=BUCKET_NAME,
         connection_qualified_name=connection.qualified_name,
         aws_arn=BUCKET_ARN,
     )
-    response = client.upsert(to_create)
+    response = client.save(to_create)
     result = response.assets_created(asset_type=S3Bucket)[0]
     yield result
     delete_asset(client, guid=result.guid, asset_type=S3Bucket)
 
 
 def test_bucket(
     client: AtlanClient,
```

### Comparing `pyatlan-0.4.2/tests/integration/test_client.py` & `pyatlan-0.4.3/tests/integration/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     with pytest.raises(
         NotFoundError, match="Given instance guid 76d54dd6 is invalid/not found"
     ):
         client.get_asset_by_guid("76d54dd6", AtlasGlossary)
 
 
 def test_upsert_when_no_changes(client: AtlanClient, glossary: AtlasGlossary):
-    response = client.upsert(glossary)
+    response = client.save(glossary)
     assert not response.guid_assignments
     assert not response.mutated_entities
 
 
 def test_get_by_qualified_name(client: AtlanClient, glossary: AtlasGlossary):
     qualified_name = glossary.qualified_name
     glossary = client.get_asset_by_qualified_name(
```

### Comparing `pyatlan-0.4.2/tests/integration/test_index_search.py` & `pyatlan-0.4.3/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/integration/test_sql_assets.py` & `pyatlan-0.4.3/tests/integration/test_sql_assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 @pytest.fixture(scope="module")
 def upsert(client: AtlanClient):
     guids: list[str] = []
 
     def _upsert(asset: Asset) -> AssetMutationResponse:
-        _response = client.upsert(asset)
+        _response = client.save(asset)
         if (
             _response
             and _response.mutated_entities
             and _response.mutated_entities.CREATE
         ):
             guids.append(_response.mutated_entities.CREATE[0].guid)
         return _response
@@ -328,15 +328,15 @@
         assert TestTable.table is not None
         column = Column.create(
             name=column_name,
             parent_qualified_name=TestTable.table.qualified_name,
             parent_type=Table,
             order=1,
         )
-        response = client.upsert(column)
+        response = client.save(column)
         assert (columns := response.assets_created(asset_type=Column))
         assert len(columns) == 1
         column = client.get_asset_by_guid(asset_type=Column, guid=columns[0].guid)
         table = client.get_asset_by_guid(asset_type=Table, guid=TestTable.table.guid)
         assert table.attributes.columns
         columns = table.attributes.columns
         assert len(columns) == 1
```

### Comparing `pyatlan-0.4.2/tests/unit/conftest.py` & `pyatlan-0.4.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/badge_condition_test.py` & `pyatlan-0.4.3/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/badge_test.py` & `pyatlan-0.4.3/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/column_test.py` & `pyatlan-0.4.3/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/connection_test.py` & `pyatlan-0.4.3/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/constants.py` & `pyatlan-0.4.3/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/database_test.py` & `pyatlan-0.4.3/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/file_test.py` & `pyatlan-0.4.3/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/glossary_category_test.py` & `pyatlan-0.4.3/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/glossary_term_test.py` & `pyatlan-0.4.3/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/glossary_test.py` & `pyatlan-0.4.3/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/materialised_view_test.py` & `pyatlan-0.4.3/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/process_test.py` & `pyatlan-0.4.3/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/readme_test.py` & `pyatlan-0.4.3/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/s3_bucket_test.py` & `pyatlan-0.4.3/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/s3object_test.py` & `pyatlan-0.4.3/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/schema_test.py` & `pyatlan-0.4.3/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/table_test.py` & `pyatlan-0.4.3/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/model/view_test.py` & `pyatlan-0.4.3/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_atlan_tag_name.py` & `pyatlan-0.4.3/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_client.py` & `pyatlan-0.4.3/tests/unit/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,19 +104,19 @@
 def test_append_with_valid_guid_when_no_terms_present_returns_asset_with_given_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
     with patch.multiple(
-        AtlanClient, get_asset_by_guid=DEFAULT, upsert=DEFAULT
+        AtlanClient, get_asset_by_guid=DEFAULT, save=DEFAULT
     ) as mock_methods:
         table = Table()
         mock_methods["get_asset_by_guid"].return_value = table
-        mock_methods["upsert"].return_value.assets_updated.return_value = [table]
+        mock_methods["save"].return_value.assets_updated.return_value = [table]
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.append_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
@@ -126,22 +126,22 @@
 def test_append_with_valid_guid_when_deleted_terms_present_returns_asset_with_given_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
     with patch.multiple(
-        AtlanClient, get_asset_by_guid=DEFAULT, upsert=DEFAULT
+        AtlanClient, get_asset_by_guid=DEFAULT, save=DEFAULT
     ) as mock_methods:
         table = Table(attributes=Table.Attributes())
         term = AtlasGlossaryTerm()
         term.relationship_status = "DELETED"
         table.attributes.meanings = [term]
         mock_methods["get_asset_by_guid"].return_value = table
-        mock_methods["upsert"].return_value.assets_updated.return_value = [table]
+        mock_methods["save"].return_value.assets_updated.return_value = [table]
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.append_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
@@ -151,21 +151,21 @@
 def test_append_with_valid_guid_when_terms_present_returns_asset_with_combined_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
     with patch.multiple(
-        AtlanClient, get_asset_by_guid=DEFAULT, upsert=DEFAULT
+        AtlanClient, get_asset_by_guid=DEFAULT, save=DEFAULT
     ) as mock_methods:
         table = Table(attributes=Table.Attributes())
         exisiting_term = AtlasGlossaryTerm()
         table.attributes.meanings = [exisiting_term]
         mock_methods["get_asset_by_guid"].return_value = table
-        mock_methods["upsert"].return_value.assets_updated.return_value = [table]
+        mock_methods["save"].return_value.assets_updated.return_value = [table]
         client = AtlanClient()
         guid = "123"
 
         new_term = AtlasGlossaryTerm()
         terms = [new_term]
 
         assert (
@@ -234,19 +234,19 @@
 def test_replace_terms(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
     with patch.multiple(
-        AtlanClient, get_asset_by_guid=DEFAULT, upsert=DEFAULT
+        AtlanClient, get_asset_by_guid=DEFAULT, save=DEFAULT
     ) as mock_methods:
         table = Table()
         mock_methods["get_asset_by_guid"].return_value = table
-        mock_methods["upsert"].return_value.assets_updated.return_value = [table]
+        mock_methods["save"].return_value.assets_updated.return_value = [table]
         client = AtlanClient()
         guid = "123"
         terms = [AtlasGlossaryTerm()]
 
         assert (
             asset := client.replace_terms(guid=guid, asset_type=asset_type, terms=terms)
         )
@@ -317,24 +317,24 @@
 def test_remove_with_valid_guid_when_terms_present_returns_asset_with_terms_removed(
     monkeypatch,
 ):
     monkeypatch.setenv("ATLAN_BASE_URL", "https://name.atlan.com")
     monkeypatch.setenv("ATLAN_API_KEY", "abkj")
     asset_type = Table
     with patch.multiple(
-        AtlanClient, get_asset_by_guid=DEFAULT, upsert=DEFAULT
+        AtlanClient, get_asset_by_guid=DEFAULT, save=DEFAULT
     ) as mock_methods:
         table = Table(attributes=Table.Attributes())
         exisiting_term = AtlasGlossaryTerm()
         exisiting_term.guid = "b4113341-251b-4adc-81fb-2420501c30e6"
         other_term = AtlasGlossaryTerm()
         other_term.guid = "b267858d-8316-4c41-a56a-6e9b840cef4a"
         table.attributes.meanings = [exisiting_term, other_term]
         mock_methods["get_asset_by_guid"].return_value = table
-        mock_methods["upsert"].return_value.assets_updated.return_value = [table]
+        mock_methods["save"].return_value.assets_updated.return_value = [table]
         client = AtlanClient()
         guid = "123"
 
         assert (
             asset := client.remove_terms(
                 guid=guid, asset_type=asset_type, terms=[exisiting_term]
             )
```

### Comparing `pyatlan-0.4.2/tests/unit/test_custom_metadata.py` & `pyatlan-0.4.3/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_events.py` & `pyatlan-0.4.3/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_glossary_term.py` & `pyatlan-0.4.3/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_lineage.py` & `pyatlan-0.4.3/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_model.py` & `pyatlan-0.4.3/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_search_model.py` & `pyatlan-0.4.3/tests/unit/test_search_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,18 @@
     },
 }
 
 
 @pytest.mark.parametrize(
     "parameters, expected",
     [
-        ({}, "__init__() missing 2 required positional arguments: 'field' and 'value'"),
+        (
+            {},
+            "__init__() missing 2 required positional arguments: 'field' and 'value'",
+        ),
         (
             [
                 {"field": "bob"},
                 "__init__() missing 1 required positional argument: 'value'",
             ]
         ),
         (
```

### Comparing `pyatlan-0.4.2/tests/unit/test_typedef_model.py` & `pyatlan-0.4.3/tests/unit/test_typedef_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-0.4.2/tests/unit/test_utils.py` & `pyatlan-0.4.3/tests/unit/test_utils.py`

 * *Files identical despite different names*

