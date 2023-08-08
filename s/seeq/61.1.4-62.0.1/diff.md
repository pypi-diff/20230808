# Comparing `tmp/seeq-61.1.4.tar.gz` & `tmp/seeq-62.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seeq-61.1.4.tar", last modified: Tue Aug  1 20:06:26 2023, max compression
+gzip compressed data, was "seeq-62.0.1.tar", last modified: Tue Aug  1 18:09:05 2023, max compression
```

## Comparing `seeq-61.1.4.tar` & `seeq-62.0.1.tar`

### file list

```diff
@@ -1,398 +1,423 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2023-08-01 17:57:45.000000 seeq-61.1.4/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-08-01 17:57:45.000000 seeq-61.1.4/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2023-08-01 20:06:26.000000 seeq-61.1.4/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2023-08-01 17:57:45.000000 seeq-61.1.4/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 17:57:45.000000 seeq-61.1.4/pyproject.toml
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq/sdk/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23508 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq/sdk/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/access_keys_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/add_ons_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   115090 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/agents_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/annotations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/assets_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/audit_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/auth_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27268 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/condition_monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52073 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/api/conditions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   125736 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/content_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/datafiles_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/datasources_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/display_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/displays_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/export_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50020 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/folders_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   103619 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/formulas_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   156487 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/items_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/jobs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21325 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/logs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/metrics_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/networks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/notification_configurations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9809 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/notifier_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/plugins_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/projects_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/report_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/reports_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/requests_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/scalars_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   111618 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/signals_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/subscriptions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   100419 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/system_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19860 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/table_definitions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/trees_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12541 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/usage_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/user_groups_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49743 2023-08-01 18:02:41.000000 seeq-61.1.4/seeq/sdk/api/users_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94110 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/api/workbooks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30236 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9184 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/configuration.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq/sdk/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19297 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/access_key_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/access_key_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/access_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/ace_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/ace_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/acl_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/acl_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/activity_graph_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/activity_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_preview_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_tool_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/add_on_tool_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/administrator_contact_information_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/agent_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/agent_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/agent_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7830 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/agent_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_image_link_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_interest_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_interest_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29168 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/annotation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/archive_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/asset_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/asset_error.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/asset_group_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/asset_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2023-08-01 18:02:35.000000 seeq-61.1.4/seeq/sdk/models/asset_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_group_root_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_group_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_selection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_selection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9347 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_tree_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/asset_tree_single_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/audit_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/audit_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/auth_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/auth_providers_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/cache_info_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/calculated_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsule_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsule_property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8056 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsule_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsules_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10386 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsules_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/capsules_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/channel_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7499 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6960 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4674 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_ancestor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4577 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_concat_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_event_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6087 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_item_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/column_rule_path_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8948 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11131 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18964 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_notification_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_notification_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24429 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/condition_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configuration_option_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configuration_option_output_simple_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configuration_option_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8677 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/configured_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23840 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17187 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connection_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16912 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connection_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connections_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connector_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connector_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/connectors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/content_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/content_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/content_with_metadata_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/content_with_metadata_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2023-08-01 18:02:36.000000 seeq-61.1.4/seeq/sdk/models/csv_datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datafile_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datafiles_csv_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_clean_up_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_clean_up_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13247 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20066 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_statistics_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25918 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasource_summary_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10073 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/datasources_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/date_range_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/date_range_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/detailed_meter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/detailed_timer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/directive_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_template_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/display_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/document_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/email_notification_recipient_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/emailer_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/export_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18835 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/export_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18526 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/export_items_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/export_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/export_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/folded_stack_node_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/folder_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/folder_navigation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/folder_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_compile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_compiler_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_dependency_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_example_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_example_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_summaries_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_doc_summary_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8237 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_example_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_item_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_log_entry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_log_entry_details.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_log_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_package_import_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_package_import_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_package_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_package_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_parameter_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13589 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_run_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_run_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2023-08-01 18:02:37.000000 seeq-61.1.4/seeq/sdk/models/formula_token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/formula_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/formula_upgrade_change_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/formula_upgrade_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/function_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/function_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/function_variant_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/gauge_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/generic_table_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_add_on_tools_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_channels_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_condition_monitor_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_content_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_date_ranges_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_jobs_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_metrics_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_projects_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_requests_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11325 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/get_signals_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/id_images_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/identity_mapping_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/identity_mapping_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/identity_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/identity_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/indexing_parameters_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/installer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/interval_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/invalid_swap_out_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_batch_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_dependency_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_id_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_parameter_of_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_preview_with_assets_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_search_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_search_preview_paginated_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14132 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_search_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_swap_result_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_update_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_user_attributes_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_user_attributes_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/item_with_swap_pairs_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/job_accepted_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/job_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/json_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/license_importer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12576 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/license_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/licensed_feature_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/log_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/meter_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/migrate_editor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitor_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitor_definitions_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12288 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitor_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/monitors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/notifiable_report_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8191 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/notifiable_report_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12017 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/notification_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/optional_report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/parameter_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/permissions_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/plugin_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/plugin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/plugins_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/priority_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/progress_information_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/project_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/project_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/property_href_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/put_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/put_scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7200 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/put_scalars_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/put_signals_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/put_user_groups_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2023-08-01 18:02:38.000000 seeq-61.1.4/seeq/sdk/models/referenced_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/regression_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/remote_agent_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/remote_agent_status_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/remote_agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/report_input_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/report_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/report_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/report_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/sample_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/samples_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/samples_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scalar_evaluate_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5260 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scalar_property_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scalar_value_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scale_across_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedulable_admin_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedulable_admin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedulable_summary_day_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedulable_summary_week_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/schedule_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9014 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scheduled_notebook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scheduled_notebook_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17468 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/scheduled_notebook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/screenshot_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/see_also_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/send_email_attachment_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/send_email_contact_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/send_email_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4682 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/send_logs_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/server_build_info_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/server_load_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/server_spec_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10968 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/server_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/signal_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27753 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/signal_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/signal_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/status_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/status_message_base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/subscription_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/subscription_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/subscription_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/supported_units_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/swap_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/swap_option_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/swap_option_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/swap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/sync_progress.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/sync_progress_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/system_license_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/table_column_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10520 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/table_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/table_definition_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11160 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/table_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/threshold_metric_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/threshold_metric_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/threshold_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/timer_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/tree_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/treemap_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/treemap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/units_of_measure_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/units_of_measure_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/units_of_measure_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/unsubscribe_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/usage_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9112 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/usage_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/usage_types_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_group_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18031 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26275 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/user_password_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/validate_cron_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/validate_cron_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7096 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/validate_cron_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/workbench_item_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/workbench_search_result_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/workbook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/workbook_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2023-08-01 18:02:39.000000 seeq-61.1.4/seeq/sdk/models/workbook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/models/worksheet_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/models/worksheet_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13061 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/models/worksheet_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/models/workstep_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2023-08-01 18:02:40.000000 seeq-61.1.4/seeq/sdk/models/workstep_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13287 2023-08-01 18:02:42.000000 seeq-61.1.4/seeq/sdk/rest.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15639 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-08-01 20:06:26.000000 seeq-61.1.4/seeq.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-01 20:06:26.000000 seeq-61.1.4/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2023-08-01 17:59:54.000000 seeq-61.1.4/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.212312 seeq-62.0.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2023-08-01 15:55:18.000000 seeq-62.0.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-08-01 15:55:18.000000 seeq-62.0.1/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2023-08-01 18:09:05.212312 seeq-62.0.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2023-08-01 15:55:18.000000 seeq-62.0.1/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 15:55:18.000000 seeq-62.0.1/pyproject.toml
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.176310 seeq-62.0.1/seeq/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.176310 seeq-62.0.1/seeq/sdk/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25065 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.184311 seeq-62.0.1/seeq/sdk/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2049 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/access_keys_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/add_ons_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   115090 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/agents_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/annotations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/assets_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/audit_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/auth_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27275 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/condition_monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52073 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/conditions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   125736 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/content_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    88975 2023-08-01 15:58:19.000000 seeq-62.0.1/seeq/sdk/api/context_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/datafiles_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/datasources_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/display_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/displays_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/export_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50020 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/folders_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   103619 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/formulas_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5495 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/graph_ql_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   180714 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/items_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/jobs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21471 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/logs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/metrics_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/networks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/notification_configurations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9809 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/notifier_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/plugins_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/projects_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/report_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/reports_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/requests_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/scalars_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   111618 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/signals_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/subscriptions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   100419 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/system_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19860 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/table_definitions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/trees_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12541 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/usage_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/user_groups_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49743 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/users_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94110 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api/workbooks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30236 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9184 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/configuration.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.212312 seeq-62.0.1/seeq/sdk/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20612 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/access_key_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/access_key_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/access_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/ace_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/ace_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/acl_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/acl_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/activity_graph_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/activity_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/add_on_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/add_on_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/add_on_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/add_on_preview_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2023-08-01 15:58:13.000000 seeq-62.0.1/seeq/sdk/models/add_on_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/add_on_tool_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/add_on_tool_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/administrator_contact_information_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/agent_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/agent_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/agent_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7830 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/agent_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_image_link_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_interest_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_interest_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29166 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/annotation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/archive_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_group_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_group_root_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_group_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_selection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_selection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_tree_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/asset_tree_single_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/attachment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/audit_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/audit_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/auth_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/auth_providers_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/cache_info_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/calculated_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsule_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsule_property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8056 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsule_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsules_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10386 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsules_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/capsules_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/channel_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8308 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7346 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6960 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4700 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_ancestor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4577 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_concat_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_event_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6087 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_item_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/column_rule_path_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9576 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11131 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19957 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_notification_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_notification_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24429 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/condition_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configuration_option_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configuration_option_output_simple_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configuration_option_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8677 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/configured_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2023-08-01 15:58:14.000000 seeq-62.0.1/seeq/sdk/models/connection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23840 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18799 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connection_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16922 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connection_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connections_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connector_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connector_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/connectors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/content_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/content_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/content_with_metadata_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/content_with_metadata_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4040 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_comment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9461 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_comment_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4025 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11197 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4920 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_opaque_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10181 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_opaque_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5958 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/context_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/csv_datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datafile_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datafiles_csv_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_clean_up_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_clean_up_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20066 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_statistics_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26873 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasource_summary_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10073 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/datasources_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/date_range_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/date_range_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/detailed_meter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/detailed_timer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/directive_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_template_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/display_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/document_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/email_notification_recipient_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/emailer_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/export_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21130 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/export_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18526 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/export_items_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/export_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/export_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/folded_stack_node_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/folder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/folder_navigation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/folder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_compile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_compiler_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_dependency_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_example_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_example_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_summaries_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_doc_summary_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8260 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2023-08-01 15:58:15.000000 seeq-62.0.1/seeq/sdk/models/formula_example_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_item_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_log_entry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_log_entry_details.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_log_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_package_import_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_package_import_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_package_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_package_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_parameter_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13589 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_run_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_run_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_upgrade_change_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/formula_upgrade_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/function_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/function_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/function_variant_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/gauge_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/generic_table_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_add_on_tools_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_channels_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_content_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_date_ranges_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_jobs_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_metrics_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_projects_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_requests_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11325 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/get_signals_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3806 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/graph_ql_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3765 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/graph_ql_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/id_images_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/identity_mapping_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/identity_mapping_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/identity_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/identity_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/indexing_parameters_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/installer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/interval_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/invalid_swap_out_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_batch_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_dependency_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_finder_configuration_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8479 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_finder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_finder_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15489 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_finder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_id_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_parameter_of_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_preview_with_assets_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_search_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_search_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_swap_result_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_update_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_user_attributes_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_user_attributes_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/item_with_swap_pairs_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/jira_attachment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6025 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/jira_attachment_media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/job_accepted_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/job_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/json_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3798 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_category_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_category_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_category_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4621 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5063 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/license_importer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12576 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/license_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/licensed_feature_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/log_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2023-08-01 15:58:16.000000 seeq-62.0.1/seeq/sdk/models/meter_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/migrate_editor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitor_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitor_definitions_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12288 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitor_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/monitors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/notifiable_report_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8191 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/notifiable_report_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12017 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/notification_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/optional_report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/parameter_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/permissions_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/plugin_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/plugin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/plugins_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/priority_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/progress_information_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/project_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/project_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/property_href_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/put_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/put_scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5797 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/put_scalars_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/put_signals_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/put_user_groups_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/referenced_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/regression_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/remote_agent_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/remote_agent_status_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/remote_agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/report_input_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/report_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/report_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/report_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/sample_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/samples_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/samples_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scalar_evaluate_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5290 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scalar_property_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scalar_value_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scale_across_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedulable_admin_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedulable_admin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedulable_summary_day_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedulable_summary_week_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/schedule_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9014 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scheduled_notebook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17468 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/scheduled_notebook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/screenshot_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/see_also_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/send_email_attachment_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/send_email_contact_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/send_email_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/server_build_info_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/server_load_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/server_spec_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10968 2023-08-01 15:58:17.000000 seeq-62.0.1/seeq/sdk/models/server_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/signal_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27753 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/signal_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/signal_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/status_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/status_message_base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/subscription_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/subscription_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/subscription_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10912 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/support_request_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4180 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/support_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/supported_units_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/swap_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/swap_option_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/swap_option_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/swap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/sync_progress.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/sync_progress_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/system_license_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/table_column_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10792 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/table_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/table_definition_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12081 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/table_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/threshold_metric_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/threshold_metric_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/threshold_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/timer_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/tree_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/treemap_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/treemap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/units_of_measure_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/units_of_measure_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/units_of_measure_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/unsubscribe_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/usage_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9112 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/usage_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/usage_types_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_group_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18031 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26275 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/user_password_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/validate_cron_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/validate_cron_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7096 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/validate_cron_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workbench_item_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workbench_search_result_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workbook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workbook_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workbook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/worksheet_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/worksheet_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13061 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/worksheet_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workstep_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2023-08-01 15:58:18.000000 seeq-62.0.1/seeq/sdk/models/workstep_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13287 2023-08-01 15:58:20.000000 seeq-62.0.1/seeq/sdk/rest.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-08-01 18:09:05.176310 seeq-62.0.1/seeq.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16675 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-08-01 18:09:05.000000 seeq-62.0.1/seeq.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-08-01 18:09:05.212312 seeq-62.0.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2023-08-01 15:56:50.000000 seeq-62.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `seeq-61.1.4/LICENSE` & `seeq-62.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-61.1.4/PKG-INFO` & `seeq-62.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 61.1.4
+Version: 62.0.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-61.1.4/README.md` & `seeq-62.0.1/README.md`

 * *Files identical despite different names*

### Comparing `seeq-61.1.4/seeq/sdk/__init__.py` & `seeq-62.0.1/seeq/sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "61.1.4"
+__version__ = "62.0.1"
 
 # import apis into sdk package
 from .api.access_keys_api import AccessKeysApi
 from .api.add_ons_api import AddOnsApi
 from .api.agents_api import AgentsApi
 from .api.annotations_api import AnnotationsApi
 from .api.assets_api import AssetsApi
 from .api.audit_api import AuditApi
 from .api.auth_api import AuthApi
 from .api.condition_monitors_api import ConditionMonitorsApi
 from .api.conditions_api import ConditionsApi
 from .api.content_api import ContentApi
+from .api.context_api import ContextApi
 from .api.datafiles_api import DatafilesApi
 from .api.datasources_api import DatasourcesApi
 from .api.display_templates_api import DisplayTemplatesApi
 from .api.displays_api import DisplaysApi
 from .api.export_api import ExportApi
 from .api.folders_api import FoldersApi
 from .api.formulas_api import FormulasApi
+from .api.graph_ql_api import GraphQLApi
 from .api.items_api import ItemsApi
 from .api.jobs_api import JobsApi
 from .api.logs_api import LogsApi
 from .api.metrics_api import MetricsApi
 from .api.monitors_api import MonitorsApi
 from .api.networks_api import NetworksApi
 from .api.notification_configurations_api import NotificationConfigurationsApi
@@ -98,30 +100,31 @@
 from .models.asset_input_v1 import AssetInputV1
 from .models.asset_output_v1 import AssetOutputV1
 from .models.asset_selection_input_v1 import AssetSelectionInputV1
 from .models.asset_selection_output_v1 import AssetSelectionOutputV1
 from .models.asset_tree_batch_input_v1 import AssetTreeBatchInputV1
 from .models.asset_tree_output_v1 import AssetTreeOutputV1
 from .models.asset_tree_single_input_v1 import AssetTreeSingleInputV1
+from .models.attachment_input_v1 import AttachmentInputV1
 from .models.audit_output_list_v1 import AuditOutputListV1
 from .models.audit_output_v1 import AuditOutputV1
 from .models.auth_input_v1 import AuthInputV1
 from .models.auth_providers_output_v1 import AuthProvidersOutputV1
 from .models.cache_info_v1 import CacheInfoV1
 from .models.calculated_item_output_v1 import CalculatedItemOutputV1
 from .models.capsule_input_v1 import CapsuleInputV1
 from .models.capsule_property_input_v1 import CapsulePropertyInputV1
 from .models.capsule_property_output_v1 import CapsulePropertyOutputV1
 from .models.capsule_v1 import CapsuleV1
 from .models.capsules_input_v1 import CapsulesInputV1
 from .models.capsules_output_v1 import CapsulesOutputV1
 from .models.capsules_overwrite_input_v1 import CapsulesOverwriteInputV1
 from .models.channel_output_v1 import ChannelOutputV1
-from .models.column_definition import ColumnDefinition
 from .models.column_definition_input_v1 import ColumnDefinitionInputV1
+from .models.column_definition_output_v1 import ColumnDefinitionOutputV1
 from .models.column_rule import ColumnRule
 from .models.column_rule_ancestor_input_v1 import ColumnRuleAncestorInputV1
 from .models.column_rule_concat_input_v1 import ColumnRuleConcatInputV1
 from .models.column_rule_event_property_input_v1 import ColumnRuleEventPropertyInputV1
 from .models.column_rule_input_v1 import ColumnRuleInputV1
 from .models.column_rule_item_property_input_v1 import ColumnRuleItemPropertyInputV1
 from .models.column_rule_path_input_v1 import ColumnRulePathInputV1
@@ -148,14 +151,21 @@
 from .models.connector_input_v1 import ConnectorInputV1
 from .models.connector_output_v1 import ConnectorOutputV1
 from .models.connectors_output_v1 import ConnectorsOutputV1
 from .models.content_input_v1 import ContentInputV1
 from .models.content_output_v1 import ContentOutputV1
 from .models.content_with_metadata_list_output_v1 import ContentWithMetadataListOutputV1
 from .models.content_with_metadata_output_v1 import ContentWithMetadataOutputV1
+from .models.context_comment_input_v1 import ContextCommentInputV1
+from .models.context_comment_output_v1 import ContextCommentOutputV1
+from .models.context_label_input_v1 import ContextLabelInputV1
+from .models.context_label_output_v1 import ContextLabelOutputV1
+from .models.context_opaque_input_v1 import ContextOpaqueInputV1
+from .models.context_opaque_output_v1 import ContextOpaqueOutputV1
+from .models.context_output_list_v1 import ContextOutputListV1
 from .models.csv_datafile_output_v1 import CsvDatafileOutputV1
 from .models.datafile_input_v1 import DatafileInputV1
 from .models.datafile_output_v1 import DatafileOutputV1
 from .models.datafiles_csv_body import DatafilesCsvBody
 from .models.datasource_clean_up_input_v1 import DatasourceCleanUpInputV1
 from .models.datasource_clean_up_output_v1 import DatasourceCleanUpOutputV1
 from .models.datasource_input_v1 import DatasourceInputV1
@@ -233,42 +243,56 @@
 from .models.get_metrics_output_v1 import GetMetricsOutputV1
 from .models.get_projects_output_v1 import GetProjectsOutputV1
 from .models.get_request_output_v1 import GetRequestOutputV1
 from .models.get_requests_output_v1 import GetRequestsOutputV1
 from .models.get_sample_output_v1 import GetSampleOutputV1
 from .models.get_samples_output_v1 import GetSamplesOutputV1
 from .models.get_signals_output_v1 import GetSignalsOutputV1
+from .models.graph_ql_input_v1 import GraphQLInputV1
+from .models.graph_ql_output_v1 import GraphQLOutputV1
 from .models.id_images_body import IdImagesBody
 from .models.identity_mapping_list_v1 import IdentityMappingListV1
 from .models.identity_mapping_v1 import IdentityMappingV1
 from .models.identity_preview_list_v1 import IdentityPreviewListV1
 from .models.identity_preview_v1 import IdentityPreviewV1
 from .models.indexing_parameters_input_v1 import IndexingParametersInputV1
 from .models.installer_output_v1 import InstallerOutputV1
 from .models.interval_v1 import IntervalV1
 from .models.invalid_swap_out_v1 import InvalidSwapOutV1
 from .models.item_batch_output_v1 import ItemBatchOutputV1
 from .models.item_dependency_output_v1 import ItemDependencyOutputV1
+from .models.item_finder_configuration_v1 import ItemFinderConfigurationV1
+from .models.item_finder_input_v1 import ItemFinderInputV1
+from .models.item_finder_output_list_v1 import ItemFinderOutputListV1
+from .models.item_finder_output_v1 import ItemFinderOutputV1
 from .models.item_id_list_input_v1 import ItemIdListInputV1
 from .models.item_output_v1 import ItemOutputV1
 from .models.item_parameter_of_output_v1 import ItemParameterOfOutputV1
 from .models.item_preview_list_v1 import ItemPreviewListV1
 from .models.item_preview_v1 import ItemPreviewV1
 from .models.item_preview_with_assets_v1 import ItemPreviewWithAssetsV1
 from .models.item_search_preview_list_v1 import ItemSearchPreviewListV1
 from .models.item_search_preview_paginated_list_v1 import ItemSearchPreviewPaginatedListV1
 from .models.item_search_preview_v1 import ItemSearchPreviewV1
 from .models.item_swap_result_output_v1 import ItemSwapResultOutputV1
 from .models.item_update_output_v1 import ItemUpdateOutputV1
 from .models.item_user_attributes_input_v1 import ItemUserAttributesInputV1
 from .models.item_user_attributes_output_v1 import ItemUserAttributesOutputV1
 from .models.item_with_swap_pairs_v1 import ItemWithSwapPairsV1
+from .models.jira_attachment import JiraAttachment
+from .models.jira_attachment_media_type import JiraAttachmentMediaType
 from .models.job_accepted_output_v1 import JobAcceptedOutputV1
 from .models.job_output_v1 import JobOutputV1
 from .models.json_backup_output_v1 import JsonBackupOutputV1
+from .models.label_category_input_v1 import LabelCategoryInputV1
+from .models.label_category_output_list_v1 import LabelCategoryOutputListV1
+from .models.label_category_output_v1 import LabelCategoryOutputV1
+from .models.label_input_v1 import LabelInputV1
+from .models.label_output_list_v1 import LabelOutputListV1
+from .models.label_output_v1 import LabelOutputV1
 from .models.license_importer_output_v1 import LicenseImporterOutputV1
 from .models.license_status_output_v1 import LicenseStatusOutputV1
 from .models.licensed_feature_status_output_v1 import LicensedFeatureStatusOutputV1
 from .models.log_message import LogMessage
 from .models.meter_datum_v1 import MeterDatumV1
 from .models.migrate_editor_input_v1 import MigrateEditorInputV1
 from .models.monitor_definition_output_v1 import MonitorDefinitionOutputV1
@@ -329,27 +353,28 @@
 from .models.scheduled_notebook_list_output_v1 import ScheduledNotebookListOutputV1
 from .models.scheduled_notebook_output_v1 import ScheduledNotebookOutputV1
 from .models.screenshot_output_v1 import ScreenshotOutputV1
 from .models.see_also_doc_output_v1 import SeeAlsoDocOutputV1
 from .models.send_email_attachment_v1 import SendEmailAttachmentV1
 from .models.send_email_contact_v1 import SendEmailContactV1
 from .models.send_email_input_v1 import SendEmailInputV1
-from .models.send_logs_input_v1 import SendLogsInputV1
 from .models.server_build_info_output_v1 import ServerBuildInfoOutputV1
 from .models.server_load_output_v1 import ServerLoadOutputV1
 from .models.server_spec_output_v1 import ServerSpecOutputV1
 from .models.server_status_output_v1 import ServerStatusOutputV1
 from .models.signal_input_v1 import SignalInputV1
 from .models.signal_output_v1 import SignalOutputV1
 from .models.signal_with_id_input_v1 import SignalWithIdInputV1
 from .models.status_message import StatusMessage
 from .models.status_message_base import StatusMessageBase
 from .models.subscription_input_v1 import SubscriptionInputV1
 from .models.subscription_output_v1 import SubscriptionOutputV1
 from .models.subscription_update_input_v1 import SubscriptionUpdateInputV1
+from .models.support_request_input_v1 import SupportRequestInputV1
+from .models.support_request_output_v1 import SupportRequestOutputV1
 from .models.supported_units_output_v1 import SupportedUnitsOutputV1
 from .models.swap_input_v1 import SwapInputV1
 from .models.swap_option_list_v1 import SwapOptionListV1
 from .models.swap_option_v1 import SwapOptionV1
 from .models.swap_output_v1 import SwapOutputV1
 from .models.sync_progress import SyncProgress
 from .models.sync_progress_output_v1 import SyncProgressOutputV1
```

### Comparing `seeq-61.1.4/seeq/sdk/api/__init__.py` & `seeq-62.0.1/seeq/sdk/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,43 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "61.1.4"
+__version__ = "62.0.1"
 
 # import apis into sdk package
 from .access_keys_api import AccessKeysApi
 from .add_ons_api import AddOnsApi
 from .agents_api import AgentsApi
 from .annotations_api import AnnotationsApi
 from .assets_api import AssetsApi
 from .audit_api import AuditApi
 from .auth_api import AuthApi
 from .condition_monitors_api import ConditionMonitorsApi
 from .conditions_api import ConditionsApi
 from .content_api import ContentApi
+from .context_api import ContextApi
 from .datafiles_api import DatafilesApi
 from .datasources_api import DatasourcesApi
 from .display_templates_api import DisplayTemplatesApi
 from .displays_api import DisplaysApi
 from .export_api import ExportApi
 from .folders_api import FoldersApi
 from .formulas_api import FormulasApi
+from .graph_ql_api import GraphQLApi
 from .items_api import ItemsApi
 from .jobs_api import JobsApi
 from .logs_api import LogsApi
 from .metrics_api import MetricsApi
 from .monitors_api import MonitorsApi
 from .networks_api import NetworksApi
 from .notification_configurations_api import NotificationConfigurationsApi
```

### Comparing `seeq-61.1.4/seeq/sdk/api/access_keys_api.py` & `seeq-62.0.1/seeq/sdk/api/access_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/add_ons_api.py` & `seeq-62.0.1/seeq/sdk/api/add_ons_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/agents_api.py` & `seeq-62.0.1/seeq/sdk/api/agents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/annotations_api.py` & `seeq-62.0.1/seeq/sdk/api/annotations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/assets_api.py` & `seeq-62.0.1/seeq/sdk/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/audit_api.py` & `seeq-62.0.1/seeq/sdk/api/audit_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/auth_api.py` & `seeq-62.0.1/seeq/sdk/api/auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/condition_monitors_api.py` & `seeq-62.0.1/seeq/sdk/api/condition_monitors_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
@@ -384,15 +384,15 @@
         >>> def callback_function(response):
         >>>     pprint(response)
         >>>
         >>> thread = api.get_condition_monitors(callback=callback_function)
 
         :param callback function: The callback function
             for asynchronous request. (optional)
-        :param list[str] creator_ids: Filter condition monitors to only those created by the specified user IDs
+        :param list[str] executor_ids: Filter condition monitors to only those created by the specified user IDs
         :param str name_search: Filter the condition monitors to those whose name match any part of the specified string
         :param list[str] condition_ids: Filter condition monitors to only those that are monitoring one of the specified conditions as specified by the list of IDs
         :param bool enabled_filter: Filter condition monitors by their enabled status
         :param int offset: Whether to filter condition monitors to only users who are enabled.
         :param int limit: The pagination limit, the total number of condition monitor that will be returned in this page of results
         :param str sort_field: Orders the condition monitors by either name, createdAt or workbook
         :param bool sort_asc: Sorts the sort field in ascending order when true and descending when false
@@ -417,29 +417,29 @@
         >>> def callback_function(response):
         >>>     pprint(response)
         >>>
         >>> thread = api.get_condition_monitors_with_http_info(callback=callback_function)
 
         :param callback function: The callback function
             for asynchronous request. (optional)
