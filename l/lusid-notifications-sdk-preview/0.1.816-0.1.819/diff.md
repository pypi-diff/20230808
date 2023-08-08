# Comparing `tmp/lusid-notifications-sdk-preview-0.1.816.tar.gz` & `tmp/lusid-notifications-sdk-preview-0.1.819.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.816.tar", last modified: Fri Aug  4 17:26:47 2023, max compression
+gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.819.tar", last modified: Tue Aug  8 09:30:15 2023, max compression
```

## Comparing `lusid-notifications-sdk-preview-0.1.816.tar` & `lusid-notifications-sdk-preview-0.1.819.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/
--rw-r--r--   0 root         (0) root         (0)       54 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9646 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/
--rw-r--r--   0 root         (0) root         (0)     4432 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/
--rw-r--r--   0 root         (0) root         (0)      501 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10524 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   122660 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47801 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/
--rw-r--r--   0 root         (0) root         (0)     3078 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9027 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    13280 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16934 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_details.py
--rw-r--r--   0 root         (0) root         (0)     4727 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)    10747 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9540 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10705 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7437 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18059 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6099 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7775 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16992 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    17006 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/utilities/
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2745 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 17:26:47.000000 lusid-notifications-sdk-preview-0.1.816/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2322 2023-08-04 17:26:15.000000 lusid-notifications-sdk-preview-0.1.816/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      373 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9646 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10524 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   122660 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47801 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13280 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_details.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9540 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10705 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    18059 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7775 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7327 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16992 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    17006 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/utilities/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 09:30:15.000000 lusid-notifications-sdk-preview-0.1.819/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-08-08 09:27:17.000000 lusid-notifications-sdk-preview-0.1.819/setup.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/README.md` & `lusid-notifications-sdk-preview-0.1.819/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.816
-- Package version: 0.1.816
+- API version: 0.1.819
+- Package version: 0.1.819
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/__init__.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.816"
+__version__ = "0.1.819"
 
 # import apis into sdk package
 from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notifications.api.deliveries_api import DeliveriesApi
 from lusid_notifications.api.event_types_api import EventTypesApi
 from lusid_notifications.api.events_api import EventsApi
 from lusid_notifications.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/application_metadata_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/application_metadata_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/deliveries_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/event_types_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/events_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -150,15 +150,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "EventDetails",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/notifications_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -201,15 +201,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -384,15 +384,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -567,15 +567,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -750,15 +750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -930,15 +930,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1107,15 +1107,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1277,15 +1277,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -1480,15 +1480,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1683,15 +1683,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1886,15 +1886,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -2089,15 +2089,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api/subscriptions_api.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.816'
+        header_params['X-LUSID-SDK-Version'] = '0.1.819'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/api_client.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.816/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.819/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/configuration.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.816\n"\
-               "SDK Package Version: 0.1.816".\
+               "Version of the API: 0.1.819\n"\
+               "SDK Package Version: 0.1.819".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/exceptions.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/__init__.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/access_controlled_action.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/action_id.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/attempt.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/attempt_status.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/attempt_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_email_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_subscription.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/create_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/create_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/delivery.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_details.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_field_definition.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/id_selector_definition.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/identifier_part_schema.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/link.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/lusid_problem_details.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/matching_pattern.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/notification_status.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_id.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_delivery.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/resource_list_of_subscription.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/subscription.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_aws_sqs_notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_email_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_subscription.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/models/update_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/models/update_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/rest.py` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.816
+    The version of the OpenAPI document: 0.1.819
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications/utilities/config_keys.json` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.816/lusid_notifications_sdk_preview.egg-info/SOURCES.txt` & `lusid-notifications-sdk-preview-0.1.819/lusid_notifications_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.816/setup.py` & `lusid-notifications-sdk-preview-0.1.819/setup.py`

 * *Files identical despite different names*

