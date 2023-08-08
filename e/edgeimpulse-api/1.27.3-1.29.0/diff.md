# Comparing `tmp/edgeimpulse_api-1.27.3.tar.gz` & `tmp/edgeimpulse_api-1.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.27.3.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.29.0.tar", max compression
```

## Comparing `edgeimpulse_api-1.27.3.tar` & `edgeimpulse_api-1.29.0.tar`

### file list

```diff
@@ -1,813 +1,814 @@
--rw-r--r--   0        0        0      377 2023-08-01 11:35:57.749276 edgeimpulse_api-1.27.3/README.md
--rw-r--r--   0        0        0    77565 2023-08-01 11:36:21.936966 edgeimpulse_api-1.27.3/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     3004 2023-08-01 11:35:57.749276 edgeimpulse_api-1.27.3/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   280031 2023-08-01 11:35:57.749276 edgeimpulse_api-1.27.3/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0   303232 2023-08-01 11:35:57.749276 edgeimpulse_api-1.27.3/edgeimpulse_api/api/allows_read_only_api.py
--rw-r--r--   0        0        0    11231 2023-08-01 11:35:57.749276 edgeimpulse_api-1.27.3/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    28575 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0     7426 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/content_disposition_inline_api.py
--rw-r--r--   0        0        0    72480 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    38974 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   131256 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0    19442 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/email_verification_api.py
--rw-r--r--   0        0        0     6435 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0    11921 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   239208 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   147712 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    17897 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    67457 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   300920 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_allow_developer_profile_api.py
--rw-r--r--   0        0        0    63140 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_allow_guest_access_api.py
--rw-r--r--   0        0        0   141131 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    91908 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   255365 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    47178 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   273394 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_requires_admin_api.py
--rw-r--r--   0        0        0   183341 2023-08-01 11:35:57.753275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
--rw-r--r--   0        0        0   314188 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    54671 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0    12662 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/project_requires_admin_api.py
--rw-r--r--   0        0        0   228112 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   378158 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    24481 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/requires_sudo_api.py
--rw-r--r--   0        0        0     7730 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
--rw-r--r--   0        0        0    13690 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/supports_range_api.py
--rw-r--r--   0        0        0    35671 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45393 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   223338 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    74108 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1982 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/activate_user_or_verify_email_request.py
--rw-r--r--   0        0        0     2610 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2806 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2656 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4588 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     4868 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     1940 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2542 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2146 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     4696 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3459 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7260 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5706 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2262 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     1905 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_enable_feature_request.py
--rw-r--r--   0        0        0     2546 2023-08-01 11:35:57.757275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2844 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response.py
--rw-r--r--   0        0        0     2544 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response_all_of.py
--rw-r--r--   0        0        0     2153 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response_all_of_flags.py
--rw-r--r--   0        0        0     2217 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3046 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     2452 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2507 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_trial_response.py
--rw-r--r--   0        0        0     2183 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
--rw-r--r--   0        0        0     2807 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     3087 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     7695 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3752 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     3269 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2661 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2532 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_trial_request.py
--rw-r--r--   0        0        0     2525 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0     5499 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3029 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0      506 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0     2044 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     3932 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3644 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     4783 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3004 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     2183 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2850 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_response.py
--rw-r--r--   0        0        0     2319 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
--rw-r--r--   0        0        0     5798 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_user_request.py
--rw-r--r--   0        0        0     3321 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
--rw-r--r--   0        0        0     2491 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2185 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2254 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     4000 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4157 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2051 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2023-08-01 11:35:57.761275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     4054 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2851 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4355 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      679 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1983 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_board.py
--rw-r--r--   0        0        0     2831 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2531 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     3677 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0     2199 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     2870 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     3779 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4667 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2210 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5144 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5502 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     3019 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3513 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3234 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4142 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     3875 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     3886 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2741 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
--rw-r--r--   0        0        0     2397 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2367 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2077 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/entity_created_response_all_of.py
--rw-r--r--   0        0        0     2656 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2511 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2023-08-01 11:35:57.765275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0      490 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/feature.py
--rw-r--r--   0        0        0     2206 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3385 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response.py
--rw-r--r--   0        0        0     3108 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
--rw-r--r--   0        0        0     2610 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
--rw-r--r--   0        0        0     1968 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
--rw-r--r--   0        0        0     3400 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4226 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     2350 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_email_verification_status_response.py
--rw-r--r--   0        0        0     2045 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
--rw-r--r--   0        0        0     3930 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2454 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     2650 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2977 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     2699 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2701 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2561 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3398 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2603 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2905 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3861 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2414 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3543 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     3276 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7717 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5708 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      526 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2023-08-01 11:35:57.769275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2445 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     3668 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     4699 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      516 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0     2965 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     2510 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5431 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5164 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     4792 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     3228 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0     9842 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0     9575 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     2424 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      883 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2682 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2630 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2333 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2767 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_enterprise_trials_response.py
--rw-r--r--   0        0        0     2467 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
--rw-r--r--   0        0        0     2813 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2857 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2550 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2995 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
--rw-r--r--   0        0        0     2902 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2744 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2723 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_response.py
--rw-r--r--   0        0        0     2416 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_response_all_of.py
--rw-r--r--   0        0        0     2857 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2265 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2786 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     1937 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2713 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2416 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     2553 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     3933 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2367 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_analytics_event_request.py
--rw-r--r--   0        0        0     2900 2023-08-01 11:35:57.773275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2430 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0     2521 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2687 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      621 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6418 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6871 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2067 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     4897 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     4618 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3419 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2366 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2760 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2463 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     4594 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2359 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2549 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2460 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     8598 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0     5422 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2501 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0     9493 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3034 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3476 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     3529 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2767 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     4689 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     3646 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     5707 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6331 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6041 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0      525 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     3453 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6132 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4109 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     4930 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     5146 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     6142 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3907 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     4225 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1763 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2211 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2413 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2955 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     2640 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2023-08-01 11:35:57.777275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     2565 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     6139 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     3888 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2680 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    13550 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    13283 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     3130 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     2979 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0     2670 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2353 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0      606 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0     2664 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     2028 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/request_email_verification_request.py
--rw-r--r--   0        0        0     1873 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1985 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2244 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_auto_segmenter_request.py
--rw-r--r--   0        0        0     2669 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0     9841 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2539 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
--rw-r--r--   0        0        0     2085 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2355 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
--rw-r--r--   0        0        0     2038 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3364 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     8028 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     1915 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     4814 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2226 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1967 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3460 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2433 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5295 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      588 2023-08-01 11:35:57.781275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2570 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4257 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2304 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2028 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2578 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2764 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2624 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2881 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2582 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     4664 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     5010 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0     8081 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     2603 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2059 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2168 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3673 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     2192 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     3200 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     1844 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     2407 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2633 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_email_response.py
--rw-r--r--   0        0        0     2354 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_email_response_all_of.py
--rw-r--r--   0        0        0     2708 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     2897 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     2597 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1937 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     5887 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2443 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_admin_create_project_request.py
--rw-r--r--   0        0        0     2120 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2023-08-01 11:35:57.785275 edgeimpulse_api-1.27.3/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0      967 2023-08-01 11:36:21.932966 edgeimpulse_api-1.27.3/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.27.3/PKG-INFO
+-rw-r--r--   0        0        0      377 2023-08-08 08:52:34.175696 edgeimpulse_api-1.29.0/README.md
+-rw-r--r--   0        0        0    77638 2023-08-08 08:53:00.331257 edgeimpulse_api-1.29.0/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     3004 2023-08-08 08:52:34.175696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   280031 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0   303232 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/allows_read_only_api.py
+-rw-r--r--   0        0        0    11231 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    28575 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0     7426 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/content_disposition_inline_api.py
+-rw-r--r--   0        0        0    72480 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    38974 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   131256 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0    11921 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   239208 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   147712 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    17897 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    67457 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   300920 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py
+-rw-r--r--   0        0        0    63140 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_allow_guest_access_api.py
+-rw-r--r--   0        0        0   141131 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    91908 2023-08-08 08:52:34.179696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   255365 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58218 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    47178 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   273394 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_requires_admin_api.py
+-rw-r--r--   0        0        0   183341 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py
+-rw-r--r--   0        0        0   314188 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    54671 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0    12662 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/project_requires_admin_api.py
+-rw-r--r--   0        0        0   228112 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   378158 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    24481 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/requires_sudo_api.py
+-rw-r--r--   0        0        0     7730 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py
+-rw-r--r--   0        0        0    13690 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/supports_range_api.py
+-rw-r--r--   0        0        0    35671 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45393 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   223338 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    74181 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2610 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2806 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2656 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4588 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2023-08-08 08:52:34.183696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     4868 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     1940 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2542 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2146 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     4696 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3459 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7260 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5706 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2262 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     1905 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2844 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response.py
+-rw-r--r--   0        0        0     2544 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2153 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     2217 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3046 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     3087 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     7695 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3752 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     3269 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2661 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0     5499 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3029 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0      506 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0     2044 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     3932 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3644 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     4783 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3004 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     2183 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     5798 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     3321 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2185 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2254 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2023-08-08 08:52:34.187696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4000 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4157 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2051 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     4054 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2851 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4355 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      679 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1983 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_board.py
+-rw-r--r--   0        0        0     2831 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2531 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     3677 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0     2199 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     2870 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     3779 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4667 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2210 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5144 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5502 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     3019 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3513 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3234 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4142 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     3875 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     3886 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2960 2023-08-08 08:52:34.191696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2397 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2511 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      490 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3385 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response.py
+-rw-r--r--   0        0        0     3108 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py
+-rw-r--r--   0        0        0     2610 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1968 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py
+-rw-r--r--   0        0        0     3400 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4226 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2350 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     3930 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2454 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     2650 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2977 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     2699 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2701 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2561 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3398 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2603 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2905 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3861 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2414 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     7717 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5708 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      526 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2023-08-08 08:52:34.195696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2445 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     3668 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     4699 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      516 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0     2965 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     1993 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_custom_metric.py
+-rw-r--r--   0        0        0     2510 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5431 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5164 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     4792 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     3989 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0     9842 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0     9575 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     2424 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      883 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2682 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2630 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2333 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2857 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2550 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2995 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py
+-rw-r--r--   0        0        0     2902 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2744 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2723 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_response.py
+-rw-r--r--   0        0        0     2416 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py
+-rw-r--r--   0        0        0     2857 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2265 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2786 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     1937 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2713 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2416 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     2553 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     3933 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2367 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_analytics_event_request.py
+-rw-r--r--   0        0        0     2900 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2430 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0     2521 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2023-08-08 08:52:34.199696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2687 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      621 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6418 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6871 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2067 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     4897 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     4618 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3419 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2366 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2760 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2463 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     4594 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2359 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2549 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2460 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     8598 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0     5422 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2501 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0     9493 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3034 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3476 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     3529 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2767 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     4689 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     3646 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     5707 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6331 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6041 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0      525 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3453 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6132 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4109 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     4930 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     5146 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     6142 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3907 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     4225 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1763 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2211 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2413 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2955 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     2640 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     2565 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     6139 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     3888 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2680 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    13692 2023-08-08 08:52:34.203696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    13425 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     3130 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     2979 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0     2670 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2353 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0      606 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0     2664 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1985 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2244 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_auto_segmenter_request.py
+-rw-r--r--   0        0        0     2669 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0     9841 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2539 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py
+-rw-r--r--   0        0        0     2085 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2355 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py
+-rw-r--r--   0        0        0     2038 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3364 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     8028 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     1915 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     4814 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1967 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3460 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2433 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5295 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      588 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2570 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4257 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2304 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2028 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2578 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2764 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2624 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2881 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2582 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     4664 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     5010 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     8271 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     2603 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2059 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2168 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2023-08-08 08:52:34.207696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     3673 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     2192 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     3200 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     1844 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     2407 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     2897 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     2597 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1937 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     5887 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2443 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_admin_create_project_request.py
+-rw-r--r--   0        0        0     2120 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2023-08-08 08:52:34.211696 edgeimpulse_api-1.29.0/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0      967 2023-08-08 08:53:00.327257 edgeimpulse_api-1.29.0/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.29.0/PKG-INFO
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.27.3" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.29.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.allows_read_only_api import AllowsReadOnlyApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
@@ -449,14 +449,15 @@
 from edgeimpulse_api.models.job_parent_type_enum import JobParentTypeEnum
 from edgeimpulse_api.models.job_state import JobState
 from edgeimpulse_api.models.job_state_execution_details import JobStateExecutionDetails
 from edgeimpulse_api.models.job_step import JobStep
 from edgeimpulse_api.models.job_summary_response import JobSummaryResponse
 from edgeimpulse_api.models.job_summary_response_all_of import JobSummaryResponseAllOf
 from edgeimpulse_api.models.job_summary_response_all_of_summary import JobSummaryResponseAllOfSummary