-        :param list[str] creator_ids: Filter condition monitors to only those created by the specified user IDs
+        :param list[str] executor_ids: Filter condition monitors to only those created by the specified user IDs
         :param str name_search: Filter the condition monitors to those whose name match any part of the specified string
         :param list[str] condition_ids: Filter condition monitors to only those that are monitoring one of the specified conditions as specified by the list of IDs
         :param bool enabled_filter: Filter condition monitors by their enabled status
         :param int offset: Whether to filter condition monitors to only users who are enabled.
         :param int limit: The pagination limit, the total number of condition monitor that will be returned in this page of results
         :param str sort_field: Orders the condition monitors by either name, createdAt or workbook
         :param bool sort_asc: Sorts the sort field in ascending order when true and descending when false
         :return: GetConditionMonitorItemsOutputV1
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GetConditionMonitorItemsOutputV1
         """
 
-        all_params = ['creator_ids', 'name_search', 'condition_ids', 'enabled_filter', 'offset', 'limit', 'sort_field', 'sort_asc']
+        all_params = ['executor_ids', 'name_search', 'condition_ids', 'enabled_filter', 'offset', 'limit', 'sort_field', 'sort_asc']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         all_params.append('_response_type')
         all_params.append('_custom_headers')
 
@@ -455,17 +455,17 @@
 
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'creator_ids' in params:
-            query_params.append(('creatorIds', params['creator_ids']))
-            collection_formats['creatorIds'] = 'multi'
+        if 'executor_ids' in params:
+            query_params.append(('executorIds', params['executor_ids']))
+            collection_formats['executorIds'] = 'multi'
         if 'name_search' in params:
             query_params.append(('nameSearch', params['name_search']))
         if 'condition_ids' in params:
             query_params.append(('conditionIds', params['condition_ids']))
             collection_formats['conditionIds'] = 'multi'
         if 'enabled_filter' in params:
             query_params.append(('enabledFilter', params['enabled_filter']))
```

### Comparing `seeq-61.1.4/seeq/sdk/api/conditions_api.py` & `seeq-62.0.1/seeq/sdk/api/conditions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/content_api.py` & `seeq-62.0.1/seeq/sdk/api/content_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/datafiles_api.py` & `seeq-62.0.1/seeq/sdk/api/datafiles_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/datasources_api.py` & `seeq-62.0.1/seeq/sdk/api/datasources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/display_templates_api.py` & `seeq-62.0.1/seeq/sdk/api/display_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/displays_api.py` & `seeq-62.0.1/seeq/sdk/api/displays_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/export_api.py` & `seeq-62.0.1/seeq/sdk/api/export_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/folders_api.py` & `seeq-62.0.1/seeq/sdk/api/folders_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/formulas_api.py` & `seeq-62.0.1/seeq/sdk/api/formulas_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 00000040: 6465 6420 2867 656e 6572 6174 6564 2062  ded (generated b
 00000050: 7920 5377 6167 6765 7220 436f 6465 6765  y Swagger Codege
 00000060: 6e20 6874 7470 733a 2f2f 6769 7468 7562  n https://github
 00000070: 2e63 6f6d 2f73 7761 6767 6572 2d61 7069  .com/swagger-api
 00000080: 2f73 7761 6767 6572 2d63 6f64 6567 656e  /swagger-codegen
 00000090: 2920 2023 206e 6f71 613a 2045 3530 310a  )  # noqa: E501.
 000000a0: 0a20 2020 204f 7065 6e41 5049 2073 7065  .    OpenAPI spe
-000000b0: 6320 7665 7273 696f 6e3a 2036 312e 312e  c version: 61.1.
-000000c0: 342d 7632 3032 3330 3830 3131 3830 300a  4-v202308011800.
+000000b0: 6320 7665 7273 696f 6e3a 2036 322e 302e  c version: 62.0.
+000000c0: 312d 7632 3032 3330 3830 3131 3535 370a  1-v202308011557.
 000000d0: 2020 2020 0a20 2020 2047 656e 6572 6174      .    Generat
 000000e0: 6564 2062 793a 2068 7474 7073 3a2f 2f67  ed by: https://g
 000000f0: 6974 6875 622e 636f 6d2f 7377 6167 6765  ithub.com/swagge
 00000100: 722d 6170 692f 7377 6167 6765 722d 636f  r-api/swagger-co
 00000110: 6465 6765 6e2e 6769 740a 2222 220a 0a66  degen.git."""..f
 00000120: 726f 6d20 5f5f 6675 7475 7265 5f5f 2069  rom __future__ i
 00000130: 6d70 6f72 7420 6162 736f 6c75 7465 5f69  mport absolute_i
```

### Comparing `seeq-61.1.4/seeq/sdk/api/items_api.py` & `seeq-62.0.1/seeq/sdk/api/items_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
@@ -278,14 +278,126 @@
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
 
