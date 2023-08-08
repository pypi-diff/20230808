# Comparing `tmp/osidb-bindings-3.3.0.tar.gz` & `tmp/osidb-bindings-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osidb-bindings-3.3.0.tar", last modified: Wed Jun 28 11:35:12 2023, max compression
+gzip compressed data, was "osidb-bindings-3.3.1.tar", last modified: Tue Aug  8 13:56:02 2023, max compression
```

## Comparing `osidb-bindings-3.3.0.tar` & `osidb-bindings-3.3.1.tar`

### file list

```diff
@@ -1,272 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.573502 osidb-bindings-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-28 11:35:12.573502 osidb-bindings-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.533498 osidb-bindings-3.3.0/osidb_bindings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.533498 osidb-bindings-3.3.0/osidb_bindings/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.533498 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.537499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.537499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.537499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.537499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.541499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)    61427 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
--rw-r--r--   0 runner    (1001) docker     (123)    69414 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.541499 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.545500 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_unassigned_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.569502 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affectedness_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/blank_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/epss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/erratum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    31519 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_meta_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    30809 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/impact_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_204.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    21859 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/resolution_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/source_666_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/supported_products.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_unassigned_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/osidb_bindings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.533498 osidb-bindings-3.3.0/osidb_bindings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-28 11:35:12.000000 osidb-bindings-3.3.0/osidb_bindings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-06-28 11:35:12.000000 osidb-bindings-3.3.0/osidb_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:35:12.000000 osidb-bindings-3.3.0/osidb_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-28 11:35:12.000000 osidb-bindings-3.3.0/osidb_bindings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 11:35:12.000000 osidb-bindings-3.3.0/osidb_bindings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:35:12.573502 osidb-bindings-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:35:12.573502 osidb-bindings-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-28 11:34:53.000000 osidb-bindings-3.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.138483 osidb-bindings-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-08 13:56:02.138483 osidb-bindings-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.106482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.110482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61427 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69414 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68643 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.110482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.110482 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_unassigned_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.134483 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18827 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affectedness_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/blank_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/comment_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/epss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/erratum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploit_only_report_data_source_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31519 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_meta_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30809 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post_classification_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_reference_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/impact_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/maturity_preliminary_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/meta_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_trackers_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_204.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21859 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_affectedness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_affect_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_epss_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/resolution_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/source_666_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/supported_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_unassigned_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_obtain_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/osidb_bindings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.102482 osidb-bindings-3.3.1/osidb_bindings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-08 13:56:02.000000 osidb-bindings-3.3.1/osidb_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-08-08 13:56:02.000000 osidb-bindings-3.3.1/osidb_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:56:02.000000 osidb-bindings-3.3.1/osidb_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 13:56:02.000000 osidb-bindings-3.3.1/osidb_bindings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-08 13:56:02.000000 osidb-bindings-3.3.1/osidb_bindings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:56:02.138483 osidb-bindings-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:56:02.138483 osidb-bindings-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-08 13:55:44.000000 osidb-bindings-3.3.1/tests/test_core.py
```

### Comparing `osidb-bindings-3.3.0/LICENSE` & `osidb-bindings-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/PKG-INFO` & `osidb-bindings-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.3.0
+Version: 3.3.1
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.3.0/README.md` & `osidb-bindings-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_refresh_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/auth/auth_token_verify_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/collectors/collectors_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_collect_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_cve_map_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_flaw_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_date_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_explanations_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_report_pending_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/exploits/exploits_api_v1_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/__init__.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/__init__.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_affects_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_comments_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_destroy.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_references_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_flaws_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_manifest_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_schema_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_status_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_api_v1_trackers_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osidb/osidb_whoami_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_adjust_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_api_v1_workflows_retrieve_2.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/osim/osim_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/__init__.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/__init__.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_group_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_assignee_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_comment_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_create.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_flaw_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_status_update.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_unassigned_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_api_v1_task_unassigned_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/api/taskman/taskman_healthy_retrieve.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/client.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/client.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/__init__.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_post.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_post.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/affect_report_data.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/affect_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_refresh_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/auth_token_verify_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_api_v1_status_retrieve_response_200_collectors_item_error.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/collectors_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/comment.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/comment.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/comment_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/comment_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/cv_ev_5_package_versions.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/cv_ev_5_versions.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/epss.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/epss.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/erratum.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/erratum.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploit_only_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_collect_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_cve_map_retrieve_response_200_cves.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_epss_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_flaw_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_data_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_action_required_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_no_action_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_date_retrieve_response_200_not_relevant_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_explanations_retrieve_response_200_explanations_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_report_pending_retrieve_response_200_pending_actions_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/exploits_api_v1_supported_products_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_classification.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_classification.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment_post.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment_post.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_comment_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post_classification.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post_classification.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_post_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_reference.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_reference.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_reference_post.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_reference_post.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/flaw_report_data.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/flaw_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_comment.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_comment.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_fields.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_fields.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_query_result.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_query_result.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_issue_type.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_issue_type.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/jira_user.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/jira_user.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/meta.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/meta.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/meta_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/meta_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_create_response_201.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_destroy_response_204.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_flaw_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_order_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_affects_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_create_response_201.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_comments_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_create_response_201.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_order_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_list_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_create_response_201.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_204.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_destroy_response_204.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_references_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_flaws_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_manifest_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_lang.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_schema_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_status_retrieve_response_200_osidb_service.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_affects_flaw_source.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_order_item.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_list_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_api_v1_trackers_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osidb_whoami_retrieve_response_200_profile.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_adjust_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_2_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_api_v1_workflows_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/osim_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_affect_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_affect_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_epss_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_epss_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_exploit_only_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_comment_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_reference_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_flaw_report_data_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_supported_products_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/paginated_tracker_list.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/source_666_enum.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/source_666_enum.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/supported_products.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/supported_products.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_group_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_assignee_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_comment_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_create_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_flaw_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_status_update_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_unassigned_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_api_v1_task_unassigned_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/taskman_healthy_retrieve_response_200.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_obtain_pair.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_obtain_pair.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_refresh.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_refresh.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/token_verify.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/token_verify.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker_meta_attr.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/models/tracker_report_data.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/models/tracker_report_data.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/bindings/python_client/types.py` & `osidb-bindings-3.3.1/osidb_bindings/bindings/python_client/types.py`

 * *Files identical despite different names*

### Comparing `osidb-bindings-3.3.0/osidb_bindings/session.py` & `osidb-bindings-3.3.1/osidb_bindings/session.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+osidb-bindings session
+"""
+
+
 import importlib
 import os
 import re
 from functools import partial
 from types import ModuleType
 from typing import Any, Callable, Dict, List
 
@@ -17,38 +22,52 @@
 from .bindings.python_client.types import UNSET
 from .constants import (
     ALL_SESSION_OPERATIONS,
     OSIDB_API_VERSION,
     OSIDB_BINDINGS_API_PATH,
     OSIDB_BINDINGS_USERAGENT,
 )
+from .exceptions import OperationUnsupported, UndefinedRequestBody
+from .iterators import Paginator
 
 osidb_status_retrieve = importlib.import_module(
     f"{OSIDB_BINDINGS_API_PATH}.osidb_api_{OSIDB_API_VERSION}_status_retrieve",
     package="osidb_bindings",
 )
 
 
-class OperationUnsupported(Exception):
-    """Session operation is unsupported exception"""
+def double_underscores_to_single_underscores(fn):
+    """
+    Function decorator which changes all the keyword arguments which include
+    double underscore to use single underscore instead.
 
