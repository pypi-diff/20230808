# Comparing `tmp/mercoa-0.2.8.tar.gz` & `tmp/mercoa-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.2.8.tar", max compression
+gzip compressed data, was "mercoa-0.2.9.tar", max compression
```

## Comparing `mercoa-0.2.8.tar` & `mercoa-0.2.9.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0     1930 2023-08-01 01:57:14.703607 mercoa-0.2.8/README.md
--rw-r--r--   0        0        0      368 2023-08-01 01:57:14.703607 mercoa-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     8859 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/__init__.py
--rw-r--r--   0        0        0     2384 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/py.typed
--rw-r--r--   0        0        0     8978 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     3801 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      499 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      314 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      225 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      469 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-08-01 01:57:14.703607 mercoa-0.2.8/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      523 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    40498 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0      501 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      228 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    17689 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4109 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    11215 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10326 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    22306 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    12767 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0      175 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    21722 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0      166 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
--rw-r--r--   0        0        0    10769 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
--rw-r--r--   0        0        0     8720 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
--rw-r--r--   0        0        0     2745 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/__init__.py
--rw-r--r--   0        0        0     4074 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/__init__.py
--rw-r--r--   0        0        0      487 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/account_type.py
--rw-r--r--   0        0        0      849 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/amount_trigger.py
--rw-r--r--   0        0        0       88 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_id.py
--rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_request.py
--rw-r--r--   0        0        0     1036 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_response.py
--rw-r--r--   0        0        0     1067 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/approver_rule.py
--rw-r--r--   0        0        0     1451 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_request.py
--rw-r--r--   0        0        0     1509 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_type.py
--rw-r--r--   0        0        0     1013 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/counterparty_response.py
--rw-r--r--   0        0        0      741 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/ein.py
--rw-r--r--   0        0        0      914 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_update_request.py
--rw-r--r--   0        0        0       84 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_response.py
--rw-r--r--   0        0        0     1446 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py
--rw-r--r--   0        0        0     1343 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_entity_response.py
--rw-r--r--   0        0        0     1367 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_notification_response.py
--rw-r--r--   0        0        0      633 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_response.py
--rw-r--r--   0        0        0       86 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_id.py
--rw-r--r--   0        0        0     1051 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_request.py
--rw-r--r--   0        0        0     1127 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_response.py
--rw-r--r--   0        0        0     1129 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_response.py
--rw-r--r--   0        0        0     1945 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_type.py
--rw-r--r--   0        0        0      974 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_response.py
--rw-r--r--   0        0        0       88 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/responsibilities.py
--rw-r--r--   0        0        0      391 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/rule.py
--rw-r--r--   0        0        0      761 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/tax_id.py
--rw-r--r--   0        0        0      854 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
--rw-r--r--   0        0        0     1269 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_options.py
--rw-r--r--   0        0        0      963 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
--rw-r--r--   0        0        0      857 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py
--rw-r--r--   0        0        0      951 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
--rw-r--r--   0        0        0      573 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/trigger.py
--rw-r--r--   0        0        0      947 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
--rw-r--r--   0        0        0      627 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/entity_types/types/vendor_network.py
--rw-r--r--   0        0        0      163 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    20874 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      154 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0     6559 2023-08-01 01:57:14.707607 mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    15332 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     3870 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0      991 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/__init__.py
--rw-r--r--   0        0        0     1480 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/__init__.py
--rw-r--r--   0        0        0     1017 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_request.py
--rw-r--r--   0        0        0     1592 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot.py
--rw-r--r--   0        0        0     1147 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
--rw-r--r--   0        0        0       86 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_id.py
--rw-r--r--   0        0        0      631 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approver_action.py
--rw-r--r--   0        0        0      984 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py
--rw-r--r--   0        0        0       81 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_request.py
--rw-r--r--   0        0        0     1428 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_response.py
--rw-r--r--   0        0        0      851 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/document_response.py
--rw-r--r--   0        0        0     1347 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py
--rw-r--r--   0        0        0       81 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_id.py
--rw-r--r--   0        0        0     1331 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     1072 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      870 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3578 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_request.py
--rw-r--r--   0        0        0     4306 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_status.py
--rw-r--r--   0        0        0      123 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4438 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      130 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      157 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    11712 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0      148 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
--rw-r--r--   0        0        0    10288 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/client.py
--rw-r--r--   0        0        0     1607 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/__init__.py
--rw-r--r--   0        0        0     2348 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/__init__.py
--rw-r--r--   0        0        0      948 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_response.py
--rw-r--r--   0        0        0      926 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py
--rw-r--r--   0        0        0      774 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
--rw-r--r--   0        0        0     1004 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
--rw-r--r--   0        0        0      627 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py
--rw-r--r--   0        0        0      633 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py
--rw-r--r--   0        0        0       86 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_id.py
--rw-r--r--   0        0        0     1711 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_request.py
--rw-r--r--   0        0        0     1808 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1151 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_request.py
--rw-r--r--   0        0        0      843 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_response.py
--rw-r--r--   0        0        0       65 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    15390 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0     2547 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/__init__.py
--rw-r--r--   0        0        0     3587 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/__init__.py
--rw-r--r--   0        0        0     1336 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
--rw-r--r--   0        0        0     1466 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
--rw-r--r--   0        0        0     1026 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py
--rw-r--r--   0        0        0     1014 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_type.py
--rw-r--r--   0        0        0     1247 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_request.py
--rw-r--r--   0        0        0     1468 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_response.py
--rw-r--r--   0        0        0      819 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_brand.py
--rw-r--r--   0        0        0      961 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_request.py
--rw-r--r--   0        0        0      935 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_response.py
--rw-r--r--   0        0        0      750 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_type.py
--rw-r--r--   0        0        0     1258 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_request.py
--rw-r--r--   0        0        0     1494 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_response.py
--rw-r--r--   0        0        0      967 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_request.py
--rw-r--r--   0        0        0      941 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/currency_code.py
--rw-r--r--   0        0        0     1607 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
--rw-r--r--   0        0        0     2026 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
--rw-r--r--   0        0        0     1040 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1028 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1613 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
--rw-r--r--   0        0        0     1071 2023-08-01 01:57:14.711608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_id.py
--rw-r--r--   0        0        0     1264 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py
--rw-r--r--   0        0        0     1298 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py
--rw-r--r--   0        0        0     1984 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1581 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1693 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
--rw-r--r--   0        0        0     1229 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py
--rw-r--r--   0        0        0      514 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
--rw-r--r--   0        0        0     1042 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
--rw-r--r--   0        0        0      271 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     6642 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1138 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1582 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-08-01 01:57:14.715608 mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-08-08 01:11:43.353956 mercoa-0.2.9/README.md
+-rw-r--r--   0        0        0      368 2023-08-08 01:11:43.353956 mercoa-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     8819 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/py.typed
+-rw-r--r--   0        0        0     8938 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      499 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      469 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      523 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    40498 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0      501 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17689 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4109 2023-08-08 01:11:43.353956 mercoa-0.2.9/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    12326 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10326 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22306 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12767 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      175 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    21722 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      166 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10769 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
+-rw-r--r--   0        0        0     8720 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
+-rw-r--r--   0        0        0     2745 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0     4074 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      849 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1100 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1036 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1067 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     1451 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1509 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0     1013 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      741 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0      914 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1446 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1343 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_entity_response.py
+-rw-r--r--   0        0        0     1367 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_notification_response.py
+-rw-r--r--   0        0        0      633 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0       86 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_id.py
+-rw-r--r--   0        0        0     1051 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_policy_request.py
+-rw-r--r--   0        0        0     1127 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_policy_response.py
+-rw-r--r--   0        0        0     1129 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_response.py
+-rw-r--r--   0        0        0     1945 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_type.py
+-rw-r--r--   0        0        0      974 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      391 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      761 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0      854 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py
+-rw-r--r--   0        0        0     1269 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_options.py
+-rw-r--r--   0        0        0      963 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_pages_options.py
+-rw-r--r--   0        0        0      857 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_style_options.py
+-rw-r--r--   0        0        0      951 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py
+-rw-r--r--   0        0        0      573 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0      947 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/user_notification_policy_response.py
+-rw-r--r--   0        0        0      627 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/entity_types/types/vendor_network.py
+-rw-r--r--   0        0        0      163 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    21453 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6559 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15332 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3870 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0     1041 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0     1559 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0     1592 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_slot.py
+-rw-r--r--   0        0        0     1147 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py
+-rw-r--r--   0        0        0       86 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_slot_id.py
+-rw-r--r--   0        0        0      631 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0      984 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1428 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      851 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1347 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/find_invoice_response.py
+-rw-r--r--   0        0        0     1273 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_failure_type.py
+-rw-r--r--   0        0        0       81 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     1331 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1258 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1072 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      870 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3578 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     4582 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1623 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      123 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4438 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      130 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1258 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      157 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    11367 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0      148 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization/resources/notification_configuration/__init__.py
+-rw-r--r--   0        0        0    13033 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization/resources/notification_configuration/client.py
+-rw-r--r--   0        0        0     1517 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/__init__.py
+-rw-r--r--   0        0        0     2208 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_response.py
+-rw-r--r--   0        0        0      774 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py
+-rw-r--r--   0        0        0     1004 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py
+-rw-r--r--   0        0        0      627 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/notification_configuration_request.py
+-rw-r--r--   0        0        0      633 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/notification_configuration_response.py
+-rw-r--r--   0        0        0       86 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1151 2023-08-08 01:11:43.357956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    15390 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2547 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0     3587 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1336 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
+-rw-r--r--   0        0        0     1466 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
+-rw-r--r--   0        0        0     1026 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1014 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0     1247 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_base_request.py
+-rw-r--r--   0        0        0     1468 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_base_response.py
+-rw-r--r--   0        0        0      819 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0      961 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0      935 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1258 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_base_request.py
+-rw-r--r--   0        0        0     1494 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_base_response.py
+-rw-r--r--   0        0        0      967 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0      941 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1607 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
+-rw-r--r--   0        0        0     2026 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
+-rw-r--r--   0        0        0     1040 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1028 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1613 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
+-rw-r--r--   0        0        0     1071 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1264 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     1984 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1581 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1693 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1229 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0     1042 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/plaid_link_request.py
+-rw-r--r--   0        0        0      271 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1138 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1582 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-08-08 01:11:43.361956 mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.9/PKG-INFO
```

### Comparing `mercoa-0.2.8/README.md` & `mercoa-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/__init__.py` & `mercoa-0.2.9/src/mercoa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,21 +71,21 @@
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
     FindEntityResponse,
     FindInvoiceResponse,
     FindNotificationResponse,
     FullName,