+    def archive_item_finder(self, **kwargs):
+        """
+        Archive an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.archive_item_finder(id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str id: ID of the item finder to archive. (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.archive_item_finder_with_http_info(**kwargs)
+        else:
+            (data) = self.archive_item_finder_with_http_info(**kwargs)
+            return data
+
+    def archive_item_finder_with_http_info(self, **kwargs):
+        """
+        Archive an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.archive_item_finder_with_http_info(id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str id: ID of the item finder to archive. (required)
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        all_params = ['id']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('_response_type')
+        all_params.append('_custom_headers')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method archive_item_finder" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params) or (params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `archive_item_finder`")
+
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']
+
+        query_params = []
+
+        header_params = {}
+
+        for key, value in params.get('_custom_headers', {}).items():
+            header_params[key] = value
+
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/vnd.seeq.v1+json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/vnd.seeq.v1+json', ])
+
+        # Authentication setting
+        auth_settings = ['api_key']
+
+        return self.api_client.call_api('/items/finders/{id}', 'DELETE',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type=params.get('_response_type', None),
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
+
     def change_owner(self, **kwargs):
         """
         Change the owner of the specified item to the specified user. You need to be an administrator to be able to change the owner.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please define a `callback` function
         to be invoked when receiving the response.
         >>> def callback_function(response):
@@ -513,14 +625,126 @@
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
 
+    def create_item_finder(self, **kwargs):
+        """
+        Create a new item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.create_item_finder(body=body_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param ItemFinderInputV1 body: (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.create_item_finder_with_http_info(**kwargs)
+        else:
+            (data) = self.create_item_finder_with_http_info(**kwargs)
+            return data
+
+    def create_item_finder_with_http_info(self, **kwargs):
+        """
+        Create a new item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.create_item_finder_with_http_info(body=body_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param ItemFinderInputV1 body: (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+
+        all_params = ['body']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('_response_type')
+        all_params.append('_custom_headers')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_item_finder" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params) or (params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `create_item_finder`")
+
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        for key, value in params.get('_custom_headers', {}).items():
+            header_params[key] = value
+
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/vnd.seeq.v1+json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/vnd.seeq.v1+json', ])
+
+        # Authentication setting
+        auth_settings = ['api_key']
+
+        return self.api_client.call_api('/items/finders', 'POST',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type=params.get('_response_type', 'ItemFinderOutputV1'),
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
+
     def delete_property(self, **kwargs):
         """
         Delete a property
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please define a `callback` function
         to be invoked when receiving the response.
         >>> def callback_function(response):
@@ -1443,14 +1667,239 @@
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
 
+    def get_item_finder(self, **kwargs):
+        """
+        Get an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.get_item_finder(id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str id: The Seeq ID for the item finder (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.get_item_finder_with_http_info(**kwargs)
+        else:
+            (data) = self.get_item_finder_with_http_info(**kwargs)
+            return data
+
+    def get_item_finder_with_http_info(self, **kwargs):
+        """
+        Get an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.get_item_finder_with_http_info(id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param str id: The Seeq ID for the item finder (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+
+        all_params = ['id']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('_response_type')
+        all_params.append('_custom_headers')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_item_finder" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'id' is set
+        if ('id' not in params) or (params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `get_item_finder`")
+
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']
+
+        query_params = []
+
+        header_params = {}
+
+        for key, value in params.get('_custom_headers', {}).items():
+            header_params[key] = value
+
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/vnd.seeq.v1+json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/vnd.seeq.v1+json', ])
+
+        # Authentication setting
+        auth_settings = ['api_key']
+
+        return self.api_client.call_api('/items/finders/{id}', 'GET',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type=params.get('_response_type', 'ItemFinderOutputV1'),
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
+
+    def get_item_finders(self, **kwargs):
+        """
+        Get a list of item finders
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.get_item_finders(callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param int offset:
+        :param int limit: The pagination limit, the total number of item finders that will be returned in this page of results
+        :return: ItemFinderOutputListV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputListV1
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.get_item_finders_with_http_info(**kwargs)
+        else:
+            (data) = self.get_item_finders_with_http_info(**kwargs)
+            return data
+
+    def get_item_finders_with_http_info(self, **kwargs):
+        """
+        Get a list of item finders
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.get_item_finders_with_http_info(callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param int offset:
+        :param int limit: The pagination limit, the total number of item finders that will be returned in this page of results
+        :return: ItemFinderOutputListV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputListV1
+        """
+
+        all_params = ['offset', 'limit']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('_response_type')
+        all_params.append('_custom_headers')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_item_finders" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'offset' in params:
+            query_params.append(('offset', params['offset']))
+        if 'limit' in params:
+            query_params.append(('limit', params['limit']))
+
+        header_params = {}
+
+        for key, value in params.get('_custom_headers', {}).items():
+            header_params[key] = value
+
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/vnd.seeq.v1+json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/vnd.seeq.v1+json', ])
+
+        # Authentication setting
+        auth_settings = ['api_key']
+
+        return self.api_client.call_api('/items/finders', 'GET',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type=params.get('_response_type', 'ItemFinderOutputListV1'),
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
+
     def get_item_usages(self, **kwargs):
         """
         Finds all Threshold Metrics and Formulas that are directly built off the specified item.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please define a `callback` function
         to be invoked when receiving the response.
         >>> def callback_function(response):
@@ -2392,14 +2841,15 @@
 
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param list[str] filters: A list of item filters to reduce the result set. To logical AND multiple filters, use <b>\"filter1 && filter2</b>\" on a single line. To logical OR multiple filters, put each onto a new line. Filters can include any of the following options:<br><b>Empty</b>: returns the first ceiling number of items<br><b>\"value\"</b>: name or description of the item contains the case-insensitive value<br><b>\"field==value\"</b>: specified field exactly matches the case-sensitive value or regex<br><b>\"field~=value\"</b>: specified field contains the case-insensitive value or case-sensitive regex<br>To search for all items in the desired scope you may also use \"\\*\" character as filter.<br><b>Example:</b> Find items where (name or description contains case-insensitive \"bulb\" AND description contains case-insensitive \"area a\") OR (items hosted by datasource \"Example Data\" where name exactly matches the regex \".\\*[ABC]_Temperature\")<br><b>bulb && Description~=area a</b><br><b>Datasource ID==Example Data && Name==/.\\*[ABC]_Temperature/</b><br>To allow items with the 'unsearchable' property to be returned, include <b>\"@includeUnsearchable\"</b> on its own line<br>To exclude globally scoped items when using the \"scope\" filter include <b>\"@excludeGloballyScoped\"</b> on its own line
         :param list[str] scope: IDs that limit the results to those which are in the global scope or are scoped to the items referenced by the IDs. <br>The following item types can act as a scope: <b>Workbook</b><br>If the scope is set to the Empty GUID then the scoped items are excluded
         :param str asset: An ID that limits the results to items which are in the tree below the Asset referenced by the ID.
         :param list[str] types: A list of one or more case-sensitive item types which will restrict results to only those items that exactly match, or are children of, one of the specified types. If no types are provided then items of any type are returned
+        :param list[str] include_properties: A list of one or more case-sensitive item properties to include in every item this search finds. Use a single entry set to <b>\"@allProperties\"</b> to specify that all item properties should be returned. Specified properties not present for an item are simply omitted and do not cause errors.
         :param int offset: The pagination offset, the index of the first collection item that will be returned in this page of results. When using limit or offset values to query different item subsets it is important to sort the results using orderBy. Otherwise inconsistent results may be returned.
         :param int limit: The pagination limit, the total number of collection items that will be returned in this page of results. When using limit or offset values to query different item subsets it is important to sort the results using orderBy. Otherwise inconsistent results may be returned.
         :param list[str] order_by: An optional list of one or more fields used to sort the results.
         :return: ItemSearchPreviewPaginatedListV1
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ItemSearchPreviewPaginatedListV1
@@ -2424,24 +2874,25 @@
 
         :param callback function: The callback function
             for asynchronous request. (optional)
         :param list[str] filters: A list of item filters to reduce the result set. To logical AND multiple filters, use <b>\"filter1 && filter2</b>\" on a single line. To logical OR multiple filters, put each onto a new line. Filters can include any of the following options:<br><b>Empty</b>: returns the first ceiling number of items<br><b>\"value\"</b>: name or description of the item contains the case-insensitive value<br><b>\"field==value\"</b>: specified field exactly matches the case-sensitive value or regex<br><b>\"field~=value\"</b>: specified field contains the case-insensitive value or case-sensitive regex<br>To search for all items in the desired scope you may also use \"\\*\" character as filter.<br><b>Example:</b> Find items where (name or description contains case-insensitive \"bulb\" AND description contains case-insensitive \"area a\") OR (items hosted by datasource \"Example Data\" where name exactly matches the regex \".\\*[ABC]_Temperature\")<br><b>bulb && Description~=area a</b><br><b>Datasource ID==Example Data && Name==/.\\*[ABC]_Temperature/</b><br>To allow items with the 'unsearchable' property to be returned, include <b>\"@includeUnsearchable\"</b> on its own line<br>To exclude globally scoped items when using the \"scope\" filter include <b>\"@excludeGloballyScoped\"</b> on its own line
         :param list[str] scope: IDs that limit the results to those which are in the global scope or are scoped to the items referenced by the IDs. <br>The following item types can act as a scope: <b>Workbook</b><br>If the scope is set to the Empty GUID then the scoped items are excluded
         :param str asset: An ID that limits the results to items which are in the tree below the Asset referenced by the ID.
         :param list[str] types: A list of one or more case-sensitive item types which will restrict results to only those items that exactly match, or are children of, one of the specified types. If no types are provided then items of any type are returned
+        :param list[str] include_properties: A list of one or more case-sensitive item properties to include in every item this search finds. Use a single entry set to <b>\"@allProperties\"</b> to specify that all item properties should be returned. Specified properties not present for an item are simply omitted and do not cause errors.
         :param int offset: The pagination offset, the index of the first collection item that will be returned in this page of results. When using limit or offset values to query different item subsets it is important to sort the results using orderBy. Otherwise inconsistent results may be returned.
         :param int limit: The pagination limit, the total number of collection items that will be returned in this page of results. When using limit or offset values to query different item subsets it is important to sort the results using orderBy. Otherwise inconsistent results may be returned.
         :param list[str] order_by: An optional list of one or more fields used to sort the results.
         :return: ItemSearchPreviewPaginatedListV1
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ItemSearchPreviewPaginatedListV1
         """
 
-        all_params = ['filters', 'scope', 'asset', 'types', 'offset', 'limit', 'order_by']
+        all_params = ['filters', 'scope', 'asset', 'types', 'include_properties', 'offset', 'limit', 'order_by']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         all_params.append('_response_type')
         all_params.append('_custom_headers')
 
@@ -2468,14 +2919,17 @@
             query_params.append(('scope', params['scope']))
             collection_formats['scope'] = 'multi'
         if 'asset' in params:
             query_params.append(('asset', params['asset']))
         if 'types' in params:
             query_params.append(('types', params['types']))
             collection_formats['types'] = 'multi'
+        if 'include_properties' in params:
+            query_params.append(('includeProperties', params['include_properties']))
+            collection_formats['includeProperties'] = 'multi'
         if 'offset' in params:
             query_params.append(('offset', params['offset']))
         if 'limit' in params:
             query_params.append(('limit', params['limit']))
         if 'order_by' in params:
             query_params.append(('orderBy', params['order_by']))
             collection_formats['orderBy'] = 'multi'
@@ -3464,7 +3918,126 @@
                                         response_type=params.get('_response_type', 'ItemSearchPreviewListV1'),
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
+
+    def update_item_finder(self, **kwargs):
+        """
+        Update an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.update_item_finder(body=body_value, id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param ItemFinderInputV1 body: (required)
+        :param str id: The Seeq ID for the item finder (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('callback'):
+            return self.update_item_finder_with_http_info(**kwargs)
+        else:
+            (data) = self.update_item_finder_with_http_info(**kwargs)
+            return data
+
+    def update_item_finder_with_http_info(self, **kwargs):
+        """
+        Update an item finder
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please define a `callback` function
+        to be invoked when receiving the response.
+        >>> def callback_function(response):
+        >>>     pprint(response)
+        >>>
+        >>> thread = api.update_item_finder_with_http_info(body=body_value, id=id_value, callback=callback_function)
+
+        :param callback function: The callback function
+            for asynchronous request. (optional)
+        :param ItemFinderInputV1 body: (required)
+        :param str id: The Seeq ID for the item finder (required)
+        :return: ItemFinderOutputV1
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ItemFinderOutputV1
+        """
+
+        all_params = ['body', 'id']
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        all_params.append('_response_type')
+        all_params.append('_custom_headers')
+
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_item_finder" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params) or (params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `update_item_finder`")
+        # verify the required parameter 'id' is set
+        if ('id' not in params) or (params['id'] is None):
+            raise ValueError("Missing the required parameter `id` when calling `update_item_finder`")
+
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'id' in params:
+            path_params['id'] = params['id']
+
+        query_params = []
+
+        header_params = {}
+
+        for key, value in params.get('_custom_headers', {}).items():
+            header_params[key] = value
+
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.\
+            select_header_accept(['application/vnd.seeq.v1+json'])
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.\
+            select_header_content_type(['application/vnd.seeq.v1+json', ])
+
+        # Authentication setting
+        auth_settings = ['api_key']
+
+        return self.api_client.call_api('/items/finders/{id}', 'POST',
+                                        path_params,
+                                        query_params,
+                                        header_params,
+                                        body=body_params,
+                                        post_params=form_params,
+                                        files=local_var_files,
+                                        response_type=params.get('_response_type', 'ItemFinderOutputV1'),
+                                        auth_settings=auth_settings,
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=collection_formats)
```

### Comparing `seeq-61.1.4/seeq/sdk/api/jobs_api.py` & `seeq-62.0.1/seeq/sdk/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/logs_api.py` & `seeq-62.0.1/seeq/sdk/api/logs_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
@@ -394,58 +394,58 @@
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
 
-    def send_logs(self, **kwargs):
+    def send(self, **kwargs):
         """
-        Send the log files to Seeq.
+        Send a support request along with the log files to Seeq.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please define a `callback` function
         to be invoked when receiving the response.
         >>> def callback_function(response):
         >>>     pprint(response)
         >>>
-        >>> thread = api.send_logs(body=body_value, callback=callback_function)
+        >>> thread = api.send(body=body_value, callback=callback_function)
 
         :param callback function: The callback function
             for asynchronous request. (optional)
-        :param SendLogsInputV1 body: Log information (required)
-        :return: None
+        :param SupportRequestInputV1 body: Support request information (required)
+        :return: SupportRequestOutputV1
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: SupportRequestOutputV1
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('callback'):
-            return self.send_logs_with_http_info(**kwargs)
+            return self.send_with_http_info(**kwargs)
         else:
-            (data) = self.send_logs_with_http_info(**kwargs)
+            (data) = self.send_with_http_info(**kwargs)
             return data
 
-    def send_logs_with_http_info(self, **kwargs):
+    def send_with_http_info(self, **kwargs):
         """
-        Send the log files to Seeq.
+        Send a support request along with the log files to Seeq.
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please define a `callback` function
         to be invoked when receiving the response.
         >>> def callback_function(response):
         >>>     pprint(response)
         >>>
-        >>> thread = api.send_logs_with_http_info(body=body_value, callback=callback_function)
+        >>> thread = api.send_with_http_info(body=body_value, callback=callback_function)
 
         :param callback function: The callback function
             for asynchronous request. (optional)
-        :param SendLogsInputV1 body: Log information (required)
-        :return: None
+        :param SupportRequestInputV1 body: Support request information (required)
+        :return: SupportRequestOutputV1
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: SupportRequestOutputV1
         """
 
         all_params = ['body']
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
@@ -453,21 +453,21 @@
         all_params.append('_custom_headers')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method send_logs" % key
+                    " to method send" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params) or (params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `send_logs`")
+            raise ValueError("Missing the required parameter `body` when calling `send`")
 
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
@@ -498,14 +498,14 @@
         return self.api_client.call_api('/logs/send', 'POST',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
-                                        response_type=params.get('_response_type', None),
+                                        response_type=params.get('_response_type', 'SupportRequestOutputV1'),
                                         auth_settings=auth_settings,
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=collection_formats)
```

### Comparing `seeq-61.1.4/seeq/sdk/api/metrics_api.py` & `seeq-62.0.1/seeq/sdk/api/metrics_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/monitors_api.py` & `seeq-62.0.1/seeq/sdk/api/monitors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/networks_api.py` & `seeq-62.0.1/seeq/sdk/api/networks_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/notification_configurations_api.py` & `seeq-62.0.1/seeq/sdk/api/notification_configurations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/notifier_api.py` & `seeq-62.0.1/seeq/sdk/api/notifier_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/plugins_api.py` & `seeq-62.0.1/seeq/sdk/api/plugins_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/projects_api.py` & `seeq-62.0.1/seeq/sdk/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/report_templates_api.py` & `seeq-62.0.1/seeq/sdk/api/report_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/reports_api.py` & `seeq-62.0.1/seeq/sdk/api/reports_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/requests_api.py` & `seeq-62.0.1/seeq/sdk/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/scalars_api.py` & `seeq-62.0.1/seeq/sdk/api/scalars_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/signals_api.py` & `seeq-62.0.1/seeq/sdk/api/signals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/subscriptions_api.py` & `seeq-62.0.1/seeq/sdk/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/system_api.py` & `seeq-62.0.1/seeq/sdk/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/table_definitions_api.py` & `seeq-62.0.1/seeq/sdk/api/table_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/trees_api.py` & `seeq-62.0.1/seeq/sdk/api/trees_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/usage_api.py` & `seeq-62.0.1/seeq/sdk/api/usage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/user_groups_api.py` & `seeq-62.0.1/seeq/sdk/api/user_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/users_api.py` & `seeq-62.0.1/seeq/sdk/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api/workbooks_api.py` & `seeq-62.0.1/seeq/sdk/api/workbooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-61.1.4/seeq/sdk/api_client.py` & `seeq-62.0.1/seeq/sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import json
 import mimetypes
@@ -72,15 +72,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = self.configuration.host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/61.1.4/python'
+        self.user_agent = 'Swagger-Codegen/62.0.1/python'
         self.auth_token = None
         self.identity_path = None
         self.csrf_token = None
 
     @property
     def user_agent(self):
         """
```

### Comparing `seeq-61.1.4/seeq/sdk/configuration.py` & `seeq-62.0.1/seeq/sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import urllib3
@@ -250,16 +250,16 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 61.1.4-v202308011800\n"\
-               "SDK Package Version: 61.1.4".\
+               "Version of the API: 62.0.1-v202308011557\n"\
+               "SDK Package Version: 62.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
 
 default_configuration = ClientConfiguration()
 
 
 def Configuration():
```

### Comparing `seeq-61.1.4/seeq/sdk/models/__init__.py` & `seeq-62.0.1/seeq/sdk/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "61.1.4"
+__version__ = "62.0.1"
 
 # import models into sdk package
 from .access_key_input_v1 import AccessKeyInputV1
 from .access_key_output_list_v1 import AccessKeyOutputListV1
 from .access_key_output_v1 import AccessKeyOutputV1
 from .ace_input_v1 import AceInputV1
 from .ace_output_v1 import AceOutputV1
@@ -56,30 +56,31 @@
 from .asset_input_v1 import AssetInputV1
 from .asset_output_v1 import AssetOutputV1
 from .asset_selection_input_v1 import AssetSelectionInputV1
 from .asset_selection_output_v1 import AssetSelectionOutputV1
 from .asset_tree_batch_input_v1 import AssetTreeBatchInputV1
 from .asset_tree_output_v1 import AssetTreeOutputV1
 from .asset_tree_single_input_v1 import AssetTreeSingleInputV1
+from .attachment_input_v1 import AttachmentInputV1
 from .audit_output_list_v1 import AuditOutputListV1
 from .audit_output_v1 import AuditOutputV1
 from .auth_input_v1 import AuthInputV1
 from .auth_providers_output_v1 import AuthProvidersOutputV1
 from .cache_info_v1 import CacheInfoV1
 from .calculated_item_output_v1 import CalculatedItemOutputV1
 from .capsule_input_v1 import CapsuleInputV1
 from .capsule_property_input_v1 import CapsulePropertyInputV1
 from .capsule_property_output_v1 import CapsulePropertyOutputV1
 from .capsule_v1 import CapsuleV1
 from .capsules_input_v1 import CapsulesInputV1
 from .capsules_output_v1 import CapsulesOutputV1
 from .capsules_overwrite_input_v1 import CapsulesOverwriteInputV1
 from .channel_output_v1 import ChannelOutputV1
-from .column_definition import ColumnDefinition
 from .column_definition_input_v1 import ColumnDefinitionInputV1
+from .column_definition_output_v1 import ColumnDefinitionOutputV1
 from .column_rule import ColumnRule
 from .column_rule_ancestor_input_v1 import ColumnRuleAncestorInputV1
 from .column_rule_concat_input_v1 import ColumnRuleConcatInputV1
 from .column_rule_event_property_input_v1 import ColumnRuleEventPropertyInputV1
 from .column_rule_input_v1 import ColumnRuleInputV1
 from .column_rule_item_property_input_v1 import ColumnRuleItemPropertyInputV1
 from .column_rule_path_input_v1 import ColumnRulePathInputV1
@@ -106,14 +107,21 @@
 from .connector_input_v1 import ConnectorInputV1
 from .connector_output_v1 import ConnectorOutputV1
 from .connectors_output_v1 import ConnectorsOutputV1
 from .content_input_v1 import ContentInputV1
 from .content_output_v1 import ContentOutputV1
 from .content_with_metadata_list_output_v1 import ContentWithMetadataListOutputV1
 from .content_with_metadata_output_v1 import ContentWithMetadataOutputV1
+from .context_comment_input_v1 import ContextCommentInputV1
+from .context_comment_output_v1 import ContextCommentOutputV1
+from .context_label_input_v1 import ContextLabelInputV1
+from .context_label_output_v1 import ContextLabelOutputV1
+from .context_opaque_input_v1 import ContextOpaqueInputV1
+from .context_opaque_output_v1 import ContextOpaqueOutputV1
+from .context_output_list_v1 import ContextOutputListV1
 from .csv_datafile_output_v1 import CsvDatafileOutputV1
 from .datafile_input_v1 import DatafileInputV1
 from .datafile_output_v1 import DatafileOutputV1
 from .datafiles_csv_body import DatafilesCsvBody
 from .datasource_clean_up_input_v1 import DatasourceCleanUpInputV1
 from .datasource_clean_up_output_v1 import DatasourceCleanUpOutputV1
 from .datasource_input_v1 import DatasourceInputV1
@@ -191,42 +199,56 @@
 from .get_metrics_output_v1 import GetMetricsOutputV1
 from .get_projects_output_v1 import GetProjectsOutputV1
 from .get_request_output_v1 import GetRequestOutputV1
 from .get_requests_output_v1 import GetRequestsOutputV1
 from .get_sample_output_v1 import GetSampleOutputV1
 from .get_samples_output_v1 import GetSamplesOutputV1
 from .get_signals_output_v1 import GetSignalsOutputV1
+from .graph_ql_input_v1 import GraphQLInputV1
+from .graph_ql_output_v1 import GraphQLOutputV1
 from .id_images_body import IdImagesBody
 from .identity_mapping_list_v1 import IdentityMappingListV1
 from .identity_mapping_v1 import IdentityMappingV1
 from .identity_preview_list_v1 import IdentityPreviewListV1
 from .identity_preview_v1 import IdentityPreviewV1
 from .indexing_parameters_input_v1 import IndexingParametersInputV1
 from .installer_output_v1 import InstallerOutputV1
 from .interval_v1 import IntervalV1
 from .invalid_swap_out_v1 import InvalidSwapOutV1
 from .item_batch_output_v1 import ItemBatchOutputV1
 from .item_dependency_output_v1 import ItemDependencyOutputV1
+from .item_finder_configuration_v1 import ItemFinderConfigurationV1
+from .item_finder_input_v1 import ItemFinderInputV1
+from .item_finder_output_list_v1 import ItemFinderOutputListV1
+from .item_finder_output_v1 import ItemFinderOutputV1
 from .item_id_list_input_v1 import ItemIdListInputV1
 from .item_output_v1 import ItemOutputV1
 from .item_parameter_of_output_v1 import ItemParameterOfOutputV1
 from .item_preview_list_v1 import ItemPreviewListV1
 from .item_preview_v1 import ItemPreviewV1
 from .item_preview_with_assets_v1 import ItemPreviewWithAssetsV1
 from .item_search_preview_list_v1 import ItemSearchPreviewListV1
 from .item_search_preview_paginated_list_v1 import ItemSearchPreviewPaginatedListV1
 from .item_search_preview_v1 import ItemSearchPreviewV1
 from .item_swap_result_output_v1 import ItemSwapResultOutputV1
 from .item_update_output_v1 import ItemUpdateOutputV1
 from .item_user_attributes_input_v1 import ItemUserAttributesInputV1
 from .item_user_attributes_output_v1 import ItemUserAttributesOutputV1
 from .item_with_swap_pairs_v1 import ItemWithSwapPairsV1
+from .jira_attachment import JiraAttachment
+from .jira_attachment_media_type import JiraAttachmentMediaType
 from .job_accepted_output_v1 import JobAcceptedOutputV1
 from .job_output_v1 import JobOutputV1
 from .json_backup_output_v1 import JsonBackupOutputV1
+from .label_category_input_v1 import LabelCategoryInputV1
+from .label_category_output_list_v1 import LabelCategoryOutputListV1
+from .label_category_output_v1 import LabelCategoryOutputV1
+from .label_input_v1 import LabelInputV1
+from .label_output_list_v1 import LabelOutputListV1
+from .label_output_v1 import LabelOutputV1
 from .license_importer_output_v1 import LicenseImporterOutputV1
 from .license_status_output_v1 import LicenseStatusOutputV1
 from .licensed_feature_status_output_v1 import LicensedFeatureStatusOutputV1
 from .log_message import LogMessage
 from .meter_datum_v1 import MeterDatumV1
 from .migrate_editor_input_v1 import MigrateEditorInputV1
 from .monitor_definition_output_v1 import MonitorDefinitionOutputV1
@@ -287,27 +309,28 @@
 from .scheduled_notebook_list_output_v1 import ScheduledNotebookListOutputV1
 from .scheduled_notebook_output_v1 import ScheduledNotebookOutputV1
 from .screenshot_output_v1 import ScreenshotOutputV1
 from .see_also_doc_output_v1 import SeeAlsoDocOutputV1
 from .send_email_attachment_v1 import SendEmailAttachmentV1
 from .send_email_contact_v1 import SendEmailContactV1
 from .send_email_input_v1 import SendEmailInputV1
-from .send_logs_input_v1 import SendLogsInputV1
 from .server_build_info_output_v1 import ServerBuildInfoOutputV1
 from .server_load_output_v1 import ServerLoadOutputV1
 from .server_spec_output_v1 import ServerSpecOutputV1
 from .server_status_output_v1 import ServerStatusOutputV1
 from .signal_input_v1 import SignalInputV1
 from .signal_output_v1 import SignalOutputV1
 from .signal_with_id_input_v1 import SignalWithIdInputV1
 from .status_message import StatusMessage
 from .status_message_base import StatusMessageBase
 from .subscription_input_v1 import SubscriptionInputV1
 from .subscription_output_v1 import SubscriptionOutputV1
 from .subscription_update_input_v1 import SubscriptionUpdateInputV1
+from .support_request_input_v1 import SupportRequestInputV1
+from .support_request_output_v1 import SupportRequestOutputV1
 from .supported_units_output_v1 import SupportedUnitsOutputV1
 from .swap_input_v1 import SwapInputV1
 from .swap_option_list_v1 import SwapOptionListV1
 from .swap_option_v1 import SwapOptionV1
 from .swap_output_v1 import SwapOutputV1
 from .sync_progress import SyncProgress
 from .sync_progress_output_v1 import SyncProgressOutputV1
```

### Comparing `seeq-61.1.4/seeq/sdk/models/access_key_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/access_key_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/access_key_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/access_key_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/access_key_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/access_key_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/ace_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/ace_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/ace_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/ace_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/acl_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/acl_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/acl_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/acl_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/activity_graph_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/activity_graph_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/activity_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/activity_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_preview_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_preview_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_tool_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_tool_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/add_on_tool_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/add_on_tool_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/administrator_contact_information_v1.py` & `seeq-62.0.1/seeq/sdk/models/administrator_contact_information_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/agent_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/agent_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/agent_key_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/agent_key_output_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/agent_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/agent_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/agent_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/agent_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/agent_status_v1.py` & `seeq-62.0.1/seeq/sdk/models/agent_status_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_image_link_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_image_link_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_interest_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_interest_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_interest_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_interest_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_list_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/annotation_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/annotation_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -810,26 +810,26 @@
 
         self._status_message = status_message
 
     @property
     def timezone(self):
         """
         Gets the timezone of this AnnotationOutputV1.
-        The IANA string name of the time zone of the report. Ignored for Journals.
+        The IANA string name of the time zone of the report. Ignored for Journals
 
         :return: The timezone of this AnnotationOutputV1.
         :rtype: str
         """
         return self._timezone
 
     @timezone.setter
     def timezone(self, timezone):
         """
         Sets the timezone of this AnnotationOutputV1.
-        The IANA string name of the time zone of the report. Ignored for Journals.
+        The IANA string name of the time zone of the report. Ignored for Journals
 
         :param timezone: The timezone of this AnnotationOutputV1.
         :type: str
         """
 
         self._timezone = timezone
```

### Comparing `seeq-61.1.4/seeq/sdk/models/archive_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/archive_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_batch_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_batch_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_error.py` & `seeq-62.0.1/seeq/sdk/models/asset_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_group_asset_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_group_asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_group_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_group_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_group_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_group_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_group_root_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_group_root_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_group_tree_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_group_tree_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_selection_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_selection_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_selection_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_selection_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_tree_batch_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_group_input_v1.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,218 +1,274 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class AssetTreeBatchInputV1(object):
+class UserGroupInputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'asset_tree_relationships': 'list[AssetTreeSingleInputV1]',
-        'child_host_id': 'str',
-        'disable_asset_tree_index_update_during_sync': 'bool',
-        'parent_host_id': 'str',
-        'relationships': 'list[AssetTreeSingleInputV1]',
-        'update_asset_tree_index_during_sync': 'bool'
+        'description': 'str',
+        'is_enabled': 'bool',
+        'mapping': 'bool',
+        'mappings': 'IdentityMappingListV1',
+        'name': 'str',
+        'remote_group_editable': 'bool',
+        'remove_permissions': 'bool',
+        'sync_token': 'str'
     }
 
     attribute_map = {
-        'asset_tree_relationships': 'assetTreeRelationships',
-        'child_host_id': 'childHostId',
-        'disable_asset_tree_index_update_during_sync': 'disableAssetTreeIndexUpdateDuringSync',
-        'parent_host_id': 'parentHostId',
-        'relationships': 'relationships',
-        'update_asset_tree_index_during_sync': 'updateAssetTreeIndexDuringSync'
+        'description': 'description',
+        'is_enabled': 'isEnabled',
+        'mapping': 'mapping',
+        'mappings': 'mappings',
+        'name': 'name',
+        'remote_group_editable': 'remoteGroupEditable',
+        'remove_permissions': 'removePermissions',
+        'sync_token': 'syncToken'
     }
 
-    def __init__(self, asset_tree_relationships=None, child_host_id=None, disable_asset_tree_index_update_during_sync=False, parent_host_id=None, relationships=None, update_asset_tree_index_during_sync=None):
+    def __init__(self, description=None, is_enabled=True, mapping=False, mappings=None, name=None, remote_group_editable=False, remove_permissions=False, sync_token=None):
         """
-        AssetTreeBatchInputV1 - a model defined in Swagger
+        UserGroupInputV1 - a model defined in Swagger
         """
 
-        self._asset_tree_relationships = None
-        self._child_host_id = None
-        self._disable_asset_tree_index_update_during_sync = None
-        self._parent_host_id = None
-        self._relationships = None
-        self._update_asset_tree_index_during_sync = None
-
-        if asset_tree_relationships is not None:
-          self.asset_tree_relationships = asset_tree_relationships
-        if child_host_id is not None:
-          self.child_host_id = child_host_id
-        if disable_asset_tree_index_update_during_sync is not None:
-          self.disable_asset_tree_index_update_during_sync = disable_asset_tree_index_update_during_sync
-        if parent_host_id is not None:
-          self.parent_host_id = parent_host_id
-        if relationships is not None:
-          self.relationships = relationships
-        if update_asset_tree_index_during_sync is not None:
-          self.update_asset_tree_index_during_sync = update_asset_tree_index_during_sync
+        self._description = None
+        self._is_enabled = None
+        self._mapping = None
+        self._mappings = None
+        self._name = None
+        self._remote_group_editable = None
+        self._remove_permissions = None
+        self._sync_token = None
+
+        if description is not None:
+          self.description = description
+        if is_enabled is not None:
+          self.is_enabled = is_enabled
+        if mapping is not None:
+          self.mapping = mapping
+        if mappings is not None:
+          self.mappings = mappings
+        if name is not None:
+          self.name = name
+        if remote_group_editable is not None:
+          self.remote_group_editable = remote_group_editable
+        if remove_permissions is not None:
+          self.remove_permissions = remove_permissions
+        if sync_token is not None:
+          self.sync_token = sync_token
 
     @property
-    def asset_tree_relationships(self):
+    def description(self):
         """
-        Gets the asset_tree_relationships of this AssetTreeBatchInputV1.
+        Gets the description of this UserGroupInputV1.
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :return: The asset_tree_relationships of this AssetTreeBatchInputV1.
-        :rtype: list[AssetTreeSingleInputV1]
+        :return: The description of this UserGroupInputV1.
+        :rtype: str
         """
-        return self._asset_tree_relationships
+        return self._description
 
-    @asset_tree_relationships.setter
-    def asset_tree_relationships(self, asset_tree_relationships):
+    @description.setter
+    def description(self, description):
         """
-        Sets the asset_tree_relationships of this AssetTreeBatchInputV1.
+        Sets the description of this UserGroupInputV1.
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :param asset_tree_relationships: The asset_tree_relationships of this AssetTreeBatchInputV1.
-        :type: list[AssetTreeSingleInputV1]
+        :param description: The description of this UserGroupInputV1.
+        :type: str
         """
 
-        self._asset_tree_relationships = asset_tree_relationships
+        self._description = description
 
     @property
-    def child_host_id(self):
+    def is_enabled(self):
         """
-        Gets the child_host_id of this AssetTreeBatchInputV1.
-        The Seeq ID of the datasource host in which the children are located.
+        Gets the is_enabled of this UserGroupInputV1.
+        Whether the user group is enabled or disabled (default true).
 
-        :return: The child_host_id of this AssetTreeBatchInputV1.
-        :rtype: str
+        :return: The is_enabled of this UserGroupInputV1.
+        :rtype: bool
         """
-        return self._child_host_id
+        return self._is_enabled
 
-    @child_host_id.setter
-    def child_host_id(self, child_host_id):
+    @is_enabled.setter
+    def is_enabled(self, is_enabled):
         """
-        Sets the child_host_id of this AssetTreeBatchInputV1.
-        The Seeq ID of the datasource host in which the children are located.
+        Sets the is_enabled of this UserGroupInputV1.
+        Whether the user group is enabled or disabled (default true).
 
-        :param child_host_id: The child_host_id of this AssetTreeBatchInputV1.
-        :type: str
+        :param is_enabled: The is_enabled of this UserGroupInputV1.
+        :type: bool
         """
-        if child_host_id is None:
-            raise ValueError("Invalid value for `child_host_id`, must not be `None`")
 
-        self._child_host_id = child_host_id
+        self._is_enabled = is_enabled
 
     @property
-    def disable_asset_tree_index_update_during_sync(self):
+    def mapping(self):
         """
-        Gets the disable_asset_tree_index_update_during_sync of this AssetTreeBatchInputV1.
-        Whether to keep asset tree search index up to date during the sync or not
+        Gets the mapping of this UserGroupInputV1.
+        Whether the user group is a mapping (default false).
 
-        :return: The disable_asset_tree_index_update_during_sync of this AssetTreeBatchInputV1.
+        :return: The mapping of this UserGroupInputV1.
         :rtype: bool
         """
-        return self._disable_asset_tree_index_update_during_sync
+        return self._mapping
 
-    @disable_asset_tree_index_update_during_sync.setter
-    def disable_asset_tree_index_update_during_sync(self, disable_asset_tree_index_update_during_sync):
+    @mapping.setter
+    def mapping(self, mapping):
         """
-        Sets the disable_asset_tree_index_update_during_sync of this AssetTreeBatchInputV1.
-        Whether to keep asset tree search index up to date during the sync or not
+        Sets the mapping of this UserGroupInputV1.
+        Whether the user group is a mapping (default false).
 
-        :param disable_asset_tree_index_update_during_sync: The disable_asset_tree_index_update_during_sync of this AssetTreeBatchInputV1.
+        :param mapping: The mapping of this UserGroupInputV1.
         :type: bool
         """
 
-        self._disable_asset_tree_index_update_during_sync = disable_asset_tree_index_update_during_sync
+        self._mapping = mapping
+
+    @property
+    def mappings(self):
+        """
+        Gets the mappings of this UserGroupInputV1.
+
+        :return: The mappings of this UserGroupInputV1.
+        :rtype: IdentityMappingListV1
+        """
+        return self._mappings
+
+    @mappings.setter
+    def mappings(self, mappings):
+        """
+        Sets the mappings of this UserGroupInputV1.
+
+        :param mappings: The mappings of this UserGroupInputV1.
+        :type: IdentityMappingListV1
+        """
+
+        self._mappings = mappings
 
     @property
-    def parent_host_id(self):
+    def name(self):
         """
-        Gets the parent_host_id of this AssetTreeBatchInputV1.
-        The Seeq ID of the datasource host in which the parents are located.
+        Gets the name of this UserGroupInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :return: The parent_host_id of this AssetTreeBatchInputV1.
+        :return: The name of this UserGroupInputV1.
         :rtype: str
         """
-        return self._parent_host_id
+        return self._name
 
-    @parent_host_id.setter
-    def parent_host_id(self, parent_host_id):
+    @name.setter
+    def name(self, name):
         """
-        Sets the parent_host_id of this AssetTreeBatchInputV1.
-        The Seeq ID of the datasource host in which the parents are located.
+        Sets the name of this UserGroupInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :param parent_host_id: The parent_host_id of this AssetTreeBatchInputV1.
+        :param name: The name of this UserGroupInputV1.
         :type: str
         """
-        if parent_host_id is None:
-            raise ValueError("Invalid value for `parent_host_id`, must not be `None`")
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._parent_host_id = parent_host_id
+        self._name = name
 
     @property
-    def relationships(self):
+    def remote_group_editable(self):
         """
-        Gets the relationships of this AssetTreeBatchInputV1.
-        The list containing AssetTreeSingleInputV1s to create/update parent-child relationships with.
+        Gets the remote_group_editable of this UserGroupInputV1.
+        Whether the user group remains editable in Seeq even when sourced from a remote system.
 
-        :return: The relationships of this AssetTreeBatchInputV1.
-        :rtype: list[AssetTreeSingleInputV1]
+        :return: The remote_group_editable of this UserGroupInputV1.
+        :rtype: bool
         """
-        return self._relationships
+        return self._remote_group_editable
 
-    @relationships.setter
-    def relationships(self, relationships):
+    @remote_group_editable.setter
+    def remote_group_editable(self, remote_group_editable):
         """
-        Sets the relationships of this AssetTreeBatchInputV1.
-        The list containing AssetTreeSingleInputV1s to create/update parent-child relationships with.
+        Sets the remote_group_editable of this UserGroupInputV1.
+        Whether the user group remains editable in Seeq even when sourced from a remote system.
 
-        :param relationships: The relationships of this AssetTreeBatchInputV1.
-        :type: list[AssetTreeSingleInputV1]
+        :param remote_group_editable: The remote_group_editable of this UserGroupInputV1.
+        :type: bool
         """
 
-        self._relationships = relationships
+        self._remote_group_editable = remote_group_editable
 
     @property
-    def update_asset_tree_index_during_sync(self):
+    def remove_permissions(self):
         """
-        Gets the update_asset_tree_index_during_sync of this AssetTreeBatchInputV1.
+        Gets the remove_permissions of this UserGroupInputV1.
+        Whether permissions associated with the group should be removed when disabling the group (default false).
 
-        :return: The update_asset_tree_index_during_sync of this AssetTreeBatchInputV1.
+        :return: The remove_permissions of this UserGroupInputV1.
         :rtype: bool
         """
-        return self._update_asset_tree_index_during_sync
+        return self._remove_permissions
 
-    @update_asset_tree_index_during_sync.setter
-    def update_asset_tree_index_during_sync(self, update_asset_tree_index_during_sync):
+    @remove_permissions.setter
+    def remove_permissions(self, remove_permissions):
         """
-        Sets the update_asset_tree_index_during_sync of this AssetTreeBatchInputV1.
+        Sets the remove_permissions of this UserGroupInputV1.
+        Whether permissions associated with the group should be removed when disabling the group (default false).
 
-        :param update_asset_tree_index_during_sync: The update_asset_tree_index_during_sync of this AssetTreeBatchInputV1.
+        :param remove_permissions: The remove_permissions of this UserGroupInputV1.
         :type: bool
         """
 
-        self._update_asset_tree_index_during_sync = update_asset_tree_index_during_sync
+        self._remove_permissions = remove_permissions
+
+    @property
+    def sync_token(self):
+        """
+        Gets the sync_token of this UserGroupInputV1.
+        An arbitrary token (often a date or random ID) that is used during metadata syncs. At the end of a full sync, items with mismatching sync tokens are identified as stale and may be archived using the Datasources clean-up API.
+
+        :return: The sync_token of this UserGroupInputV1.
+        :rtype: str
+        """
+        return self._sync_token
+
+    @sync_token.setter
+    def sync_token(self, sync_token):
+        """
+        Sets the sync_token of this UserGroupInputV1.
+        An arbitrary token (often a date or random ID) that is used during metadata syncs. At the end of a full sync, items with mismatching sync tokens are identified as stale and may be archived using the Datasources clean-up API.
+
+        :param sync_token: The sync_token of this UserGroupInputV1.
+        :type: str
+        """
+
+        self._sync_token = sync_token
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -248,15 +304,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, AssetTreeBatchInputV1):
+        if not isinstance(other, UserGroupInputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_tree_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/asset_tree_single_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/asset_tree_single_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/audit_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/audit_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/audit_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/audit_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/auth_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/auth_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/auth_providers_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/auth_providers_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/cache_info_v1.py` & `seeq-62.0.1/seeq/sdk/models/cache_info_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/calculated_item_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/calculated_item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsule_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsule_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsule_property_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsule_property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsule_property_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsule_property_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsule_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsule_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsules_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsules_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsules_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsules_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/capsules_overwrite_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/capsules_overwrite_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/channel_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/channel_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_definition.py` & `seeq-62.0.1/seeq/sdk/models/column_rule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,186 +1,232 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ColumnDefinition(object):
+class ColumnRule(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'column_name': 'str',
-        'column_type': 'str',
-        'column_uom': 'str',
+        'arguments': 'dict(str, str)',
+        'column_id': 'str',
+        'evaluation_order': 'int',
         'id': 'str',
-        'rules': 'list[ColumnRule]'
+        'input_column1': 'str',
+        'input_column2': 'str',
+        'rule': 'str'
     }
 
     attribute_map = {
-        'column_name': 'columnName',
-        'column_type': 'columnType',
-        'column_uom': 'columnUom',
+        'arguments': 'arguments',
+        'column_id': 'columnId',
+        'evaluation_order': 'evaluationOrder',
         'id': 'id',
-        'rules': 'rules'
+        'input_column1': 'inputColumn1',
+        'input_column2': 'inputColumn2',
+        'rule': 'rule'
     }
 
-    def __init__(self, column_name=None, column_type=None, column_uom=None, id=None, rules=None):
+    def __init__(self, arguments=None, column_id=None, evaluation_order=None, id=None, input_column1=None, input_column2=None, rule=None):
         """
-        ColumnDefinition - a model defined in Swagger
+        ColumnRule - a model defined in Swagger
         """
 
-        self._column_name = None
-        self._column_type = None
-        self._column_uom = None
+        self._arguments = None
+        self._column_id = None
+        self._evaluation_order = None
         self._id = None
-        self._rules = None
-
-        if column_name is not None:
-          self.column_name = column_name
-        if column_type is not None:
-          self.column_type = column_type
-        if column_uom is not None:
-          self.column_uom = column_uom
+        self._input_column1 = None
+        self._input_column2 = None
+        self._rule = None
+
+        if arguments is not None:
+          self.arguments = arguments
+        if column_id is not None:
+          self.column_id = column_id
+        if evaluation_order is not None:
+          self.evaluation_order = evaluation_order
         if id is not None:
           self.id = id
-        if rules is not None:
-          self.rules = rules
+        if input_column1 is not None:
+          self.input_column1 = input_column1
+        if input_column2 is not None:
+          self.input_column2 = input_column2
+        if rule is not None:
+          self.rule = rule
 
     @property
-    def column_name(self):
+    def arguments(self):
         """
-        Gets the column_name of this ColumnDefinition.
+        Gets the arguments of this ColumnRule.
 
-        :return: The column_name of this ColumnDefinition.
-        :rtype: str
+        :return: The arguments of this ColumnRule.
+        :rtype: dict(str, str)
         """
-        return self._column_name
+        return self._arguments
 
-    @column_name.setter
-    def column_name(self, column_name):
+    @arguments.setter
+    def arguments(self, arguments):
         """
-        Sets the column_name of this ColumnDefinition.
+        Sets the arguments of this ColumnRule.
 
-        :param column_name: The column_name of this ColumnDefinition.
-        :type: str
+        :param arguments: The arguments of this ColumnRule.
+        :type: dict(str, str)
         """
 
-        self._column_name = column_name
+        self._arguments = arguments
 
     @property
-    def column_type(self):
+    def column_id(self):
         """
-        Gets the column_type of this ColumnDefinition.
+        Gets the column_id of this ColumnRule.
 
-        :return: The column_type of this ColumnDefinition.
+        :return: The column_id of this ColumnRule.
         :rtype: str
         """
-        return self._column_type
+        return self._column_id
 
-    @column_type.setter
-    def column_type(self, column_type):
+    @column_id.setter
+    def column_id(self, column_id):
         """
-        Sets the column_type of this ColumnDefinition.
+        Sets the column_id of this ColumnRule.
 
-        :param column_type: The column_type of this ColumnDefinition.
+        :param column_id: The column_id of this ColumnRule.
         :type: str
         """
-        allowed_values = ["UUID", "TEXT", "NUMERIC", "TIMESTAMPTZ", "BOOLEAN"]
-        if column_type not in allowed_values:
-            raise ValueError(
-                "Invalid value for `column_type` ({0}), must be one of {1}"
-                .format(column_type, allowed_values)
-            )
 
-        self._column_type = column_type
+        self._column_id = column_id
 
     @property
-    def column_uom(self):
+    def evaluation_order(self):
         """
-        Gets the column_uom of this ColumnDefinition.
+        Gets the evaluation_order of this ColumnRule.
 
-        :return: The column_uom of this ColumnDefinition.
-        :rtype: str
+        :return: The evaluation_order of this ColumnRule.
+        :rtype: int
         """
-        return self._column_uom
+        return self._evaluation_order
 
-    @column_uom.setter
-    def column_uom(self, column_uom):
+    @evaluation_order.setter
+    def evaluation_order(self, evaluation_order):
         """
-        Sets the column_uom of this ColumnDefinition.
+        Sets the evaluation_order of this ColumnRule.
 
-        :param column_uom: The column_uom of this ColumnDefinition.
-        :type: str
+        :param evaluation_order: The evaluation_order of this ColumnRule.
+        :type: int
         """
 
-        self._column_uom = column_uom
+        self._evaluation_order = evaluation_order
 
     @property
     def id(self):
         """
-        Gets the id of this ColumnDefinition.
+        Gets the id of this ColumnRule.
 
-        :return: The id of this ColumnDefinition.
+        :return: The id of this ColumnRule.
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
         """
-        Sets the id of this ColumnDefinition.
+        Sets the id of this ColumnRule.
 
-        :param id: The id of this ColumnDefinition.
+        :param id: The id of this ColumnRule.
         :type: str
         """
 
         self._id = id
 
     @property
-    def rules(self):
+    def input_column1(self):
+        """
+        Gets the input_column1 of this ColumnRule.
+
+        :return: The input_column1 of this ColumnRule.
+        :rtype: str
         """
-        Gets the rules of this ColumnDefinition.
+        return self._input_column1
 
-        :return: The rules of this ColumnDefinition.
-        :rtype: list[ColumnRule]
+    @input_column1.setter
+    def input_column1(self, input_column1):
         """
-        return self._rules
+        Sets the input_column1 of this ColumnRule.
 
-    @rules.setter
-    def rules(self, rules):
+        :param input_column1: The input_column1 of this ColumnRule.
+        :type: str
+        """
+
+        self._input_column1 = input_column1
+
+    @property
+    def input_column2(self):
+        """
+        Gets the input_column2 of this ColumnRule.
+
+        :return: The input_column2 of this ColumnRule.
+        :rtype: str
         """
-        Sets the rules of this ColumnDefinition.
+        return self._input_column2
 
-        :param rules: The rules of this ColumnDefinition.
-        :type: list[ColumnRule]
+    @input_column2.setter
+    def input_column2(self, input_column2):
+        """
+        Sets the input_column2 of this ColumnRule.
+
+        :param input_column2: The input_column2 of this ColumnRule.
+        :type: str
+        """
+
+        self._input_column2 = input_column2
+
+    @property
+    def rule(self):
+        """
+        Gets the rule of this ColumnRule.
+
+        :return: The rule of this ColumnRule.
+        :rtype: str
+        """
+        return self._rule
+
+    @rule.setter
+    def rule(self, rule):
+        """
+        Sets the rule of this ColumnRule.
+
+        :param rule: The rule of this ColumnRule.
+        :type: str
         """
 
-        self._rules = rules
+        self._rule = rule
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -216,15 +262,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ColumnDefinition):
+        if not isinstance(other, ColumnRule):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_definition_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_definition_input_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -29,42 +29,47 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'column_name': 'str',
         'column_rules': 'list[ColumnRuleInputV1]',
         'column_type': 'str',
-        'column_uom': 'str'
+        'column_uom': 'str',
+        'is_indexed': 'bool'
     }
 
     attribute_map = {
         'column_name': 'columnName',
         'column_rules': 'columnRules',
         'column_type': 'columnType',
-        'column_uom': 'columnUom'
+        'column_uom': 'columnUom',
+        'is_indexed': 'isIndexed'
     }
 
-    def __init__(self, column_name=None, column_rules=None, column_type=None, column_uom=None):
+    def __init__(self, column_name=None, column_rules=None, column_type=None, column_uom=None, is_indexed=None):
         """
         ColumnDefinitionInputV1 - a model defined in Swagger
         """
 
         self._column_name = None
         self._column_rules = None
         self._column_type = None
         self._column_uom = None
+        self._is_indexed = None
 
         if column_name is not None:
           self.column_name = column_name
         if column_rules is not None:
           self.column_rules = column_rules
         if column_type is not None:
           self.column_type = column_type
         if column_uom is not None:
           self.column_uom = column_uom
+        if is_indexed is not None:
+          self.is_indexed = is_indexed
 
     @property
     def column_name(self):
         """
         Gets the column_name of this ColumnDefinitionInputV1.
         Name of the column. This will be used as the header for this column. It must be unique for this table
 
@@ -143,35 +148,54 @@
 
         self._column_type = column_type
 
     @property
     def column_uom(self):
         """
         Gets the column_uom of this ColumnDefinitionInputV1.
-        The unit of measure for this column. If provided, this will              enforce that data in this column must be in this unit. For example, if the user specifies Fahrenheit and              the value comes in as Meters, the value will not be inserted. If not provided, values with different              units will be allowed to be stored and an extra column will be added to the generated table for the UOM
+        The unit of measure for this column. This is only applicable to columns whose type                      is NUMERIC. If provided, this will enforce that data in this column must be in this unit. For                      example, if the user specifies Fahrenheit and the value comes in as Meters, the value will not be                      inserted. If not provided, values with different units will be allowed to be stored and an extra                       column will be added to the generated table for the UOM
 
         :return: The column_uom of this ColumnDefinitionInputV1.
         :rtype: str
         """
         return self._column_uom
 
     @column_uom.setter
     def column_uom(self, column_uom):
         """
         Sets the column_uom of this ColumnDefinitionInputV1.
-        The unit of measure for this column. If provided, this will              enforce that data in this column must be in this unit. For example, if the user specifies Fahrenheit and              the value comes in as Meters, the value will not be inserted. If not provided, values with different              units will be allowed to be stored and an extra column will be added to the generated table for the UOM
+        The unit of measure for this column. This is only applicable to columns whose type                      is NUMERIC. If provided, this will enforce that data in this column must be in this unit. For                      example, if the user specifies Fahrenheit and the value comes in as Meters, the value will not be                      inserted. If not provided, values with different units will be allowed to be stored and an extra                       column will be added to the generated table for the UOM
 
         :param column_uom: The column_uom of this ColumnDefinitionInputV1.
         :type: str
         """
-        if column_uom is None:
-            raise ValueError("Invalid value for `column_uom`, must not be `None`")
 
         self._column_uom = column_uom
 
+    @property
+    def is_indexed(self):
+        """
+        Gets the is_indexed of this ColumnDefinitionInputV1.
+
+        :return: The is_indexed of this ColumnDefinitionInputV1.
+        :rtype: bool
+        """
+        return self._is_indexed
+
+    @is_indexed.setter
+    def is_indexed(self, is_indexed):
+        """
+        Sets the is_indexed of this ColumnDefinitionInputV1.
+
+        :param is_indexed: The is_indexed of this ColumnDefinitionInputV1.
+        :type: bool
+        """
+
+        self._is_indexed = is_indexed
+
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
         for attr, _ in iteritems(self.swagger_types):
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule.py` & `seeq-62.0.1/seeq/sdk/models/item_preview_v1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,232 +1,224 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ColumnRule(object):
+class ItemPreviewV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'arguments': 'dict(str, str)',
-        'column_id': 'str',
-        'evaluation_order': 'int',
         'id': 'str',
-        'input_column1': 'str',
-        'input_column2': 'str',
-        'rule': 'str'
+        'is_archived': 'bool',
+        'is_redacted': 'bool',
+        'name': 'str',
+        'translation_key': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
-        'arguments': 'arguments',
-        'column_id': 'columnId',
-        'evaluation_order': 'evaluationOrder',
         'id': 'id',
-        'input_column1': 'inputColumn1',
-        'input_column2': 'inputColumn2',
-        'rule': 'rule'
+        'is_archived': 'isArchived',
+        'is_redacted': 'isRedacted',
+        'name': 'name',
+        'translation_key': 'translationKey',
+        'type': 'type'
     }
 
-    def __init__(self, arguments=None, column_id=None, evaluation_order=None, id=None, input_column1=None, input_column2=None, rule=None):
+    def __init__(self, id=None, is_archived=False, is_redacted=False, name=None, translation_key=None, type=None):
         """
-        ColumnRule - a model defined in Swagger
+        ItemPreviewV1 - a model defined in Swagger
         """
 
-        self._arguments = None
-        self._column_id = None
-        self._evaluation_order = None
         self._id = None
-        self._input_column1 = None
-        self._input_column2 = None
-        self._rule = None
-
-        if arguments is not None:
-          self.arguments = arguments
-        if column_id is not None:
-          self.column_id = column_id
-        if evaluation_order is not None:
-          self.evaluation_order = evaluation_order
+        self._is_archived = None
+        self._is_redacted = None
+        self._name = None
+        self._translation_key = None
+        self._type = None
+
         if id is not None:
           self.id = id
-        if input_column1 is not None:
-          self.input_column1 = input_column1
-        if input_column2 is not None:
-          self.input_column2 = input_column2
-        if rule is not None:
-          self.rule = rule
-
-    @property
-    def arguments(self):
-        """
-        Gets the arguments of this ColumnRule.
-
-        :return: The arguments of this ColumnRule.
-        :rtype: dict(str, str)
-        """
-        return self._arguments
-
-    @arguments.setter
-    def arguments(self, arguments):
-        """
-        Sets the arguments of this ColumnRule.
-
-        :param arguments: The arguments of this ColumnRule.
-        :type: dict(str, str)
-        """
-
-        self._arguments = arguments
+        if is_archived is not None:
+          self.is_archived = is_archived
+        if is_redacted is not None:
+          self.is_redacted = is_redacted
+        if name is not None:
+          self.name = name
+        if translation_key is not None:
+          self.translation_key = translation_key
+        if type is not None:
+          self.type = type
 
     @property
-    def column_id(self):
+    def id(self):
         """
-        Gets the column_id of this ColumnRule.
+        Gets the id of this ItemPreviewV1.
+        The ID that can be used to interact with the item
 
-        :return: The column_id of this ColumnRule.
+        :return: The id of this ItemPreviewV1.
         :rtype: str
         """
-        return self._column_id
+        return self._id
 
-    @column_id.setter
-    def column_id(self, column_id):
+    @id.setter
+    def id(self, id):
         """
-        Sets the column_id of this ColumnRule.
+        Sets the id of this ItemPreviewV1.
+        The ID that can be used to interact with the item
 
-        :param column_id: The column_id of this ColumnRule.
+        :param id: The id of this ItemPreviewV1.
         :type: str
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")
 
-        self._column_id = column_id
+        self._id = id
 
     @property
-    def evaluation_order(self):
+    def is_archived(self):
         """
-        Gets the evaluation_order of this ColumnRule.
+        Gets the is_archived of this ItemPreviewV1.
+        Whether item is archived
 
-        :return: The evaluation_order of this ColumnRule.
-        :rtype: int
+        :return: The is_archived of this ItemPreviewV1.
+        :rtype: bool
         """
-        return self._evaluation_order
+        return self._is_archived
 
-    @evaluation_order.setter
-    def evaluation_order(self, evaluation_order):
+    @is_archived.setter
+    def is_archived(self, is_archived):
         """
-        Sets the evaluation_order of this ColumnRule.
+        Sets the is_archived of this ItemPreviewV1.
+        Whether item is archived
 
-        :param evaluation_order: The evaluation_order of this ColumnRule.
-        :type: int
+        :param is_archived: The is_archived of this ItemPreviewV1.
+        :type: bool
         """
 
-        self._evaluation_order = evaluation_order
+        self._is_archived = is_archived
 
     @property
-    def id(self):
+    def is_redacted(self):
         """
-        Gets the id of this ColumnRule.
+        Gets the is_redacted of this ItemPreviewV1.
+        Whether item is redacted
 
-        :return: The id of this ColumnRule.
-        :rtype: str
+        :return: The is_redacted of this ItemPreviewV1.
+        :rtype: bool
         """
-        return self._id
+        return self._is_redacted
 
-    @id.setter
-    def id(self, id):
+    @is_redacted.setter
+    def is_redacted(self, is_redacted):
         """
-        Sets the id of this ColumnRule.
+        Sets the is_redacted of this ItemPreviewV1.
+        Whether item is redacted
 
-        :param id: The id of this ColumnRule.
-        :type: str
+        :param is_redacted: The is_redacted of this ItemPreviewV1.
+        :type: bool
         """
 
-        self._id = id
+        self._is_redacted = is_redacted
 
     @property
-    def input_column1(self):
+    def name(self):
         """
-        Gets the input_column1 of this ColumnRule.
+        Gets the name of this ItemPreviewV1.
+        The human readable name
 
-        :return: The input_column1 of this ColumnRule.
+        :return: The name of this ItemPreviewV1.
         :rtype: str
         """
-        return self._input_column1
+        return self._name
 
-    @input_column1.setter
-    def input_column1(self, input_column1):
+    @name.setter
+    def name(self, name):
         """
-        Sets the input_column1 of this ColumnRule.
+        Sets the name of this ItemPreviewV1.
+        The human readable name
 
-        :param input_column1: The input_column1 of this ColumnRule.
+        :param name: The name of this ItemPreviewV1.
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._input_column1 = input_column1
+        self._name = name
 
     @property
-    def input_column2(self):
+    def translation_key(self):
         """
-        Gets the input_column2 of this ColumnRule.
+        Gets the translation_key of this ItemPreviewV1.
+        The item's translation key, if any
 
-        :return: The input_column2 of this ColumnRule.
+        :return: The translation_key of this ItemPreviewV1.
         :rtype: str
         """
-        return self._input_column2
+        return self._translation_key
 
-    @input_column2.setter
-    def input_column2(self, input_column2):
+    @translation_key.setter
+    def translation_key(self, translation_key):
         """
-        Sets the input_column2 of this ColumnRule.
+        Sets the translation_key of this ItemPreviewV1.
+        The item's translation key, if any
 
-        :param input_column2: The input_column2 of this ColumnRule.
+        :param translation_key: The translation_key of this ItemPreviewV1.
         :type: str
         """
 
-        self._input_column2 = input_column2
+        self._translation_key = translation_key
 
     @property
-    def rule(self):
+    def type(self):
         """
-        Gets the rule of this ColumnRule.
+        Gets the type of this ItemPreviewV1.
+        The type of the item
 
-        :return: The rule of this ColumnRule.
+        :return: The type of this ItemPreviewV1.
         :rtype: str
         """
-        return self._rule
+        return self._type
 
-    @rule.setter
-    def rule(self, rule):
+    @type.setter
+    def type(self, type):
         """
-        Sets the rule of this ColumnRule.
+        Sets the type of this ItemPreviewV1.
+        The type of the item
 
-        :param rule: The rule of this ColumnRule.
+        :param type: The type of this ItemPreviewV1.
         :type: str
         """
+        if type is None:
+            raise ValueError("Invalid value for `type`, must not be `None`")
 
-        self._rule = rule
+        self._type = type
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -262,15 +254,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ColumnRule):
+        if not isinstance(other, ItemPreviewV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_ancestor_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_ancestor_input_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -77,26 +77,26 @@
 
         self._column_index = column_index
 
     @property
     def level(self):
         """
         Gets the level of this ColumnRuleAncestorInputV1.
-        The number of levels to go up in the tree. Must be >= 1. For                  a capsule, a level of 1 yields a condition, as a capsule's parent is a condition. A level > 1 returns                  a tree item, such as an asset
+        The number of levels to go up in the tree. Must be >= 1. For example, if columnIndex                  references a Condition ID and level is 1 then the rule would return the UUID of the asset to                  which the condition belongs
 
         :return: The level of this ColumnRuleAncestorInputV1.
         :rtype: int
         """
         return self._level
 
     @level.setter
     def level(self, level):
         """
         Sets the level of this ColumnRuleAncestorInputV1.
-        The number of levels to go up in the tree. Must be >= 1. For                  a capsule, a level of 1 yields a condition, as a capsule's parent is a condition. A level > 1 returns                  a tree item, such as an asset
+        The number of levels to go up in the tree. Must be >= 1. For example, if columnIndex                  references a Condition ID and level is 1 then the rule would return the UUID of the asset to                  which the condition belongs
 
         :param level: The level of this ColumnRuleAncestorInputV1.
         :type: int
         """
         if level is None:
             raise ValueError("Invalid value for `level`, must not be `None`")
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_concat_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_concat_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_event_property_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_event_property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_item_property_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_item_property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/column_rule_path_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/column_rule_path_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_batch_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_monitor_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_monitor_input_v1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -26,85 +26,62 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'archived': 'bool',
         'condition_ids': 'list[str]',
         'cron_schedule': 'list[str]',
         'description': 'str',
         'enabled': 'bool',
+        'item_finder_id': 'str',
         'name': 'str',
         'query_range_look_ahead': 'str'
     }
 
     attribute_map = {
-        'archived': 'archived',
         'condition_ids': 'conditionIds',
         'cron_schedule': 'cronSchedule',
         'description': 'description',
         'enabled': 'enabled',
+        'item_finder_id': 'itemFinderId',
         'name': 'name',
         'query_range_look_ahead': 'queryRangeLookAhead'
     }
 
-    def __init__(self, archived=False, condition_ids=None, cron_schedule=None, description=None, enabled=True, name=None, query_range_look_ahead=None):
+    def __init__(self, condition_ids=None, cron_schedule=None, description=None, enabled=True, item_finder_id=None, name=None, query_range_look_ahead=None):
         """
         ConditionMonitorInputV1 - a model defined in Swagger
         """
 
-        self._archived = None
         self._condition_ids = None
         self._cron_schedule = None
         self._description = None
         self._enabled = None
+        self._item_finder_id = None
         self._name = None
         self._query_range_look_ahead = None
 
-        if archived is not None:
-          self.archived = archived
         if condition_ids is not None:
           self.condition_ids = condition_ids
         if cron_schedule is not None:
           self.cron_schedule = cron_schedule
         if description is not None:
           self.description = description
         if enabled is not None:
           self.enabled = enabled
+        if item_finder_id is not None:
+          self.item_finder_id = item_finder_id
         if name is not None:
           self.name = name
         if query_range_look_ahead is not None:
           self.query_range_look_ahead = query_range_look_ahead
 
     @property
-    def archived(self):
-        """
-        Gets the archived of this ConditionMonitorInputV1.
-        Whether the condition monitor should be archived
-
-        :return: The archived of this ConditionMonitorInputV1.
-        :rtype: bool
-        """
-        return self._archived
-
-    @archived.setter
-    def archived(self, archived):
-        """
-        Sets the archived of this ConditionMonitorInputV1.
-        Whether the condition monitor should be archived
-
-        :param archived: The archived of this ConditionMonitorInputV1.
-        :type: bool
-        """
-
-        self._archived = archived
-
-    @property
     def condition_ids(self):
         """
         Gets the condition_ids of this ConditionMonitorInputV1.
         The IDs of conditions to monitor
 
         :return: The condition_ids of this ConditionMonitorInputV1.
         :rtype: list[str]
@@ -148,26 +125,26 @@
 
         self._cron_schedule = cron_schedule
 
     @property
     def description(self):
         """
         Gets the description of this ConditionMonitorInputV1.
-        The condition monitor's description
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
         :return: The description of this ConditionMonitorInputV1.
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
         Sets the description of this ConditionMonitorInputV1.
-        The condition monitor's description
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
         :param description: The description of this ConditionMonitorInputV1.
         :type: str
         """
 
         self._description = description
 
@@ -191,29 +168,52 @@
         :param enabled: The enabled of this ConditionMonitorInputV1.
         :type: bool
         """
 
         self._enabled = enabled
 
     @property
+    def item_finder_id(self):
+        """
+        Gets the item_finder_id of this ConditionMonitorInputV1.
+        The ID of an Item Finder to use to populate the list of conditions. If this is provided it will overwrite the list of conditionIds
+
+        :return: The item_finder_id of this ConditionMonitorInputV1.
+        :rtype: str
+        """
+        return self._item_finder_id
+
+    @item_finder_id.setter
+    def item_finder_id(self, item_finder_id):
+        """
+        Sets the item_finder_id of this ConditionMonitorInputV1.
+        The ID of an Item Finder to use to populate the list of conditions. If this is provided it will overwrite the list of conditionIds
+
+        :param item_finder_id: The item_finder_id of this ConditionMonitorInputV1.
+        :type: str
+        """
+
+        self._item_finder_id = item_finder_id
+
+    @property
     def name(self):
         """
         Gets the name of this ConditionMonitorInputV1.
-        The condition monitor's name
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
         :return: The name of this ConditionMonitorInputV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Sets the name of this ConditionMonitorInputV1.
-        The condition monitor's name
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
         :param name: The name of this ConditionMonitorInputV1.
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_monitor_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_monitor_output_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -29,100 +29,105 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'condition_ids': 'list[str]',
         'created_at': 'str',
         'creator': 'IdentityPreviewV1',
-        'creator_id': 'str',
         'cron_schedule': 'list[str]',
         'cron_schedule_description': 'str',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
         'enabled': 'bool',
+        'executor_id': 'str',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
+        'item_finder_id': 'str',
         'name': 'str',
         'query_range_look_ahead': 'str',
         'status_message': 'str',
         'translation_key': 'str',
         'type': 'str',
         'updated_at': 'str'
     }
 
     attribute_map = {
         'condition_ids': 'conditionIds',
         'created_at': 'createdAt',
         'creator': 'creator',
-        'creator_id': 'creatorId',
         'cron_schedule': 'cronSchedule',
         'cron_schedule_description': 'cronScheduleDescription',
         'description': 'description',
         'effective_permissions': 'effectivePermissions',
         'enabled': 'enabled',
+        'executor_id': 'executorId',
         'id': 'id',
         'is_archived': 'isArchived',
         'is_redacted': 'isRedacted',
+        'item_finder_id': 'itemFinderId',
         'name': 'name',
         'query_range_look_ahead': 'queryRangeLookAhead',
         'status_message': 'statusMessage',
         'translation_key': 'translationKey',
         'type': 'type',
         'updated_at': 'updatedAt'
     }
 
-    def __init__(self, condition_ids=None, created_at=None, creator=None, creator_id=None, cron_schedule=None, cron_schedule_description=None, description=None, effective_permissions=None, enabled=None, id=None, is_archived=False, is_redacted=False, name=None, query_range_look_ahead=None, status_message=None, translation_key=None, type=None, updated_at=None):
+    def __init__(self, condition_ids=None, created_at=None, creator=None, cron_schedule=None, cron_schedule_description=None, description=None, effective_permissions=None, enabled=None, executor_id=None, id=None, is_archived=False, is_redacted=False, item_finder_id=None, name=None, query_range_look_ahead=None, status_message=None, translation_key=None, type=None, updated_at=None):
         """
         ConditionMonitorOutputV1 - a model defined in Swagger
         """
 
         self._condition_ids = None
         self._created_at = None
         self._creator = None
-        self._creator_id = None
         self._cron_schedule = None
         self._cron_schedule_description = None
         self._description = None
         self._effective_permissions = None
         self._enabled = None
+        self._executor_id = None
         self._id = None
         self._is_archived = None
         self._is_redacted = None
+        self._item_finder_id = None
         self._name = None
         self._query_range_look_ahead = None
         self._status_message = None
         self._translation_key = None
         self._type = None
         self._updated_at = None
 
         if condition_ids is not None:
           self.condition_ids = condition_ids
         if created_at is not None:
           self.created_at = created_at
         if creator is not None:
           self.creator = creator
-        if creator_id is not None:
-          self.creator_id = creator_id
         if cron_schedule is not None:
           self.cron_schedule = cron_schedule
         if cron_schedule_description is not None:
           self.cron_schedule_description = cron_schedule_description
         if description is not None:
           self.description = description
         if effective_permissions is not None:
           self.effective_permissions = effective_permissions
         if enabled is not None:
           self.enabled = enabled
+        if executor_id is not None:
+          self.executor_id = executor_id
         if id is not None:
           self.id = id
         if is_archived is not None:
           self.is_archived = is_archived
         if is_redacted is not None:
           self.is_redacted = is_redacted
+        if item_finder_id is not None:
+          self.item_finder_id = item_finder_id
         if name is not None:
           self.name = name
         if query_range_look_ahead is not None:
           self.query_range_look_ahead = query_range_look_ahead
         if status_message is not None:
           self.status_message = status_message
         if translation_key is not None:
@@ -200,39 +205,14 @@
         :param creator: The creator of this ConditionMonitorOutputV1.
         :type: IdentityPreviewV1
         """
 
         self._creator = creator
 
     @property
-    def creator_id(self):
-        """
-        Gets the creator_id of this ConditionMonitorOutputV1.
-        ID of the monitor's creator
-
-        :return: The creator_id of this ConditionMonitorOutputV1.
-        :rtype: str
-        """
-        return self._creator_id
-
-    @creator_id.setter
-    def creator_id(self, creator_id):
-        """
-        Sets the creator_id of this ConditionMonitorOutputV1.
-        ID of the monitor's creator
-
-        :param creator_id: The creator_id of this ConditionMonitorOutputV1.
-        :type: str
-        """
-        if creator_id is None:
-            raise ValueError("Invalid value for `creator_id`, must not be `None`")
-
-        self._creator_id = creator_id
-
-    @property
     def cron_schedule(self):
         """
         Gets the cron_schedule of this ConditionMonitorOutputV1.
         The condition monitor's check interval(s) as a list of cron expressions (see https://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html)
 
         :return: The cron_schedule of this ConditionMonitorOutputV1.
         :rtype: list[str]
@@ -340,14 +320,39 @@
         """
         if enabled is None:
             raise ValueError("Invalid value for `enabled`, must not be `None`")
 
         self._enabled = enabled
 
     @property
+    def executor_id(self):
+        """
+        Gets the executor_id of this ConditionMonitorOutputV1.
+        ID of the monitor's creator
+
+        :return: The executor_id of this ConditionMonitorOutputV1.
+        :rtype: str
+        """
+        return self._executor_id
+
+    @executor_id.setter
+    def executor_id(self, executor_id):
+        """
+        Sets the executor_id of this ConditionMonitorOutputV1.
+        ID of the monitor's creator
+
+        :param executor_id: The executor_id of this ConditionMonitorOutputV1.
+        :type: str
+        """
+        if executor_id is None:
+            raise ValueError("Invalid value for `executor_id`, must not be `None`")
+
+        self._executor_id = executor_id
+
+    @property
     def id(self):
         """
         Gets the id of this ConditionMonitorOutputV1.
         The ID that can be used to interact with the item
 
         :return: The id of this ConditionMonitorOutputV1.
         :rtype: str
@@ -411,14 +416,37 @@
         :param is_redacted: The is_redacted of this ConditionMonitorOutputV1.
         :type: bool
         """
 
         self._is_redacted = is_redacted
 
     @property
+    def item_finder_id(self):
+        """
+        Gets the item_finder_id of this ConditionMonitorOutputV1.
+        The ID, if present, of the Item Finder that populates the list of condition IDs
+
+        :return: The item_finder_id of this ConditionMonitorOutputV1.
+        :rtype: str
+        """
+        return self._item_finder_id
+
+    @item_finder_id.setter
+    def item_finder_id(self, item_finder_id):
+        """
+        Sets the item_finder_id of this ConditionMonitorOutputV1.
+        The ID, if present, of the Item Finder that populates the list of condition IDs
+
+        :param item_finder_id: The item_finder_id of this ConditionMonitorOutputV1.
+        :type: str
+        """
+
+        self._item_finder_id = item_finder_id
+
+    @property
     def name(self):
         """
         Gets the name of this ConditionMonitorOutputV1.
         The human readable name
 
         :return: The name of this ConditionMonitorOutputV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_notification_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_notification_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_notification_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_notification_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/condition_update_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/condition_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configuration_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/configuration_input_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configuration_option_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/configuration_option_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configuration_option_output_simple_v1.py` & `seeq-62.0.1/seeq/sdk/models/configuration_option_output_simple_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configuration_option_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/configuration_option_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configuration_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/configured_directives_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/configured_directives_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connection_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/connection_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connection_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/connection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connection_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/connection_status_output_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -32,53 +32,59 @@
     swagger_types = {
         'agent_name': 'str',
         'connection_id': 'str',
         'connection_message': 'str',
         'connector_developer_name': 'str',
         'connector_developer_support_url': 'str',
         'connector_name': 'str',
+        'created_at': 'str',
         'datasource_managed': 'bool',
         'disabled_at': 'str',
         'disabled_by': 'str',
+        'has_error': 'bool',
         'last_successful_connected_at': 'str',
         'name': 'str',
         'status': 'str',
         'sync_status': 'str'
     }
 
     attribute_map = {
         'agent_name': 'agentName',
         'connection_id': 'connectionId',
         'connection_message': 'connectionMessage',
         'connector_developer_name': 'connectorDeveloperName',
         'connector_developer_support_url': 'connectorDeveloperSupportUrl',
         'connector_name': 'connectorName',
+        'created_at': 'createdAt',
         'datasource_managed': 'datasourceManaged',
         'disabled_at': 'disabledAt',
         'disabled_by': 'disabledBy',
+        'has_error': 'hasError',
         'last_successful_connected_at': 'lastSuccessfulConnectedAt',
         'name': 'name',
         'status': 'status',
         'sync_status': 'syncStatus'
     }
 
-    def __init__(self, agent_name=None, connection_id=None, connection_message=None, connector_developer_name=None, connector_developer_support_url=None, connector_name=None, datasource_managed=False, disabled_at=None, disabled_by=None, last_successful_connected_at=None, name=None, status=None, sync_status=None):
+    def __init__(self, agent_name=None, connection_id=None, connection_message=None, connector_developer_name=None, connector_developer_support_url=None, connector_name=None, created_at=None, datasource_managed=False, disabled_at=None, disabled_by=None, has_error=False, last_successful_connected_at=None, name=None, status=None, sync_status=None):
         """
         ConnectionStatusOutputV1 - a model defined in Swagger
         """
 
         self._agent_name = None
         self._connection_id = None
         self._connection_message = None
         self._connector_developer_name = None
         self._connector_developer_support_url = None
         self._connector_name = None
+        self._created_at = None
         self._datasource_managed = None
         self._disabled_at = None
         self._disabled_by = None
+        self._has_error = None
         self._last_successful_connected_at = None
         self._name = None
         self._status = None
         self._sync_status = None
 
         if agent_name is not None:
           self.agent_name = agent_name
@@ -88,20 +94,24 @@
           self.connection_message = connection_message
         if connector_developer_name is not None:
           self.connector_developer_name = connector_developer_name
         if connector_developer_support_url is not None:
           self.connector_developer_support_url = connector_developer_support_url
         if connector_name is not None:
           self.connector_name = connector_name
+        if created_at is not None:
+          self.created_at = created_at
         if datasource_managed is not None:
           self.datasource_managed = datasource_managed
         if disabled_at is not None:
           self.disabled_at = disabled_at
         if disabled_by is not None:
           self.disabled_by = disabled_by
+        if has_error is not None:
+          self.has_error = has_error
         if last_successful_connected_at is not None:
           self.last_successful_connected_at = last_successful_connected_at
         if name is not None:
           self.name = name
         if status is not None:
           self.status = status
         if sync_status is not None:
@@ -246,14 +256,37 @@
         :param connector_name: The connector_name of this ConnectionStatusOutputV1.
         :type: str
         """
 
         self._connector_name = connector_name
 
     @property
+    def created_at(self):
+        """
+        Gets the created_at of this ConnectionStatusOutputV1.
+        The timestamp of the connection creation
+
+        :return: The created_at of this ConnectionStatusOutputV1.
+        :rtype: str
+        """
+        return self._created_at
+
+    @created_at.setter
+    def created_at(self, created_at):
+        """
+        Sets the created_at of this ConnectionStatusOutputV1.
+        The timestamp of the connection creation
+
+        :param created_at: The created_at of this ConnectionStatusOutputV1.
+        :type: str
+        """
+
+        self._created_at = created_at
+
+    @property
     def datasource_managed(self):
         """
         Gets the datasource_managed of this ConnectionStatusOutputV1.
         Indicates if the configuration is managed by the datasource and cannot be changed in Seeq
 
         :return: The datasource_managed of this ConnectionStatusOutputV1.
         :rtype: bool
@@ -315,14 +348,37 @@
         :param disabled_by: The disabled_by of this ConnectionStatusOutputV1.
         :type: str
         """
 
         self._disabled_by = disabled_by
 
     @property
+    def has_error(self):
+        """
+        Gets the has_error of this ConnectionStatusOutputV1.
+        Indicates if the connection has an error
+
+        :return: The has_error of this ConnectionStatusOutputV1.
+        :rtype: bool
+        """
+        return self._has_error
+
+    @has_error.setter
+    def has_error(self, has_error):
+        """
+        Sets the has_error of this ConnectionStatusOutputV1.
+        Indicates if the connection has an error
+
+        :param has_error: The has_error of this ConnectionStatusOutputV1.
+        :type: bool
+        """
+
+        self._has_error = has_error
+
+    @property
     def last_successful_connected_at(self):
         """
         Gets the last_successful_connected_at of this ConnectionStatusOutputV1.
         The ISO 8601 date of the last successful connection to the external datasource (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
         :return: The last_successful_connected_at of this ConnectionStatusOutputV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connection_status_v1.py` & `seeq-62.0.1/seeq/sdk/models/connection_status_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -395,26 +395,26 @@
 
         self._sync_progress = sync_progress
 
     @property
     def sync_status(self):
         """
         Gets the sync_status of this ConnectionStatusV1.
-        The synchronization status of the current connection between the datasource and this connector. Valid values are UNKNOWN, SYNC_INITIALIZING, SYNC_IN_PROGRESS, SYNC_COMPLETE, SYNC_ARCHIVING_DELETED_ITEMS
+        The synchronization status of the current connection between the datasource and this connector. Valid values are SYNC_UNKNOWN, SYNC_INITIALIZING, SYNC_IN_PROGRESS, SYNC_COMPLETE, SYNC_ARCHIVING_DELETED_ITEMS
 
         :return: The sync_status of this ConnectionStatusV1.
         :rtype: str
         """
         return self._sync_status
 
     @sync_status.setter
     def sync_status(self, sync_status):
         """
         Sets the sync_status of this ConnectionStatusV1.
-        The synchronization status of the current connection between the datasource and this connector. Valid values are UNKNOWN, SYNC_INITIALIZING, SYNC_IN_PROGRESS, SYNC_COMPLETE, SYNC_ARCHIVING_DELETED_ITEMS
+        The synchronization status of the current connection between the datasource and this connector. Valid values are SYNC_UNKNOWN, SYNC_INITIALIZING, SYNC_IN_PROGRESS, SYNC_COMPLETE, SYNC_ARCHIVING_DELETED_ITEMS
 
         :param sync_status: The sync_status of this ConnectionStatusV1.
         :type: str
         """
 
         self._sync_status = sync_status
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connections_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/connections_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connector_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/connector_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connector_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/connector_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/connectors_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/connectors_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/content_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/content_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/content_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/content_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/content_with_metadata_list_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/content_with_metadata_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/content_with_metadata_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/content_with_metadata_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/csv_datafile_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/csv_datafile_output_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datafile_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/datafile_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datafile_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datafile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datafiles_csv_body.py` & `seeq-62.0.1/seeq/sdk/models/datafiles_csv_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_clean_up_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_clean_up_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_clean_up_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_clean_up_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -51,15 +51,15 @@
         'description': 'description',
         'indexing_schedule_supported': 'indexingScheduleSupported',
         'name': 'name',
         'signal_location': 'signalLocation',
         'stored_in_seeq': 'storedInSeeq'
     }
 
-    def __init__(self, additional_properties=None, cache_enabled=False, condition_location=None, datasource_class=None, datasource_id=None, description=None, indexing_schedule_supported=False, name=None, signal_location=None, stored_in_seeq=False):
+    def __init__(self, additional_properties=None, cache_enabled=None, condition_location=None, datasource_class=None, datasource_id=None, description=None, indexing_schedule_supported=False, name=None, signal_location=None, stored_in_seeq=False):
         """
         DatasourceInputV1 - a model defined in Swagger
         """
 
         self._additional_properties = None
         self._cache_enabled = None
         self._condition_location = None
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_statistics_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_statistics_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_status_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_status_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasource_summary_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasource_summary_status_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -42,14 +42,15 @@
         'datasource_class': 'str',
         'datasource_id': 'str',
         'id': 'str',
         'indexing_schedule_supported': 'bool',
         'local_datasource': 'bool',
         'name': 'str',
         'next_scheduled_index_at': 'str',
+        'placeholder': 'bool',
         'previous_index_at': 'str',
         'remaining_indexing_duration': 'int',
         'sync_progress': 'SyncProgressOutputV1',
         'sync_status': 'str',
         'total_connections_count': 'int'
     }
 
@@ -66,22 +67,23 @@
         'datasource_class': 'datasourceClass',
         'datasource_id': 'datasourceId',
         'id': 'id',
         'indexing_schedule_supported': 'indexingScheduleSupported',
         'local_datasource': 'localDatasource',
         'name': 'name',
         'next_scheduled_index_at': 'nextScheduledIndexAt',
+        'placeholder': 'placeholder',
         'previous_index_at': 'previousIndexAt',
         'remaining_indexing_duration': 'remainingIndexingDuration',
         'sync_progress': 'syncProgress',
         'sync_status': 'syncStatus',
         'total_connections_count': 'totalConnectionsCount'
     }
 
-    def __init__(self, allow_requests=False, average_indexing_duration=None, cache_enabled=False, connections=None, connections_connected_count=None, current_index_at=None, current_indexing_duration=None, current_indexing_percentage=None, current_indexing_started_at=None, datasource_class=None, datasource_id=None, id=None, indexing_schedule_supported=False, local_datasource=None, name=None, next_scheduled_index_at=None, previous_index_at=None, remaining_indexing_duration=None, sync_progress=None, sync_status=None, total_connections_count=None):
+    def __init__(self, allow_requests=False, average_indexing_duration=None, cache_enabled=False, connections=None, connections_connected_count=None, current_index_at=None, current_indexing_duration=None, current_indexing_percentage=None, current_indexing_started_at=None, datasource_class=None, datasource_id=None, id=None, indexing_schedule_supported=False, local_datasource=None, name=None, next_scheduled_index_at=None, placeholder=False, previous_index_at=None, remaining_indexing_duration=None, sync_progress=None, sync_status=None, total_connections_count=None):
         """
         DatasourceSummaryStatusOutputV1 - a model defined in Swagger
         """
 
         self._allow_requests = None
         self._average_indexing_duration = None
         self._cache_enabled = None
@@ -94,14 +96,15 @@
         self._datasource_class = None
         self._datasource_id = None
         self._id = None
         self._indexing_schedule_supported = None
         self._local_datasource = None
         self._name = None
         self._next_scheduled_index_at = None
+        self._placeholder = None
         self._previous_index_at = None
         self._remaining_indexing_duration = None
         self._sync_progress = None
         self._sync_status = None
         self._total_connections_count = None
 
         if allow_requests is not None:
@@ -132,14 +135,16 @@
           self.indexing_schedule_supported = indexing_schedule_supported
         if local_datasource is not None:
           self.local_datasource = local_datasource
         if name is not None:
           self.name = name
         if next_scheduled_index_at is not None:
           self.next_scheduled_index_at = next_scheduled_index_at
+        if placeholder is not None:
+          self.placeholder = placeholder
         if previous_index_at is not None:
           self.previous_index_at = previous_index_at
         if remaining_indexing_duration is not None:
           self.remaining_indexing_duration = remaining_indexing_duration
         if sync_progress is not None:
           self.sync_progress = sync_progress
         if sync_status is not None:
@@ -520,14 +525,37 @@
         :param next_scheduled_index_at: The next_scheduled_index_at of this DatasourceSummaryStatusOutputV1.
         :type: str
         """
 
         self._next_scheduled_index_at = next_scheduled_index_at
 
     @property
+    def placeholder(self):
+        """
+        Gets the placeholder of this DatasourceSummaryStatusOutputV1.
+        Whether this is a placeholder datasource created for a connection without datasource
+
+        :return: The placeholder of this DatasourceSummaryStatusOutputV1.
+        :rtype: bool
+        """
+        return self._placeholder
+
+    @placeholder.setter
+    def placeholder(self, placeholder):
+        """
+        Sets the placeholder of this DatasourceSummaryStatusOutputV1.
+        Whether this is a placeholder datasource created for a connection without datasource
+
+        :param placeholder: The placeholder of this DatasourceSummaryStatusOutputV1.
+        :type: bool
+        """
+
+        self._placeholder = placeholder
+
+    @property
     def previous_index_at(self):
         """
         Gets the previous_index_at of this DatasourceSummaryStatusOutputV1.
         The ISO 8601 date of when previous index occurred (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
         :return: The previous_index_at of this DatasourceSummaryStatusOutputV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/datasources_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/datasources_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/date_range_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/date_range_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/date_range_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/date_range_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/detailed_meter_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/detailed_meter_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/detailed_timer_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/detailed_timer_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/directive_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/directive_input_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_template_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_template_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_template_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/display_template_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/display_template_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/document_backup_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/document_backup_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/email_notification_recipient_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/email_notification_recipient_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/emailer_configuration_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/emailer_configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/export_item_v1.py` & `seeq-62.0.1/seeq/sdk/models/export_item_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/export_items_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/export_items_output_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -33,70 +33,79 @@
         'autoupdate_time_range': 'bool',
         'capsule_time': 'bool',
         'chain_view': 'bool',
         'created_at': 'str',
         'export_capsules': 'bool',
         'export_name': 'str',
         'grid_enabled': 'bool',
+        'grid_origin': 'str',
         'grid_size': 'str',
+        'href': 'str',
         'id': 'str',
         'is_archived': 'bool',
         'items': 'list[ExportItemV1]',
         'name': 'str',
         'original_timestamps_enabled': 'bool',
         'scoped_to': 'str',
         'status_message': 'str',
         'swap_in': 'str',
         'swap_out': 'str',
+        'time_zone': 'str',
         'updated_at': 'str'
     }
 
     attribute_map = {
         'autoupdate_time_range': 'autoupdateTimeRange',
         'capsule_time': 'capsuleTime',
         'chain_view': 'chainView',
         'created_at': 'createdAt',
         'export_capsules': 'exportCapsules',
         'export_name': 'exportName',
         'grid_enabled': 'gridEnabled',
+        'grid_origin': 'gridOrigin',
         'grid_size': 'gridSize',
+        'href': 'href',
         'id': 'id',
         'is_archived': 'isArchived',
         'items': 'items',
         'name': 'name',
         'original_timestamps_enabled': 'originalTimestampsEnabled',
         'scoped_to': 'scopedTo',
         'status_message': 'statusMessage',
         'swap_in': 'swapIn',
         'swap_out': 'swapOut',
+        'time_zone': 'timeZone',
         'updated_at': 'updatedAt'
     }
 
-    def __init__(self, autoupdate_time_range=False, capsule_time=False, chain_view=False, created_at=None, export_capsules=False, export_name=None, grid_enabled=False, grid_size=None, id=None, is_archived=False, items=None, name=None, original_timestamps_enabled=False, scoped_to=None, status_message=None, swap_in=None, swap_out=None, updated_at=None):
+    def __init__(self, autoupdate_time_range=False, capsule_time=False, chain_view=False, created_at=None, export_capsules=False, export_name=None, grid_enabled=False, grid_origin=None, grid_size=None, href=None, id=None, is_archived=False, items=None, name=None, original_timestamps_enabled=False, scoped_to=None, status_message=None, swap_in=None, swap_out=None, time_zone=None, updated_at=None):
         """
         ExportItemsOutputV1 - a model defined in Swagger
         """
 
         self._autoupdate_time_range = None
         self._capsule_time = None
         self._chain_view = None
         self._created_at = None
         self._export_capsules = None
         self._export_name = None
         self._grid_enabled = None
+        self._grid_origin = None
         self._grid_size = None
+        self._href = None
         self._id = None
         self._is_archived = None
         self._items = None
         self._name = None
         self._original_timestamps_enabled = None
         self._scoped_to = None
         self._status_message = None
         self._swap_in = None
         self._swap_out = None
+        self._time_zone = None
         self._updated_at = None
 
         if autoupdate_time_range is not None:
           self.autoupdate_time_range = autoupdate_time_range
         if capsule_time is not None:
           self.capsule_time = capsule_time
         if chain_view is not None:
@@ -105,16 +114,20 @@
           self.created_at = created_at
         if export_capsules is not None:
           self.export_capsules = export_capsules
         if export_name is not None:
           self.export_name = export_name
         if grid_enabled is not None:
           self.grid_enabled = grid_enabled
+        if grid_origin is not None:
+          self.grid_origin = grid_origin
         if grid_size is not None:
           self.grid_size = grid_size
+        if href is not None:
+          self.href = href
         if id is not None:
           self.id = id
         if is_archived is not None:
           self.is_archived = is_archived
         if items is not None:
           self.items = items
         if name is not None:
@@ -125,14 +138,16 @@
           self.scoped_to = scoped_to
         if status_message is not None:
           self.status_message = status_message
         if swap_in is not None:
           self.swap_in = swap_in
         if swap_out is not None:
           self.swap_out = swap_out
+        if time_zone is not None:
+          self.time_zone = time_zone
         if updated_at is not None:
           self.updated_at = updated_at
 
     @property
     def autoupdate_time_range(self):
         """
         Gets the autoupdate_time_range of this ExportItemsOutputV1.
@@ -290,14 +305,37 @@
         :param grid_enabled: The grid_enabled of this ExportItemsOutputV1.
         :type: bool
         """
 
         self._grid_enabled = grid_enabled
 
     @property
+    def grid_origin(self):
+        """
+        Gets the grid_origin of this ExportItemsOutputV1.
+        The origin timestamp for gridding.
+
+        :return: The grid_origin of this ExportItemsOutputV1.
+        :rtype: str
+        """
+        return self._grid_origin
+
+    @grid_origin.setter
+    def grid_origin(self, grid_origin):
+        """
+        Sets the grid_origin of this ExportItemsOutputV1.
+        The origin timestamp for gridding.
+
+        :param grid_origin: The grid_origin of this ExportItemsOutputV1.
+        :type: str
+        """
+
+        self._grid_origin = grid_origin
+
+    @property
     def grid_size(self):
         """
         Gets the grid_size of this ExportItemsOutputV1.
         The desired sample period for the export. An automatic grid size is used when gridSize is set to 'false'.
 
         :return: The grid_size of this ExportItemsOutputV1.
         :rtype: str
@@ -313,14 +351,37 @@
         :param grid_size: The grid_size of this ExportItemsOutputV1.
         :type: str
         """
 
         self._grid_size = grid_size
 
     @property
+    def href(self):
+        """
+        Gets the href of this ExportItemsOutputV1.
+        The HREF where the export data is accessible
+
+        :return: The href of this ExportItemsOutputV1.
+        :rtype: str
+        """
+        return self._href
+
+    @href.setter
+    def href(self, href):
+        """
+        Sets the href of this ExportItemsOutputV1.
+        The HREF where the export data is accessible
+
+        :param href: The href of this ExportItemsOutputV1.
+        :type: str
+        """
+
+        self._href = href
+
+    @property
     def id(self):
         """
         Gets the id of this ExportItemsOutputV1.
         The ID that can be used to interact with the item
 
         :return: The id of this ExportItemsOutputV1.
         :rtype: str
@@ -524,14 +585,37 @@
         :param swap_out: The swap_out of this ExportItemsOutputV1.
         :type: str
         """
 
         self._swap_out = swap_out
 
     @property
+    def time_zone(self):
+        """
+        Gets the time_zone of this ExportItemsOutputV1.
+        The IANA time zone name for all timestamps in this export.
+
+        :return: The time_zone of this ExportItemsOutputV1.
+        :rtype: str
+        """
+        return self._time_zone
+
+    @time_zone.setter
+    def time_zone(self, time_zone):
+        """
+        Sets the time_zone of this ExportItemsOutputV1.
+        The IANA time zone name for all timestamps in this export.
+
+        :param time_zone: The time_zone of this ExportItemsOutputV1.
+        :type: str
+        """
+
+        self._time_zone = time_zone
+
+    @property
     def updated_at(self):
         """
         Gets the updated_at of this ExportItemsOutputV1.
         The ISO 8601 date and time of when the export was updated/run (YYYY-MM-DDThh:mm:ss.sssssssss±hh:mm)
 
         :return: The updated_at of this ExportItemsOutputV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/export_items_v1.py` & `seeq-62.0.1/seeq/sdk/models/export_items_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/export_preview_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/export_preview_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/export_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/export_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/folded_stack_node_v1.py` & `seeq-62.0.1/seeq/sdk/models/folded_stack_node_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/folder_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/folder_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/folder_navigation_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/folder_navigation_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/folder_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/folder_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_compile_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_compile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_compiler_error_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_compiler_error_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_dependency_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_dependency_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_example_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_example_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_example_list_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_example_list_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_keyword_list_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_summaries_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_summaries_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_doc_summary_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_doc_summary_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_error_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_error_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -140,15 +140,15 @@
         """
         Sets the error_type of this FormulaErrorOutputV1.
         The type of formula error that occurred
 
         :param error_type: The error_type of this FormulaErrorOutputV1.
         :type: str
         """
-        allowed_values = ["SYNTAX_ERROR", "METADATA_ERROR", "DATA_SPEC_ERROR", "RUNTIME_ERROR", "INCOMPATIBLE_UNITS", "MAX_DURATION_REQUIRED", "MAX_DURATION_PROHIBITED", "CONTINUOUS_REQUIRED", "PROPERTY_ERROR", "LOCALLY_CONSTANT", "ILLEGAL_VALUE", "ILLEGAL_PARAMETER", "UPSTREAM_ERROR"]
+        allowed_values = ["SYNTAX_ERROR", "METADATA_ERROR", "DATA_SPEC_ERROR", "RUNTIME_ERROR", "INCOMPATIBLE_UNITS", "MAX_DURATION_REQUIRED", "MAX_DURATION_PROHIBITED", "CONTINUOUS_REQUIRED", "PROPERTY_ERROR", "LOCALLY_CONSTANT", "ILLEGAL_VALUE", "ILLEGAL_PARAMETER", "UPSTREAM_ERROR", "UDF_NOT_FOUND_ERROR"]
         if error_type not in allowed_values:
             raise ValueError(
                 "Invalid value for `error_type` ({0}), must be one of {1}"
                 .format(error_type, allowed_values)
             )
 
         self._error_type = error_type
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_example_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_example_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_item_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_item_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_item_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_log_entry.py` & `seeq-62.0.1/seeq/sdk/models/formula_log_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_log_entry_details.py` & `seeq-62.0.1/seeq/sdk/models/formula_log_entry_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_log_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_log_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_package_import_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_package_import_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_package_import_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_package_import_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_package_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_package_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_package_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_package_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_parameter_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_parameter_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_parameter_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_parameter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_run_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_run_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_run_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_run_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_token.py` & `seeq-62.0.1/seeq/sdk/models/formula_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_update_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_update_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_upgrade_change_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_upgrade_change_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/formula_upgrade_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/formula_upgrade_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/function_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/function_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/function_parameter_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/function_parameter_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/function_variant_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/function_variant_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/gauge_datum_v1.py` & `seeq-62.0.1/seeq/sdk/models/gauge_datum_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/generic_table_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/generic_table_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_add_on_tools_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_add_on_tools_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_channels_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_channels_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_condition_monitor_items_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_content_items_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_content_items_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_date_ranges_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_date_ranges_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_jobs_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_jobs_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_metrics_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_metrics_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_projects_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_projects_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_request_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_requests_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_requests_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_sample_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_samples_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_samples_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/get_signals_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/get_signals_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/id_images_body.py` & `seeq-62.0.1/seeq/sdk/models/id_images_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/identity_mapping_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/identity_mapping_list_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/identity_mapping_v1.py` & `seeq-62.0.1/seeq/sdk/models/identity_mapping_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/identity_preview_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/identity_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/identity_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/identity_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/indexing_parameters_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/indexing_parameters_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/installer_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/installer_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/interval_v1.py` & `seeq-62.0.1/seeq/sdk/models/interval_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/invalid_swap_out_v1.py` & `seeq-62.0.1/seeq/sdk/models/invalid_swap_out_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_batch_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_batch_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_dependency_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_dependency_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_id_list_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_id_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_parameter_of_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_parameter_of_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_preview_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_update_output_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,224 +1,188 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ItemPreviewV1(object):
+class ItemUpdateOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'is_archived': 'bool',
-        'is_redacted': 'bool',
-        'name': 'str',
-        'translation_key': 'str',
-        'type': 'str'
+        'data_id': 'str',
+        'datasource_class': 'str',
+        'datasource_id': 'str',
+        'error_message': 'str',
+        'item': 'ItemPreviewV1'
     }
 
     attribute_map = {
-        'id': 'id',
-        'is_archived': 'isArchived',
-        'is_redacted': 'isRedacted',
-        'name': 'name',
-        'translation_key': 'translationKey',
-        'type': 'type'
+        'data_id': 'dataId',
+        'datasource_class': 'datasourceClass',
+        'datasource_id': 'datasourceId',
+        'error_message': 'errorMessage',
+        'item': 'item'
     }
 
-    def __init__(self, id=None, is_archived=False, is_redacted=False, name=None, translation_key=None, type=None):
+    def __init__(self, data_id=None, datasource_class=None, datasource_id=None, error_message=None, item=None):
         """
-        ItemPreviewV1 - a model defined in Swagger
+        ItemUpdateOutputV1 - a model defined in Swagger
         """
 
-        self._id = None
-        self._is_archived = None
-        self._is_redacted = None
-        self._name = None
-        self._translation_key = None
-        self._type = None
-
-        if id is not None:
-          self.id = id
-        if is_archived is not None:
-          self.is_archived = is_archived
-        if is_redacted is not None:
-          self.is_redacted = is_redacted
-        if name is not None:
-          self.name = name
-        if translation_key is not None:
-          self.translation_key = translation_key
-        if type is not None:
-          self.type = type
+        self._data_id = None
+        self._datasource_class = None
+        self._datasource_id = None
+        self._error_message = None
+        self._item = None
+
+        if data_id is not None:
+          self.data_id = data_id
+        if datasource_class is not None:
+          self.datasource_class = datasource_class
+        if datasource_id is not None:
+          self.datasource_id = datasource_id
+        if error_message is not None:
+          self.error_message = error_message
+        if item is not None:
+          self.item = item
 
     @property
-    def id(self):
+    def data_id(self):
         """
-        Gets the id of this ItemPreviewV1.
-        The ID that can be used to interact with the item
+        Gets the data_id of this ItemUpdateOutputV1.
+        An ID which uniquely identifies the item within the datasource that hosts it
 
-        :return: The id of this ItemPreviewV1.
+        :return: The data_id of this ItemUpdateOutputV1.
         :rtype: str
         """
-        return self._id
+        return self._data_id
 
-    @id.setter
-    def id(self, id):
+    @data_id.setter
+    def data_id(self, data_id):
         """
-        Sets the id of this ItemPreviewV1.
-        The ID that can be used to interact with the item
+        Sets the data_id of this ItemUpdateOutputV1.
+        An ID which uniquely identifies the item within the datasource that hosts it
 
-        :param id: The id of this ItemPreviewV1.
+        :param data_id: The data_id of this ItemUpdateOutputV1.
         :type: str
         """
-        if id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")
 
-        self._id = id
+        self._data_id = data_id
 
     @property
-    def is_archived(self):
-        """
-        Gets the is_archived of this ItemPreviewV1.
-        Whether item is archived
-
-        :return: The is_archived of this ItemPreviewV1.
-        :rtype: bool
-        """
-        return self._is_archived
-
-    @is_archived.setter
-    def is_archived(self, is_archived):
-        """
-        Sets the is_archived of this ItemPreviewV1.
-        Whether item is archived
-
-        :param is_archived: The is_archived of this ItemPreviewV1.
-        :type: bool
+    def datasource_class(self):
         """
+        Gets the datasource_class of this ItemUpdateOutputV1.
+        The class of the datasource that hosts the item
 
-        self._is_archived = is_archived
-
-    @property
-    def is_redacted(self):
-        """
-        Gets the is_redacted of this ItemPreviewV1.
-        Whether item is redacted
-
-        :return: The is_redacted of this ItemPreviewV1.
-        :rtype: bool
+        :return: The datasource_class of this ItemUpdateOutputV1.
+        :rtype: str
         """
-        return self._is_redacted
+        return self._datasource_class
 
-    @is_redacted.setter
-    def is_redacted(self, is_redacted):
+    @datasource_class.setter
+    def datasource_class(self, datasource_class):
         """
-        Sets the is_redacted of this ItemPreviewV1.
-        Whether item is redacted
+        Sets the datasource_class of this ItemUpdateOutputV1.
+        The class of the datasource that hosts the item
 
-        :param is_redacted: The is_redacted of this ItemPreviewV1.
-        :type: bool
+        :param datasource_class: The datasource_class of this ItemUpdateOutputV1.
+        :type: str
         """
 
-        self._is_redacted = is_redacted
+        self._datasource_class = datasource_class
 
     @property
-    def name(self):
+    def datasource_id(self):
         """
-        Gets the name of this ItemPreviewV1.
-        The human readable name
+        Gets the datasource_id of this ItemUpdateOutputV1.
+        The ID of the datasource that hosts the item.
 
-        :return: The name of this ItemPreviewV1.
+        :return: The datasource_id of this ItemUpdateOutputV1.
         :rtype: str
         """
-        return self._name
+        return self._datasource_id
 
-    @name.setter
-    def name(self, name):
+    @datasource_id.setter
+    def datasource_id(self, datasource_id):
         """
-        Sets the name of this ItemPreviewV1.
-        The human readable name
+        Sets the datasource_id of this ItemUpdateOutputV1.
+        The ID of the datasource that hosts the item.
 
-        :param name: The name of this ItemPreviewV1.
+        :param datasource_id: The datasource_id of this ItemUpdateOutputV1.
         :type: str
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._name = name
+        self._datasource_id = datasource_id
 
     @property
-    def translation_key(self):
+    def error_message(self):
         """
-        Gets the translation_key of this ItemPreviewV1.
-        The item's translation key, if any
+        Gets the error_message of this ItemUpdateOutputV1.
+        If the update failed, this field will contain an error message explaining the problem
 
-        :return: The translation_key of this ItemPreviewV1.
+        :return: The error_message of this ItemUpdateOutputV1.
         :rtype: str
         """
-        return self._translation_key
+        return self._error_message
 
-    @translation_key.setter
-    def translation_key(self, translation_key):
+    @error_message.setter
+    def error_message(self, error_message):
         """
-        Sets the translation_key of this ItemPreviewV1.
-        The item's translation key, if any
+        Sets the error_message of this ItemUpdateOutputV1.
+        If the update failed, this field will contain an error message explaining the problem
 
-        :param translation_key: The translation_key of this ItemPreviewV1.
+        :param error_message: The error_message of this ItemUpdateOutputV1.
         :type: str
         """
 
-        self._translation_key = translation_key
+        self._error_message = error_message
 
     @property
-    def type(self):
+    def item(self):
         """
-        Gets the type of this ItemPreviewV1.
-        The type of the item
+        Gets the item of this ItemUpdateOutputV1.
 
-        :return: The type of this ItemPreviewV1.
-        :rtype: str
+        :return: The item of this ItemUpdateOutputV1.
+        :rtype: ItemPreviewV1
         """
-        return self._type
+        return self._item
 
-    @type.setter
-    def type(self, type):
+    @item.setter
+    def item(self, item):
         """
-        Sets the type of this ItemPreviewV1.
-        The type of the item
+        Sets the item of this ItemUpdateOutputV1.
 
-        :param type: The type of this ItemPreviewV1.
-        :type: str
+        :param item: The item of this ItemUpdateOutputV1.
+        :type: ItemPreviewV1
         """
-        if type is None:
-            raise ValueError("Invalid value for `type`, must not be `None`")
 
-        self._type = type
+        self._item = item
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -254,15 +218,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ItemPreviewV1):
+        if not isinstance(other, ItemUpdateOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_preview_with_assets_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_preview_with_assets_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_search_preview_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_search_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_search_preview_paginated_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_search_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_search_preview_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -31,54 +31,60 @@
     """
     swagger_types = {
         'ancestors': 'list[ItemPreviewV1]',
         'datasource': 'ItemPreviewV1',
         'description': 'str',
         'has_children': 'bool',
         'id': 'str',
+        'included_properties': 'dict(str, ScalarPropertyV1)',
         'is_archived': 'bool',
         'is_asset_group_item': 'bool',
         'is_redacted': 'bool',
         'name': 'str',
+        'parameters': 'list[FormulaParameterOutputV1]',
         'source_value_unit_of_measure': 'str',
         'translation_key': 'str',
         'type': 'str',
         'value_unit_of_measure': 'str'
     }
 
     attribute_map = {
         'ancestors': 'ancestors',
         'datasource': 'datasource',
         'description': 'description',
         'has_children': 'hasChildren',
         'id': 'id',
+        'included_properties': 'includedProperties',
         'is_archived': 'isArchived',
         'is_asset_group_item': 'isAssetGroupItem',
         'is_redacted': 'isRedacted',
         'name': 'name',
+        'parameters': 'parameters',
         'source_value_unit_of_measure': 'sourceValueUnitOfMeasure',
         'translation_key': 'translationKey',
         'type': 'type',
         'value_unit_of_measure': 'valueUnitOfMeasure'
     }
 
-    def __init__(self, ancestors=None, datasource=None, description=None, has_children=False, id=None, is_archived=False, is_asset_group_item=False, is_redacted=False, name=None, source_value_unit_of_measure=None, translation_key=None, type=None, value_unit_of_measure=None):
+    def __init__(self, ancestors=None, datasource=None, description=None, has_children=False, id=None, included_properties=None, is_archived=False, is_asset_group_item=False, is_redacted=False, name=None, parameters=None, source_value_unit_of_measure=None, translation_key=None, type=None, value_unit_of_measure=None):
         """
         ItemSearchPreviewV1 - a model defined in Swagger
         """
 
         self._ancestors = None
         self._datasource = None
         self._description = None
         self._has_children = None
         self._id = None
+        self._included_properties = None
         self._is_archived = None
         self._is_asset_group_item = None
         self._is_redacted = None
         self._name = None
+        self._parameters = None
         self._source_value_unit_of_measure = None
         self._translation_key = None
         self._type = None
         self._value_unit_of_measure = None
 
         if ancestors is not None:
           self.ancestors = ancestors
@@ -86,22 +92,26 @@
           self.datasource = datasource
         if description is not None:
           self.description = description
         if has_children is not None:
           self.has_children = has_children
         if id is not None:
           self.id = id
+        if included_properties is not None:
+          self.included_properties = included_properties
         if is_archived is not None:
           self.is_archived = is_archived
         if is_asset_group_item is not None:
           self.is_asset_group_item = is_asset_group_item
         if is_redacted is not None:
           self.is_redacted = is_redacted
         if name is not None:
           self.name = name
+        if parameters is not None:
+          self.parameters = parameters
         if source_value_unit_of_measure is not None:
           self.source_value_unit_of_measure = source_value_unit_of_measure
         if translation_key is not None:
           self.translation_key = translation_key
         if type is not None:
           self.type = type
         if value_unit_of_measure is not None:
@@ -219,14 +229,37 @@
         """
         if id is None:
             raise ValueError("Invalid value for `id`, must not be `None`")
 
         self._id = id
 
     @property
+    def included_properties(self):
+        """
+        Gets the included_properties of this ItemSearchPreviewV1.
+        Item properties mapped by name, corresponding to the properties requested for the search. Note that this will be empty if no properties were requested.
+
+        :return: The included_properties of this ItemSearchPreviewV1.
+        :rtype: dict(str, ScalarPropertyV1)
+        """
+        return self._included_properties
+
+    @included_properties.setter
+    def included_properties(self, included_properties):
+        """
+        Sets the included_properties of this ItemSearchPreviewV1.
+        Item properties mapped by name, corresponding to the properties requested for the search. Note that this will be empty if no properties were requested.
+
+        :param included_properties: The included_properties of this ItemSearchPreviewV1.
+        :type: dict(str, ScalarPropertyV1)
+        """
+
+        self._included_properties = included_properties
+
+    @property
     def is_archived(self):
         """
         Gets the is_archived of this ItemSearchPreviewV1.
         Whether item is archived
 
         :return: The is_archived of this ItemSearchPreviewV1.
         :rtype: bool
@@ -313,14 +346,35 @@
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
 
         self._name = name
 
     @property
+    def parameters(self):
+        """
+        Gets the parameters of this ItemSearchPreviewV1.
+
+        :return: The parameters of this ItemSearchPreviewV1.
+        :rtype: list[FormulaParameterOutputV1]
+        """
+        return self._parameters
+
+    @parameters.setter
+    def parameters(self, parameters):
+        """
+        Sets the parameters of this ItemSearchPreviewV1.
+
+        :param parameters: The parameters of this ItemSearchPreviewV1.
+        :type: list[FormulaParameterOutputV1]
+        """
+
+        self._parameters = parameters
+
+    @property
     def source_value_unit_of_measure(self):
         """
         Gets the source_value_unit_of_measure of this ItemSearchPreviewV1.
         The datasource's original, unparsed unit of measure for the values, if it exists
 
         :return: The source_value_unit_of_measure of this ItemSearchPreviewV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_swap_result_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_swap_result_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_update_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/property_output_v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,188 +1,194 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class ItemUpdateOutputV1(object):
+class PropertyOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data_id': 'str',
-        'datasource_class': 'str',
-        'datasource_id': 'str',
-        'error_message': 'str',
-        'item': 'ItemPreviewV1'
+        'href': 'str',
+        'name': 'str',
+        'status_message': 'str',
+        'unit_of_measure': 'str',
+        'value': 'str'
     }
 
     attribute_map = {
-        'data_id': 'dataId',
-        'datasource_class': 'datasourceClass',
-        'datasource_id': 'datasourceId',
-        'error_message': 'errorMessage',
-        'item': 'item'
+        'href': 'href',
+        'name': 'name',
+        'status_message': 'statusMessage',
+        'unit_of_measure': 'unitOfMeasure',
+        'value': 'value'
     }
 
-    def __init__(self, data_id=None, datasource_class=None, datasource_id=None, error_message=None, item=None):
+    def __init__(self, href=None, name=None, status_message=None, unit_of_measure=None, value=None):
         """
-        ItemUpdateOutputV1 - a model defined in Swagger
+        PropertyOutputV1 - a model defined in Swagger
         """
 
-        self._data_id = None
-        self._datasource_class = None
-        self._datasource_id = None
-        self._error_message = None
-        self._item = None
-
-        if data_id is not None:
-          self.data_id = data_id
-        if datasource_class is not None:
-          self.datasource_class = datasource_class
-        if datasource_id is not None:
-          self.datasource_id = datasource_id
-        if error_message is not None:
-          self.error_message = error_message
-        if item is not None:
-          self.item = item
+        self._href = None
+        self._name = None
+        self._status_message = None
+        self._unit_of_measure = None
+        self._value = None
+
+        if href is not None:
+          self.href = href
+        if name is not None:
+          self.name = name
+        if status_message is not None:
+          self.status_message = status_message
+        if unit_of_measure is not None:
+          self.unit_of_measure = unit_of_measure
+        if value is not None:
+          self.value = value
 
     @property
-    def data_id(self):
+    def href(self):
         """
-        Gets the data_id of this ItemUpdateOutputV1.
-        An ID which uniquely identifies the item within the datasource that hosts it
+        Gets the href of this PropertyOutputV1.
+        The href that can be used to interact with the property
 
-        :return: The data_id of this ItemUpdateOutputV1.
+        :return: The href of this PropertyOutputV1.
         :rtype: str
         """
-        return self._data_id
+        return self._href
 
-    @data_id.setter
-    def data_id(self, data_id):
+    @href.setter
+    def href(self, href):
         """
-        Sets the data_id of this ItemUpdateOutputV1.
-        An ID which uniquely identifies the item within the datasource that hosts it
+        Sets the href of this PropertyOutputV1.
+        The href that can be used to interact with the property
 
-        :param data_id: The data_id of this ItemUpdateOutputV1.
+        :param href: The href of this PropertyOutputV1.
         :type: str
         """
+        if href is None:
+            raise ValueError("Invalid value for `href`, must not be `None`")
 
-        self._data_id = data_id
+        self._href = href
 
     @property
-    def datasource_class(self):
+    def name(self):
         """
-        Gets the datasource_class of this ItemUpdateOutputV1.
-        The class of the datasource that hosts the item
+        Gets the name of this PropertyOutputV1.
+        The name of this property
 
-        :return: The datasource_class of this ItemUpdateOutputV1.
+        :return: The name of this PropertyOutputV1.
         :rtype: str
         """
-        return self._datasource_class
+        return self._name
 
-    @datasource_class.setter
-    def datasource_class(self, datasource_class):
+    @name.setter
+    def name(self, name):
         """
-        Sets the datasource_class of this ItemUpdateOutputV1.
-        The class of the datasource that hosts the item
+        Sets the name of this PropertyOutputV1.
+        The name of this property
 
-        :param datasource_class: The datasource_class of this ItemUpdateOutputV1.
+        :param name: The name of this PropertyOutputV1.
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._datasource_class = datasource_class
+        self._name = name
 
     @property
-    def datasource_id(self):
+    def status_message(self):
         """
-        Gets the datasource_id of this ItemUpdateOutputV1.
-        The ID of the datasource that hosts the item.
+        Gets the status_message of this PropertyOutputV1.
+        A plain language status message with information about any issues that may have been encountered during an operation
 
-        :return: The datasource_id of this ItemUpdateOutputV1.
+        :return: The status_message of this PropertyOutputV1.
         :rtype: str
         """
-        return self._datasource_id
+        return self._status_message
 
-    @datasource_id.setter
-    def datasource_id(self, datasource_id):
+    @status_message.setter
+    def status_message(self, status_message):
         """
-        Sets the datasource_id of this ItemUpdateOutputV1.
-        The ID of the datasource that hosts the item.
+        Sets the status_message of this PropertyOutputV1.
+        A plain language status message with information about any issues that may have been encountered during an operation
 
-        :param datasource_id: The datasource_id of this ItemUpdateOutputV1.
+        :param status_message: The status_message of this PropertyOutputV1.
         :type: str
         """
 
-        self._datasource_id = datasource_id
+        self._status_message = status_message
 
     @property
-    def error_message(self):
+    def unit_of_measure(self):
         """
-        Gets the error_message of this ItemUpdateOutputV1.
-        If the update failed, this field will contain an error message explaining the problem
+        Gets the unit_of_measure of this PropertyOutputV1.
+        The unit of measure for this property's value
 
-        :return: The error_message of this ItemUpdateOutputV1.
+        :return: The unit_of_measure of this PropertyOutputV1.
         :rtype: str
         """
-        return self._error_message
+        return self._unit_of_measure
 
-    @error_message.setter
-    def error_message(self, error_message):
+    @unit_of_measure.setter
+    def unit_of_measure(self, unit_of_measure):
         """
-        Sets the error_message of this ItemUpdateOutputV1.
-        If the update failed, this field will contain an error message explaining the problem
+        Sets the unit_of_measure of this PropertyOutputV1.
+        The unit of measure for this property's value
 
-        :param error_message: The error_message of this ItemUpdateOutputV1.
+        :param unit_of_measure: The unit_of_measure of this PropertyOutputV1.
         :type: str
         """
 
-        self._error_message = error_message
+        self._unit_of_measure = unit_of_measure
 
     @property
-    def item(self):
+    def value(self):
         """
-        Gets the item of this ItemUpdateOutputV1.
+        Gets the value of this PropertyOutputV1.
+        The value of this property
 
-        :return: The item of this ItemUpdateOutputV1.
-        :rtype: ItemPreviewV1
+        :return: The value of this PropertyOutputV1.
+        :rtype: str
         """
-        return self._item
+        return self._value
 
-    @item.setter
-    def item(self, item):
+    @value.setter
+    def value(self, value):
         """
-        Sets the item of this ItemUpdateOutputV1.
+        Sets the value of this PropertyOutputV1.
+        The value of this property
 
-        :param item: The item of this ItemUpdateOutputV1.
-        :type: ItemPreviewV1
+        :param value: The value of this PropertyOutputV1.
+        :type: str
         """
 
-        self._item = item
+        self._value = value
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -218,15 +224,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ItemUpdateOutputV1):
+        if not isinstance(other, PropertyOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_user_attributes_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_user_attributes_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_user_attributes_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_user_attributes_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/item_with_swap_pairs_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_with_swap_pairs_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/job_accepted_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/job_accepted_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/job_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/job_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/json_backup_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/json_backup_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/license_importer_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/license_importer_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/license_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/license_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/licensed_feature_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/licensed_feature_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/log_message.py` & `seeq-62.0.1/seeq/sdk/models/log_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/meter_datum_v1.py` & `seeq-62.0.1/seeq/sdk/models/meter_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/migrate_editor_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/migrate_editor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitor_definition_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/monitor_definition_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitor_definitions_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/monitor_definitions_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitor_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/monitor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitor_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/monitor_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitor_values.py` & `seeq-62.0.1/seeq/sdk/models/monitor_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/monitors_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/monitors_output_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/notifiable_report_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/notifiable_report_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/notifiable_report_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/notifiable_report_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/notification_configuration_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/notification_configuration_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/optional_report_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/optional_report_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/parameter_doc_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/parameter_doc_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/permissions_v1.py` & `seeq-62.0.1/seeq/sdk/models/permissions_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/plugin_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/plugin_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/plugin_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/plugin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/plugins_body.py` & `seeq-62.0.1/seeq/sdk/models/plugins_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/priority_v1.py` & `seeq-62.0.1/seeq/sdk/models/priority_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/progress_information_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/progress_information_output_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/project_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/project_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/project_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/project_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/property_href_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/property_href_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/property_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/property_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/property_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/workbook_output_list_v1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,194 +1,218 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class PropertyOutputV1(object):
+class WorkbookOutputListV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'href': 'str',
-        'name': 'str',
+        'limit': 'int',
+        'next': 'str',
+        'offset': 'int',
+        'prev': 'str',
         'status_message': 'str',
-        'unit_of_measure': 'str',
-        'value': 'str'
+        'workbooks': 'list[WorkbookOutputV1]'
     }
 
     attribute_map = {
-        'href': 'href',
-        'name': 'name',
+        'limit': 'limit',
+        'next': 'next',
+        'offset': 'offset',
+        'prev': 'prev',
         'status_message': 'statusMessage',
-        'unit_of_measure': 'unitOfMeasure',
-        'value': 'value'
+        'workbooks': 'workbooks'
     }
 
-    def __init__(self, href=None, name=None, status_message=None, unit_of_measure=None, value=None):
+    def __init__(self, limit=None, next=None, offset=None, prev=None, status_message=None, workbooks=None):
         """
-        PropertyOutputV1 - a model defined in Swagger
+        WorkbookOutputListV1 - a model defined in Swagger
         """
 
-        self._href = None
-        self._name = None
+        self._limit = None
+        self._next = None
+        self._offset = None
+        self._prev = None
         self._status_message = None
-        self._unit_of_measure = None
-        self._value = None
+        self._workbooks = None
 
-        if href is not None:
-          self.href = href
-        if name is not None:
-          self.name = name
+        if limit is not None:
+          self.limit = limit
+        if next is not None:
+          self.next = next
+        if offset is not None:
+          self.offset = offset
+        if prev is not None:
+          self.prev = prev
         if status_message is not None:
           self.status_message = status_message
-        if unit_of_measure is not None:
-          self.unit_of_measure = unit_of_measure
-        if value is not None:
-          self.value = value
+        if workbooks is not None:
+          self.workbooks = workbooks
 
     @property
-    def href(self):
+    def limit(self):
         """
-        Gets the href of this PropertyOutputV1.
-        The href that can be used to interact with the property
+        Gets the limit of this WorkbookOutputListV1.
+        The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :return: The href of this PropertyOutputV1.
-        :rtype: str
+        :return: The limit of this WorkbookOutputListV1.
+        :rtype: int
         """
-        return self._href
+        return self._limit
 
-    @href.setter
-    def href(self, href):
+    @limit.setter
+    def limit(self, limit):
         """
-        Sets the href of this PropertyOutputV1.
-        The href that can be used to interact with the property
+        Sets the limit of this WorkbookOutputListV1.
+        The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :param href: The href of this PropertyOutputV1.
-        :type: str
+        :param limit: The limit of this WorkbookOutputListV1.
+        :type: int
         """
-        if href is None:
-            raise ValueError("Invalid value for `href`, must not be `None`")
 
-        self._href = href
+        self._limit = limit
 
     @property
-    def name(self):
+    def next(self):
         """
-        Gets the name of this PropertyOutputV1.
-        The name of this property
+        Gets the next of this WorkbookOutputListV1.
+        The href of the next set of paginated results
 
-        :return: The name of this PropertyOutputV1.
+        :return: The next of this WorkbookOutputListV1.
         :rtype: str
         """
-        return self._name
+        return self._next
 
-    @name.setter
-    def name(self, name):
+    @next.setter
+    def next(self, next):
         """
-        Sets the name of this PropertyOutputV1.
-        The name of this property
+        Sets the next of this WorkbookOutputListV1.
+        The href of the next set of paginated results
 
-        :param name: The name of this PropertyOutputV1.
+        :param next: The next of this WorkbookOutputListV1.
         :type: str
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._name = name
+        self._next = next
 
     @property
-    def status_message(self):
+    def offset(self):
         """
-        Gets the status_message of this PropertyOutputV1.
-        A plain language status message with information about any issues that may have been encountered during an operation
+        Gets the offset of this WorkbookOutputListV1.
+        The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :return: The status_message of this PropertyOutputV1.
-        :rtype: str
+        :return: The offset of this WorkbookOutputListV1.
+        :rtype: int
         """
-        return self._status_message
+        return self._offset
 
-    @status_message.setter
-    def status_message(self, status_message):
+    @offset.setter
+    def offset(self, offset):
         """
-        Sets the status_message of this PropertyOutputV1.
-        A plain language status message with information about any issues that may have been encountered during an operation
+        Sets the offset of this WorkbookOutputListV1.
+        The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :param status_message: The status_message of this PropertyOutputV1.
-        :type: str
+        :param offset: The offset of this WorkbookOutputListV1.
+        :type: int
         """
 
-        self._status_message = status_message
+        self._offset = offset
 
     @property
-    def unit_of_measure(self):
+    def prev(self):
         """
-        Gets the unit_of_measure of this PropertyOutputV1.
-        The unit of measure for this property's value
+        Gets the prev of this WorkbookOutputListV1.
+        The href of the previous set of paginated results
 
-        :return: The unit_of_measure of this PropertyOutputV1.
+        :return: The prev of this WorkbookOutputListV1.
         :rtype: str
         """
-        return self._unit_of_measure
+        return self._prev
 
-    @unit_of_measure.setter
-    def unit_of_measure(self, unit_of_measure):
+    @prev.setter
+    def prev(self, prev):
         """
-        Sets the unit_of_measure of this PropertyOutputV1.
-        The unit of measure for this property's value
+        Sets the prev of this WorkbookOutputListV1.
+        The href of the previous set of paginated results
 
-        :param unit_of_measure: The unit_of_measure of this PropertyOutputV1.
+        :param prev: The prev of this WorkbookOutputListV1.
         :type: str
         """
 
-        self._unit_of_measure = unit_of_measure
+        self._prev = prev
 
     @property
-    def value(self):
+    def status_message(self):
         """
-        Gets the value of this PropertyOutputV1.
-        The value of this property
+        Gets the status_message of this WorkbookOutputListV1.
+        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :return: The value of this PropertyOutputV1.
+        :return: The status_message of this WorkbookOutputListV1.
         :rtype: str
         """
-        return self._value
+        return self._status_message
 
-    @value.setter
-    def value(self, value):
+    @status_message.setter
+    def status_message(self, status_message):
         """
-        Sets the value of this PropertyOutputV1.
-        The value of this property
+        Sets the status_message of this WorkbookOutputListV1.
+        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :param value: The value of this PropertyOutputV1.
+        :param status_message: The status_message of this WorkbookOutputListV1.
         :type: str
         """
 
-        self._value = value
+        self._status_message = status_message
+
+    @property
+    def workbooks(self):
+        """
+        Gets the workbooks of this WorkbookOutputListV1.
+        The list of workbooks
+
+        :return: The workbooks of this WorkbookOutputListV1.
+        :rtype: list[WorkbookOutputV1]
+        """
+        return self._workbooks
+
+    @workbooks.setter
+    def workbooks(self, workbooks):
+        """
+        Sets the workbooks of this WorkbookOutputListV1.
+        The list of workbooks
+
+        :param workbooks: The workbooks of this WorkbookOutputListV1.
+        :type: list[WorkbookOutputV1]
+        """
+
+        self._workbooks = workbooks
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -224,15 +248,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, PropertyOutputV1):
+        if not isinstance(other, WorkbookOutputListV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/put_asset_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/put_asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/put_scalar_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/put_scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/put_scalars_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/put_scalars_input_v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -28,41 +28,36 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'datasource_class': 'str',
         'datasource_id': 'str',
-        'force_calculated_scalars': 'bool',
         'scalars': 'list[PutScalarInputV1]'
     }
 
     attribute_map = {
         'datasource_class': 'datasourceClass',
         'datasource_id': 'datasourceId',
-        'force_calculated_scalars': 'forceCalculatedScalars',
         'scalars': 'scalars'
     }
 
-    def __init__(self, datasource_class=None, datasource_id=None, force_calculated_scalars=False, scalars=None):
+    def __init__(self, datasource_class=None, datasource_id=None, scalars=None):
         """
         PutScalarsInputV1 - a model defined in Swagger
         """
 
         self._datasource_class = None
         self._datasource_id = None
-        self._force_calculated_scalars = None
         self._scalars = None
 
         if datasource_class is not None:
           self.datasource_class = datasource_class
         if datasource_id is not None:
           self.datasource_id = datasource_id
-        if force_calculated_scalars is not None:
-          self.force_calculated_scalars = force_calculated_scalars
         if scalars is not None:
           self.scalars = scalars
 
     @property
     def datasource_class(self):
         """
         Gets the datasource_class of this PutScalarsInputV1.
@@ -109,37 +104,14 @@
         """
         if datasource_id is None:
             raise ValueError("Invalid value for `datasource_id`, must not be `None`")
 
         self._datasource_id = datasource_id
 
     @property
-    def force_calculated_scalars(self):
-        """
-        Gets the force_calculated_scalars of this PutScalarsInputV1.
-        Set to true to force creation of CalculatedScalar (formula) types, which are editable in the UI. If false, scalars will be represented as LiteralScalar (constants) if possible, otherwise as CalculatedScalar.
-
-        :return: The force_calculated_scalars of this PutScalarsInputV1.
-        :rtype: bool
-        """
-        return self._force_calculated_scalars
-
-    @force_calculated_scalars.setter
-    def force_calculated_scalars(self, force_calculated_scalars):
-        """
-        Sets the force_calculated_scalars of this PutScalarsInputV1.
-        Set to true to force creation of CalculatedScalar (formula) types, which are editable in the UI. If false, scalars will be represented as LiteralScalar (constants) if possible, otherwise as CalculatedScalar.
-
-        :param force_calculated_scalars: The force_calculated_scalars of this PutScalarsInputV1.
-        :type: bool
-        """
-
-        self._force_calculated_scalars = force_calculated_scalars
-
-    @property
     def scalars(self):
         """
         Gets the scalars of this PutScalarsInputV1.
         A list of scalars to create or update
 
         :return: The scalars of this PutScalarsInputV1.
         :rtype: list[PutScalarInputV1]
```

### Comparing `seeq-61.1.4/seeq/sdk/models/put_signals_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/put_signals_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/put_user_groups_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/put_user_groups_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/referenced_items_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/referenced_items_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/regression_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/regression_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/remote_agent_directives_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/remote_agent_directives_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/remote_agent_status_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/remote_agent_status_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/remote_agent_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/remote_agent_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/report_input_item_v1.py` & `seeq-62.0.1/seeq/sdk/models/report_input_item_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/report_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/report_notification_configuration_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/report_notification_configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/report_template_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/report_template_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/report_template_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/report_template_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/request_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/sample_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/sample_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/sample_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/sample_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/samples_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/samples_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/samples_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/samples_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/samples_overwrite_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/samples_overwrite_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scalar_evaluate_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/scalar_evaluate_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scalar_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/scalar_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scalar_property_v1.py` & `seeq-62.0.1/seeq/sdk/models/scalar_property_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -57,26 +57,26 @@
         if value is not None:
           self.value = value
 
     @property
     def name(self):
         """
         Gets the name of this ScalarPropertyV1.
-        Human readable name.  Null or whitespace names are not permitted
+        Human readable name of the property. Null or whitespace names are not permitted
 
         :return: The name of this ScalarPropertyV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
         Sets the name of this ScalarPropertyV1.
-        Human readable name.  Null or whitespace names are not permitted
+        Human readable name of the property. Null or whitespace names are not permitted
 
         :param name: The name of this ScalarPropertyV1.
         :type: str
         """
         if name is None:
             raise ValueError("Invalid value for `name`, must not be `None`")
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scalar_value_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/scalar_value_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scale_across_tree_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/scale_across_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedulable_admin_list_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedulable_admin_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedulable_admin_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedulable_admin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedulable_summary_day_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedulable_summary_day_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedulable_summary_week_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedulable_summary_week_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedule_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedule_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/schedule_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/schedule_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scheduled_notebook_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/scheduled_notebook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scheduled_notebook_list_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/scheduled_notebook_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/scheduled_notebook_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/screenshot_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/screenshot_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/see_also_doc_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/see_also_doc_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/send_email_attachment_v1.py` & `seeq-62.0.1/seeq/sdk/models/send_email_attachment_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/send_email_contact_v1.py` & `seeq-62.0.1/seeq/sdk/models/send_email_contact_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/send_email_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/send_email_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/send_logs_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/label_category_output_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,128 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class SendLogsInputV1(object):
+class LabelCategoryOutputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'description': 'str',
-        'email': 'str',
+        'id': 'str',
+        'is_autocomplete': 'bool',
         'name': 'str'
     }
 
     attribute_map = {
-        'description': 'description',
-        'email': 'email',
+        'id': 'id',
+        'is_autocomplete': 'isAutocomplete',
         'name': 'name'
     }
 
-    def __init__(self, description=None, email=None, name=None):
+    def __init__(self, id=None, is_autocomplete=None, name=None):
         """
-        SendLogsInputV1 - a model defined in Swagger
+        LabelCategoryOutputV1 - a model defined in Swagger
         """
 
-        self._description = None
-        self._email = None
+        self._id = None
+        self._is_autocomplete = None
         self._name = None
 
-        if description is not None:
-          self.description = description
-        if email is not None:
-          self.email = email
+        if id is not None:
+          self.id = id
+        if is_autocomplete is not None:
+          self.is_autocomplete = is_autocomplete
         if name is not None:
           self.name = name
 
     @property
-    def description(self):
+    def id(self):
         """
-        Gets the description of this SendLogsInputV1.
-        The description to be sent with the logs
+        Gets the id of this LabelCategoryOutputV1.
+        ID of the label category
 
-        :return: The description of this SendLogsInputV1.
+        :return: The id of this LabelCategoryOutputV1.
         :rtype: str
         """
-        return self._description
+        return self._id
 
-    @description.setter
-    def description(self, description):
+    @id.setter
+    def id(self, id):
         """
-        Sets the description of this SendLogsInputV1.
-        The description to be sent with the logs
+        Sets the id of this LabelCategoryOutputV1.
+        ID of the label category
 
-        :param description: The description of this SendLogsInputV1.
+        :param id: The id of this LabelCategoryOutputV1.
         :type: str
         """
-        if description is None:
-            raise ValueError("Invalid value for `description`, must not be `None`")
 
-        self._description = description
+        self._id = id
 
     @property
-    def email(self):
+    def is_autocomplete(self):
         """
-        Gets the email of this SendLogsInputV1.
-        The log sender's email
+        Gets the is_autocomplete of this LabelCategoryOutputV1.
 
-        :return: The email of this SendLogsInputV1.
-        :rtype: str
+        :return: The is_autocomplete of this LabelCategoryOutputV1.
+        :rtype: bool
         """
-        return self._email
+        return self._is_autocomplete
 
-    @email.setter
-    def email(self, email):
+    @is_autocomplete.setter
+    def is_autocomplete(self, is_autocomplete):
         """
-        Sets the email of this SendLogsInputV1.
-        The log sender's email
+        Sets the is_autocomplete of this LabelCategoryOutputV1.
 
-        :param email: The email of this SendLogsInputV1.
-        :type: str
+        :param is_autocomplete: The is_autocomplete of this LabelCategoryOutputV1.
+        :type: bool
         """
-        if email is None:
-            raise ValueError("Invalid value for `email`, must not be `None`")
 
-        self._email = email
+        self._is_autocomplete = is_autocomplete
 
     @property
     def name(self):
         """
-        Gets the name of this SendLogsInputV1.
-        The log sender's name
+        Gets the name of this LabelCategoryOutputV1.
+        Name of the label category
 
-        :return: The name of this SendLogsInputV1.
+        :return: The name of this LabelCategoryOutputV1.
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """
-        Sets the name of this SendLogsInputV1.
-        The log sender's name
+        Sets the name of this LabelCategoryOutputV1.
+        Name of the label category
 
-        :param name: The name of this SendLogsInputV1.
+        :param name: The name of this LabelCategoryOutputV1.
         :type: str
         """
 
         self._name = name
 
     def to_dict(self):
         """
@@ -168,15 +162,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, SendLogsInputV1):
+        if not isinstance(other, LabelCategoryOutputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/server_build_info_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/server_build_info_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/server_load_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/server_load_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/server_spec_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/server_spec_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/server_status_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/server_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/signal_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/signal_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/signal_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/signal_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/signal_with_id_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/signal_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/status_message.py` & `seeq-62.0.1/seeq/sdk/models/status_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/status_message_base.py` & `seeq-62.0.1/seeq/sdk/models/status_message_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/subscription_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/subscription_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/subscription_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/subscription_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/subscription_update_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/subscription_update_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/supported_units_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/supported_units_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/swap_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/swap_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/swap_option_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/swap_option_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/swap_option_v1.py` & `seeq-62.0.1/seeq/sdk/models/swap_option_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/swap_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/swap_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/sync_progress.py` & `seeq-62.0.1/seeq/sdk/models/sync_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/sync_progress_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/sync_progress_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/system_license_body.py` & `seeq-62.0.1/seeq/sdk/models/system_license_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/table_column_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/table_column_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/table_definition_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/table_definition_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -82,26 +82,26 @@
         if subscription_id is not None:
           self.subscription_id = subscription_id
 
     @property
     def column_definitions(self):
         """
         Gets the column_definitions of this TableDefinitionInputV1.
-        Column definitions for the Table. A column definition contains all the properties that define each column in the table
+        Column definitions for the Table. A column definition contains all the properties that define each column in the table. An \"item id\" column is required and must reference a Seeq item (e.g. Condition ID). A \"datum id\" column is required because it is used to uniquely identify a row (e.g. Capsule Start property).
 
         :return: The column_definitions of this TableDefinitionInputV1.
         :rtype: list[ColumnDefinitionInputV1]
         """
         return self._column_definitions
 
     @column_definitions.setter
     def column_definitions(self, column_definitions):
         """
         Sets the column_definitions of this TableDefinitionInputV1.
-        Column definitions for the Table. A column definition contains all the properties that define each column in the table
+        Column definitions for the Table. A column definition contains all the properties that define each column in the table. An \"item id\" column is required and must reference a Seeq item (e.g. Condition ID). A \"datum id\" column is required because it is used to uniquely identify a row (e.g. Capsule Start property).
 
         :param column_definitions: The column_definitions of this TableDefinitionInputV1.
         :type: list[ColumnDefinitionInputV1]
         """
         if column_definitions is None:
             raise ValueError("Invalid value for `column_definitions`, must not be `None`")
 
@@ -263,16 +263,14 @@
         """
         Sets the subscription_id of this TableDefinitionInputV1.
         The ID of the item (only condition monitors supported for now) to subscribe to.
 
         :param subscription_id: The subscription_id of this TableDefinitionInputV1.
         :type: str
         """
-        if subscription_id is None:
-            raise ValueError("Invalid value for `subscription_id`, must not be `None`")
 
         self._subscription_id = subscription_id
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
```

### Comparing `seeq-61.1.4/seeq/sdk/models/table_definition_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/table_definition_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/table_definition_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/table_definition_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -26,52 +26,55 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'column_definitions': 'list[ColumnDefinition]',
+        'column_definitions': 'list[ColumnDefinitionOutputV1]',
         'description': 'str',
         'effective_permissions': 'PermissionsV1',
         'id': 'str',
         'is_archived': 'bool',
         'is_redacted': 'bool',
         'name': 'str',
         'status_message': 'str',
+        'subscription': 'ItemPreviewV1',
         'translation_key': 'str',
         'type': 'str'
     }
 
     attribute_map = {
         'column_definitions': 'columnDefinitions',
         'description': 'description',
         'effective_permissions': 'effectivePermissions',
         'id': 'id',
         'is_archived': 'isArchived',
         'is_redacted': 'isRedacted',
         'name': 'name',
         'status_message': 'statusMessage',
+        'subscription': 'subscription',
         'translation_key': 'translationKey',
         'type': 'type'
     }
 
-    def __init__(self, column_definitions=None, description=None, effective_permissions=None, id=None, is_archived=False, is_redacted=False, name=None, status_message=None, translation_key=None, type=None):
+    def __init__(self, column_definitions=None, description=None, effective_permissions=None, id=None, is_archived=False, is_redacted=False, name=None, status_message=None, subscription=None, translation_key=None, type=None):
         """
         TableDefinitionOutputV1 - a model defined in Swagger
         """
 
         self._column_definitions = None
         self._description = None
         self._effective_permissions = None
         self._id = None
         self._is_archived = None
         self._is_redacted = None
         self._name = None
         self._status_message = None
+        self._subscription = None
         self._translation_key = None
         self._type = None
 
         if column_definitions is not None:
           self.column_definitions = column_definitions
         if description is not None:
           self.description = description
@@ -83,36 +86,40 @@
           self.is_archived = is_archived
         if is_redacted is not None:
           self.is_redacted = is_redacted
         if name is not None:
           self.name = name
         if status_message is not None:
           self.status_message = status_message
+        if subscription is not None:
+          self.subscription = subscription
         if translation_key is not None:
           self.translation_key = translation_key
         if type is not None:
           self.type = type
 
     @property
     def column_definitions(self):
         """
         Gets the column_definitions of this TableDefinitionOutputV1.
+        The Column Definitions for this Table Definition
 
         :return: The column_definitions of this TableDefinitionOutputV1.
-        :rtype: list[ColumnDefinition]
+        :rtype: list[ColumnDefinitionOutputV1]
         """
         return self._column_definitions
 
     @column_definitions.setter
     def column_definitions(self, column_definitions):
         """
         Sets the column_definitions of this TableDefinitionOutputV1.
+        The Column Definitions for this Table Definition
 
         :param column_definitions: The column_definitions of this TableDefinitionOutputV1.
-        :type: list[ColumnDefinition]
+        :type: list[ColumnDefinitionOutputV1]
         """
         if column_definitions is None:
             raise ValueError("Invalid value for `column_definitions`, must not be `None`")
 
         self._column_definitions = column_definitions
 
     @property
@@ -275,14 +282,35 @@
         :param status_message: The status_message of this TableDefinitionOutputV1.
         :type: str
         """
 
         self._status_message = status_message
 
     @property
+    def subscription(self):
+        """
+        Gets the subscription of this TableDefinitionOutputV1.
+
+        :return: The subscription of this TableDefinitionOutputV1.
+        :rtype: ItemPreviewV1
+        """
+        return self._subscription
+
+    @subscription.setter
+    def subscription(self, subscription):
+        """
+        Sets the subscription of this TableDefinitionOutputV1.
+
+        :param subscription: The subscription of this TableDefinitionOutputV1.
+        :type: ItemPreviewV1
+        """
+
+        self._subscription = subscription
+
+    @property
     def translation_key(self):
         """
         Gets the translation_key of this TableDefinitionOutputV1.
         The item's translation key, if any
 
         :return: The translation_key of this TableDefinitionOutputV1.
         :rtype: str
```

### Comparing `seeq-61.1.4/seeq/sdk/models/threshold_metric_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/threshold_metric_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/threshold_metric_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/threshold_metric_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/threshold_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/threshold_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/timer_datum_v1.py` & `seeq-62.0.1/seeq/sdk/models/timer_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/tree_item_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/tree_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/treemap_item_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/treemap_item_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/treemap_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/treemap_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/units_of_measure_batch_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/units_of_measure_batch_input_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/units_of_measure_item_v1.py` & `seeq-62.0.1/seeq/sdk/models/units_of_measure_item_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/units_of_measure_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/units_of_measure_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/unsubscribe_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/unsubscribe_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/usage_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/usage_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/usage_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/usage_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/usage_types_v1.py` & `seeq-62.0.1/seeq/sdk/models/usage_types_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_group_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/workbench_item_output_list_v1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,274 +1,276 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class UserGroupInputV1(object):
+class WorkbenchItemOutputListV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'description': 'str',
-        'is_enabled': 'bool',
-        'mapping': 'bool',
-        'mappings': 'IdentityMappingListV1',
-        'name': 'str',
-        'remote_group_editable': 'bool',
-        'remove_permissions': 'bool',
-        'sync_token': 'str'
+        'content': 'list[WorkbenchSearchResultPreviewV1]',
+        'limit': 'int',
+        'next': 'str',
+        'offset': 'int',
+        'path': 'list[ItemPreviewV1]',
+        'prev': 'str',
+        'status_message': 'str',
+        'total_results': 'int'
     }
 
     attribute_map = {
-        'description': 'description',
-        'is_enabled': 'isEnabled',
-        'mapping': 'mapping',
-        'mappings': 'mappings',
-        'name': 'name',
-        'remote_group_editable': 'remoteGroupEditable',
-        'remove_permissions': 'removePermissions',
-        'sync_token': 'syncToken'
+        'content': 'content',
+        'limit': 'limit',
+        'next': 'next',
+        'offset': 'offset',
+        'path': 'path',
+        'prev': 'prev',
+        'status_message': 'statusMessage',
+        'total_results': 'totalResults'
     }
 
-    def __init__(self, description=None, is_enabled=True, mapping=False, mappings=None, name=None, remote_group_editable=False, remove_permissions=False, sync_token=None):
+    def __init__(self, content=None, limit=None, next=None, offset=None, path=None, prev=None, status_message=None, total_results=None):
         """
-        UserGroupInputV1 - a model defined in Swagger
+        WorkbenchItemOutputListV1 - a model defined in Swagger
         """
 
-        self._description = None
-        self._is_enabled = None
-        self._mapping = None
-        self._mappings = None
-        self._name = None
-        self._remote_group_editable = None
-        self._remove_permissions = None
-        self._sync_token = None
-
-        if description is not None:
-          self.description = description
-        if is_enabled is not None:
-          self.is_enabled = is_enabled
-        if mapping is not None:
-          self.mapping = mapping
-        if mappings is not None:
-          self.mappings = mappings
-        if name is not None:
-          self.name = name
-        if remote_group_editable is not None:
-          self.remote_group_editable = remote_group_editable
-        if remove_permissions is not None:
-          self.remove_permissions = remove_permissions
-        if sync_token is not None:
-          self.sync_token = sync_token
+        self._content = None
+        self._limit = None
+        self._next = None
+        self._offset = None
+        self._path = None
+        self._prev = None
+        self._status_message = None
+        self._total_results = None
+
+        if content is not None:
+          self.content = content
+        if limit is not None:
+          self.limit = limit
+        if next is not None:
+          self.next = next
+        if offset is not None:
+          self.offset = offset
+        if path is not None:
+          self.path = path
+        if prev is not None:
+          self.prev = prev
+        if status_message is not None:
+          self.status_message = status_message
+        if total_results is not None:
+          self.total_results = total_results
 
     @property
-    def description(self):
+    def content(self):
         """
-        Gets the description of this UserGroupInputV1.
-        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
+        Gets the content of this WorkbenchItemOutputListV1.
+        Workbench items
 
-        :return: The description of this UserGroupInputV1.
-        :rtype: str
+        :return: The content of this WorkbenchItemOutputListV1.
+        :rtype: list[WorkbenchSearchResultPreviewV1]
         """
-        return self._description
+        return self._content
 
-    @description.setter
-    def description(self, description):
+    @content.setter
+    def content(self, content):
         """
-        Sets the description of this UserGroupInputV1.
-        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
+        Sets the content of this WorkbenchItemOutputListV1.
+        Workbench items
 
-        :param description: The description of this UserGroupInputV1.
-        :type: str
+        :param content: The content of this WorkbenchItemOutputListV1.
+        :type: list[WorkbenchSearchResultPreviewV1]
         """
 
-        self._description = description
+        self._content = content
 
     @property
-    def is_enabled(self):
+    def limit(self):
         """
-        Gets the is_enabled of this UserGroupInputV1.
-        Whether the user group is enabled or disabled (default true).
+        Gets the limit of this WorkbenchItemOutputListV1.
+        The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :return: The is_enabled of this UserGroupInputV1.
-        :rtype: bool
+        :return: The limit of this WorkbenchItemOutputListV1.
+        :rtype: int
         """
-        return self._is_enabled
+        return self._limit
 
-    @is_enabled.setter
-    def is_enabled(self, is_enabled):
+    @limit.setter
+    def limit(self, limit):
         """
-        Sets the is_enabled of this UserGroupInputV1.
-        Whether the user group is enabled or disabled (default true).
+        Sets the limit of this WorkbenchItemOutputListV1.
+        The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :param is_enabled: The is_enabled of this UserGroupInputV1.
-        :type: bool
+        :param limit: The limit of this WorkbenchItemOutputListV1.
+        :type: int
         """
 
-        self._is_enabled = is_enabled
+        self._limit = limit
 
     @property
-    def mapping(self):
+    def next(self):
         """
-        Gets the mapping of this UserGroupInputV1.
-        Whether the user group is a mapping (default false).
+        Gets the next of this WorkbenchItemOutputListV1.
+        The href of the next set of paginated results
 
-        :return: The mapping of this UserGroupInputV1.
-        :rtype: bool
+        :return: The next of this WorkbenchItemOutputListV1.
+        :rtype: str
         """
-        return self._mapping
+        return self._next
 
-    @mapping.setter
-    def mapping(self, mapping):
+    @next.setter
+    def next(self, next):
         """
-        Sets the mapping of this UserGroupInputV1.
-        Whether the user group is a mapping (default false).
+        Sets the next of this WorkbenchItemOutputListV1.
+        The href of the next set of paginated results
 
-        :param mapping: The mapping of this UserGroupInputV1.
-        :type: bool
+        :param next: The next of this WorkbenchItemOutputListV1.
+        :type: str
         """
 
-        self._mapping = mapping
+        self._next = next
 
     @property
-    def mappings(self):
+    def offset(self):
         """
-        Gets the mappings of this UserGroupInputV1.
+        Gets the offset of this WorkbenchItemOutputListV1.
+        The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :return: The mappings of this UserGroupInputV1.
-        :rtype: IdentityMappingListV1
+        :return: The offset of this WorkbenchItemOutputListV1.
+        :rtype: int
         """
-        return self._mappings
+        return self._offset
 
-    @mappings.setter
-    def mappings(self, mappings):
+    @offset.setter
+    def offset(self, offset):
         """
-        Sets the mappings of this UserGroupInputV1.
+        Sets the offset of this WorkbenchItemOutputListV1.
+        The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :param mappings: The mappings of this UserGroupInputV1.
-        :type: IdentityMappingListV1
+        :param offset: The offset of this WorkbenchItemOutputListV1.
+        :type: int
         """
 
-        self._mappings = mappings
+        self._offset = offset
 
     @property
-    def name(self):
+    def path(self):
         """
-        Gets the name of this UserGroupInputV1.
-        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
+        Gets the path of this WorkbenchItemOutputListV1.
+        The list of folders that specify where this these items are in the folder hierarchy.
 
-        :return: The name of this UserGroupInputV1.
-        :rtype: str
+        :return: The path of this WorkbenchItemOutputListV1.
+        :rtype: list[ItemPreviewV1]
         """
-        return self._name
+        return self._path
 
-    @name.setter
-    def name(self, name):
+    @path.setter
+    def path(self, path):
         """
-        Sets the name of this UserGroupInputV1.
-        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
+        Sets the path of this WorkbenchItemOutputListV1.
+        The list of folders that specify where this these items are in the folder hierarchy.
 
-        :param name: The name of this UserGroupInputV1.
-        :type: str
+        :param path: The path of this WorkbenchItemOutputListV1.
+        :type: list[ItemPreviewV1]
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._name = name
+        self._path = path
 
     @property
-    def remote_group_editable(self):
+    def prev(self):
         """
-        Gets the remote_group_editable of this UserGroupInputV1.
-        Whether the user group remains editable in Seeq even when sourced from a remote system.
+        Gets the prev of this WorkbenchItemOutputListV1.
+        The href of the previous set of paginated results
 
-        :return: The remote_group_editable of this UserGroupInputV1.
-        :rtype: bool
+        :return: The prev of this WorkbenchItemOutputListV1.
+        :rtype: str
         """
-        return self._remote_group_editable
+        return self._prev
 
-    @remote_group_editable.setter
-    def remote_group_editable(self, remote_group_editable):
+    @prev.setter
+    def prev(self, prev):
         """
-        Sets the remote_group_editable of this UserGroupInputV1.
-        Whether the user group remains editable in Seeq even when sourced from a remote system.
+        Sets the prev of this WorkbenchItemOutputListV1.
+        The href of the previous set of paginated results
 
-        :param remote_group_editable: The remote_group_editable of this UserGroupInputV1.
-        :type: bool
+        :param prev: The prev of this WorkbenchItemOutputListV1.
+        :type: str
         """
 
-        self._remote_group_editable = remote_group_editable
+        self._prev = prev
 
     @property
-    def remove_permissions(self):
+    def status_message(self):
         """
-        Gets the remove_permissions of this UserGroupInputV1.
-        Whether permissions associated with the group should be removed when disabling the group (default false).
+        Gets the status_message of this WorkbenchItemOutputListV1.
+        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :return: The remove_permissions of this UserGroupInputV1.
-        :rtype: bool
+        :return: The status_message of this WorkbenchItemOutputListV1.
+        :rtype: str
         """
-        return self._remove_permissions
+        return self._status_message
 
-    @remove_permissions.setter
-    def remove_permissions(self, remove_permissions):
+    @status_message.setter
+    def status_message(self, status_message):
         """
-        Sets the remove_permissions of this UserGroupInputV1.
-        Whether permissions associated with the group should be removed when disabling the group (default false).
+        Sets the status_message of this WorkbenchItemOutputListV1.
+        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :param remove_permissions: The remove_permissions of this UserGroupInputV1.
-        :type: bool
+        :param status_message: The status_message of this WorkbenchItemOutputListV1.
+        :type: str
         """
 
-        self._remove_permissions = remove_permissions
+        self._status_message = status_message
 
     @property
-    def sync_token(self):
+    def total_results(self):
         """
-        Gets the sync_token of this UserGroupInputV1.
-        An arbitrary token (often a date or random ID) that is used during metadata syncs. At the end of a full sync, items with mismatching sync tokens are identified as stale and may be archived using the Datasources clean-up API.
+        Gets the total_results of this WorkbenchItemOutputListV1.
+        The total number of items
 
-        :return: The sync_token of this UserGroupInputV1.
-        :rtype: str
+        :return: The total_results of this WorkbenchItemOutputListV1.
+        :rtype: int
         """
-        return self._sync_token
+        return self._total_results
 
-    @sync_token.setter
-    def sync_token(self, sync_token):
+    @total_results.setter
+    def total_results(self, total_results):
         """
-        Sets the sync_token of this UserGroupInputV1.
-        An arbitrary token (often a date or random ID) that is used during metadata syncs. At the end of a full sync, items with mismatching sync tokens are identified as stale and may be archived using the Datasources clean-up API.
+        Sets the total_results of this WorkbenchItemOutputListV1.
+        The total number of items
 
-        :param sync_token: The sync_token of this UserGroupInputV1.
-        :type: str
+        :param total_results: The total_results of this WorkbenchItemOutputListV1.
+        :type: int
         """
+        if total_results is None:
+            raise ValueError("Invalid value for `total_results`, must not be `None`")
 
-        self._sync_token = sync_token
+        self._total_results = total_results
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -304,15 +306,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, UserGroupInputV1):
+        if not isinstance(other, WorkbenchItemOutputListV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_group_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_group_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_group_with_id_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_group_with_id_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/user_password_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/user_password_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/validate_cron_list_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/validate_cron_list_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/validate_cron_list_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/validate_cron_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/validate_cron_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/validate_cron_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workbench_item_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/workbook_input_v1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,276 +1,220 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class WorkbenchItemOutputListV1(object):
+class WorkbookInputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'content': 'list[WorkbenchSearchResultPreviewV1]',
-        'limit': 'int',
-        'next': 'str',
-        'offset': 'int',
-        'path': 'list[ItemPreviewV1]',
-        'prev': 'str',
-        'status_message': 'str',
-        'total_results': 'int'
+        'branch_from': 'str',
+        'description': 'str',
+        'folder_id': 'str',
+        'name': 'str',
+        'owner_id': 'str',
+        'type': 'str'
     }
 
     attribute_map = {
-        'content': 'content',
-        'limit': 'limit',
-        'next': 'next',
-        'offset': 'offset',
-        'path': 'path',
-        'prev': 'prev',
-        'status_message': 'statusMessage',
-        'total_results': 'totalResults'
+        'branch_from': 'branchFrom',
+        'description': 'description',
+        'folder_id': 'folderId',
+        'name': 'name',
+        'owner_id': 'ownerId',
+        'type': 'type'
     }
 
-    def __init__(self, content=None, limit=None, next=None, offset=None, path=None, prev=None, status_message=None, total_results=None):
+    def __init__(self, branch_from=None, description=None, folder_id=None, name=None, owner_id=None, type=None):
         """
-        WorkbenchItemOutputListV1 - a model defined in Swagger
+        WorkbookInputV1 - a model defined in Swagger
         """
 
-        self._content = None
-        self._limit = None
-        self._next = None
-        self._offset = None
-        self._path = None
-        self._prev = None
-        self._status_message = None
-        self._total_results = None
-
-        if content is not None:
-          self.content = content
-        if limit is not None:
-          self.limit = limit
-        if next is not None:
-          self.next = next
-        if offset is not None:
-          self.offset = offset
-        if path is not None:
-          self.path = path
-        if prev is not None:
-          self.prev = prev
-        if status_message is not None:
-          self.status_message = status_message
-        if total_results is not None:
-          self.total_results = total_results
+        self._branch_from = None
+        self._description = None
+        self._folder_id = None
+        self._name = None
+        self._owner_id = None
+        self._type = None
+
+        if branch_from is not None:
+          self.branch_from = branch_from
+        if description is not None:
+          self.description = description
+        if folder_id is not None:
+          self.folder_id = folder_id
+        if name is not None:
+          self.name = name
+        if owner_id is not None:
+          self.owner_id = owner_id
+        if type is not None:
+          self.type = type
 
     @property
-    def content(self):
+    def branch_from(self):
         """
-        Gets the content of this WorkbenchItemOutputListV1.
-        Workbench items
+        Gets the branch_from of this WorkbookInputV1.
+        Create a new workbook by duplicating the contents and history of the workbook with the specified ID. When null, no branching will occur; resulting workbook will be empty.
 
-        :return: The content of this WorkbenchItemOutputListV1.
-        :rtype: list[WorkbenchSearchResultPreviewV1]
-        """
-        return self._content
-
-    @content.setter
-    def content(self, content):
-        """
-        Sets the content of this WorkbenchItemOutputListV1.
-        Workbench items
-
-        :param content: The content of this WorkbenchItemOutputListV1.
-        :type: list[WorkbenchSearchResultPreviewV1]
-        """
-
-        self._content = content
-
-    @property
-    def limit(self):
-        """
-        Gets the limit of this WorkbenchItemOutputListV1.
-        The pagination limit, the total number of collection items that will be returned in this page of results
-
-        :return: The limit of this WorkbenchItemOutputListV1.
-        :rtype: int
-        """
-        return self._limit
-
-    @limit.setter
-    def limit(self, limit):
-        """
-        Sets the limit of this WorkbenchItemOutputListV1.
-        The pagination limit, the total number of collection items that will be returned in this page of results
-
-        :param limit: The limit of this WorkbenchItemOutputListV1.
-        :type: int
-        """
-
-        self._limit = limit
-
-    @property
-    def next(self):
-        """
-        Gets the next of this WorkbenchItemOutputListV1.
-        The href of the next set of paginated results
-
-        :return: The next of this WorkbenchItemOutputListV1.
+        :return: The branch_from of this WorkbookInputV1.
         :rtype: str
         """
-        return self._next
+        return self._branch_from
 
-    @next.setter
-    def next(self, next):
+    @branch_from.setter
+    def branch_from(self, branch_from):
         """
-        Sets the next of this WorkbenchItemOutputListV1.
-        The href of the next set of paginated results
+        Sets the branch_from of this WorkbookInputV1.
+        Create a new workbook by duplicating the contents and history of the workbook with the specified ID. When null, no branching will occur; resulting workbook will be empty.
 
-        :param next: The next of this WorkbenchItemOutputListV1.
+        :param branch_from: The branch_from of this WorkbookInputV1.
         :type: str
         """
 
-        self._next = next
+        self._branch_from = branch_from
 
     @property
-    def offset(self):
+    def description(self):
         """
-        Gets the offset of this WorkbenchItemOutputListV1.
-        The pagination offset, the index of the first collection item that will be returned in this page of results
+        Gets the description of this WorkbookInputV1.
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :return: The offset of this WorkbenchItemOutputListV1.
-        :rtype: int
+        :return: The description of this WorkbookInputV1.
+        :rtype: str
         """
-        return self._offset
+        return self._description
 
-    @offset.setter
-    def offset(self, offset):
+    @description.setter
+    def description(self, description):
         """
-        Sets the offset of this WorkbenchItemOutputListV1.
-        The pagination offset, the index of the first collection item that will be returned in this page of results
+        Sets the description of this WorkbookInputV1.
+        Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :param offset: The offset of this WorkbenchItemOutputListV1.
-        :type: int
+        :param description: The description of this WorkbookInputV1.
+        :type: str
         """
 
-        self._offset = offset
+        self._description = description
 
     @property
-    def path(self):
+    def folder_id(self):
         """
-        Gets the path of this WorkbenchItemOutputListV1.
-        The list of folders that specify where this these items are in the folder hierarchy.
+        Gets the folder_id of this WorkbookInputV1.
+        The id of the folder to place the new workbook into. Special values of 'mine' or 'corporate' to place the item in the authenticated user's home folder or the corporate folder, respectively. If null, the workbook will be created in the authenticated user's home folder.
 
-        :return: The path of this WorkbenchItemOutputListV1.
-        :rtype: list[ItemPreviewV1]
+        :return: The folder_id of this WorkbookInputV1.
+        :rtype: str
         """
-        return self._path
+        return self._folder_id
 
-    @path.setter
-    def path(self, path):
+    @folder_id.setter
+    def folder_id(self, folder_id):
         """
-        Sets the path of this WorkbenchItemOutputListV1.
-        The list of folders that specify where this these items are in the folder hierarchy.
+        Sets the folder_id of this WorkbookInputV1.
+        The id of the folder to place the new workbook into. Special values of 'mine' or 'corporate' to place the item in the authenticated user's home folder or the corporate folder, respectively. If null, the workbook will be created in the authenticated user's home folder.
 
-        :param path: The path of this WorkbenchItemOutputListV1.
-        :type: list[ItemPreviewV1]
+        :param folder_id: The folder_id of this WorkbookInputV1.
+        :type: str
         """
 
-        self._path = path
+        self._folder_id = folder_id
 
     @property
-    def prev(self):
+    def name(self):
         """
-        Gets the prev of this WorkbenchItemOutputListV1.
-        The href of the previous set of paginated results
+        Gets the name of this WorkbookInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :return: The prev of this WorkbenchItemOutputListV1.
+        :return: The name of this WorkbookInputV1.
         :rtype: str
         """
-        return self._prev
+        return self._name
 
-    @prev.setter
-    def prev(self, prev):
+    @name.setter
+    def name(self, name):
         """
-        Sets the prev of this WorkbenchItemOutputListV1.
-        The href of the previous set of paginated results
+        Sets the name of this WorkbookInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :param prev: The prev of this WorkbenchItemOutputListV1.
+        :param name: The name of this WorkbookInputV1.
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._prev = prev
+        self._name = name
 
     @property
-    def status_message(self):
+    def owner_id(self):
         """
-        Gets the status_message of this WorkbenchItemOutputListV1.
-        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
+        Gets the owner_id of this WorkbookInputV1.
+        The ID of the User that owns this workbook. If omitted when creating a new Workbook, the authenticated user is used by default. Only administrators may set this value.
 
-        :return: The status_message of this WorkbenchItemOutputListV1.
+        :return: The owner_id of this WorkbookInputV1.
         :rtype: str
         """
-        return self._status_message
+        return self._owner_id
 
-    @status_message.setter
-    def status_message(self, status_message):
+    @owner_id.setter
+    def owner_id(self, owner_id):
         """
-        Sets the status_message of this WorkbenchItemOutputListV1.
-        A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
+        Sets the owner_id of this WorkbookInputV1.
+        The ID of the User that owns this workbook. If omitted when creating a new Workbook, the authenticated user is used by default. Only administrators may set this value.
 
-        :param status_message: The status_message of this WorkbenchItemOutputListV1.
+        :param owner_id: The owner_id of this WorkbookInputV1.
         :type: str
         """
 
-        self._status_message = status_message
+        self._owner_id = owner_id
 
     @property
-    def total_results(self):
+    def type(self):
         """
-        Gets the total_results of this WorkbenchItemOutputListV1.
-        The total number of items
+        Gets the type of this WorkbookInputV1.
+        The type of workbook, either 'Analysis' or 'Topic'. Defaults to 'Analysis'.
 
-        :return: The total_results of this WorkbenchItemOutputListV1.
-        :rtype: int
+        :return: The type of this WorkbookInputV1.
+        :rtype: str
         """
-        return self._total_results
+        return self._type
 
-    @total_results.setter
-    def total_results(self, total_results):
+    @type.setter
+    def type(self, type):
         """
-        Sets the total_results of this WorkbenchItemOutputListV1.
-        The total number of items
+        Sets the type of this WorkbookInputV1.
+        The type of workbook, either 'Analysis' or 'Topic'. Defaults to 'Analysis'.
 
-        :param total_results: The total_results of this WorkbenchItemOutputListV1.
-        :type: int
+        :param type: The type of this WorkbookInputV1.
+        :type: str
         """
-        if total_results is None:
-            raise ValueError("Invalid value for `total_results`, must not be `None`")
 
-        self._total_results = total_results
+        self._type = type
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -306,15 +250,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorkbenchItemOutputListV1):
+        if not isinstance(other, WorkbookInputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workbench_search_result_preview_v1.py` & `seeq-62.0.1/seeq/sdk/models/workbench_search_result_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workbook_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_finder_input_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,220 +1,222 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class WorkbookInputV1(object):
+class ItemFinderInputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'branch_from': 'str',
+        'cron_schedule': 'list[str]',
         'description': 'str',
-        'folder_id': 'str',
+        'enabled': 'bool',
+        'finder_configurations': 'list[ItemFinderConfigurationV1]',
         'name': 'str',
-        'owner_id': 'str',
-        'type': 'str'
+        'scoped_to': 'str'
     }
 
     attribute_map = {
-        'branch_from': 'branchFrom',
+        'cron_schedule': 'cronSchedule',
         'description': 'description',
-        'folder_id': 'folderId',
+        'enabled': 'enabled',
+        'finder_configurations': 'finderConfigurations',
         'name': 'name',
-        'owner_id': 'ownerId',
-        'type': 'type'
+        'scoped_to': 'scopedTo'
     }
 