+    eg. affect__affectedness -> affect_affectedness
 
-class UndefinedRequestBody(Exception):
-    """
-    Request body is not defined for the particular
-    resource and operation combination
+    This change is needed because in OpenAPI schema query parameters might contain
+    double underscore, howerver OpenAPI Python Client package converts all these
+    double underscores into single ones and thus this creates a confusion as user
+    tries to use query parameter from the OpenAPI schema specification unaware of
+    the underscore change.
     """
 
+    def inner(*args, **kwargs):
+        new_kwargs = {name.replace("__", "_"): value for name, value in kwargs.items()}
+        return fn(*args, **new_kwargs)
+
+    return inner
+
 
 def get_sync_function(api_module: ModuleType) -> Callable:
     """
     Get 'sync' function from API module if available (response example is defined in schema)
     or get basic 'sync_detailed' function (response example is not defined in schema)
     """
-    return getattr(api_module, "sync", getattr(api_module, "sync_detailed"))
+    return double_underscores_to_single_underscores(
+        getattr(api_module, "sync", getattr(api_module, "sync_detailed"))
+    )
 
 
 def new_session(
     osidb_server_uri,
     password=None,
     username=None,
     verify_ssl=True,
@@ -60,15 +79,17 @@
         # OSIDB instances with the username/password auth for token acquirement
         auth = (username, password)
     else:
 
         # OSIDB instances with the kerberos auth for token acquirement
         auth = "kerberos"
 
-    return Session(base_url=osidb_server_uri, auth=auth, verify_ssl=verify_ssl)
+    return Session(
+        base_url=osidb_server_uri.strip("/"), auth=auth, verify_ssl=verify_ssl
+    )
 
 
 class Session:
     """Simple session wrapper which encapsulates the client"""
 
     def __init__(self, base_url, auth=None, verify_ssl=True):
 
@@ -214,209 +235,140 @@
                 SessionOperationsGroup(
                     client,
                     resource_name=f"{resource_name}_{subresource_name}",
                     **subresource_metadata,
                 ),
             )
 