-    GlobalNotificationConfigurationRequest,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
     IndividualGovernmentId,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    InvoiceFailureType,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceNotificationConfigurationRequest,
     InvoiceNotificationConfigurationResponse,
     InvoiceOrderByField,
@@ -243,21 +243,21 @@
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FindEntityResponse",
     "FindInvoiceResponse",
     "FindNotificationResponse",
     "FullName",
-    "GlobalNotificationConfigurationRequest",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "InvoiceFailureType",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationResponse",
     "InvoiceOrderByField",
```

### Comparing `mercoa-0.2.8/src/mercoa/client.py` & `mercoa-0.2.9/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.9/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.9/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     ApproverAction,
     AssociatedApprovalAction,
     CommentId,
     CommentRequest,
     CommentResponse,
     DocumentResponse,
     FindInvoiceResponse,
+    InvoiceFailureType,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
@@ -110,15 +111,14 @@
     ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
     EmailProviderResponse,
     EmailSenderProvider,
     EmailSenderRequest,
     EmailSenderResponse,
-    GlobalNotificationConfigurationRequest,
     InvoiceNotificationConfigurationRequest,
     InvoiceNotificationConfigurationResponse,
     NotificationConfigurationRequest,
     NotificationConfigurationRequest_Invoice,
     NotificationConfigurationResponse,
     NotificationConfigurationResponse_Invoice,
     OrganizationId,