-    def __init__(self, branch_from=None, description=None, folder_id=None, name=None, owner_id=None, type=None):
+    def __init__(self, cron_schedule=None, description=None, enabled=True, finder_configurations=None, name=None, scoped_to=None):
         """
-        WorkbookInputV1 - a model defined in Swagger
+        ItemFinderInputV1 - a model defined in Swagger
         """
 
-        self._branch_from = None
+        self._cron_schedule = None
         self._description = None
-        self._folder_id = None
+        self._enabled = None
+        self._finder_configurations = None
         self._name = None
-        self._owner_id = None
-        self._type = None
+        self._scoped_to = None
 
-        if branch_from is not None:
-          self.branch_from = branch_from
+        if cron_schedule is not None:
+          self.cron_schedule = cron_schedule
         if description is not None:
           self.description = description
-        if folder_id is not None:
-          self.folder_id = folder_id
+        if enabled is not None:
+          self.enabled = enabled
+        if finder_configurations is not None:
+          self.finder_configurations = finder_configurations
         if name is not None:
           self.name = name
-        if owner_id is not None:
-          self.owner_id = owner_id
-        if type is not None:
-          self.type = type
+        if scoped_to is not None:
+          self.scoped_to = scoped_to
 
     @property
-    def branch_from(self):
+    def cron_schedule(self):
         """
-        Gets the branch_from of this WorkbookInputV1.
-        Create a new workbook by duplicating the contents and history of the workbook with the specified ID. When null, no branching will occur; resulting workbook will be empty.
+        Gets the cron_schedule of this ItemFinderInputV1.
+        The item finder's check interval(s) as a list of cron expressions. If the list is empty, the system wide default check schedule is used. For more information about cron expressions, see  http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html
 
-        :return: The branch_from of this WorkbookInputV1.
-        :rtype: str
+        :return: The cron_schedule of this ItemFinderInputV1.
+        :rtype: list[str]
         """