+    def __raise_operation_unsupported(self, operation_name: str):
+        """Operation unsupported exception shortcut"""
+
+        raise OperationUnsupported(
+            f'Operation "{operation_name}" is not supported for the '
+            f'"{self.resource_name}" resource.'
+        )
+
+    def __raise_undefined_request_body(self, operation_name: str):
+        """Undefined request body shortcut"""
+
+        raise UndefinedRequestBody(
+            f'The request body for the resource "{self.resource_name}" '
+            f'and the operation "{operation_name}" is not defined.'
+        )
+
     def __get_method_module(self, resource_name: str, method: str) -> ModuleType:
         # import endpoint module based on a method
         return importlib.import_module(
             f"{OSIDB_BINDINGS_API_PATH}.osidb_api_{OSIDB_API_VERSION}_{resource_name}_{method}",
             package="osidb_bindings",
         )
 
-    def __make_iterable(self, response, *args, **kwargs):
-        """
-        Populate next, prev and iterator helper methods for paginated responses
-        """
-
-        response.iterator = Paginator(
-            session_operation=self.retrieve_list, init_response=response
-        )
-
-        for param_name, func_name in (("next_", "next"), ("previous", "prev")):
-            kwargs.pop("limit", None)
-            kwargs.pop("offset", None)
-            param = getattr(response, param_name, None)
-            if param is None:
-                setattr(response, func_name, lambda: None)
-            else:
-                limit = re.search("limit=(\d+)", param)
-                if limit is not None:
-                    kwargs["limit"] = limit.group(1)
-                offset = re.search("offset=(\d+)", param)
-                if offset is not None:
-                    kwargs["offset"] = offset.group(1)
-
-                setattr(
-                    response, func_name, partial(self.retrieve_list, *args, **kwargs)
-                )
-
-        return response
-
     # CRUD operations
 
     def retrieve(self, id, *args, **kwargs):
         if "retrieve" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="retrieve"
             )
             sync_fn = get_sync_function(method_module)
             return sync_fn(id, *args, client=self.client(), **kwargs)
         else:
-            raise OperationUnsupported(
-                'Operation "update" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
+            self.__raise_operation_unsupported("retrieve")
 
     def retrieve_list(self, *args, **kwargs):
         if "list" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="list"
             )
             sync_fn = get_sync_function(method_module)
