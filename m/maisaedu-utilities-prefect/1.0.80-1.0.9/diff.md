# Comparing `tmp/maisaedu-utilities-prefect-1.0.80.tar.gz` & `tmp/maisaedu-utilities-prefect-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-utilities-prefect-1.0.80.tar", last modified: Tue Aug  8 20:47:27 2023, max compression
+gzip compressed data, was "maisaedu-utilities-prefect-1.0.9.tar", last modified: Wed Nov 16 19:30:50 2022, max compression
```

## Comparing `maisaedu-utilities-prefect-1.0.80.tar` & `maisaedu-utilities-prefect-1.0.9.tar`

### file list

```diff
@@ -1,68 +1,59 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.307662 maisaedu-utilities-prefect-1.0.80/
--rw-r--r--   0 vsts      (1001) docker     (123)     1081 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      287 2023-08-08 20:47:27.307662 maisaedu-utilities-prefect-1.0.80/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.295662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/
--rw-r--r--   0 vsts      (1001) docker     (123)      679 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/constants/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/constants/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       41 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/constants/environment.py
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/constants/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/database/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/database/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2908 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/database/postgres.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11374 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/deploy.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4239 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/dw.py
--rw-r--r--   0 vsts      (1001) docker     (123)      349 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/environment.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/googlesheet/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/googlesheet/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2063 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/googlesheet/gspread.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/associations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1750 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/company.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5244 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/contacts.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1659 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/contacts_lists.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4275 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/deals.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2267 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/email_events.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/form_submission_events.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/forms.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2184 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/forms_submissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3845 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/landing_pages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1629 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/lineItems.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1936 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/marketing_emails.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2864 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/objects.py
--rw-r--r--   0 vsts      (1001) docker     (123)      693 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/owners.py
--rw-r--r--   0 vsts      (1001) docker     (123)      916 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/pipelines.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7439 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/tickets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2341 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/notification.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/one_drive/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/one_drive/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/one_drive/document_handling.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.299662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.303662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1955 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1007 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      981 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.303662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:07.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4921 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3371 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2584 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4403 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1111 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/user_service.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.307662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/scripts/
--rw-r--r--   0 vsts      (1001) docker     (123)     1771 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/scripts/flow-mem-limit
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/scripts/refresh-secrets
--rw-r--r--   0 vsts      (1001) docker     (123)     4543 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/secrets.py
--rw-r--r--   0 vsts      (1001) docker     (123)      783 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/tunnel.py
--rw-r--r--   0 vsts      (1001) docker     (123)      506 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-08 20:47:27.295662 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      287 2023-08-08 20:47:27.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2675 2023-08-08 20:47:27.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-08 20:47:27.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       94 2023-08-08 20:47:27.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       27 2023-08-08 20:47:27.000000 maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-08 20:47:27.307662 maisaedu-utilities-prefect-1.0.80/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      746 2023-08-08 20:47:08.000000 maisaedu-utilities-prefect-1.0.80/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1081 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/
+-rw-r--r--   0 vsts      (1001) docker     (122)      551 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/
+-rw-r--r--   0 vsts      (1001) docker     (122)       81 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/constants/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2819 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/postgres.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11374 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/deploy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3955 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/dw.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/environment.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1044 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/gspread.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/associations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/company.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5247 2022-11-16 19:30:31.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1653 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3970 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/deals.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2222 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/email_events.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1631 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2023 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3833 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/landing_pages.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1627 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/lineItems.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2060 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2864 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/objects.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      693 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/owners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      916 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/pipelines.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7425 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/tickets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2341 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/notification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1955 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4921 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2778 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2605 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1771 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/flow-mem-limit
+-rw-r--r--   0 vsts      (1001) docker     (122)      140 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/refresh-secrets
+-rw-r--r--   0 vsts      (1001) docker     (122)     4465 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/secrets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      506 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      286 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2190 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2022-11-16 19:30:50.000000 maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2022-11-16 19:30:50.506744 maisaedu-utilities-prefect-1.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      724 2022-11-16 19:30:28.000000 maisaedu-utilities-prefect-1.0.9/setup.py
```

### Comparing `maisaedu-utilities-prefect-1.0.80/LICENSE` & `maisaedu-utilities-prefect-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/__init__.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import maisaedu_utilities_prefect.secrets
 import maisaedu_utilities_prefect.dw
 import maisaedu_utilities_prefect.deploy
 import maisaedu_utilities_prefect.environment
 import maisaedu_utilities_prefect.notification
 import maisaedu_utilities_prefect.constants
 