-        return self._branch_from
+        return self._cron_schedule
 
-    @branch_from.setter
-    def branch_from(self, branch_from):
+    @cron_schedule.setter
+    def cron_schedule(self, cron_schedule):
         """
-        Sets the branch_from of this WorkbookInputV1.
-        Create a new workbook by duplicating the contents and history of the workbook with the specified ID. When null, no branching will occur; resulting workbook will be empty.
+        Sets the cron_schedule of this ItemFinderInputV1.
+        The item finder's check interval(s) as a list of cron expressions. If the list is empty, the system wide default check schedule is used. For more information about cron expressions, see  http://www.quartz-scheduler.org/documentation/quartz-2.3.0/tutorials/crontrigger.html
 
-        :param branch_from: The branch_from of this WorkbookInputV1.
-        :type: str
+        :param cron_schedule: The cron_schedule of this ItemFinderInputV1.
+        :type: list[str]
         """
 
-        self._branch_from = branch_from
+        self._cron_schedule = cron_schedule
 
     @property
     def description(self):
         """
-        Gets the description of this WorkbookInputV1.
+        Gets the description of this ItemFinderInputV1.
         Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :return: The description of this WorkbookInputV1.
+        :return: The description of this ItemFinderInputV1.
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """
-        Sets the description of this WorkbookInputV1.
+        Sets the description of this ItemFinderInputV1.
         Clarifying information or other plain language description of this item. An input of just whitespaces is equivalent to a null input.
 