-            return self.__make_iterable(
-                sync_fn(*args, client=self.client(), **kwargs), *args, **kwargs
+            response = sync_fn(*args, client=self.client(), **kwargs)
+            return Paginator.make_response_iterable(
+                response, self.retrieve_list, *args, **kwargs
             )
         else:
-            raise OperationUnsupported(
-                'Operation "update" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
+            self.__raise_operation_unsupported("retrieve_list")
 
     def create(self, form_data: Dict[str, Any], *args, **kwargs):
         if "create" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="create"
             )
             model = getattr(method_module, "REQUEST_BODY_TYPE", None)
             if model is None:
-                raise UndefinedRequestBody(
-                    "There is no defined request body "
-                    f'for the resource "{self.resource_name}" '
-                    'and "create" operation.'
-                )
+                self.__raise_undefined_request_body("create")
 
             transformed_data = model.from_dict(form_data)
             sync_fn = get_sync_function(method_module)
             return sync_fn(
                 *args,
                 client=self.client(),
                 form_data=transformed_data,
                 multipart_data=UNSET,
                 json_body=UNSET,
                 **kwargs,
             )
         else:
-            raise OperationUnsupported(
-                'Operation "update" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
+            self.__raise_operation_unsupported("create")
 
     def update(self, id, form_data: Dict[str, Any], *args, **kwargs):
         if "update" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="update"
             )
             model = getattr(method_module, "REQUEST_BODY_TYPE", None)
             if model is None:
-                raise UndefinedRequestBody(
-                    "There is no defined request body "
-                    f'for the resource "{self.resource_name}" '
-                    'and "update" operation.'
-                )
+                self.__raise_undefined_request_body("update")
 
             transformed_data = model.from_dict(form_data)
             sync_fn = get_sync_function(method_module)
             return sync_fn(
                 id,
                 *args,
                 client=self.client(),
                 form_data=transformed_data,
                 multipart_data=UNSET,
                 json_body=UNSET,
                 **kwargs,
             )
         else:
-            raise OperationUnsupported(
-                'Operation "update" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
+            self.__raise_operation_unsupported("update")
 
     def delete(self, id, *args, **kwargs):
         if "destroy" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="destroy"
             )
             sync_fn = get_sync_function(method_module)
             return sync_fn(
                 id,
                 *args,
                 client=self.client(),
                 **kwargs,
             )
         else:
-            raise OperationUnsupported(
-                'Operation "delete" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
+            self.__raise_operation_unsupported("delete")
 
     # Extra operations
 
     def search(self, searched_text: str):
         if "search" in self.allowed_operations:
             method_module = self.__get_method_module(
                 resource_name=self.resource_name, method="list"
             )
             sync_fn = get_sync_function(method_module)
             return sync_fn(client=self.client(), search=searched_text)
         else:
-            raise OperationUnsupported(
-                'Operation "search" is not supported for the '
-                f'"{self.resource_name}" resource.'
-            )
-
-
-class Paginator:
-    """
-    Iterable for handling API pagination.
-
-    Receives either starting limit and offset or already existing response from which
-    it should continue.
+            self.__raise_operation_unsupported("search")
 
-    It keeps calling `.next()` response until pages are exhausted.
-    """
-
-    def __init__(
-        self,
-        session_operation: Callable,
-        limit: int = 100,
-        offset: int = 0,
-        init_response=None,
-        **kwargs,
-    ):
-        self.session_operation = session_operation
-        self.__init_limit = limit
-        self.__init_offset = offset
-        self.__init_response = init_response
-        self.current_response = init_response
-        self.kwargs = kwargs
-
-    def __iter__(self):
-        self.current_response = self.__init_response
-        return self
-
-    def __next__(self):
-        if self.current_response is None:
-            response = self.session_operation(
-                limit=self.__init_limit, offset=self.__init_offset, **self.kwargs
+    def retrieve_list_iterator(self, *args, **kwargs):
+        if "list" in self.allowed_operations:
+            paginator = Paginator(
+                *args,
+                retrieve_list_fn=self.retrieve_list,
+                **kwargs,
             )
-            self.current_response = response
-            return response
+
+            for page in paginator:
+                for resource in page.results:
+                    yield resource
         else:
-            response = self.current_response.next()
-            if response is not None:
-                self.current_response = response
-                return response
-            else:
-                raise StopIteration
+            self.__raise_operation_unsupported("retrieve_list")
```

### Comparing `osidb-bindings-3.3.0/osidb_bindings.egg-info/PKG-INFO` & `osidb-bindings-3.3.1/osidb_bindings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osidb-bindings
-Version: 3.3.0
+Version: 3.3.1
 Summary: Python bindings for accessing OSIDB API
 Home-page: https://github.com/RedHatProductSecurity/osidb-bindings
 Author: Jakub Frejlach, Red Hat Product Security
 Author-email: jfrejlac@redhat.com
 Project-URL: Changelog, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md
 Project-URL: Source, https://github.com/RedHatProductSecurity/osidb-bindings
```

### Comparing `osidb-bindings-3.3.0/osidb_bindings.egg-info/SOURCES.txt` & `osidb-bindings-3.3.1/osidb_bindings.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.py
 osidb_bindings/__init__.py
 osidb_bindings/constants.py
+osidb_bindings/exceptions.py
+osidb_bindings/iterators.py
 osidb_bindings/session.py
 osidb_bindings/utils.py
 osidb_bindings.egg-info/PKG-INFO
 osidb_bindings.egg-info/SOURCES.txt
 osidb_bindings.egg-info/dependency_links.txt
 osidb_bindings.egg-info/requires.txt
 osidb_bindings.egg-info/top_level.txt
```

### Comparing `osidb-bindings-3.3.0/setup.py` & `osidb-bindings-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="osidb-bindings",
-    version="3.3.0",
+    version="3.3.1",
     author="Jakub Frejlach, Red Hat Product Security",
     author_email="jfrejlac@redhat.com",
     description="Python bindings for accessing OSIDB API",
     url="https://github.com/RedHatProductSecurity/osidb-bindings",
     project_urls={
         "Changelog": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/CHANGELOG.md",
         "Documentation": "https://github.com/RedHatProductSecurity/osidb-bindings/blob/master/TUTORIAL.md",
```