+from edgeimpulse_api.models.keras_custom_metric import KerasCustomMetric
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner import KerasModelMetadataMetricsOnDevicePerformanceInner
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/allows_read_only_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/allows_read_only_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/content_disposition_inline_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/content_disposition_inline_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/email_verification_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/email_verification_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_allow_developer_profile_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_allow_developer_profile_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_allow_guest_access_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_allow_guest_access_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_requires_admin_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_requires_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organization_requires_whitelabel_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/project_requires_admin_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/project_requires_admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/requires_sudo_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/requires_sudo_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/requires_third_party_auth_api_key_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/supports_range_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/supports_range_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,14 +393,15 @@
 from edgeimpulse_api.models.job_parent_type_enum import JobParentTypeEnum
 from edgeimpulse_api.models.job_state import JobState
 from edgeimpulse_api.models.job_state_execution_details import JobStateExecutionDetails
 from edgeimpulse_api.models.job_step import JobStep
 from edgeimpulse_api.models.job_summary_response import JobSummaryResponse
 from edgeimpulse_api.models.job_summary_response_all_of import JobSummaryResponseAllOf
 from edgeimpulse_api.models.job_summary_response_all_of_summary import JobSummaryResponseAllOfSummary
+from edgeimpulse_api.models.keras_custom_metric import KerasCustomMetric
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
 from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner import KerasModelMetadataMetricsOnDevicePerformanceInner
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/activate_user_or_verify_email_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_enable_feature_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_enable_feature_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_feature_flags_response_all_of_flags.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_feature_flags_response_all_of_flags.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_trial_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/admin_update_user_trial_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_board.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_board.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/enterprise_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class EnterpriseUpgradeOrTrialExtensionRequest(BaseModel):
     reason: Optional[StrictStr] = Field(None, description="Answer to the question: 'Why is this the right time for your team to invest in edge AI?'. This is optional.")
     use_case: Optional[StrictStr] = Field(None, alias="useCase", description="Answer to the question: 'What best describes your use case?'. This is optional.")
     timeline: Optional[StrictStr] = Field(None, description="Answer to the question: 'What is your timeline for solving your problem?'. This is optional.")