-        :param description: The description of this WorkbookInputV1.
+        :param description: The description of this ItemFinderInputV1.
         :type: str
         """
 
         self._description = description
 
     @property
-    def folder_id(self):
+    def enabled(self):
         """
-        Gets the folder_id of this WorkbookInputV1.
-        The id of the folder to place the new workbook into. Special values of 'mine' or 'corporate' to place the item in the authenticated user's home folder or the corporate folder, respectively. If null, the workbook will be created in the authenticated user's home folder.
+        Gets the enabled of this ItemFinderInputV1.
+        Whether the item finder is enabled
 
-        :return: The folder_id of this WorkbookInputV1.
-        :rtype: str
+        :return: The enabled of this ItemFinderInputV1.
+        :rtype: bool
         """
-        return self._folder_id
+        return self._enabled
 
-    @folder_id.setter
-    def folder_id(self, folder_id):
+    @enabled.setter
+    def enabled(self, enabled):
         """
-        Sets the folder_id of this WorkbookInputV1.
-        The id of the folder to place the new workbook into. Special values of 'mine' or 'corporate' to place the item in the authenticated user's home folder or the corporate folder, respectively. If null, the workbook will be created in the authenticated user's home folder.
+        Sets the enabled of this ItemFinderInputV1.
+        Whether the item finder is enabled
 