-from .secrets import (
-    download_secret,
-    upload_secret,
-    setup_secrets,
-    refresh_secrets,
-    async_setup_secrets,
-)
-from .tunnel import create_server_tunnel, stop_server_tunnel
-from .dw import get_dsn, get_dsn_as_url, get_red_credentials, query_file, query_str
+from .secrets import download_secret, upload_secret, setup_secrets, refresh_secrets
+from .dw import get_dsn, get_dsn_as_url, query_file, query_str
 from .notification import notifier_factory, send_teams_alert_on_failure
 from .environment import get_env
 from .constants import PRODUCTION, LOCAL
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/database/postgres.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/database/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import psycopg2
 import psycopg2.extras as extras
 import pandas as pd
 import numpy as np
 import os
-from psycopg2.extensions import register_adapter, AsIs
-
-register_adapter(np.int64, AsIs)
 
 
 def connect(params_dic):
     """Connect to the PostgreSQL database server"""
 
     conn = psycopg2.connect(params_dic)
     return conn
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/deploy.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/deploy.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/dw.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/dw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import json
 import psycopg2
 import urllib.parse
 
 from prefect import task, Task
 
 from typing import Optional
 
@@ -12,25 +11,14 @@
     try:
         return os.environ["DATAWAREHOUSE_DSN"]
     except KeyError:
         with open(fallback) as f:
             return f.read()
 
 
-def get_red_credentials(env="prod"):
-    if env == "prod":
-        path = "data/dw-redshift-prod-credentials.json"
-    elif env == "dev":
-        path = "data/dw-redshift-dev-credentials.json"
-
-    with open(path) as f:
-        r = f.read()
-        return json.loads(r)
-
-
 def get_dsn_as_url(fallback: str = "data/dw-credentials.txt") -> Optional[str]:
     dsn = get_dsn(fallback)
     if dsn is not None:
         param_list = [part.split("=") for part in dsn.split()]
         params = {key: value for key, value in param_list}
         quoted_user = urllib.parse.quote(params["user"].encode("utf-8"))
         quoted_pass = urllib.parse.quote(params["password"].encode("utf-8"))
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/googlesheet/gspread.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/googlesheet/gspread.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,33 @@
-try:
-    from prefect.utilities.tasks import defaults_from_attrs
-    from prefect import Task
-
-    prefect_2 = False
-except Exception as e:
-    prefect_2 = True
-
-from typing import Any, List, Union
+from prefect.utilities.tasks import defaults_from_attrs
 import gspread
+from typing import Any, List, Union
+from prefect import Task
 import pathlib
 
-if prefect_2 is False:
-
-    class ReadGsheetRow(Task):
-        def __init__(
-            self,
-            credentials_filename: Union[str, pathlib.Path] = None,
-            sheet_key: str = None,
-            worksheet_name: str = None,
-            **kwargs: Any
-        ):
-            self.credentials_filename = credentials_filename
-            self.sheet_key = sheet_key
-            self.worksheet_name = worksheet_name
-            super().__init__(**kwargs)
-
-        @defaults_from_attrs("credentials_filename", "sheet_key", "worksheet_name")
-        def run(
-            self,
-            row: int,
-            credentials_filename: Union[str, pathlib.Path] = None,
-            sheet_key: str = None,
-            worksheet_name: str = None,
-        ) -> List[Any]:
-            client = gspread.service_account(filename=credentials_filename)
-            google_sheet = client.open_by_key(sheet_key)
-            worksheet = google_sheet.worksheet(worksheet_name)
-            return worksheet.row_values(row)
-
-else:
-
-    class ReadGsheetRow:
-        def __init__(
-            self,
-            credentials_filename: Union[str, pathlib.Path] = None,
-            sheet_key: str = None,
-            worksheet_name: str = None,
-            **kwargs: Any
-        ):
-            self.credentials_filename = credentials_filename
-            self.sheet_key = sheet_key
-            self.worksheet_name = worksheet_name
+class ReadGsheetRow(Task):
 
-        def get_rows(self, rows: int) -> List[Any]:
-            client = gspread.service_account(filename=self.credentials_filename)
-            google_sheet = client.open_by_key(self.sheet_key)
-            worksheet = google_sheet.worksheet(self.worksheet_name)
-            all_values = worksheet.get_all_values()
-            if rows <= len(all_values):
-                return all_values[rows - 1]
-            return []
+    def __init__(
+        self,
+        credentials_filename: Union[str, pathlib.Path] = None,
+        sheet_key: str = None,
+        worksheet_name: str = None,
+        **kwargs: Any
+    ):
+        self.credentials_filename = credentials_filename
+        self.sheet_key = sheet_key
+        self.worksheet_name = worksheet_name
+        super().__init__(**kwargs)
+
+    @defaults_from_attrs("credentials_filename", "sheet_key", "worksheet_name")
+    def run(
+        self,
+        row: int,
+        credentials_filename: Union[str, pathlib.Path] = None,
+        sheet_key: str = None,
+        worksheet_name: str = None,
+    ) -> List[Any]:
+    
+        client = gspread.service_account(filename=credentials_filename)
+        google_sheet = client.open_by_key(sheet_key)
+        worksheet = google_sheet.worksheet(worksheet_name)
+        return worksheet.row_values(row)
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/associations.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/associations.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,40 +10,34 @@
         toType,
     )
     if hapikey is not None:
         parameter_dict = {"hapikey": hapikey}
         headers = {"content-type": "application/json", "cache-control": "no-cache"}
 
     else:
-        parameter_dict = {"a": "a"}
-        headers = {
-            "content-type": "application/json",
-            "cache-control": "no-cache",
-            "Authorization": f"Bearer {app_private_token}",
-        }
-
+        parameter_dict = {"a":"a"}
+        headers = {"content-type": "application/json", "cache-control": "no-cache", 'Authorization': f"Bearer {app_private_token}"}
+        
     parameters = urllib.parse.urlencode(parameter_dict)
 
     body = json.dumps({"inputs": ids})
 
     post_url = url + parameters
     for i in range(tries):
         try:
             r = requests.post(url=post_url, headers=headers, data=body)
             response_dict = json.loads(r.text)
 
             return response_dict
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
 
 
-def get_all_associations(
-    hapikey, app_private_token, fromType, toType, ids, batch_size=5000
-):
+def get_all_associations(hapikey, app_private_token, fromType, toType, ids, batch_size=5000):
     list_df = [ids[i : i + batch_size] for i in range(0, len(ids), batch_size)]
 
     for i in list_df:
         try:
             resp = get_associations(hapikey, app_private_token, fromType, toType, i)
             yield resp["results"]
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/company.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/company.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     get_url = url + parameters
     for i in range(tries):
         try:
             r = requests.get(url=get_url, headers=headers)
             response_dict = json.loads(r.text)
             return response_dict
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
 
 
 def getAllCompanies(hapikey, app_private_token, properties):
     hasmore = True
     offset = 0
     attempts = 0
     while hasmore:
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/contacts.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
                 else:
                     hasmore = False
         except Exception as e:
             hasmore = False
 
 
 def get_contacts_full_load(hapikey, app_private_token, properties, after, tries=5):
+
     if hapikey is not None:
         url = "https://api.hubapi.com/crm/v3/objects/contacts?"
         parameter_dict = {"hapikey": hapikey}
         headers = {"content-type": "application/json", "cache-control": "no-cache"}
 
         parameters = urllib.parse.urlencode(parameter_dict)
     else:
@@ -149,20 +150,20 @@
             yield resp["results"]
             after = resp["paging"]["next"]["after"]
             attempts = 0
         except KeyError as e:
             if "message" in resp:
                 if resp["message"] == "You have reached your secondly limit.":
                     attempts += 1
-                    sleep(4)
+                    sleep(10)
                     if attempts > 2:
                         raise Exception(resp["message"])
             else:
                 if "status" in resp and resp["status"] == "error":
                     attempts += 1
-                    sleep(4)
+                    sleep(10)
                     if attempts > 2:
                         raise Exception(resp["message"])
                 else:
                     hasmore = False
         except Exception as e:
             hasmore = False
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/contacts_lists.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import requests
 import json
 import urllib
 import time
 import prefect
 
 
-def get_contacts_lists(api_key, app_private_token, offset=None, limit=250):
-    url = "https://api.hubapi.com/contacts/v1/lists?"
+def get_forms(api_key, app_private_token, offset=None, limit=1000):
+    url = "https://api.hubapi.com/forms/v2/forms?"
     if api_key is not None:
-        parameter_dict = {"hapikey": api_key, "count": limit}
+        parameter_dict = {"hapikey": api_key, "limit": limit}
         headers = {"content-type": "application/json", "cache-control": "no-cache"}
     else:
-        parameter_dict = {"count": limit}
+        parameter_dict = {"limit": limit}
         headers = {
             "content-type": "application/json",
             "cache-control": "no-cache",
             "Authorization": f"Bearer {app_private_token}",
         }
 
     if offset is not None:
@@ -29,27 +29,28 @@
         r = requests.get(url=url, headers=headers)
         response_dict = json.loads(r.text)
         return response_dict
     except Exception as e:
         print(e)
 
 
-def get_all_contacts_lists(api_key, app_private_token, limit=250):
+def get_all_forms(api_key, app_private_token, limit=1000):
     offset = 0
     has_more = True
     while has_more:
-        resp = get_contacts_lists(api_key, app_private_token, offset, limit)
+        resp = get_forms(api_key, app_private_token, offset, limit)
 
         try:
-            yield resp["lists"]
-            offset = offset + len(resp["lists"])
-            has_more = resp["has-more"]
+            yield resp
+            offset = offset + len(resp)
+            if len(resp) == 0:
+                has_more = False
         except Exception as e:
             if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/deals.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/deals.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     get_url = url + parameters
     for i in range(tries):
         try:
             r = requests.get(url=get_url, headers=headers)
             response_dict = json.loads(r.text)
             return response_dict
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
 
 
 def get_deals_v1_recent_modified(
     hapikey, app_private_token, properties, offset, extraparams, since, tries=5
 ):
     url = "https://api.hubapi.com/deals/v1/deal/recent/modified?"
     if hapikey is not None:
@@ -79,34 +79,34 @@
     get_url = url + parameters
     for i in range(tries):
         try:
             r = requests.get(url=get_url, headers=headers)
             response_dict = json.loads(r.text)
             return response_dict
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
 
 
 def get_all_deals_v1(hapikey, app_private_token, properties, extraparams):
     data = list()
     hasmore = True
     offset = 0
     attempts = 0
     while hasmore:
         resp = get_deals_v1(hapikey, app_private_token, properties, offset, extraparams)
         try:
             yield resp["deals"]
             hasmore = resp["hasMore"]
             offset = resp["offset"]
+            yield resp["deals"]
             attempts = 0
         except KeyError as e:
             attempts += 1
             sleep(10)
             if attempts > 2:
-                prefect.get_run_logger().error(resp)
                 raise Exception(e)
     return data
 
 
 def get_all_deals_v1_recent_modified(
     hapikey, app_private_token, properties, extraparams, since
 ):
@@ -116,25 +116,17 @@
     attempts = 0
     while hasmore:
         resp = get_deals_v1_recent_modified(
             hapikey, app_private_token, properties, offset, extraparams, since
         )
         try:
             yield resp["results"]
-            lasttimestamp = list(resp["results"])[0]["properties"][
-                "hs_lastmodifieddate"
-            ]["timestamp"]
-            attempts = 0
             hasmore = resp["hasMore"]
             offset = resp["offset"]
+            yield resp["results"]
             attempts = 0
         except KeyError as e:
-            if offset >= 10000:
-                since = str(lasttimestamp)
-                offset = 0
-
             attempts += 1
             sleep(10)
             if attempts > 2:
-                prefect.get_run_logger().error(resp)
                 raise Exception(e)
     return data
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/email_events.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/email_events.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,22 +34,26 @@
     if end_timestamp is not None:
         parameter_dict["endTimestamp"] = end_timestamp
 
     parameters = urllib.parse.urlencode(parameter_dict)
 
     url = url + parameters
 
-    r = requests.get(url=url, headers=headers, timeout=10)
-    response_dict = json.loads(r.text)
-    return response_dict
+    try:
+        r = requests.get(url=url, headers=headers)
+        response_dict = json.loads(r.text)
+        return response_dict
+    except Exception as e:
+        print(e)
 
 
 def get_all_email_events(
     api_key, app_private_token, start_timestamp=None, end_timestamp=None, limit=1000
 ):
+
     offset = None
     has_more = True
     attempts = 0
     while has_more:
         resp = get_events(
             api_key, app_private_token, start_timestamp, end_timestamp, offset, limit
         )
@@ -62,20 +66,16 @@
 
                 yield resp["events"]
             else:
                 attempts += 1
                 if attempts > 2:
                     has_more = False
         except Exception as e:
-            if (
-                isinstance(e, TypeError)
-                and "errorType" in e
-                and e["errorType"] == "RATE_LIMIT"
-            ):
+            if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/form_submission_events.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/marketing_emails.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,68 @@
-import prefect
 import requests
 import json
 import urllib
-from time import sleep
-
-
-def get_hubspot_form_submission_events(
-        hapikey, app_private_token, occurred_after, occurred_before, after, limit
-):
-    url = "https://api.hubapi.com/events/v3/events?"
-
-    parameter_dict = {
-        "eventType": "e_form_submission_v2",
-        "occurredAfter": occurred_after,
-        "limit": limit
-    }
-
-    if occurred_before:
-        parameter_dict["occurredBefore"] = occurred_before
+import time
+import prefect
 
-    if after:
-        parameter_dict["after"] = after
 