+    objective: Optional[StrictStr] = Field(None, description="Answer to the question: 'What are you hoping to achieve with an extension?'. This is optional.")
     trial_id: Optional[float] = Field(None, alias="trialId", description="The user's trial ID. This is optional.")
-    __properties = ["reason", "useCase", "timeline", "trialId"]
+    __properties = ["reason", "useCase", "timeline", "objective", "trialId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -61,11 +62,12 @@
         if type(obj) is not dict:
             return EnterpriseUpgradeOrTrialExtensionRequest.construct(**obj)
 
         _obj = EnterpriseUpgradeOrTrialExtensionRequest.construct(**{
             "reason": obj.get("reason"),
             "use_case": obj.get("useCase"),
             "timeline": obj.get("timeline"),
+            "objective": obj.get("objective"),
             "trial_id": obj.get("trialId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/entity_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/entity_created_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_auto_segmenter_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_email_verification_status_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_email_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_email_verification_status_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_email_verification_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,69 +14,58 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-from edgeimpulse_api.models.keras_model_metadata_metrics_on_device_performance_inner_tflite import KerasModelMetadataMetricsOnDevicePerformanceInnerTflite
+from pydantic import BaseModel, Field, StrictInt
 
-class KerasModelMetadataMetricsOnDevicePerformanceInner(BaseModel):
-    mcu: StrictStr = ...
-    name: StrictStr = ...
-    is_default: StrictBool = Field(..., alias="isDefault")
-    latency: float = ...
-    tflite: KerasModelMetadataMetricsOnDevicePerformanceInnerTflite = ...
-    eon: KerasModelMetadataMetricsOnDevicePerformanceInnerTflite = ...
-    __properties = ["mcu", "name", "isDefault", "latency", "tflite", "eon"]
+class KerasModelMetadataMetricsOnDevicePerformanceInnerTflite(BaseModel):
+    ram_required: StrictInt = Field(..., alias="ramRequired")
+    rom_required: StrictInt = Field(..., alias="romRequired")
+    arena_size: StrictInt = Field(..., alias="arenaSize")
+    model_size: StrictInt = Field(..., alias="modelSize")
+    __properties = ["ramRequired", "romRequired", "arenaSize", "modelSize"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadataMetricsOnDevicePerformanceInner:
-        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInner from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasModelMetadataMetricsOnDevicePerformanceInnerTflite:
+        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInnerTflite from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of tflite
-        if self.tflite:
-            _dict['tflite'] = self.tflite.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of eon
-        if self.eon:
-            _dict['eon'] = self.eon.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadataMetricsOnDevicePerformanceInner:
-        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInner from a dict"""
+    def from_dict(cls, obj: dict) -> KerasModelMetadataMetricsOnDevicePerformanceInnerTflite:
+        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInnerTflite from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadataMetricsOnDevicePerformanceInner.construct(**obj)
+            return KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.construct(**obj)
 
-        _obj = KerasModelMetadataMetricsOnDevicePerformanceInner.construct(**{
-            "mcu": obj.get("mcu"),
-            "name": obj.get("name"),
-            "is_default": obj.get("isDefault"),
-            "latency": obj.get("latency"),
-            "tflite": KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.from_dict(obj.get("tflite")) if obj.get("tflite") is not None else None,
-            "eon": KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.from_dict(obj.get("eon")) if obj.get("eon") is not None else None
+        _obj = KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.construct(**{
+            "ram_required": obj.get("ramRequired"),
+            "rom_required": obj.get("romRequired"),
+            "arena_size": obj.get("arenaSize"),
+            "model_size": obj.get("modelSize")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_custom_metric.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,58 +14,54 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, Field, StrictStr
 
-class KerasModelMetadataMetricsOnDevicePerformanceInnerTflite(BaseModel):
-    ram_required: StrictInt = Field(..., alias="ramRequired")
-    rom_required: StrictInt = Field(..., alias="romRequired")
-    arena_size: StrictInt = Field(..., alias="arenaSize")
-    model_size: StrictInt = Field(..., alias="modelSize")
-    __properties = ["ramRequired", "romRequired", "arenaSize", "modelSize"]
+class KerasCustomMetric(BaseModel):
+    name: StrictStr = Field(..., description="The name of the metric")
+    value: StrictStr = Field(..., description="The value of this metric for this model type")
+    __properties = ["name", "value"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadataMetricsOnDevicePerformanceInnerTflite:
-        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInnerTflite from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasCustomMetric:
+        """Create an instance of KerasCustomMetric from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadataMetricsOnDevicePerformanceInnerTflite:
-        """Create an instance of KerasModelMetadataMetricsOnDevicePerformanceInnerTflite from a dict"""
+    def from_dict(cls, obj: dict) -> KerasCustomMetric:
+        """Create an instance of KerasCustomMetric from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.construct(**obj)
+            return KerasCustomMetric.construct(**obj)
 
-        _obj = KerasModelMetadataMetricsOnDevicePerformanceInnerTflite.construct(**{
-            "ram_required": obj.get("ramRequired"),
-            "rom_required": obj.get("romRequired"),
-            "arena_size": obj.get("arenaSize"),
-            "model_size": obj.get("modelSize")
+        _obj = KerasCustomMetric.construct(**{
+            "name": obj.get("name"),
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_enterprise_trials_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_enterprise_trials_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_projects_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_analytics_event_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_analytics_event_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/portal_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_collaborator.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
     model_testing_job_notification_uids: List[StrictInt] = Field(..., alias="modelTestingJobNotificationUids", description="The IDs of users who should be notified when a model testing job is finished.")
     auto_segmenter_job_notification_uids: List[StrictInt] = Field(..., alias="autoSegmenterJobNotificationUids", description="The IDs of users who should be notified when an auto segmentation job is finished.")
     export_job_notification_uids: List[StrictInt] = Field(..., alias="exportJobNotificationUids", description="The IDs of users who should be notified when an export job is finished.")
     has_new_training_data: StrictBool = Field(..., alias="hasNewTrainingData")
     csv_import_config: Optional[Dict[str, Any]] = Field(None, alias="csvImportConfig", description="Config file specifying how to process CSV files.")
     studio_url: StrictStr = Field(..., alias="studioUrl")
     in_pretrained_model_flow: StrictBool = Field(..., alias="inPretrainedModelFlow")
-    __properties = ["success", "error", "project", "developmentKeys", "impulse", "devices", "dataSummary", "dataSummaryPerCategory", "computeTime", "acquisitionSettings", "collaborators", "deploySettings", "experiments", "latencyDevices", "urls", "showCreateFirstImpulse", "showGettingStartedWizard", "performance", "readme", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "hasNewTrainingData", "csvImportConfig", "studioUrl", "inPretrainedModelFlow"]
+    dsp_page_size: Optional[StrictInt] = Field(None, alias="dspPageSize")
+    __properties = ["success", "error", "project", "developmentKeys", "impulse", "devices", "dataSummary", "dataSummaryPerCategory", "computeTime", "acquisitionSettings", "collaborators", "deploySettings", "experiments", "latencyDevices", "urls", "showCreateFirstImpulse", "showGettingStartedWizard", "performance", "readme", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "hasNewTrainingData", "csvImportConfig", "studioUrl", "inPretrainedModelFlow", "dspPageSize"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -189,11 +190,12 @@
             "dsp_job_notification_uids": obj.get("dspJobNotificationUids"),
             "model_testing_job_notification_uids": obj.get("modelTestingJobNotificationUids"),
             "auto_segmenter_job_notification_uids": obj.get("autoSegmenterJobNotificationUids"),
             "export_job_notification_uids": obj.get("exportJobNotificationUids"),
             "has_new_training_data": obj.get("hasNewTrainingData"),
             "csv_import_config": obj.get("csvImportConfig"),
             "studio_url": obj.get("studioUrl"),
-            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow")
+            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow"),
+            "dsp_page_size": obj.get("dspPageSize")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     model_testing_job_notification_uids: List[StrictInt] = Field(..., alias="modelTestingJobNotificationUids", description="The IDs of users who should be notified when a model testing job is finished.")
     auto_segmenter_job_notification_uids: List[StrictInt] = Field(..., alias="autoSegmenterJobNotificationUids", description="The IDs of users who should be notified when an auto segmentation job is finished.")
     export_job_notification_uids: List[StrictInt] = Field(..., alias="exportJobNotificationUids", description="The IDs of users who should be notified when an export job is finished.")
     has_new_training_data: StrictBool = Field(..., alias="hasNewTrainingData")
     csv_import_config: Optional[Dict[str, Any]] = Field(None, alias="csvImportConfig", description="Config file specifying how to process CSV files.")
     studio_url: StrictStr = Field(..., alias="studioUrl")
     in_pretrained_model_flow: StrictBool = Field(..., alias="inPretrainedModelFlow")
-    __properties = ["project", "developmentKeys", "impulse", "devices", "dataSummary", "dataSummaryPerCategory", "computeTime", "acquisitionSettings", "collaborators", "deploySettings", "experiments", "latencyDevices", "urls", "showCreateFirstImpulse", "showGettingStartedWizard", "performance", "readme", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "hasNewTrainingData", "csvImportConfig", "studioUrl", "inPretrainedModelFlow"]
+    dsp_page_size: Optional[StrictInt] = Field(None, alias="dspPageSize")
+    __properties = ["project", "developmentKeys", "impulse", "devices", "dataSummary", "dataSummaryPerCategory", "computeTime", "acquisitionSettings", "collaborators", "deploySettings", "experiments", "latencyDevices", "urls", "showCreateFirstImpulse", "showGettingStartedWizard", "performance", "readme", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "hasNewTrainingData", "csvImportConfig", "studioUrl", "inPretrainedModelFlow", "dspPageSize"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -185,11 +186,12 @@
             "dsp_job_notification_uids": obj.get("dspJobNotificationUids"),
             "model_testing_job_notification_uids": obj.get("modelTestingJobNotificationUids"),
             "auto_segmenter_job_notification_uids": obj.get("autoSegmenterJobNotificationUids"),
             "export_job_notification_uids": obj.get("exportJobNotificationUids"),
             "has_new_training_data": obj.get("hasNewTrainingData"),
             "csv_import_config": obj.get("csvImportConfig"),
             "studio_url": obj.get("studioUrl"),
-            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow")
+            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow"),
+            "dsp_page_size": obj.get("dspPageSize")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/request_email_verification_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/request_email_verification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_auto_segmenter_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_auto_segmenter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_auto_segmenter_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_enterprise_trial_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_enterprise_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_project_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     train_job_notification_uids: Optional[List[StrictInt]] = Field(None, alias="trainJobNotificationUids", description="The IDs of users who should be notified when a Keras or retrain job is finished.")
     dsp_job_notification_uids: Optional[List[StrictInt]] = Field(None, alias="dspJobNotificationUids", description="The IDs of users who should be notified when a DSP job is finished.")
     model_testing_job_notification_uids: Optional[List[StrictInt]] = Field(None, alias="modelTestingJobNotificationUids", description="The IDs of users who should be notified when a model testing job is finished.")
     auto_segmenter_job_notification_uids: Optional[List[StrictInt]] = Field(None, alias="autoSegmenterJobNotificationUids", description="The IDs of users who should be notified when an auto segmentation job is finished.")
     export_job_notification_uids: Optional[List[StrictInt]] = Field(None, alias="exportJobNotificationUids", description="The IDs of users who should be notified when an export job is finished.")
     csv_import_config: Optional[Dict[str, Any]] = Field(None, alias="csvImportConfig", description="Config file specifying how to process CSV files.")
     in_pretrained_model_flow: Optional[StrictBool] = Field(None, alias="inPretrainedModelFlow")
-    __properties = ["logo", "name", "description", "lastDeployEonCompiler", "latencyDevice", "experiments", "showCreateFirstImpulse", "labelingMethod", "selectedProjectTypeInWizard", "gettingStartedStep", "useGpu", "computeTimeLimitM", "dspFileSizeMb", "enterprisePerformance", "trainJobRamMb", "metadata", "readme", "lastAcquisitionLabel", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "csvImportConfig", "inPretrainedModelFlow"]
+    dsp_page_size: Optional[StrictInt] = Field(None, alias="dspPageSize", description="Set to '0' to disable DSP paging")
+    __properties = ["logo", "name", "description", "lastDeployEonCompiler", "latencyDevice", "experiments", "showCreateFirstImpulse", "labelingMethod", "selectedProjectTypeInWizard", "gettingStartedStep", "useGpu", "computeTimeLimitM", "dspFileSizeMb", "enterprisePerformance", "trainJobRamMb", "metadata", "readme", "lastAcquisitionLabel", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "csvImportConfig", "inPretrainedModelFlow", "dspPageSize"]
 
     @validator('labeling_method')
     def labeling_method_validate_enum(cls, v):
         if v is None:
             return v
 
         if v not in ('single_label', 'object_detection'):
@@ -121,11 +122,12 @@
             "last_acquisition_label": obj.get("lastAcquisitionLabel"),
             "train_job_notification_uids": obj.get("trainJobNotificationUids"),
             "dsp_job_notification_uids": obj.get("dspJobNotificationUids"),
             "model_testing_job_notification_uids": obj.get("modelTestingJobNotificationUids"),
             "auto_segmenter_job_notification_uids": obj.get("autoSegmenterJobNotificationUids"),
             "export_job_notification_uids": obj.get("exportJobNotificationUids"),
             "csv_import_config": obj.get("csvImportConfig"),
-            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow")
+            "in_pretrained_model_flow": obj.get("inPretrainedModelFlow"),
+            "dsp_page_size": obj.get("dspPageSize")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/user_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_email_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_email_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_admin_create_project_request.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_admin_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.29.0/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.27.3/pyproject.toml` & `edgeimpulse_api-1.29.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.27.3" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.29.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.27.3/PKG-INFO` & `edgeimpulse_api-1.29.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.27.3
+Version: 1.29.0
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