-        :param folder_id: The folder_id of this WorkbookInputV1.
-        :type: str
+        :param enabled: The enabled of this ItemFinderInputV1.
+        :type: bool
         """
 
-        self._folder_id = folder_id
+        self._enabled = enabled
 
     @property
-    def name(self):
+    def finder_configurations(self):
         """
-        Gets the name of this WorkbookInputV1.
-        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
+        Gets the finder_configurations of this ItemFinderInputV1.
+        The list of configurations for finding items
 
-        :return: The name of this WorkbookInputV1.
-        :rtype: str
+        :return: The finder_configurations of this ItemFinderInputV1.
+        :rtype: list[ItemFinderConfigurationV1]
         """
-        return self._name
+        return self._finder_configurations
 
-    @name.setter
-    def name(self, name):
+    @finder_configurations.setter
+    def finder_configurations(self, finder_configurations):
         """
-        Sets the name of this WorkbookInputV1.
-        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
+        Sets the finder_configurations of this ItemFinderInputV1.
+        The list of configurations for finding items
 
-        :param name: The name of this WorkbookInputV1.
-        :type: str
+        :param finder_configurations: The finder_configurations of this ItemFinderInputV1.
+        :type: list[ItemFinderConfigurationV1]
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")
+        if finder_configurations is None:
+            raise ValueError("Invalid value for `finder_configurations`, must not be `None`")
 