-    if hapikey is not None:
-        parameter_dict = {"hapikey": hapikey}
+def get_marketing_emails(api_key, app_private_token, updated_at=None, offset=None):
+    url = "https://api.hubapi.com/marketing-emails/v1/emails/with-statistics?"
+    if api_key is not None:
+        parameter_dict = {"hapikey": api_key, "limit": 100}
         headers = {"content-type": "application/json", "cache-control": "no-cache"}
     else:
+        parameter_dict = {"limit": 100}
         headers = {
             "content-type": "application/json",
             "cache-control": "no-cache",
             "Authorization": f"Bearer {app_private_token}",
         }
 
+    if offset is not None:
+        parameter_dict["offset"] = offset
+
+    if updated_at is not None:
+        parameter_dict["updated__gte"] = updated_at
+
+    parameter_dict["orderBy"] = "updated"
+
     parameters = urllib.parse.urlencode(parameter_dict)
 
-    url += parameters
+    url = url + parameters
+
     try:
-        response = requests.get(url=url, headers=headers)
-        response_dict = json.loads(response.text)
+        r = requests.get(url=url, headers=headers)
+        response_dict = json.loads(r.text)
         return response_dict
     except Exception as e:
         print(e)
 
 
-def get_form_submission_events(
-        hapikey, app_private_token, occurred_after, occurred_before=None, limit=100
-):
-    after = None
-    has_more = True
+def get_all_marketing_emails(api_key, app_private_token, updated_at=None):
+    offset = 0
+    total = 1
     attempts = 0
-    while has_more:
-        response = get_hubspot_form_submission_events(
-            hapikey, app_private_token, occurred_after, occurred_before, after, limit
-        )
+    while total > offset:
+        resp = get_marketing_emails(api_key, app_private_token, updated_at, offset)
 
         try:
-            if "results" in response:
+            if "objects" in resp and "offset" in resp:
                 attempts = 0
-                yield response["results"]
-                if "paging" not in response:
-                    has_more = False
-                else:
-                    after = response["paging"]["next"]["after"]
+                offset = resp["offset"] + len(resp["objects"])
+                total = resp["total"]
+
+                yield resp["objects"]
             else:
                 attempts += 1
                 if attempts > 2:
-                    has_more = False
-        except TypeError as e:
-            print("Erro de tipo encontrado:", e)
-            print(response)
-            sleep(10)
+                    offset = total
         except Exception as e:
             if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
-                print(response)
-                sleep(10)
+                print(resp)
+                time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(response)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/forms.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/contacts_lists.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 import requests
 import json
 import urllib
 import time
 import prefect
 
 
-def get_forms(api_key, app_private_token, offset=None, limit=1000):
-    url = "https://api.hubapi.com/forms/v2/forms?"
-
-    parameter_dict = {
-        "limit": limit,
-        "formTypes": "ALL"
-    }
-
-    headers = {"content-type": "application/json", "cache-control": "no-cache"}
+def get_contacts_lists(api_key, app_private_token, offset=None, limit=250):
+    url = "https://api.hubapi.com/contacts/v1/lists?"
     if api_key is not None:
-        parameter_dict["hapikey"] = api_key
+        parameter_dict = {"hapikey": api_key, "count": limit}
+        headers = {"content-type": "application/json", "cache-control": "no-cache"}
     else:
-        headers["Authorization"] = f"Bearer {app_private_token}"
+        parameter_dict = {"count": limit}
+        headers = {
+            "content-type": "application/json",
+            "cache-control": "no-cache",
+            "Authorization": f"Bearer {app_private_token}",
+        }
 
-    if offset:
+    if offset is not None:
         parameter_dict["offset"] = offset
 
     parameters = urllib.parse.urlencode(parameter_dict)
-    url += parameters
+
+    url = url + parameters
 
     try:
         r = requests.get(url=url, headers=headers)
         response_dict = json.loads(r.text)
         return response_dict
     except Exception as e:
         print(e)
 
 
-def get_all_forms(api_key, app_private_token, limit=1000):
+def get_all_contacts_lists(api_key, app_private_token, limit=250):
     offset = 0
     has_more = True
     while has_more:
-        resp = get_forms(api_key, app_private_token, offset, limit)
+        resp = get_contacts_lists(api_key, app_private_token, offset, limit)
 
         try:
-            yield resp
-            offset = offset + len(resp)
-            if len(resp) == 0:
-                has_more = False
+            yield resp["lists"]
+            offset = offset + len(resp["lists"])
+            has_more = resp["has-more"]
         except Exception as e:
             if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/forms_submissions.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/forms_submissions.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,20 +53,16 @@
                 else:
                     after = resp["paging"]["next"]["after"]
             else:
                 attempts += 1
                 if attempts > 2:
                     has_more = False
         except Exception as e:
-            if isinstance(e, TypeError):
-                print("Erro de tipo encontrado:", e)
-                print(resp)
-                time.sleep(10)
-            elif "errorType" in e and e["errorType"] == "RATE_LIMIT":
+            if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/landing_pages.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/landing_pages.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,17 @@
                     has_more = False
         except Exception as e:
             if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
 
 
 def get_landing_pages_stats(api_key, app_private_token, limit=50, offset=None):
     url = f"https://api.hubapi.com/analytics/v2/reports/landing-pages/total?"
     if api_key is not None:
         parameter_dict = {"hapikey": api_key, "limit": limit}
@@ -113,11 +113,11 @@
                     has_more = False
         except Exception as e:
             if "errorType" in e and e["errorType"] == "RATE_LIMIT":
                 print(e)
                 print(resp)
                 time.sleep(10)
             else:
-                prefect.get_run_logger().error("Failed")
-                prefect.get_run_logger().error(e)
-                prefect.get_run_logger().error(resp)
+                prefect.context.logger.error("Failed")
+                prefect.context.logger.error(e)
+                prefect.context.logger.error(resp)
                 raise e
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/lineItems.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/lineItems.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     get_url = url + parameters
     for i in range(tries):
         try:
             r = requests.get(url=get_url, headers=headers)
             response_dict = json.loads(r.text)
             return response_dict
         except Exception as e:
-            prefect.get_run_logger().error(e)
+            prefect.context.logger.error(e)
 
 
 def getLineItemsFull(hapikey, app_private_token, properties):
     after = 0
     hasmore = True
     attempts = 0
     while hasmore:
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/objects.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/objects.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/owners.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/owners.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/pipelines.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/pipelines.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/hubspot/tickets.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/hubspot/tickets.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         strAfter = ', "after":"%s"' % (after)
     else:
         strAfter = ""
     publicObjectSearchRequest = """{
         "filterGroups": [ 
             { "filters": [
                 { "propertyName": "hs_lastmodifieddate", "operator": "GTE", "value": "%s" },
-                { "propertyName": "hs_object_id", "operator": "GT", "value": %d }
+                { "propertyName": "id", "operator": "GT", "value": %d }
             ] 
         }],
         "sorts": [{ "propertyName": "hs_lastmodifieddate", "direction": "ASCENDING" }],
         "query":"",
         "properties":["%s"],
         "limit":%d %s
     }""" % (
@@ -100,15 +100,15 @@
             attempts = 0
             response_dict = json.loads(r.text)
             if len(response_dict["results"]) == 0:
                 break
             results_part_1 = response_dict["results"]
         except Exception as e:
             attempts += 1
-            prefect.get_run_logger().info(f"Error {e}")
+            prefect.context.logger.info(f"Error {e}")
             if attempts > 2:
                 raise e
             sleep(10)
 
     attempts = 0
 
     while len(results_part_2) == 0:
@@ -119,15 +119,15 @@
             attempts = 0
             response_dict = json.loads(r.text)
             if len(response_dict["results"]) == 0:
                 break
             results_part_2 = response_dict["results"]
         except Exception as e:
             attempts += 1
-            prefect.get_run_logger().info(f"Error {e}")
+            prefect.context.logger.info(f"Error {e}")
             if attempts > 2:
                 raise e
             sleep(10)
 
     return results_part_1 + results_part_2
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/notification.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/notification.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,27 +59,14 @@
         if response.status_code != 200:
             raise HTTPError(
                 response, f"Get Groups request returned http error: {response.json()}"
             )
 
         return self.admin_groups_from_get_groups_as_admin_response(response)
 
-    def add_user_as_admin(self, group_id, username, access_right="Viewer"):
-        """Grants user permissions to the specified workspace."""
-        url = f"{self.base_url}/{self.groups_snippet}/{group_id}/{self.users_snippet}"
-        body = {"userEmailAddress": username, "groupUserAccessRight": access_right}
-
-        response = requests.post(url, body, headers=self.client.auth_header)
-
-        if response.status_code != 200:
-            raise HTTPError(
-                response,
-                f"Request to add user {username} permissions to group {group_id} failed.",
-            )
-
     @classmethod
     def admin_groups_from_get_groups_as_admin_response(cls, response):
         """
         Creates a list of groups from a http response object
         :param response:
             The http response object
         :return: list
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/powerbi_api/services/client.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/powerbi_api/services/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,25 @@
+import json
+import datetime
 import adal
 
 from .adminGroupsService import adminGroups
 from .activityLogs import activityLogs
-from .dataset_service import DatasetService
-from .user_service import UserService
-
 
 class PowerBIClient:
-    default_resource_url = "https://analysis.windows.net/powerbi/api"
-    default_api_url = "https://api.powerbi.com"
-    default_authority_url = "https://login.windows.net/common"
-
-    api_version_snippet = "v1.0"
-    api_myorg_snippet = "myorg"
-    api_admin_snippet = "admin"
+    default_resource_url = 'https://analysis.windows.net/powerbi/api'
+    default_api_url = 'https://api.powerbi.com'
+    default_authority_url = 'https://login.windows.net/common'
+
+    api_version_snippet = 'v1.0'
+    api_myorg_snippet = 'myorg'
+    api_admin_snippet = 'admin'
 
     @staticmethod
-    def get_client_with_username_password(
-        client_id,
-        username,
-        password,
-        authority_url=None,
-        resource_url=None,
-        api_url=None,
-    ):
+    def get_client_with_username_password(client_id, username, password, authority_url=None, resource_url=None, api_url=None):
         """
         Constructs a client with the option of using common defaults.
 
         :param client_id: The Power BI Client ID
         :param username: Username
         :param password: Password
         :param authority_url: The authority_url; defaults to 'https://login.windows.net/common'
@@ -40,42 +32,40 @@
 
         if resource_url is None:
             resource_url = PowerBIClient.default_resource_url
 
         if api_url is None:
             api_url = PowerBIClient.default_api_url
 
-        context = adal.AuthenticationContext(
-            authority=authority_url, validate_authority=True, api_version=None
-        )
+        context = adal.AuthenticationContext(authority=authority_url,
+                                             validate_authority=True,
+                                             api_version=None)
 
         # get your authentication token
-        token = context.acquire_token_with_username_password(
-            resource=resource_url,
-            client_id=client_id,
-            username=username,
-            password=password,
-        )
+        token = context.acquire_token_with_username_password(resource=resource_url,
+                                                             client_id=client_id,
+                                                             username=username,
+                                                             password=password)
 
         return PowerBIClient(api_url, token)
 
     def __init__(self, api_url, token):
-        self.__auth_header = None
         self.api_url = api_url
         self.token = token
-        self.activityLogs = activityLogs(self)
         self.adminGroups = adminGroups(self)
-        self.datasets = DatasetService(self)
-        self.users = UserService(self)
-        # self.reports = Reports(self)
-        # self.imports = Imports(self)
-        # self.groups = Groups(self)
-        # self.gateways = Gateways(self)
+        self.activityLogs = activityLogs(self)
+        #self.datasets = Datasets(self)
+        #self.reports = Reports(self)
+        #self.imports = Imports(self)
+        #self.groups = Groups(self)
+        #self.gateways = Gateways(self)
 
     @property
     def auth_header(self):
-        if self.__auth_header is None:
-            self.__auth_header = {
-                "Authorization": f'Bearer {self.token["accessToken"]}'
+        if self._auth_header is None:
+            self._auth_header = {
+                'Authorization': f'Bearer {self.token["accessToken"]}'
             }
 
-        return self.__auth_header
+        return self._auth_header
+
+    _auth_header = None
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/scripts/flow-mem-limit` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/scripts/flow-mem-limit`

 * *Files identical despite different names*

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect/secrets.py` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect/secrets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import json
+import prefect
 import os
 import psycopg2
 
 from dataclasses import dataclass
 from abc import abstractmethod, ABC
 from prefect import task
 from typing import Optional
@@ -105,45 +106,37 @@
                 f"Environment variable {self.env_var} already set"
             )
             return
 
         os.environ[self.env_var] = bytes(contents).decode("utf8")
 
 
-def task_setup_secrets(secrets_path: str = "secrets.json", **kwargs):
+def setup_secrets(secrets_path: str = "secrets.json", **kwargs):
     fallback_path = "secrets.json"
-    try:
+    try: 
         with open(secrets_path) as secrets_file:
             secrets = json.load(secrets_file)
     except Exception as e:
         with open(fallback_path) as secrets_file:
             secrets = json.load(secrets_file)
 
-    with psycopg2.connect(get_dsn()) as connection, connection.cursor() as cursor:
-        for secret_name, definition in secrets.items():
-            cursor.execute("select meta.get_secret(%s)", [secret_name])
-            (content,) = cursor.fetchone()
-            if content is None:
-                print("Secret does not exist or is not accessible", secret_name)
-            else:
-                Secret.parse(definition).store(content)
-
-
-@task()
-async def async_setup_secrets(secrets_path: str = "secrets.json"):
-    task_setup_secrets(secrets_path)
-
-    return True
-
-
-@task()
-def setup_secrets(secrets_path: str = "secrets.json"):
-    task_setup_secrets(secrets_path)
+    @task(**kwargs)
+    def setup_secrets():
+        with psycopg2.connect(get_dsn()) as connection, connection.cursor() as cursor:
+            for secret_name, definition in secrets.items():
+                cursor.execute("select meta.get_secret(%s)", [secret_name])
+                (content,) = cursor.fetchone()
+                if content is None:
+                    raise Exception(
+                        "Secret does not exist or is not accessible", secret_name
+                    )
+                else:
+                    Secret.parse(definition).store(content)
 
-    return True
+    return setup_secrets()
 
 
 def refresh_secrets(secrets_path: str = "secrets.json"):
     with open(secrets_path) as secrets_file:
         secrets = json.load(secrets_file)
 
         with psycopg2.connect(get_dsn()) as connection, connection.cursor() as cursor:
```

### Comparing `maisaedu-utilities-prefect-1.0.80/maisaedu_utilities_prefect.egg-info/SOURCES.txt` & `maisaedu-utilities-prefect-1.0.9/maisaedu_utilities_prefect.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.py
 maisaedu_utilities_prefect/__init__.py
 maisaedu_utilities_prefect/deploy.py
 maisaedu_utilities_prefect/dw.py
 maisaedu_utilities_prefect/environment.py
 maisaedu_utilities_prefect/notification.py
 maisaedu_utilities_prefect/secrets.py
-maisaedu_utilities_prefect/tunnel.py
 maisaedu_utilities_prefect/utils.py
 maisaedu_utilities_prefect.egg-info/PKG-INFO
 maisaedu_utilities_prefect.egg-info/SOURCES.txt
 maisaedu_utilities_prefect.egg-info/dependency_links.txt
 maisaedu_utilities_prefect.egg-info/requires.txt
 maisaedu_utilities_prefect.egg-info/top_level.txt
 maisaedu_utilities_prefect/constants/__init__.py
@@ -23,32 +22,25 @@
 maisaedu_utilities_prefect/hubspot/__init__.py
 maisaedu_utilities_prefect/hubspot/associations.py
 maisaedu_utilities_prefect/hubspot/company.py
 maisaedu_utilities_prefect/hubspot/contacts.py
 maisaedu_utilities_prefect/hubspot/contacts_lists.py
 maisaedu_utilities_prefect/hubspot/deals.py
 maisaedu_utilities_prefect/hubspot/email_events.py
-maisaedu_utilities_prefect/hubspot/form_submission_events.py
 maisaedu_utilities_prefect/hubspot/forms.py
 maisaedu_utilities_prefect/hubspot/forms_submissions.py
 maisaedu_utilities_prefect/hubspot/landing_pages.py
 maisaedu_utilities_prefect/hubspot/lineItems.py
 maisaedu_utilities_prefect/hubspot/marketing_emails.py
 maisaedu_utilities_prefect/hubspot/objects.py
 maisaedu_utilities_prefect/hubspot/owners.py
 maisaedu_utilities_prefect/hubspot/pipelines.py
 maisaedu_utilities_prefect/hubspot/tickets.py
-maisaedu_utilities_prefect/one_drive/__init__.py
-maisaedu_utilities_prefect/one_drive/document_handling.py
 maisaedu_utilities_prefect/powerbi_api/__init__.py
 maisaedu_utilities_prefect/powerbi_api/models/__init__.py
 maisaedu_utilities_prefect/powerbi_api/models/adminGroupModel.py
-maisaedu_utilities_prefect/powerbi_api/models/datasetDatasourceModel.py
-maisaedu_utilities_prefect/powerbi_api/models/datasetRefreshScheduleModel.py
 maisaedu_utilities_prefect/powerbi_api/services/__init__.py
 maisaedu_utilities_prefect/powerbi_api/services/activityLogs.py
 maisaedu_utilities_prefect/powerbi_api/services/adminGroupsService.py
 maisaedu_utilities_prefect/powerbi_api/services/client.py
-maisaedu_utilities_prefect/powerbi_api/services/dataset_service.py
-maisaedu_utilities_prefect/powerbi_api/services/user_service.py
 maisaedu_utilities_prefect/scripts/flow-mem-limit
 maisaedu_utilities_prefect/scripts/refresh-secrets
```

### Comparing `maisaedu-utilities-prefect-1.0.80/setup.py` & `maisaedu-utilities-prefect-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-utilities-prefect",
-    version="1.0.80",
+    version="1.0.9",
     description="Utilities for interaction with Prefect, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[
         "maisaedu_utilities_prefect/scripts/refresh-secrets",
@@ -19,10 +19,9 @@
         "wheel",
         "prefect",
         "papermill",
         "psycopg2-binary",
         "aiopg",
         "aiochannel",
         "gspread",
-        "sshtunnel",
     ],  # external packages as dependencies
 )
```