@@ -248,21 +248,21 @@
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
     "FindEntityResponse",
     "FindInvoiceResponse",
     "FindNotificationResponse",
     "FullName",
-    "GlobalNotificationConfigurationRequest",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "InvoiceFailureType",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationResponse",
     "InvoiceOrderByField",
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.9/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.9/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.9/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
 from ....commons.types.order_direction import OrderDirection
 from ....entity_types.types.entity_id import EntityId
+from ....entity_types.types.entity_user_id import EntityUserId
 from ....invoice_types.types.find_invoice_response import FindInvoiceResponse
 from ....invoice_types.types.invoice_id import InvoiceId
 from ....invoice_types.types.invoice_metrics_response import InvoiceMetricsResponse
 from ....invoice_types.types.invoice_order_by_field import InvoiceOrderByField
 from ....invoice_types.types.invoice_status import InvoiceStatus
 from ....payment_method_types.types.currency_code import CurrencyCode
 
@@ -37,27 +38,31 @@
         start_date: typing.Optional[dt.datetime] = None,
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
     ) -> FindInvoiceResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
             params={
                 "startDate": serialize_datetime(start_date) if start_date is not None else None,
                 "endDate": serialize_datetime(end_date) if end_date is not None else None,
                 "orderBy": order_by,
                 "orderDirection": order_direction,
                 "limit": limit,
                 "startingAfter": starting_after,
                 "search": search,
+                "vendorId": vendor_id,
+                "approverId": approver_id,
                 "status": status,
             },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -77,26 +82,30 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def metrics(
         self,
         entity_id: EntityId,
         *,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
         due_date_start: typing.Optional[dt.datetime] = None,
         due_date_end: typing.Optional[dt.datetime] = None,
         created_date_start: typing.Optional[dt.datetime] = None,
         created_date_end: typing.Optional[dt.datetime] = None,
         currency: CurrencyCode,
     ) -> InvoiceMetricsResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
             params={
                 "search": search,
+                "vendorId": vendor_id,
+                "approverId": approver_id,
                 "status": status,
                 "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
                 "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
                 "createdDateStart": serialize_datetime(created_date_start) if created_date_start is not None else None,
                 "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
                 "currency": currency,
             },