-        self._name = name
+        self._finder_configurations = finder_configurations
 
     @property
-    def owner_id(self):
+    def name(self):
         """
-        Gets the owner_id of this WorkbookInputV1.
-        The ID of the User that owns this workbook. If omitted when creating a new Workbook, the authenticated user is used by default. Only administrators may set this value.
+        Gets the name of this ItemFinderInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :return: The owner_id of this WorkbookInputV1.
+        :return: The name of this ItemFinderInputV1.
         :rtype: str
         """
-        return self._owner_id
+        return self._name
 
-    @owner_id.setter
-    def owner_id(self, owner_id):
+    @name.setter
+    def name(self, name):
         """
-        Sets the owner_id of this WorkbookInputV1.
-        The ID of the User that owns this workbook. If omitted when creating a new Workbook, the authenticated user is used by default. Only administrators may set this value.
+        Sets the name of this ItemFinderInputV1.
+        Human readable name. Required during creation. An input of just whitespaces is equivalent to a null input.
 
-        :param owner_id: The owner_id of this WorkbookInputV1.
+        :param name: The name of this ItemFinderInputV1.
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")
 
-        self._owner_id = owner_id
+        self._name = name
 
     @property
-    def type(self):
+    def scoped_to(self):
         """
-        Gets the type of this WorkbookInputV1.
-        The type of workbook, either 'Analysis' or 'Topic'. Defaults to 'Analysis'.
+        Gets the scoped_to of this ItemFinderInputV1.
+        The ID of the workbook to which the item finder will be scoped. If not provided, it will have a global scope
 
-        :return: The type of this WorkbookInputV1.
+        :return: The scoped_to of this ItemFinderInputV1.
         :rtype: str
         """
-        return self._type
+        return self._scoped_to
 
-    @type.setter
-    def type(self, type):
+    @scoped_to.setter
+    def scoped_to(self, scoped_to):
         """
-        Sets the type of this WorkbookInputV1.
-        The type of workbook, either 'Analysis' or 'Topic'. Defaults to 'Analysis'.
+        Sets the scoped_to of this ItemFinderInputV1.
+        The ID of the workbook to which the item finder will be scoped. If not provided, it will have a global scope
 
-        :param type: The type of this WorkbookInputV1.
+        :param scoped_to: The scoped_to of this ItemFinderInputV1.
         :type: str
         """
 
-        self._type = type
+        self._scoped_to = scoped_to
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -250,15 +252,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorkbookInputV1):
+        if not isinstance(other, ItemFinderInputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workbook_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/worksheet_output_list_v1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class WorkbookOutputListV1(object):
+class WorksheetOutputListV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
@@ -31,188 +31,188 @@
     """
     swagger_types = {
         'limit': 'int',
         'next': 'str',
         'offset': 'int',
         'prev': 'str',
         'status_message': 'str',
-        'workbooks': 'list[WorkbookOutputV1]'
+        'worksheets': 'list[WorksheetOutputV1]'
     }
 
     attribute_map = {
         'limit': 'limit',
         'next': 'next',
         'offset': 'offset',
         'prev': 'prev',
         'status_message': 'statusMessage',
-        'workbooks': 'workbooks'
+        'worksheets': 'worksheets'
     }
 
-    def __init__(self, limit=None, next=None, offset=None, prev=None, status_message=None, workbooks=None):
+    def __init__(self, limit=None, next=None, offset=None, prev=None, status_message=None, worksheets=None):
         """
-        WorkbookOutputListV1 - a model defined in Swagger
+        WorksheetOutputListV1 - a model defined in Swagger
         """
 
         self._limit = None
         self._next = None
         self._offset = None
         self._prev = None
         self._status_message = None
-        self._workbooks = None
+        self._worksheets = None
 
         if limit is not None:
           self.limit = limit
         if next is not None:
           self.next = next
         if offset is not None:
           self.offset = offset
         if prev is not None:
           self.prev = prev
         if status_message is not None:
           self.status_message = status_message
-        if workbooks is not None:
-          self.workbooks = workbooks
+        if worksheets is not None:
+          self.worksheets = worksheets
 
     @property
     def limit(self):
         """
-        Gets the limit of this WorkbookOutputListV1.
+        Gets the limit of this WorksheetOutputListV1.
         The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :return: The limit of this WorkbookOutputListV1.
+        :return: The limit of this WorksheetOutputListV1.
         :rtype: int
         """
         return self._limit
 
     @limit.setter
     def limit(self, limit):
         """
-        Sets the limit of this WorkbookOutputListV1.
+        Sets the limit of this WorksheetOutputListV1.
         The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :param limit: The limit of this WorkbookOutputListV1.
+        :param limit: The limit of this WorksheetOutputListV1.
         :type: int
         """
 
         self._limit = limit
 
     @property
     def next(self):
         """
-        Gets the next of this WorkbookOutputListV1.
+        Gets the next of this WorksheetOutputListV1.
         The href of the next set of paginated results
 
-        :return: The next of this WorkbookOutputListV1.
+        :return: The next of this WorksheetOutputListV1.
         :rtype: str
         """
         return self._next
 
     @next.setter
     def next(self, next):
         """
-        Sets the next of this WorkbookOutputListV1.
+        Sets the next of this WorksheetOutputListV1.
         The href of the next set of paginated results
 
-        :param next: The next of this WorkbookOutputListV1.
+        :param next: The next of this WorksheetOutputListV1.
         :type: str
         """
 
         self._next = next
 
     @property
     def offset(self):
         """
-        Gets the offset of this WorkbookOutputListV1.
+        Gets the offset of this WorksheetOutputListV1.
         The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :return: The offset of this WorkbookOutputListV1.
+        :return: The offset of this WorksheetOutputListV1.
         :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
         """
-        Sets the offset of this WorkbookOutputListV1.
+        Sets the offset of this WorksheetOutputListV1.
         The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :param offset: The offset of this WorkbookOutputListV1.
+        :param offset: The offset of this WorksheetOutputListV1.
         :type: int
         """
 
         self._offset = offset
 
     @property
     def prev(self):
         """
-        Gets the prev of this WorkbookOutputListV1.
+        Gets the prev of this WorksheetOutputListV1.
         The href of the previous set of paginated results
 
-        :return: The prev of this WorkbookOutputListV1.
+        :return: The prev of this WorksheetOutputListV1.
         :rtype: str
         """
         return self._prev
 
     @prev.setter
     def prev(self, prev):
         """
-        Sets the prev of this WorkbookOutputListV1.
+        Sets the prev of this WorksheetOutputListV1.
         The href of the previous set of paginated results
 
-        :param prev: The prev of this WorkbookOutputListV1.
+        :param prev: The prev of this WorksheetOutputListV1.
         :type: str
         """
 
         self._prev = prev
 
     @property
     def status_message(self):
         """
-        Gets the status_message of this WorkbookOutputListV1.
+        Gets the status_message of this WorksheetOutputListV1.
         A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :return: The status_message of this WorkbookOutputListV1.
+        :return: The status_message of this WorksheetOutputListV1.
         :rtype: str
         """
         return self._status_message
 
     @status_message.setter
     def status_message(self, status_message):
         """
-        Sets the status_message of this WorkbookOutputListV1.
+        Sets the status_message of this WorksheetOutputListV1.
         A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :param status_message: The status_message of this WorkbookOutputListV1.
+        :param status_message: The status_message of this WorksheetOutputListV1.
         :type: str
         """
 
         self._status_message = status_message
 
     @property
-    def workbooks(self):
+    def worksheets(self):
         """
-        Gets the workbooks of this WorkbookOutputListV1.
-        The list of workbooks
+        Gets the worksheets of this WorksheetOutputListV1.
+        The list of worksheets
 
-        :return: The workbooks of this WorkbookOutputListV1.
-        :rtype: list[WorkbookOutputV1]
+        :return: The worksheets of this WorksheetOutputListV1.
+        :rtype: list[WorksheetOutputV1]
         """
-        return self._workbooks
+        return self._worksheets
 
-    @workbooks.setter
-    def workbooks(self, workbooks):
+    @worksheets.setter
+    def worksheets(self, worksheets):
         """
-        Sets the workbooks of this WorkbookOutputListV1.
-        The list of workbooks
+        Sets the worksheets of this WorksheetOutputListV1.
+        The list of worksheets
 
-        :param workbooks: The workbooks of this WorkbookOutputListV1.
-        :type: list[WorkbookOutputV1]
+        :param worksheets: The worksheets of this WorksheetOutputListV1.
+        :type: list[WorksheetOutputV1]
         """
 
-        self._workbooks = workbooks
+        self._worksheets = worksheets
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -248,15 +248,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorkbookOutputListV1):
+        if not isinstance(other, WorksheetOutputListV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workbook_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/workbook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/worksheet_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/worksheet_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/worksheet_output_list_v1.py` & `seeq-62.0.1/seeq/sdk/models/item_finder_output_list_v1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,219 +1,221 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class WorksheetOutputListV1(object):
+class ItemFinderOutputListV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'item_finders': 'list[ItemFinderOutputV1]',
         'limit': 'int',
         'next': 'str',
         'offset': 'int',
         'prev': 'str',
-        'status_message': 'str',
-        'worksheets': 'list[WorksheetOutputV1]'
+        'status_message': 'str'
     }
 
     attribute_map = {
+        'item_finders': 'itemFinders',
         'limit': 'limit',
         'next': 'next',
         'offset': 'offset',
         'prev': 'prev',
-        'status_message': 'statusMessage',
-        'worksheets': 'worksheets'
+        'status_message': 'statusMessage'
     }
 
-    def __init__(self, limit=None, next=None, offset=None, prev=None, status_message=None, worksheets=None):
+    def __init__(self, item_finders=None, limit=None, next=None, offset=None, prev=None, status_message=None):
         """
-        WorksheetOutputListV1 - a model defined in Swagger
+        ItemFinderOutputListV1 - a model defined in Swagger
         """
 
+        self._item_finders = None
         self._limit = None
         self._next = None
         self._offset = None
         self._prev = None
         self._status_message = None
-        self._worksheets = None
 
+        if item_finders is not None:
+          self.item_finders = item_finders
         if limit is not None:
           self.limit = limit
         if next is not None:
           self.next = next
         if offset is not None:
           self.offset = offset
         if prev is not None:
           self.prev = prev
         if status_message is not None:
           self.status_message = status_message
-        if worksheets is not None:
-          self.worksheets = worksheets
+
+    @property
+    def item_finders(self):
+        """
+        Gets the item_finders of this ItemFinderOutputListV1.
+        A list of item finders
+
+        :return: The item_finders of this ItemFinderOutputListV1.
+        :rtype: list[ItemFinderOutputV1]
+        """
+        return self._item_finders
+
+    @item_finders.setter
+    def item_finders(self, item_finders):
+        """
+        Sets the item_finders of this ItemFinderOutputListV1.
+        A list of item finders
+
+        :param item_finders: The item_finders of this ItemFinderOutputListV1.
+        :type: list[ItemFinderOutputV1]
+        """
+        if item_finders is None:
+            raise ValueError("Invalid value for `item_finders`, must not be `None`")
+
+        self._item_finders = item_finders
 
     @property
     def limit(self):
         """
-        Gets the limit of this WorksheetOutputListV1.
+        Gets the limit of this ItemFinderOutputListV1.
         The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :return: The limit of this WorksheetOutputListV1.
+        :return: The limit of this ItemFinderOutputListV1.
         :rtype: int
         """
         return self._limit
 
     @limit.setter
     def limit(self, limit):
         """
-        Sets the limit of this WorksheetOutputListV1.
+        Sets the limit of this ItemFinderOutputListV1.
         The pagination limit, the total number of collection items that will be returned in this page of results
 
-        :param limit: The limit of this WorksheetOutputListV1.
+        :param limit: The limit of this ItemFinderOutputListV1.
         :type: int
         """
 
         self._limit = limit
 
     @property
     def next(self):
         """
-        Gets the next of this WorksheetOutputListV1.
+        Gets the next of this ItemFinderOutputListV1.
         The href of the next set of paginated results
 
-        :return: The next of this WorksheetOutputListV1.
+        :return: The next of this ItemFinderOutputListV1.
         :rtype: str
         """
         return self._next
 
     @next.setter
     def next(self, next):
         """
-        Sets the next of this WorksheetOutputListV1.
+        Sets the next of this ItemFinderOutputListV1.
         The href of the next set of paginated results
 
-        :param next: The next of this WorksheetOutputListV1.
+        :param next: The next of this ItemFinderOutputListV1.
         :type: str
         """
 
         self._next = next
 
     @property
     def offset(self):
         """
-        Gets the offset of this WorksheetOutputListV1.
+        Gets the offset of this ItemFinderOutputListV1.
         The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :return: The offset of this WorksheetOutputListV1.
+        :return: The offset of this ItemFinderOutputListV1.
         :rtype: int
         """
         return self._offset
 
     @offset.setter
     def offset(self, offset):
         """
-        Sets the offset of this WorksheetOutputListV1.
+        Sets the offset of this ItemFinderOutputListV1.
         The pagination offset, the index of the first collection item that will be returned in this page of results
 
-        :param offset: The offset of this WorksheetOutputListV1.
+        :param offset: The offset of this ItemFinderOutputListV1.
         :type: int
         """
 
         self._offset = offset
 
     @property
     def prev(self):
         """
-        Gets the prev of this WorksheetOutputListV1.
+        Gets the prev of this ItemFinderOutputListV1.
         The href of the previous set of paginated results
 
-        :return: The prev of this WorksheetOutputListV1.
+        :return: The prev of this ItemFinderOutputListV1.
         :rtype: str
         """
         return self._prev
 
     @prev.setter
     def prev(self, prev):
         """
-        Sets the prev of this WorksheetOutputListV1.
+        Sets the prev of this ItemFinderOutputListV1.
         The href of the previous set of paginated results
 
-        :param prev: The prev of this WorksheetOutputListV1.
+        :param prev: The prev of this ItemFinderOutputListV1.
         :type: str
         """
 
         self._prev = prev
 
     @property
     def status_message(self):
         """
-        Gets the status_message of this WorksheetOutputListV1.
+        Gets the status_message of this ItemFinderOutputListV1.
         A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :return: The status_message of this WorksheetOutputListV1.
+        :return: The status_message of this ItemFinderOutputListV1.
         :rtype: str
         """
         return self._status_message
 
     @status_message.setter
     def status_message(self, status_message):
         """
-        Sets the status_message of this WorksheetOutputListV1.
+        Sets the status_message of this ItemFinderOutputListV1.
         A plain language status message with information about any issues that may have been encountered during an operation. Null if the status message has not been set.
 
-        :param status_message: The status_message of this WorksheetOutputListV1.
+        :param status_message: The status_message of this ItemFinderOutputListV1.
         :type: str
         """
 
         self._status_message = status_message
 
-    @property
-    def worksheets(self):
-        """
-        Gets the worksheets of this WorksheetOutputListV1.
-        The list of worksheets
-
-        :return: The worksheets of this WorksheetOutputListV1.
-        :rtype: list[WorksheetOutputV1]
-        """
-        return self._worksheets
-
-    @worksheets.setter
-    def worksheets(self, worksheets):
-        """
-        Sets the worksheets of this WorksheetOutputListV1.
-        The list of worksheets
-
-        :param worksheets: The worksheets of this WorksheetOutputListV1.
-        :type: list[WorksheetOutputV1]
-        """
-
-        self._worksheets = worksheets
-
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
         for attr, _ in iteritems(self.swagger_types):
@@ -248,15 +250,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorksheetOutputListV1):
+        if not isinstance(other, ItemFinderOutputListV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-61.1.4/seeq/sdk/models/worksheet_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/worksheet_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workstep_input_v1.py` & `seeq-62.0.1/seeq/sdk/models/workstep_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/models/workstep_output_v1.py` & `seeq-62.0.1/seeq/sdk/models/workstep_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-61.1.4/seeq/sdk/rest.py` & `seeq-62.0.1/seeq/sdk/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 61.1.4-v202308011800
+    OpenAPI spec version: 62.0.1-v202308011557
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `seeq-61.1.4/seeq.egg-info/PKG-INFO` & `seeq-62.0.1/seeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 61.1.4
+Version: 62.0.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-61.1.4/seeq.egg-info/SOURCES.txt` & `seeq-62.0.1/seeq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 seeq/sdk/api/annotations_api.py
 seeq/sdk/api/assets_api.py
 seeq/sdk/api/audit_api.py
 seeq/sdk/api/auth_api.py
 seeq/sdk/api/condition_monitors_api.py
 seeq/sdk/api/conditions_api.py
 seeq/sdk/api/content_api.py
+seeq/sdk/api/context_api.py
 seeq/sdk/api/datafiles_api.py
 seeq/sdk/api/datasources_api.py
 seeq/sdk/api/display_templates_api.py
 seeq/sdk/api/displays_api.py
 seeq/sdk/api/export_api.py
 seeq/sdk/api/folders_api.py
 seeq/sdk/api/formulas_api.py
+seeq/sdk/api/graph_ql_api.py
 seeq/sdk/api/items_api.py
 seeq/sdk/api/jobs_api.py
 seeq/sdk/api/logs_api.py
 seeq/sdk/api/metrics_api.py
 seeq/sdk/api/monitors_api.py
 seeq/sdk/api/networks_api.py
 seeq/sdk/api/notification_configurations_api.py
@@ -94,30 +96,31 @@
 seeq/sdk/models/asset_input_v1.py
 seeq/sdk/models/asset_output_v1.py
 seeq/sdk/models/asset_selection_input_v1.py
 seeq/sdk/models/asset_selection_output_v1.py
 seeq/sdk/models/asset_tree_batch_input_v1.py
 seeq/sdk/models/asset_tree_output_v1.py
 seeq/sdk/models/asset_tree_single_input_v1.py
+seeq/sdk/models/attachment_input_v1.py
 seeq/sdk/models/audit_output_list_v1.py
 seeq/sdk/models/audit_output_v1.py
 seeq/sdk/models/auth_input_v1.py
 seeq/sdk/models/auth_providers_output_v1.py
 seeq/sdk/models/cache_info_v1.py
 seeq/sdk/models/calculated_item_output_v1.py
 seeq/sdk/models/capsule_input_v1.py
 seeq/sdk/models/capsule_property_input_v1.py
 seeq/sdk/models/capsule_property_output_v1.py
 seeq/sdk/models/capsule_v1.py
 seeq/sdk/models/capsules_input_v1.py
 seeq/sdk/models/capsules_output_v1.py
 seeq/sdk/models/capsules_overwrite_input_v1.py
 seeq/sdk/models/channel_output_v1.py
-seeq/sdk/models/column_definition.py
 seeq/sdk/models/column_definition_input_v1.py
+seeq/sdk/models/column_definition_output_v1.py
 seeq/sdk/models/column_rule.py
 seeq/sdk/models/column_rule_ancestor_input_v1.py
 seeq/sdk/models/column_rule_concat_input_v1.py
 seeq/sdk/models/column_rule_event_property_input_v1.py
 seeq/sdk/models/column_rule_input_v1.py
 seeq/sdk/models/column_rule_item_property_input_v1.py
 seeq/sdk/models/column_rule_path_input_v1.py
@@ -144,14 +147,21 @@
 seeq/sdk/models/connector_input_v1.py
 seeq/sdk/models/connector_output_v1.py
 seeq/sdk/models/connectors_output_v1.py
 seeq/sdk/models/content_input_v1.py
 seeq/sdk/models/content_output_v1.py
 seeq/sdk/models/content_with_metadata_list_output_v1.py
 seeq/sdk/models/content_with_metadata_output_v1.py
+seeq/sdk/models/context_comment_input_v1.py
+seeq/sdk/models/context_comment_output_v1.py
+seeq/sdk/models/context_label_input_v1.py
+seeq/sdk/models/context_label_output_v1.py
+seeq/sdk/models/context_opaque_input_v1.py
+seeq/sdk/models/context_opaque_output_v1.py
+seeq/sdk/models/context_output_list_v1.py
 seeq/sdk/models/csv_datafile_output_v1.py
 seeq/sdk/models/datafile_input_v1.py
 seeq/sdk/models/datafile_output_v1.py
 seeq/sdk/models/datafiles_csv_body.py
 seeq/sdk/models/datasource_clean_up_input_v1.py
 seeq/sdk/models/datasource_clean_up_output_v1.py
 seeq/sdk/models/datasource_input_v1.py
@@ -229,42 +239,56 @@
 seeq/sdk/models/get_metrics_output_v1.py
 seeq/sdk/models/get_projects_output_v1.py
 seeq/sdk/models/get_request_output_v1.py
 seeq/sdk/models/get_requests_output_v1.py
 seeq/sdk/models/get_sample_output_v1.py
 seeq/sdk/models/get_samples_output_v1.py
 seeq/sdk/models/get_signals_output_v1.py
+seeq/sdk/models/graph_ql_input_v1.py
+seeq/sdk/models/graph_ql_output_v1.py
 seeq/sdk/models/id_images_body.py
 seeq/sdk/models/identity_mapping_list_v1.py
 seeq/sdk/models/identity_mapping_v1.py
 seeq/sdk/models/identity_preview_list_v1.py
 seeq/sdk/models/identity_preview_v1.py
 seeq/sdk/models/indexing_parameters_input_v1.py
 seeq/sdk/models/installer_output_v1.py
 seeq/sdk/models/interval_v1.py
 seeq/sdk/models/invalid_swap_out_v1.py
 seeq/sdk/models/item_batch_output_v1.py
 seeq/sdk/models/item_dependency_output_v1.py
+seeq/sdk/models/item_finder_configuration_v1.py
+seeq/sdk/models/item_finder_input_v1.py
+seeq/sdk/models/item_finder_output_list_v1.py
+seeq/sdk/models/item_finder_output_v1.py
 seeq/sdk/models/item_id_list_input_v1.py
 seeq/sdk/models/item_output_v1.py
 seeq/sdk/models/item_parameter_of_output_v1.py
 seeq/sdk/models/item_preview_list_v1.py
 seeq/sdk/models/item_preview_v1.py
 seeq/sdk/models/item_preview_with_assets_v1.py
 seeq/sdk/models/item_search_preview_list_v1.py
 seeq/sdk/models/item_search_preview_paginated_list_v1.py
 seeq/sdk/models/item_search_preview_v1.py
 seeq/sdk/models/item_swap_result_output_v1.py
 seeq/sdk/models/item_update_output_v1.py
 seeq/sdk/models/item_user_attributes_input_v1.py
 seeq/sdk/models/item_user_attributes_output_v1.py
 seeq/sdk/models/item_with_swap_pairs_v1.py
+seeq/sdk/models/jira_attachment.py
+seeq/sdk/models/jira_attachment_media_type.py
 seeq/sdk/models/job_accepted_output_v1.py
 seeq/sdk/models/job_output_v1.py
 seeq/sdk/models/json_backup_output_v1.py
+seeq/sdk/models/label_category_input_v1.py
+seeq/sdk/models/label_category_output_list_v1.py
+seeq/sdk/models/label_category_output_v1.py
+seeq/sdk/models/label_input_v1.py
+seeq/sdk/models/label_output_list_v1.py
+seeq/sdk/models/label_output_v1.py
 seeq/sdk/models/license_importer_output_v1.py
 seeq/sdk/models/license_status_output_v1.py
 seeq/sdk/models/licensed_feature_status_output_v1.py
 seeq/sdk/models/log_message.py
 seeq/sdk/models/meter_datum_v1.py
 seeq/sdk/models/migrate_editor_input_v1.py
 seeq/sdk/models/monitor_definition_output_v1.py
@@ -325,27 +349,28 @@
 seeq/sdk/models/scheduled_notebook_list_output_v1.py
 seeq/sdk/models/scheduled_notebook_output_v1.py
 seeq/sdk/models/screenshot_output_v1.py
 seeq/sdk/models/see_also_doc_output_v1.py
 seeq/sdk/models/send_email_attachment_v1.py
 seeq/sdk/models/send_email_contact_v1.py
 seeq/sdk/models/send_email_input_v1.py
-seeq/sdk/models/send_logs_input_v1.py
 seeq/sdk/models/server_build_info_output_v1.py
 seeq/sdk/models/server_load_output_v1.py
 seeq/sdk/models/server_spec_output_v1.py
 seeq/sdk/models/server_status_output_v1.py
 seeq/sdk/models/signal_input_v1.py
 seeq/sdk/models/signal_output_v1.py
 seeq/sdk/models/signal_with_id_input_v1.py
 seeq/sdk/models/status_message.py
 seeq/sdk/models/status_message_base.py
 seeq/sdk/models/subscription_input_v1.py
 seeq/sdk/models/subscription_output_v1.py
 seeq/sdk/models/subscription_update_input_v1.py
+seeq/sdk/models/support_request_input_v1.py
+seeq/sdk/models/support_request_output_v1.py
 seeq/sdk/models/supported_units_output_v1.py
 seeq/sdk/models/swap_input_v1.py
 seeq/sdk/models/swap_option_list_v1.py
 seeq/sdk/models/swap_option_v1.py
 seeq/sdk/models/swap_output_v1.py
 seeq/sdk/models/sync_progress.py
 seeq/sdk/models/sync_progress_output_v1.py
```

### Comparing `seeq-61.1.4/setup.py` & `seeq-62.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq",
-    version="61.1.4",
+    version="62.0.1",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="The Seeq SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