@@ -133,28 +142,32 @@
         start_date: typing.Optional[dt.datetime] = None,
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
     ) -> FindInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
                 params={
                     "startDate": serialize_datetime(start_date) if start_date is not None else None,
                     "endDate": serialize_datetime(end_date) if end_date is not None else None,
                     "orderBy": order_by,
                     "orderDirection": order_direction,
                     "limit": limit,
                     "startingAfter": starting_after,
                     "search": search,
+                    "vendorId": vendor_id,
+                    "approverId": approver_id,
                     "status": status,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
@@ -174,27 +187,31 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def metrics(
         self,
         entity_id: EntityId,
         *,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
         due_date_start: typing.Optional[dt.datetime] = None,
         due_date_end: typing.Optional[dt.datetime] = None,
         created_date_start: typing.Optional[dt.datetime] = None,
         created_date_end: typing.Optional[dt.datetime] = None,
         currency: CurrencyCode,
     ) -> InvoiceMetricsResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoice-metrics"),
                 params={
                     "search": search,
+                    "vendorId": vendor_id,
+                    "approverId": approver_id,
                     "status": status,
                     "dueDateStart": serialize_datetime(due_date_start) if due_date_start is not None else None,
                     "dueDateEnd": serialize_datetime(due_date_end) if due_date_end is not None else None,
                     "createdDateStart": serialize_datetime(created_date_start)
                     if created_date_start is not None
                     else None,
                     "createdDateEnd": serialize_datetime(created_date_end) if created_date_end is not None else None,
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/notification_policy/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notification_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity/resources/user/resources/notifications/client.py` & `mercoa-0.2.9/src/mercoa/resources/entity/resources/user/resources/notifications/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/amount_trigger.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approval_policy_update_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/approver_rule.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_profile_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/business_type.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/counterparty_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/ein.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_add_payees_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_status.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_update_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/entity_user_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_counterparties_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_entity_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/find_notification_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/find_notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/identifier_list.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/individual_profile_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_policy_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/notification_type.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/notification_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/profile_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_request.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/representative_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/responsibilities.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/tax_id.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_invoice_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_options.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_pages_options.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_pages_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_style_options.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_style_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/token_generation_vendor_options.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/trigger.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/user_notification_policy_response.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/user_notification_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/entity_types/types/vendor_network.py` & `mercoa-0.2.9/src/mercoa/resources/entity_types/types/vendor_network.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.9/src/mercoa/resources/invoice/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
 from ..commons.types.order_direction import OrderDirection
 from ..entity_types.types.entity_id import EntityId
+from ..entity_types.types.entity_user_id import EntityUserId
 from ..invoice_types.types.find_invoice_response import FindInvoiceResponse
 from ..invoice_types.types.invoice_id import InvoiceId
 from ..invoice_types.types.invoice_order_by_field import InvoiceOrderByField
 from ..invoice_types.types.invoice_request import InvoiceRequest
 from ..invoice_types.types.invoice_response import InvoiceResponse
 from ..invoice_types.types.invoice_status import InvoiceStatus
 from .resources.approval.client import ApprovalClient, AsyncApprovalClient
@@ -36,36 +37,40 @@
         self.approval = ApprovalClient(environment=self._environment, token=self._token)
         self.comment = CommentClient(environment=self._environment, token=self._token)
         self.document = DocumentClient(environment=self._environment, token=self._token)
 
     def find(
         self,
         *,
-        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        entity_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
         start_date: typing.Optional[dt.datetime] = None,
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
     ) -> FindInvoiceResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
             params={
-                "entityIds": entity_ids,
+                "entityId": entity_id,
                 "startDate": serialize_datetime(start_date) if start_date is not None else None,
                 "endDate": serialize_datetime(end_date) if end_date is not None else None,
                 "orderBy": order_by,
                 "orderDirection": order_direction,
                 "limit": limit,
                 "startingAfter": starting_after,
                 "search": search,
+                "vendorId": vendor_id,
+                "approverId": approver_id,
                 "status": status,
             },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
@@ -214,37 +219,41 @@
         self.approval = AsyncApprovalClient(environment=self._environment, token=self._token)
         self.comment = AsyncCommentClient(environment=self._environment, token=self._token)
         self.document = AsyncDocumentClient(environment=self._environment, token=self._token)
 
     async def find(
         self,
         *,
-        entity_ids: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        entity_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
         start_date: typing.Optional[dt.datetime] = None,
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
+        vendor_id: typing.Union[typing.Optional[EntityId], typing.List[EntityId]],
+        approver_id: typing.Union[typing.Optional[EntityUserId], typing.List[EntityUserId]],
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
     ) -> FindInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
                 params={
-                    "entityIds": entity_ids,
+                    "entityId": entity_id,
                     "startDate": serialize_datetime(start_date) if start_date is not None else None,
                     "endDate": serialize_datetime(end_date) if end_date is not None else None,
                     "orderBy": order_by,
                     "orderDirection": order_direction,
                     "limit": limit,
                     "startingAfter": starting_after,
                     "search": search,
+                    "vendorId": vendor_id,
+                    "approverId": approver_id,
                     "status": status,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.2.9/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.2.9/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.2.9/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ApproverAction,
     AssociatedApprovalAction,
     CommentId,
     CommentRequest,
     CommentResponse,
     DocumentResponse,
     FindInvoiceResponse,
+    InvoiceFailureType,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
@@ -30,14 +31,15 @@
     "ApproverAction",
     "AssociatedApprovalAction",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "DocumentResponse",
     "FindInvoiceResponse",
+    "InvoiceFailureType",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .approver_action import ApproverAction
 from .associated_approval_action import AssociatedApprovalAction
 from .comment_id import CommentId
 from .comment_request import CommentRequest
 from .comment_response import CommentResponse
 from .document_response import DocumentResponse
 from .find_invoice_response import FindInvoiceResponse
+from .invoice_failure_type import InvoiceFailureType
 from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_metrics_response import InvoiceMetricsResponse
 from .invoice_order_by_field import InvoiceOrderByField
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
@@ -28,14 +29,15 @@
     "ApproverAction",
     "AssociatedApprovalAction",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "DocumentResponse",
     "FindInvoiceResponse",
+    "InvoiceFailureType",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_request.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_slot.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approval_slot_assignment.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/approver_action.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/associated_approval_action.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_request.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/comment_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/document_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/find_invoice_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/find_invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_request.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_response.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ...entity_types.types.entity_user_response import EntityUserResponse
 from ...payment_method_types.types.currency_code import CurrencyCode
 from ...payment_method_types.types.payment_method_id import PaymentMethodId
 from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
 from ...transaction.types.transaction_response import TransactionResponse
 from .approval_slot import ApprovalSlot
 from .comment_response import CommentResponse
+from .invoice_failure_type import InvoiceFailureType
 from .invoice_id import InvoiceId
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
@@ -55,14 +56,18 @@
     line_items: typing.Optional[typing.List[InvoiceLineItemResponse]] = pydantic.Field(alias="lineItems")
     approvers: typing.List[ApprovalSlot]
     approval_policy: typing.List[ApprovalPolicyResponse] = pydantic.Field(alias="approvalPolicy")
     metadata: typing.Dict[str, str] = pydantic.Field(description=("Metadata associated with this invoice.\n"))
     created_by: typing.Optional[EntityUserResponse] = pydantic.Field(
         alias="createdBy", description=("Entity user who created this invoice.\n")
     )
+    failure_type: typing.Optional[InvoiceFailureType] = pydantic.Field(
+        alias="failureType",
+        description=("If the invoice failed to be paid, this field will be populated with the type of failure.\n"),
+    )
     processed_at: typing.Optional[dt.datetime] = pydantic.Field(alias="processedAt")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/invoice_types/types/invoice_status.py` & `mercoa-0.2.9/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,28 @@
     APPROVED = "APPROVED"
     SCHEDULED = "SCHEDULED"
     PENDING = "PENDING"
     PAID = "PAID"
     ARCHIVED = "ARCHIVED"
     REFUSED = "REFUSED"
     CANCELED = "CANCELED"
+    FAILED = "FAILED"
 
     def visit(
         self,
         draft: typing.Callable[[], T_Result],
         new: typing.Callable[[], T_Result],
         approved: typing.Callable[[], T_Result],
         scheduled: typing.Callable[[], T_Result],
         pending: typing.Callable[[], T_Result],
         paid: typing.Callable[[], T_Result],
         archived: typing.Callable[[], T_Result],
         refused: typing.Callable[[], T_Result],
         canceled: typing.Callable[[], T_Result],
+        failed: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is InvoiceStatus.DRAFT:
             return draft()
         if self is InvoiceStatus.NEW:
             return new()
         if self is InvoiceStatus.APPROVED:
             return approved()
@@ -43,7 +45,9 @@
             return paid()
         if self is InvoiceStatus.ARCHIVED:
             return archived()
         if self is InvoiceStatus.REFUSED:
             return refused()
         if self is InvoiceStatus.CANCELED:
             return canceled()
+        if self is InvoiceStatus.FAILED:
+            return failed()
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.9/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.9/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization/client.py` & `mercoa-0.2.9/src/mercoa/resources/organization/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,19 @@
 
     def get(
         self,
         *,
         payment_methods: typing.Optional[bool] = None,
         email_provider: typing.Optional[bool] = None,
         color_scheme: typing.Optional[bool] = None,
-        notification_configuration: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
-            params={
-                "paymentMethods": payment_methods,
-                "emailProvider": email_provider,
-                "colorScheme": color_scheme,
-                "notificationConfiguration": notification_configuration,
-            },
+            params={"paymentMethods": payment_methods, "emailProvider": email_provider, "colorScheme": color_scheme},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -136,25 +130,23 @@
 
     async def get(
         self,
         *,
         payment_methods: typing.Optional[bool] = None,
         email_provider: typing.Optional[bool] = None,
         color_scheme: typing.Optional[bool] = None,
-        notification_configuration: typing.Optional[bool] = None,
     ) -> OrganizationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "organization"),
                 params={
                     "paymentMethods": payment_methods,
                     "emailProvider": email_provider,
                     "colorScheme": color_scheme,
-                    "notificationConfiguration": notification_configuration,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization/resources/notification_configuration/client.py` & `mercoa-0.2.9/src/mercoa/resources/organization/resources/notification_configuration/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     def get_all(self) -> typing.List[NotificationConfigurationResponse]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "organization/notification-policies"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "organization/notification-configurations"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -99,25 +99,51 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def reset(self, notification_type: NotificationType) -> None:
+        _response = httpx.request(
+            "DELETE",
+            urllib.parse.urljoin(
+                f"{self._environment.value}/", f"organization/notification-configuration/{notification_type}"
+            ),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
 
 class AsyncNotificationConfigurationClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
 
     async def get_all(self) -> typing.List[NotificationConfigurationResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "organization/notification-policies"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "organization/notification-configurations"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
@@ -185,8 +211,35 @@
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def reset(self, notification_type: NotificationType) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "DELETE",
+                urllib.parse.urljoin(
+                    f"{self._environment.value}/", f"organization/notification-configuration/{notification_type}"
+                ),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     ColorSchemeResponse,
     EmailLogResponse,
     EmailProviderRequest,
     EmailProviderResponse,
     EmailSenderProvider,
     EmailSenderRequest,
     EmailSenderResponse,
-    GlobalNotificationConfigurationRequest,
     InvoiceNotificationConfigurationRequest,
     InvoiceNotificationConfigurationResponse,
     NotificationConfigurationRequest,
     NotificationConfigurationRequest_Invoice,
     NotificationConfigurationResponse,
     NotificationConfigurationResponse_Invoice,
     OrganizationId,
@@ -32,15 +31,14 @@
     "ColorSchemeResponse",
     "EmailLogResponse",
     "EmailProviderRequest",
     "EmailProviderResponse",
     "EmailSenderProvider",
     "EmailSenderRequest",
     "EmailSenderResponse",
-    "GlobalNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationResponse",
     "NotificationConfigurationRequest",
     "NotificationConfigurationRequest_Invoice",
     "NotificationConfigurationResponse",
     "NotificationConfigurationResponse_Invoice",
     "OrganizationId",
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from .color_scheme_response import ColorSchemeResponse
 from .email_log_response import EmailLogResponse
 from .email_provider_request import EmailProviderRequest
 from .email_provider_response import EmailProviderResponse
 from .email_sender_provider import EmailSenderProvider
 from .email_sender_request import EmailSenderRequest
 from .email_sender_response import EmailSenderResponse
-from .global_notification_configuration_request import GlobalNotificationConfigurationRequest
 from .invoice_notification_configuration_request import InvoiceNotificationConfigurationRequest
 from .invoice_notification_configuration_response import InvoiceNotificationConfigurationResponse
 from .notification_configuration_request import (
     NotificationConfigurationRequest,
     NotificationConfigurationRequest_Invoice,
 )
 from .notification_configuration_response import (
@@ -34,15 +33,14 @@
     "ColorSchemeResponse",
     "EmailLogResponse",
     "EmailProviderRequest",
     "EmailProviderResponse",
     "EmailSenderProvider",
     "EmailSenderRequest",
     "EmailSenderResponse",
-    "GlobalNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationRequest",
     "InvoiceNotificationConfigurationResponse",
     "NotificationConfigurationRequest",
     "NotificationConfigurationRequest_Invoice",
     "NotificationConfigurationResponse",
     "NotificationConfigurationResponse_Invoice",
     "OrganizationId",
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/color_scheme_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_log_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_provider_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_provider.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/email_sender_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/global_notification_configuration_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .invoice_notification_configuration_request import InvoiceNotificationConfigurationRequest
+from .bank_account_base_request import BankAccountBaseRequest
 
 
-class GlobalNotificationConfigurationRequest(pydantic.BaseModel):
-    invoice: typing.Optional[InvoiceNotificationConfigurationRequest]
+class BankAccountRequest(BankAccountBaseRequest):
+    bank_account: typing.Optional[BankAccountBaseRequest] = pydantic.Field(
+        alias="bankAccount", description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/invoice_notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/invoice_notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/notification_configuration_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/notification_configuration_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/notification_configuration_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/organization_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,30 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .color_scheme_request import ColorSchemeRequest
-from .email_provider_request import EmailProviderRequest
-from .global_notification_configuration_request import GlobalNotificationConfigurationRequest
-from .payment_methods_request import PaymentMethodsRequest
-
-
-class OrganizationRequest(pydantic.BaseModel):
-    name: typing.Optional[str]
-    logo: typing.Optional[str]
-    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
-    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
-    payment_methods: typing.Optional[PaymentMethodsRequest] = pydantic.Field(alias="paymentMethods")
-    email_provider: typing.Optional[EmailProviderRequest] = pydantic.Field(alias="emailProvider")
-    color_scheme: typing.Optional[ColorSchemeRequest] = pydantic.Field(alias="colorScheme")
-    notification_configuration: typing.Optional[GlobalNotificationConfigurationRequest] = pydantic.Field(
-        alias="notificationConfiguration"
+from .bank_type import BankType
+from .plaid_link_request import PlaidLinkRequest
+
+
+class BankAccountBaseRequest(pydantic.BaseModel):
+    bank_name: typing.Optional[str] = pydantic.Field(alias="bankName")
+    routing_number: typing.Optional[str] = pydantic.Field(alias="routingNumber")
+    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
+    account_type: typing.Optional[BankType] = pydantic.Field(alias="accountType")
+    plaid: typing.Optional[PlaidLinkRequest] = pydantic.Field(
+        description=("If provided, will link a bank account using Plaid Link\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_methods_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_markup.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_request.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/organization_types/types/payment_rail_response.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/__init__.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/plaid_link_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,25 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_type import BankType
-from .plaid_link_request import PlaidLinkRequest
 
 
-class BankAccountBaseRequest(pydantic.BaseModel):
-    bank_name: typing.Optional[str] = pydantic.Field(alias="bankName")
-    routing_number: typing.Optional[str] = pydantic.Field(alias="routingNumber")
-    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
-    account_type: typing.Optional[BankType] = pydantic.Field(alias="accountType")
-    plaid: typing.Optional[PlaidLinkRequest] = pydantic.Field(
-        description=("If provided, will link a bank account using Plaid Link\n")
+class PlaidLinkRequest(pydantic.BaseModel):
+    account_id: typing.Optional[str] = pydantic.Field(alias="accountId", description=("Account ID from Plaid Link\n"))
+    public_token: typing.Optional[str] = pydantic.Field(
+        alias="publicToken", description=("Public token from Plaid Link\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_account_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_base_request import BankAccountBaseRequest
+from .bank_account_base_response import BankAccountBaseResponse
 
 
-class BankAccountRequest(BankAccountBaseRequest):
-    bank_account: typing.Optional[BankAccountBaseRequest] = pydantic.Field(
+class BankAccountResponse(BankAccountBaseResponse):
+    bank_account: BankAccountBaseResponse = pydantic.Field(
         alias="bankAccount", description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_account_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .bank_account_base_response import BankAccountBaseResponse
+from .check_base_response import CheckBaseResponse
 
 
-class BankAccountResponse(BankAccountBaseResponse):
-    bank_account: BankAccountBaseResponse = pydantic.Field(
-        alias="bankAccount", description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
-    )
+class CheckResponse(CheckBaseResponse):
+    check: CheckBaseResponse = pydantic.Field(description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_status.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/bank_type.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_base_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_brand.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/card_type.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_base_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/check_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .check_base_response import CheckBaseResponse
+from .custom_payment_method_update_base_request import CustomPaymentMethodUpdateBaseRequest
 
 
-class CheckResponse(CheckBaseResponse):
-    check: CheckBaseResponse = pydantic.Field(description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n"))
+class CustomPaymentMethodUpdateRequest(CustomPaymentMethodUpdateBaseRequest):
+    custom: typing.Optional[CustomPaymentMethodUpdateBaseRequest] = pydantic.Field(
+        description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/currency_code.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py` & `mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .custom_payment_method_update_base_request import CustomPaymentMethodUpdateBaseRequest
+from ...entity_types.types.entity_response import EntityResponse
+from ...invoice_types.types.invoice_id import InvoiceId
+from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
+from .transaction_response import TransactionResponse
 
 
-class CustomPaymentMethodUpdateRequest(CustomPaymentMethodUpdateBaseRequest):
-    custom: typing.Optional[CustomPaymentMethodUpdateBaseRequest] = pydantic.Field(
-        description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
-    )
+class TransactionResponseExpanded(TransactionResponse):
+    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    payer: typing.Optional[EntityResponse]
+    vendor: typing.Optional[EntityResponse]
+    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
+    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_type.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py` & `mercoa-0.2.9/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/payment_method_types/types/plaid_link_request.py` & `mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...payment_method_types.types.currency_code import CurrencyCode
+from .transaction_status import TransactionStatus
 
 
-class PlaidLinkRequest(pydantic.BaseModel):
-    account_id: typing.Optional[str] = pydantic.Field(alias="accountId", description=("Account ID from Plaid Link\n"))
-    public_token: typing.Optional[str] = pydantic.Field(
-        alias="publicToken", description=("Public token from Plaid Link\n")
-    )
+class TransactionResponse(pydantic.BaseModel):
+    id: str
+    status: TransactionStatus
+    amount: float
+    currency: typing.Optional[CurrencyCode]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/transaction/client.py` & `mercoa-0.2.9/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.2.9/src/mercoa/resources/organization_types/types/organization_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity_types.types.entity_response import EntityResponse
-from ...invoice_types.types.invoice_id import InvoiceId
-from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
-from .transaction_response import TransactionResponse
-
-
-class TransactionResponseExpanded(TransactionResponse):
-    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
-    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
-    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
-    payer: typing.Optional[EntityResponse]
-    vendor: typing.Optional[EntityResponse]
-    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
-    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
+from .color_scheme_response import ColorSchemeResponse
+from .email_provider_response import EmailProviderResponse
+from .organization_id import OrganizationId
+from .payment_methods_response import PaymentMethodsResponse
+
+
+class OrganizationResponse(pydantic.BaseModel):
+    id: OrganizationId
+    sandbox: bool
+    name: str
+    logo_url: typing.Optional[str] = pydantic.Field(alias="logoUrl")
+    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
+    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
+    payment_methods: typing.Optional[PaymentMethodsResponse] = pydantic.Field(alias="paymentMethods")
+    email_provider: typing.Optional[EmailProviderResponse] = pydantic.Field(alias="emailProvider")
+    color_scheme: typing.Optional[ColorSchemeResponse] = pydantic.Field(alias="colorScheme")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.8/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.9/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.8/PKG-INFO` & `mercoa-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

