# Comparing `tmp/hdn-research-environment-2.2.0.tar.gz` & `tmp/hdn-research-environment-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-2.2.0.tar", last modified: Mon Jun 26 17:43:39 2023, max compression
+gzip compressed data, was "hdn-research-environment-2.3.0.tar", last modified: Tue Aug  8 08:10:33 2023, max compression
```

## Comparing `hdn-research-environment-2.2.0.tar` & `hdn-research-environment-2.3.0.tar`

### file list

```diff
@@ -1,98 +1,94 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-2.2.0/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-2.2.0/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-2.2.0/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/v1/
--rw-r--r--   0 karolszuster   (501) staff       (20)     3242 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      700 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/api/v1/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/api/v2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1726 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/api/v2/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      942 2023-05-30 18:52:36.000000 hdn-research-environment-2.2.0/environment/api/v2/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3175 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1005 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1878 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2928 2023-05-29 12:32:30.000000 hdn-research-environment-2.2.0/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      869 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3711 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1720 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/mailers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1443 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1579 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      403 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2220 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      394 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0006_delete_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2347 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0007_billingaccountsharinginvite.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      476 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0008_workflow_workspace_name.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      420 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1364 2023-05-31 14:40:16.000000 hdn-research-environment-2.2.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2518 2023-06-18 19:04:20.000000 hdn-research-environment-2.2.0/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    20869 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4545 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-2.2.0/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/static/environment/css/environment-base.css
--rw-r--r--   0 karolszuster   (501) staff       (20)      117 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/css/manage_billing_account.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-2.2.0/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      291 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/static/environment/js/forms.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3154 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     2652 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     6560 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1419 2023-06-19 12:34:04.000000 hdn-research-environment-2.2.0/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1916 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/_billing_accounts_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3297 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/environment/_environment_tabs.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1073 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3863 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/templates/environment/create_research_environment.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1644 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/templates/environment/create_workspace.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      272 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/billing_sharing_confirmation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      351 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1163 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     5942 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/manage_billing_account.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      562 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/environment/manage_shared_billing_invitation.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1649 2023-06-19 11:33:54.000000 hdn-research-environment-2.2.0/environment/templates/environment/research_environments.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1473 2023-06-19 10:22:33.000000 hdn-research-environment-2.2.0/environment/templates/tag/environment_modal_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1957 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templates/tag/workspace_destroy_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     4409 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      645 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12158 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3007 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10693 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     5328 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2909 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      640 2023-05-29 11:58:39.000000 hdn-research-environment-2.2.0/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3380 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1634 2023-06-26 17:42:34.000000 hdn-research-environment-2.2.0/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1135 2023-05-29 11:59:00.000000 hdn-research-environment-2.2.0/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-2.2.0/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    15553 2023-06-26 17:42:41.000000 hdn-research-environment-2.2.0/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     3262 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-2.2.0/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-06-26 17:43:39.000000 hdn-research-environment-2.2.0/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-2.2.0/setup.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.870175 hdn-research-environment-2.3.0/
+-rw-r--r--   0 kshalot    (501) staff       (20)     1551 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/LICENSE
+-rw-r--r--   0 kshalot    (501) staff       (20)      115 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/MANIFEST.in
+-rw-r--r--   0 kshalot    (501) staff       (20)      978 2023-08-08 08:10:33.870242 hdn-research-environment-2.3.0/PKG-INFO
+-rw-r--r--   0 kshalot    (501) staff       (20)       90 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/README.md
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.861515 hdn-research-environment-2.3.0/environment/
+-rw-r--r--   0 kshalot    (501) staff       (20)        0 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/__init__.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.861799 hdn-research-environment-2.3.0/environment/api/
+-rw-r--r--   0 kshalot    (501) staff       (20)     4586 2023-08-08 08:01:12.000000 hdn-research-environment-2.3.0/environment/api/__init__.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      939 2023-08-08 08:01:56.000000 hdn-research-environment-2.3.0/environment/api/decorators.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      154 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/apps.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     3057 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/constants.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      995 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/decorators.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1418 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/deserializers.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     2834 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/entities.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      869 2023-07-04 10:33:07.000000 hdn-research-environment-2.3.0/environment/exceptions.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     3622 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/forms.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1719 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/mailers.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      155 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/managers.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.863186 hdn-research-environment-2.3.0/environment/migrations/
+-rw-r--r--   0 kshalot    (501) staff       (20)     1443 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/migrations/0001_initial.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1579 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      403 2023-05-12 08:10:12.000000 hdn-research-environment-2.3.0/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      420 2023-05-12 08:10:12.000000 hdn-research-environment-2.3.0/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     2220 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/migrations/0005_workflow.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      394 2023-05-25 10:03:32.000000 hdn-research-environment-2.3.0/environment/migrations/0006_delete_billingsetup.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     2348 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/migrations/0007_billingaccountsharinginvite.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      476 2023-05-26 13:54:02.000000 hdn-research-environment-2.3.0/environment/migrations/0008_workflow_workspace_name.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      420 2023-05-27 12:10:55.000000 hdn-research-environment-2.3.0/environment/migrations/0009_billingaccountsharinginvite_is_revoked.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1364 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py
+-rw-r--r--   0 kshalot    (501) staff       (20)        0 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/migrations/__init__.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     2518 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/models.py
+-rw-r--r--   0 kshalot    (501) staff       (20)    17413 2023-08-08 08:01:47.000000 hdn-research-environment-2.3.0/environment/services.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     4519 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/signals.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.857765 hdn-research-environment-2.3.0/environment/static/
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.857857 hdn-research-environment-2.3.0/environment/static/environment/
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.863571 hdn-research-environment-2.3.0/environment/static/environment/css/
+-rw-r--r--   0 kshalot    (501) staff       (20)      342 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 kshalot    (501) staff       (20)     6583 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/static/environment/css/environment-base.css
+-rw-r--r--   0 kshalot    (501) staff       (20)      117 2023-05-26 12:35:14.000000 hdn-research-environment-2.3.0/environment/static/environment/css/manage_billing_account.css
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.864077 hdn-research-environment-2.3.0/environment/static/environment/js/
+-rw-r--r--   0 kshalot    (501) staff       (20)      564 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/static/environment/js/cookie.js
+-rw-r--r--   0 kshalot    (501) staff       (20)      291 2023-06-09 10:19:30.000000 hdn-research-environment-2.3.0/environment/static/environment/js/forms.js
+-rw-r--r--   0 kshalot    (501) staff       (20)      516 2023-05-12 07:55:20.000000 hdn-research-environment-2.3.0/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 kshalot    (501) staff       (20)     3125 2023-08-07 10:44:17.000000 hdn-research-environment-2.3.0/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 kshalot    (501) staff       (20)     3308 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/tasks.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.865985 hdn-research-environment-2.3.0/environment/templates/
+-rw-r--r--   0 kshalot    (501) staff       (20)     6148 2023-05-17 08:57:46.000000 hdn-research-environment-2.3.0/environment/templates/.DS_Store
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.867500 hdn-research-environment-2.3.0/environment/templates/environment/
+-rw-r--r--   0 kshalot    (501) staff       (20)     6624 2023-08-07 10:44:17.000000 hdn-research-environment-2.3.0/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1419 2023-06-19 14:56:50.000000 hdn-research-environment-2.3.0/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1916 2023-06-05 16:41:15.000000 hdn-research-environment-2.3.0/environment/templates/environment/_billing_accounts_list.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     3297 2023-07-04 10:33:07.000000 hdn-research-environment-2.3.0/environment/templates/environment/_environment_tabs.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1073 2023-06-09 13:11:36.000000 hdn-research-environment-2.3.0/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     3863 2023-07-04 09:26:32.000000 hdn-research-environment-2.3.0/environment/templates/environment/create_research_environment.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1644 2023-07-04 09:26:32.000000 hdn-research-environment-2.3.0/environment/templates/environment/create_workspace.html
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.867745 hdn-research-environment-2.3.0/environment/templates/environment/email/
+-rw-r--r--   0 kshalot    (501) staff       (20)      272 2023-06-09 07:30:06.000000 hdn-research-environment-2.3.0/environment/templates/environment/email/billing_sharing_confirmation.html
+-rw-r--r--   0 kshalot    (501) staff       (20)      351 2023-06-04 18:06:42.000000 hdn-research-environment-2.3.0/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1163 2023-06-19 10:23:36.000000 hdn-research-environment-2.3.0/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     5942 2023-06-04 19:21:22.000000 hdn-research-environment-2.3.0/environment/templates/environment/manage_billing_account.html
+-rw-r--r--   0 kshalot    (501) staff       (20)      562 2023-06-05 16:41:15.000000 hdn-research-environment-2.3.0/environment/templates/environment/manage_shared_billing_invitation.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1648 2023-08-07 10:44:17.000000 hdn-research-environment-2.3.0/environment/templates/environment/research_environments.html
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.868198 hdn-research-environment-2.3.0/environment/templates/tag/
+-rw-r--r--   0 kshalot    (501) staff       (20)      241 2023-06-26 11:05:42.000000 hdn-research-environment-2.3.0/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1455 2023-08-08 08:00:13.000000 hdn-research-environment-2.3.0/environment/templates/tag/environment_modal_button.html
+-rw-r--r--   0 kshalot    (501) staff       (20)     1957 2023-07-04 10:33:07.000000 hdn-research-environment-2.3.0/environment/templates/tag/workspace_destroy_modal_button.html
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.868522 hdn-research-environment-2.3.0/environment/templatetags/
+-rw-r--r--   0 kshalot    (501) staff       (20)        0 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/templatetags/__init__.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     4470 2023-08-08 08:00:13.000000 hdn-research-environment-2.3.0/environment/templatetags/action_buttons.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      136 2023-07-04 09:26:42.000000 hdn-research-environment-2.3.0/environment/templatetags/environment_templatetags.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.869491 hdn-research-environment-2.3.0/environment/tests/
+-rw-r--r--   0 kshalot    (501) staff       (20)        0 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/environment/tests/__init__.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      645 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/tests/helpers.py
+-rw-r--r--   0 kshalot    (501) staff       (20)    12158 2023-05-26 12:39:45.000000 hdn-research-environment-2.3.0/environment/tests/mocks.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     3007 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/tests/test_decorators.py
+-rw-r--r--   0 kshalot    (501) staff       (20)    10682 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/tests/test_services.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     5327 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/tests/test_signals.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     2909 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/tests/test_utilities.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      640 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/tests/test_validators.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     3380 2023-08-07 10:44:38.000000 hdn-research-environment-2.3.0/environment/tests/test_views.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1631 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/urls.py
+-rw-r--r--   0 kshalot    (501) staff       (20)     1134 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/utilities.py
+-rw-r--r--   0 kshalot    (501) staff       (20)      235 2023-08-07 10:44:34.000000 hdn-research-environment-2.3.0/environment/validators.py
+-rw-r--r--   0 kshalot    (501) staff       (20)    16432 2023-08-08 08:00:13.000000 hdn-research-environment-2.3.0/environment/views.py
+drwxr-xr-x   0 kshalot    (501) staff       (20)        0 2023-08-08 08:10:33.870073 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/
+-rw-r--r--   0 kshalot    (501) staff       (20)      978 2023-08-08 08:10:33.000000 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 kshalot    (501) staff       (20)     3222 2023-08-08 08:10:33.000000 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 kshalot    (501) staff       (20)        1 2023-08-08 08:10:33.000000 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 kshalot    (501) staff       (20)       84 2023-08-08 08:10:33.000000 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 kshalot    (501) staff       (20)       12 2023-08-08 08:10:33.000000 hdn-research-environment-2.3.0/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 kshalot    (501) staff       (20)      109 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/pyproject.toml
+-rw-r--r--   0 kshalot    (501) staff       (20)     1056 2023-08-08 08:10:33.870468 hdn-research-environment-2.3.0/setup.cfg
+-rw-r--r--   0 kshalot    (501) staff       (20)       38 2023-04-25 08:09:06.000000 hdn-research-environment-2.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hdn-research-environment-2.2.0/LICENSE` & `hdn-research-environment-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/PKG-INFO` & `hdn-research-environment-2.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,7 +17,8 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
+License-File: LICENSE
```

### Comparing `hdn-research-environment-2.2.0/environment/api/v1/decorators.py` & `hdn-research-environment-2.3.0/environment/api/decorators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from typing import Callable
 from functools import wraps
-from requests import Request, Response, Session
+from typing import Callable
 
+import google.oauth2.id_token
 from django.conf import settings
+from requests import Request, Response, Session
+
+
+def _apply_api_credentials(request: Request, audience: str):
+    auth_request = google.auth.transport.requests.Request()
+    id_token = google.oauth2.id_token.fetch_id_token(auth_request, audience)
 
-from environment.api.v1.auth import apply_api_credentials
+    request.headers["Authorization"] = f"Bearer {id_token}"
 
 
 def api_request(
     request_creator_callable: Callable[..., Request],
 ) -> Callable:
-    api_url = settings.CLOUD_RESEARCH_ENVIRONMENTS_API_V1_URL
+    api_url = settings.CLOUD_RESEARCH_ENVIRONMENTS_API_URL
 
     @wraps(request_creator_callable)
     def wrapper(*args, **kwargs) -> Response:
         session = Session()
         request = request_creator_callable(*args, **kwargs)
         request.url = f"{api_url}{request.url}"
         prepped = request.prepare()
-        apply_api_credentials(prepped)
+        _apply_api_credentials(prepped, api_url)
 
         return session.send(prepped)
 
     return wrapper
```

### Comparing `hdn-research-environment-2.2.0/environment/constants.py` & `hdn-research-environment-2.3.0/environment/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from environment.entities import (
-    InstanceType,
-    Region,
-    GPUAcceleratorType,
-)
 from collections import namedtuple
 
+from environment.entities import GPUAcceleratorType, InstanceType, Region
+
 MAX_RUNNING_WORKSPACES = 4
 
 MAX_CPU_USAGE = 32
 
 PERSISTENT_DATA_DISK_NAME = "Persistent data disk 1GB"
 
-WorkspaceBillingInfo = namedtuple(
-    "WorkspaceBillingInfo", ["gcp_project_id", "billing_name"]
-)
-
 ProjectedWorkbenchCost = namedtuple("ProjectedWorkbenchCost", "resource cost")
 INSTANCE_PROJECTED_COSTS = {
     Region.US_CENTRAL: [
         ProjectedWorkbenchCost(*parameters)
         for parameters in [
             [InstanceType.N1_STANDARD_2.value, 0.09],
             [InstanceType.N1_STANDARD_4.value, 0.19],
@@ -87,13 +80,13 @@
     Region.NORTHAMERICA_NORTHEAST: ProjectedWorkbenchCost(
         PERSISTENT_DATA_DISK_NAME, 0.05
     ),
     Region.EUROPE_WEST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
     Region.AUSTRALIA_SOUTHEAST: ProjectedWorkbenchCost(PERSISTENT_DATA_DISK_NAME, 0.05),
 }
 
-INSTANCE_TYPE_SPECIFICATION = {
+MACHINE_TYPE_SPECIFICATION = {
     InstanceType.N1_STANDARD_2: "2 CPU, 7.5GB RAM",
     InstanceType.N1_STANDARD_4: "4 CPU, 15GB RAM",
     InstanceType.N1_STANDARD_8: "8 CPU, 30GB RAM",
     InstanceType.N1_STANDARD_16: "16 CPU, 60GB RAM",
 }
```

### Comparing `hdn-research-environment-2.2.0/environment/decorators.py` & `hdn-research-environment-2.3.0/environment/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from typing import Callable
 from functools import wraps
+from typing import Callable
 
-from django.shortcuts import redirect
+from django.db.models import Model
 from django.http import HttpRequest, HttpResponse
+from django.shortcuts import redirect
 from django.views.decorators.http import require_http_methods
-from django.db.models import Model
-
-from environment.utilities import (
-    user_has_cloud_identity,
-)
 
+from environment.utilities import user_has_cloud_identity
 
 View = Callable[[HttpRequest], HttpResponse]
 
 User = Model
 
 
 def _redirect_view_if_user(predicate: Callable[[User], bool], redirect_url: str):
```

### Comparing `hdn-research-environment-2.2.0/environment/entities.py` & `hdn-research-environment-2.3.0/environment/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Optional
 from dataclasses import dataclass
 from enum import Enum
+from typing import Optional
 
 
 class Region(Enum):
     US_CENTRAL = "us-central1"
     NORTHAMERICA_NORTHEAST = "northamerica-northeast1"
     EUROPE_WEST = "europe-west3"
     AUSTRALIA_SOUTHEAST = "australia-southeast1"
@@ -66,23 +66,26 @@
     INPROGRESS = "workspace-setup-inprogress"
     PENDING = "workspace-setup-pending"
     RETRYING = "workspace-setup-retrying"
 
 
 @dataclass
 class ResearchEnvironment:
-    id: str
-    group_granting_data_access: str
-    region: Region
-    type: EnvironmentType
-    instance_type: InstanceType
-    status: EnvironmentStatus
-    bucket_name: Optional[str]
+    gcp_identifier: str
+    dataset_identifier: str
     url: Optional[str]
     workspace_name: str
+    status: EnvironmentStatus
+    cpu: float
+    memory: float
+    region: Region
+    type: EnvironmentType
+    machine_type: Optional[str]
+    disk_size: Optional[int]
+    gpu_accelerator_type: Optional[str]
 
     @property
     def is_running(self):
         return self.status in [EnvironmentStatus.RUNNING, EnvironmentStatus.UPDATING]
 
     @property
     def is_paused(self):
@@ -99,19 +102,12 @@
         ]
 
     @property
     def is_active(self):
         return self.is_running or self.is_paused or self.is_in_progress
 
 
-@dataclass
+@dataclass(frozen=True, eq=True)
 class ResearchWorkspace:
-    user_id: str
     region: Region
     gcp_project_id: str
     gcp_billing_id: str
-    email_id: str
-    workspace_setup_status: WorkspaceStatus
-
-    @property
-    def setup_finished(self):
-        return self.workspace_setup_status == WorkspaceStatus.DONE
```

### Comparing `hdn-research-environment-2.2.0/environment/exceptions.py` & `hdn-research-environment-2.3.0/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/forms.py` & `hdn-research-environment-2.3.0/environment/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable
 
 from django import forms
 
-from environment.entities import ResearchWorkspace, InstanceType
-from environment.constants import INSTANCE_TYPE_SPECIFICATION
+from environment.constants import MACHINE_TYPE_SPECIFICATION
+from environment.entities import InstanceType, ResearchWorkspace
 
 
 class CloudIdentityPasswordForm(forms.Form):
     password = forms.CharField(widget=forms.PasswordInput())
     confirm_password = forms.CharField(widget=forms.PasswordInput())
     recovery_email = forms.EmailField(
         widget=forms.EmailInput(attrs={"class": "form-control"})
@@ -37,41 +37,41 @@
         self.fields["billing_account_id"].choices = [
             (billing_account["id"], billing_account["name"])
             for billing_account in billing_accounts_list
         ]
 
 
 class CreateResearchEnvironmentForm(forms.Form):
-    AVAILABLE_INSTANCE_TYPES = [
-        ("n1-standard-2", INSTANCE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_2]),
-        ("n1-standard-4", INSTANCE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_4]),
-        ("n1-standard-8", INSTANCE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_8]),
-        ("n1-standard-16", INSTANCE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_16]),
+    AVAILABLE_MACHINE_TYPES = [
+        ("n1-standard-2", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_2]),
+        ("n1-standard-4", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_4]),
+        ("n1-standard-8", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_8]),
+        ("n1-standard-16", MACHINE_TYPE_SPECIFICATION[InstanceType.N1_STANDARD_16]),
     ]
     AVAILABLE_ENVIRONMENT_TYPES = [
         ("jupyter", "Jupyter"),
         ("rstudio", "RStudio"),
     ]
     AVAILABLE_GPU_ACCELERATOR_TYPES = [
         ("", "Machine without GPU attached"),
         ("NVIDIA_TESLA_T4", "Nvidia Tesla T4 (16 GB GDDR6)"),
     ]
 
-    workspace_id = forms.ChoiceField(label="Workspace")
-    instance_type = forms.ChoiceField(
+    workspace = forms.ChoiceField(label="Workspace")
+    machine_type = forms.ChoiceField(
         label="Instance type",
-        choices=AVAILABLE_INSTANCE_TYPES,
+        choices=AVAILABLE_MACHINE_TYPES,
         widget=forms.Select(attrs={"class": "form-control"}),
     )
     environment_type = forms.ChoiceField(
         label="Environment type",
         choices=AVAILABLE_ENVIRONMENT_TYPES,
         widget=forms.RadioSelect(attrs={"class": "environment-type"}),
     )
-    persistent_disk = forms.IntegerField(
+    disk_size = forms.IntegerField(
         label="Persistent data disk size [GB]",
         widget=forms.NumberInput(
             attrs={"class": "form-control", "min": 0, "max": 64000}
         ),
         initial=0,
     )
     gpu_accelerator = forms.ChoiceField(
@@ -79,20 +79,18 @@
         choices=AVAILABLE_GPU_ACCELERATOR_TYPES,
         widget=forms.Select(attrs={"class": "form-control"}),
         required=False,
     )
 
     def __init__(self, *args, workspace_list: Iterable[ResearchWorkspace], **kwargs):
         super(CreateResearchEnvironmentForm, self).__init__(*args, **kwargs)
-        self.fields["workspace_id"].choices = [
-            (workspace.gcp_project_id, workspace.gcp_project_id)
-            for workspace in workspace_list
+        self.fields["workspace"].choices = [
+            (workspace, workspace.gcp_project_id) for workspace in workspace_list
         ]
 
     def clean_gpu_accelerator(self):
         gpu_accelerator = self.cleaned_data.get("gpu_accelerator")
-        gpu_accelerator = None if gpu_accelerator == "" else gpu_accelerator
-        return gpu_accelerator
+        return None if gpu_accelerator == "" else gpu_accelerator
 
 
 class ShareBillingAccountForm(forms.Form):
     user_email = forms.EmailField(label="User E-Mail")
```

### Comparing `hdn-research-environment-2.2.0/environment/mailers.py` & `hdn-research-environment-2.3.0/environment/mailers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Iterable
 
 from django.apps import apps
-from django.db.models import Model
 from django.conf import settings
-from django.urls import reverse
-from django.template import loader
 from django.core.mail import send_mail
+from django.db.models import Model
+from django.template import loader
+from django.urls import reverse
 from django.utils.html import strip_tags
 
 from environment.models import BillingAccountSharingInvite
 
-
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 User = Model
 
 
 def send_billing_sharing_confirmation(
     site_domain: str, invite: BillingAccountSharingInvite
```

### Comparing `hdn-research-environment-2.2.0/environment/migrations/0001_initial.py` & `hdn-research-environment-2.3.0/environment/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by Django 2.2.24 on 2022-02-02 09:57
 
-from django.conf import settings
 import django.core.validators
-from django.db import migrations, models
 import django.db.models.deletion
+from django.conf import settings
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
```

### Comparing `hdn-research-environment-2.2.0/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-2.3.0/environment/migrations/0002_billingsetup.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 2.2.24 on 2022-02-09 15:23
 
 import django.core.validators
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("environment", "0001_initial"),
     ]
```

### Comparing `hdn-research-environment-2.2.0/environment/migrations/0005_workflow.py` & `hdn-research-environment-2.3.0/environment/migrations/0005_workflow.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 2.2.27 on 2022-03-28 13:33
 
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("project", "0001_initial"),
         ("environment", "0004_auto_20220309_0330"),
```

### Comparing `hdn-research-environment-2.2.0/environment/migrations/0007_billingaccountsharinginvite.py` & `hdn-research-environment-2.3.0/environment/migrations/0007_billingaccountsharinginvite.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by Django 4.1.7 on 2023-05-25 19:07
 
-from django.conf import settings
+import uuid
+
 import django.core.validators
-from django.db import migrations, models
 import django.db.models.deletion
-import uuid
+from django.conf import settings
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("environment", "0006_delete_billingsetup"),
     ]
```

### Comparing `hdn-research-environment-2.2.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py` & `hdn-research-environment-2.3.0/environment/migrations/0010_alter_workflow_project_alter_workflow_type_and_more.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 4.1.5 on 2023-05-30 13:49
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("project", "0067_alter_activeproject_core_project_and_more"),
         ("environment", "0009_billingaccountsharinginvite_is_revoked"),
     ]
```

### Comparing `hdn-research-environment-2.2.0/environment/models.py` & `hdn-research-environment-2.3.0/environment/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 
-from django.db import models
 from django.core.validators import EmailValidator
+from django.db import models
 
-from environment.validators import gcp_billing_account_id_validator
 from environment.managers import WorkflowManager
+from environment.validators import gcp_billing_account_id_validator
 
 
 class CloudIdentity(models.Model):
     user = models.OneToOneField(
         "user.User", related_name="cloud_identity", on_delete=models.CASCADE
     )
     gcp_user_id = models.CharField(max_length=50, unique=True)
```

### Comparing `hdn-research-environment-2.2.0/environment/services.py` & `hdn-research-environment-2.3.0/environment/services.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,40 @@
-from typing import Tuple, Iterable, Optional, Dict
 from collections import defaultdict
+from typing import Dict, Iterable, Optional, Tuple
 
-from django.db.models import Model, Q
-from django.contrib.sites.shortcuts import get_current_site
 from django.apps import apps
+from django.contrib.sites.shortcuts import get_current_site
+from django.db.models import Model, Q
 from google.cloud.workflows import executions_v1beta
 from google.cloud.workflows.executions_v1beta.types import executions
 
+from environment import api
 import environment.constants as constants
 import environment.mailers as mailers
-import environment.api.v1 as api_v1
-import environment.api.v2 as api_v2
-from environment.models import CloudIdentity, Workflow, BillingAccountSharingInvite
+from environment.deserializers import (
+    deserialize_research_environments,
+    deserialize_workspaces,
+)
+from environment.entities import ResearchEnvironment, ResearchWorkspace
 from environment.exceptions import (
-    IdentityProvisioningFailed,
-    StopEnvironmentFailed,
-    StartEnvironmentFailed,
-    DeleteEnvironmentFailed,
-    ChangeEnvironmentInstanceTypeFailed,
-    BillingSharingFailed,
     BillingAccessRevokationFailed,
+    BillingSharingFailed,
+    ChangeEnvironmentInstanceTypeFailed,
+    CreateWorkspaceFailed,
+    DeleteEnvironmentFailed,
+    DeleteWorkspaceFailed,
     EnvironmentCreationFailed,
     GetAvailableEnvironmentsFailed,
-    GetWorkspaceDetailsFailed,
     GetBillingAccountsListFailed,
-    GetWorkspacesListFailed,
-    CreateWorkspaceFailed,
-    DeleteWorkspaceFailed,
-)
-from environment.deserializers import (
-    deserialize_research_environments,
-    deserialize_workspace_details,
-    deserialize_workspaces,
-)
-from environment.entities import (
-    ResearchEnvironment,
-    InstanceType,
-    Region,
-    ResearchWorkspace,
+    IdentityProvisioningFailed,
+    StartEnvironmentFailed,
+    StopEnvironmentFailed,
 )
-from environment.utilities import left_join_iterators, inner_join_iterators
-
+from environment.models import BillingAccountSharingInvite, CloudIdentity, Workflow
+from environment.utilities import inner_join_iterators, left_join_iterators
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 User = Model
 
 
@@ -60,22 +50,22 @@
     # Potential collisions may happen:
     # { slug: some-project, version: 1.1.0 } => someproject110
     # { slug: some-project1, version: 1.0 }  => someproject110
     return "".join(c for c in project.slug + project.version if c.isalnum())
 
 
 def _environment_data_group(environment: ResearchEnvironment) -> str:
-    return environment.group_granting_data_access
+    return environment.dataset_identifier
 
 
 def create_cloud_identity(
     user: User, password: str, recovery_email: str
 ) -> Tuple[str, CloudIdentity]:
     gcp_user_id = user.username
-    response = api_v2.create_cloud_identity(
+    response = api.create_cloud_identity(
         gcp_user_id,
         user.profile.first_names,
         user.profile.last_name,
         password,
         recovery_email,
     )
     if not response.ok:
@@ -88,25 +78,37 @@
         gcp_user_id=gcp_user_id,
         email=body["primary_email"],
     )
     return identity
 
 
 def get_billing_accounts_list(user: User):
-    response = api_v2.list_billing_accounts(user.cloud_identity.email)
+    response = api.list_billing_accounts(user.cloud_identity.email)
     if not response.ok:
         error_message = None
         try:
             error_message = response.json()
         finally:
             raise GetBillingAccountsListFailed(error_message)
 
     return response.json()
 
 
+def is_billing_account_owner(user: User, billing_account_id: str):
+    billing_account_list = get_billing_accounts_list(user)
+    for billing_account in billing_account_list:
+        if (
+            billing_account["id"] == billing_account_id
+            and billing_account["is_owner"] is True
+        ):
+            return True
+
+    return False
+
+
 def get_owned_shares_of_billing_account(owner: User, billing_account_id: str):
     return owner.owner_billingaccountsharinginvite_set.filter(
         billing_account_id=billing_account_id, is_revoked=False
     )
 
 
 def invite_user_to_shared_billing_account(
@@ -129,15 +131,15 @@
     invite.user = user
     invite.save()
 
     return invite
 
 
 def share_billing_account(owner_email: str, user_email: str, billing_account_id: str):
-    response = api_v2.share_billing_account(
+    response = api.share_billing_account(
         owner_email=owner_email,
         user_email=user_email,
         billing_account_id=billing_account_id,
     )
     if not response.ok:
         error_message = response.json()
         raise BillingSharingFailed(error_message)
@@ -157,181 +159,131 @@
 def _revoke_consumed_billing_account_access(
     billing_account_sharing_invite: BillingAccountSharingInvite,
 ):
     owner_email = billing_account_sharing_invite.owner.cloud_identity.email
     user_email = billing_account_sharing_invite.user.cloud_identity.email
     billing_account_id = billing_account_sharing_invite.billing_account_id
 
-    response = api_v2.revoke_billing_account_access(
+    response = api.revoke_billing_account_access(
         owner_email=owner_email,
         user_email=user_email,
         billing_account_id=billing_account_id,
     )
     if not response.ok:
         error_message = response.json()
         raise BillingAccessRevokationFailed(error_message)
 
 
 def create_workspace(user: User, billing_account_id: str, region: str):
-    response = api_v2.create_workspace(
+    response = api.create_workspace(
         email=user.cloud_identity.email,
         billing_account_id=billing_account_id,
         region=region,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise CreateWorkspaceFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        type=Workflow.WORKSPACE_CREATE,
-    )
-
 
-def delete_workspace(user: User, gcp_project_id: str):
-    response = api_v2.delete_workspace(
+def delete_workspace(
+    user: User, billing_account_id: str, region: str, gcp_project_id: str
+):
+    response = api.delete_workspace(
         email=user.cloud_identity.email,
         gcp_project_id=gcp_project_id,
+        billing_account_id=billing_account_id,
+        region=region,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise DeleteWorkspaceFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        type=Workflow.WORKSPACE_DESTROY,
-        workspace_name=gcp_project_id,
-    )
-
 
 def _create_workbench_kwargs(
     user: User,
     project: PublishedProject,
-    workspace_name: str,
-    instance_type: str,
-    environment_type: str,
-    persistent_disk: int,
-    gpu_accelerator: Optional[str] = None,
+    workspace_project_id: str,
+    machine_type: str,
+    region: str,
+    workbench_type: str,
+    disk_size: int,
+    gpu_accelerator_type: Optional[str] = None,
 ) -> dict:
-    gcp_user_id = user.cloud_identity.gcp_user_id
+    user_email = user.cloud_identity.email
 
     common = {
-        "gcp_user_id": gcp_user_id,
-        "gcp_project_id": workspace_name,
-        "environment_type": environment_type,
-        "instance_type": instance_type,
-        "group_granting_data_access": _project_data_group(project),
-        "persistent_disk": str(persistent_disk),
+        "user_email": user_email,
+        "workspace_project_id": workspace_project_id,
+        "workbench_type": workbench_type,
+        "machine_type": machine_type,
+        "region": region,
+        "dataset_identifier": _project_data_group(project),
+        "disk_size": disk_size,
         "bucket_name": project.project_file_root(),
     }
-    if environment_type == "jupyter":
-        vm_image = (
-            "common-cu110-notebooks"
-            if gpu_accelerator
-            else "r-4-2-cpu-experimental-notebooks"
-        )
+    if workbench_type == "jupyter":
         jupyter_kwargs = {
-            "vm_image": vm_image,
-            "gpu_accelerator": gpu_accelerator,
+            "gpu_accelerator_type": gpu_accelerator_type,
         }
         return {**common, **jupyter_kwargs}
     else:
         return common
 
 
 def create_research_environment(
     user: User,
     project: PublishedProject,
-    workspace_name: str,
-    instance_type: str,
-    environment_type: str,
-    persistent_disk: int,
-    gpu_accelerator: Optional[str] = None,
+    workspace_project_id: str,
+    machine_type: str,
+    region: str,
+    workbench_type: str,
+    disk_size: int,
+    gpu_accelerator_type: Optional[str] = None,
 ) -> str:
     kwargs = _create_workbench_kwargs(
         user,
         project,
-        workspace_name,
-        instance_type,
-        environment_type,
-        persistent_disk,
-        gpu_accelerator,
+        workspace_project_id,
+        machine_type,
+        region,
+        workbench_type,
+        disk_size,
+        gpu_accelerator_type,
     )
-    response = api_v1.create_workbench(**kwargs)
+    response = api.create_workbench(**kwargs)
     if not response.ok:
         error_message = response.json()[
             "error"
         ]  # TODO: Check all uses of "error"/"message"
         raise EnvironmentCreationFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        project_id=project.pk,
-        type=Workflow.CREATE,
-        workspace_name=workspace_name,
-    )
-
     return response.json()
 
 
-def get_workspace_details(user: User, region: Region) -> ResearchWorkspace:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.get_workspace_details(
-        gcp_user_id=gcp_user_id,
-        region=region.value,
-    )
-    if not response.ok:
-        error_message = response.json()["error"]
-        raise GetWorkspaceDetailsFailed(error_message)
-
-    research_workspace = deserialize_workspace_details(response.json())
-    return research_workspace
-
-
-def is_user_workspace_setup_done(user: User) -> bool:
-    try:
-        workspace = get_workspace_details(user, Region(DEFAULT_REGION))
-        return workspace.setup_finished
-    except GetWorkspaceDetailsFailed:
-        return False
-
-
-def mark_user_workspace_setup_as_done(user: User):
-    cloud_identity = user.cloud_identity
-    cloud_identity.initial_workspace_setup_done = True
-    cloud_identity.save()
-
-
 def get_available_projects(user: User) -> Iterable[PublishedProject]:
     return PublishedProject.objects.accessible_by(user).prefetch_related("workflows")
 
 
 def _get_projects_for_environments(
     environments: Iterable[ResearchEnvironment],
 ) -> Iterable[PublishedProject]:
-    group_granting_data_accesses = list(map(_environment_data_group, environments))
+    dataset_identifiers = list(map(_environment_data_group, environments))
     # FIXME: Given the fact that the groups are generated automatically in a non-reversible way,
     # the only way to match the projects to their environments is to fetch all the records and
     # calculate the group name for each of them.
     return [
         project
         for project in PublishedProject.objects.all()
-        if _project_data_group(project) in group_granting_data_accesses
+        if _project_data_group(project) in dataset_identifiers
     ]
 
 
 def get_active_environments(user: User) -> Iterable[ResearchEnvironment]:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.get_workspace_list(gcp_user_id)
+    email = user.cloud_identity.email
+    response = api.get_workspace_list(email)
     if not response.ok:
         error_message = response.json()["error"]
         raise GetAvailableEnvironmentsFailed(error_message)
     all_environments = deserialize_research_environments(response.json())
     return [environment for environment in all_environments if environment.is_active]
 
 
@@ -399,22 +351,18 @@
 
 
 def sort_environments_per_workspace(
     environment_project_workflow_triplets: Iterable[
         Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]
     ],
     workspaces: Iterable[ResearchWorkspace],
-    billing_accounts_list: Iterable,
 ) -> Dict[
-    constants.WorkspaceBillingInfo,
+    ResearchWorkspace,
     Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]],
 ]:
-    billing_id_mapping = match_workspace_with_billing_id(
-        workspaces, billing_accounts_list
-    )
     sorted_environments_project_workflow_triplets = defaultdict(
         list,
         {workspace.gcp_project_id: [] for workspace in workspaces},
     )
     for environment, project, workflows in environment_project_workflow_triplets:
         if environment:
             sorted_environments_project_workflow_triplets[
@@ -422,18 +370,17 @@
             ].append((environment, project, workflows))
         else:
             sorted_environments_project_workflow_triplets[
                 workflows.last().workspace_name
             ].append((environment, project, workflows))
 
     sorted_environments_project_workflow_triplets_with_billing_info = {
-        constants.WorkspaceBillingInfo(
-            workspace.gcp_project_id,
-            billing_id_mapping[workspace.gcp_billing_id],
-        ): sorted_environments_project_workflow_triplets[workspace.gcp_project_id]
+        workspace: sorted_environments_project_workflow_triplets[
+            workspace.gcp_project_id
+        ]
         for workspace in workspaces
     }
     return sorted_environments_project_workflow_triplets_with_billing_info
 
 
 def match_workspace_with_billing_id(
     workspaces: Iterable[ResearchWorkspace], billing_accounts_list: Iterable
@@ -444,149 +391,97 @@
     for billing_account in billing_accounts_list:
         if billing_account["id"] in billing_id_mapping:
             billing_id_mapping[billing_account["id"]] = billing_account["name"]
     return billing_id_mapping
 
 
 def get_workspaces_list(user: User) -> Iterable[ResearchWorkspace]:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.get_workspace_list(gcp_user_id)
-    if not response.ok:
-        error_message = response.json()["error"]
-        raise GetWorkspacesListFailed(error_message)
+    email = user.cloud_identity.email
+    response = api.get_workspace_list(email)
     return deserialize_workspaces(response.json())
 
 
 def stop_running_environment(
-    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
+    workbench_type: str,
+    workbench_resource_id: str,
+    user_email: str,
+    workspace_project_id: str,
 ) -> str:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.stop_workbench(
-        gcp_user_id=gcp_user_id,
-        workbench_id=workbench_id,
-        region=region.value,
-        gcp_project_id=gcp_project_id,
+    response = api.stop_workbench(
+        workbench_type=workbench_type,
+        workbench_resource_id=workbench_resource_id,
+        user_email=user_email,
+        workspace_project_id=workspace_project_id,
     )
     if not response.ok:
         error_message = response.json()["error"]
         raise StopEnvironmentFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        project_id=project_id,
-        type=Workflow.PAUSE,
-        workspace_name=gcp_project_id,
-    )
-
     return response.json()
 
 
 def start_stopped_environment(
-    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
+    workbench_type: str,
+    workbench_resource_id: str,
+    user_email: str,
+    workspace_project_id: str,
 ) -> str:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.start_workbench(
-        gcp_user_id=gcp_user_id,
-        workbench_id=workbench_id,
-        region=region.value,
-        gcp_project_id=gcp_project_id,
+    response = api.start_workbench(
+        workbench_type=workbench_type,
+        workbench_resource_id=workbench_resource_id,
+        user_email=user_email,
+        workspace_project_id=workspace_project_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise StartEnvironmentFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        project_id=project_id,
-        type=Workflow.START,
-        workspace_name=gcp_project_id,
-    )
-
     return response.json()
 
 
-def change_environment_instance_type(
-    user: User,
-    project_id: str,
-    workbench_id: str,
-    region: Region,
-    gcp_project_id: str,
-    new_instance_type: InstanceType,
+def change_environment_machine_type(
+    user_email: str,
+    workspace_project_id: str,
+    machine_type: str,
+    workbench_type: str,
+    workbench_resource_id: str,
 ) -> str:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.change_workbench_instance_type(
-        gcp_user_id=gcp_user_id,
-        workbench_id=workbench_id,
-        region=region.value,
-        new_instance_type=new_instance_type.value,
-        gcp_project_id=gcp_project_id,
+    response = api.change_workbench_machine_type(
+        workbench_type=workbench_type,
+        machine_type=machine_type,
+        user_email=user_email,
+        workspace_project_id=workspace_project_id,
+        workbench_resource_id=workbench_resource_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise ChangeEnvironmentInstanceTypeFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        project_id=project_id,
-        type=Workflow.CHANGE,
-        workspace_name=gcp_project_id,
-    )
-
     return response.json()
 
 
 def delete_environment(
-    user: User, project_id: str, workbench_id: str, region: Region, gcp_project_id: str
+    user_email: str,
+    workspace_project_id: str,
+    workbench_type: str,
+    workbench_resource_id: str,
 ) -> str:
-    gcp_user_id = user.cloud_identity.gcp_user_id
-    response = api_v1.delete_workbench(
-        gcp_user_id=gcp_user_id,
-        workbench_id=workbench_id,
-        region=region.value,
-        gcp_project_id=gcp_project_id,
+    response = api.delete_workbench(
+        workbench_type=workbench_type,
+        user_email=user_email,
+        workspace_project_id=workspace_project_id,
+        workbench_resource_id=workbench_resource_id,
     )
     if not response.ok:
         error_message = response.json()["message"]
         raise DeleteEnvironmentFailed(error_message)
 
-    execution_resource_name = response.json()["execution-name"]
-    persist_workflow(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        project_id=project_id,
-        type=Workflow.DESTROY,
-        workspace_name=gcp_project_id,
-    )
-
     return response.json()
 
 
-def persist_workflow(
-    user: User,
-    execution_resource_name: str,
-    type: int,
-    project_id: Optional[int] = None,
-    workspace_name: Optional[str] = None,
-) -> Workflow:
-    return Workflow.objects.create(
-        user=user,
-        execution_resource_name=execution_resource_name,
-        workspace_name=workspace_name,
-        project_id=project_id,
-        type=type,
-        status=Workflow.INPROGRESS,
-    )
-
-
 def get_execution_state(execution_resource_name) -> executions.Execution.State:
     client = executions_v1beta.ExecutionsClient()
     execution = client.get_execution(request={"name": execution_resource_name})
     return execution.state
 
 
 def mark_workflow_as_finished(
@@ -599,15 +494,15 @@
         workflow.status = Workflow.FAILED
 
     workflow.save()
 
 
 def cpu_usage(value, user) -> int:
     running_environments = get_active_environments(user)
-    cpu = sum(environment.instance_type.cpus() for environment in running_environments)
+    cpu = sum(environment.machine_type.cpus() for environment in running_environments)
     return value + cpu
 
 
 def exceeded_quotas(user) -> Iterable[str]:
     quotas_exceeded = []
     # Check if user has exceeded MAX_RUNNING_ENVIRONMENTS
     running_workspaces = get_workspaces_list(user)
```

### Comparing `hdn-research-environment-2.2.0/environment/signals.py` & `hdn-research-environment-2.3.0/environment/signals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from typing import Iterable
 from datetime import datetime
+from typing import Iterable
 
-from django.dispatch import receiver
 from django.apps import apps
 from django.contrib.auth import get_user_model
-from django.utils import timezone
 from django.db.models.signals import post_init, post_save
+from django.dispatch import receiver
+from django.utils import timezone
 
+from environment.models import BillingAccountSharingInvite, CloudIdentity
 from environment.tasks import (
+    give_user_permission_to_access_billing_account,
     stop_environments_with_expired_access,
     stop_event_participants_environments_with_expired_access,
 )
-from environment.models import CloudIdentity, BillingAccountSharingInvite
-from environment.tasks import give_user_permission_to_access_billing_account
-
 
 User = get_user_model()
 
 Training = apps.get_model("user", "Training")
 
 DataAccessRequest = apps.get_model("project", "DataAccessRequest")
```

### Comparing `hdn-research-environment-2.2.0/environment/static/environment/css/environment-base.css` & `hdn-research-environment-2.3.0/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/static/environment/js/cookie.js` & `hdn-research-environment-2.3.0/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-2.3.0/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-2.3.0/environment/static/environment/js/pricing_change.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 $(function() {
     // var current_region = $("#id_region").val()
     // HACK: Use the workspace's region
     const current_region = "us-central1"
-    var current_instance_type = $("#id_instance_type").val()
-    var current_instance_price = $(`#${current_region}-${current_instance_type}`)
-    var current_data_amount = $("#id_persistent_disk").val()
+    var current_machine_type = $("#id_machine_type").val()
+    var current_instance_price = $(`#${current_region}-${current_machine_type}`)
+    var current_data_amount = $("#id_disk_size").val()
     var current_data_price = $(`div[id*=${current_region}-Persistent]`)
 
     current_instance_price.show()
     current_data_price.show()
     $("#instance_total_cost span").text(current_instance_price.attr("data-cost"))
     $("#data_total_cost span").text((parseInt(current_data_amount) * current_data_price.attr("data-cost")).toFixed(2))
 
     function change_instance_shown_pricing() {
         // var current_region = $("#id_region").val()
-        var current_instance_type = $("#id_instance_type").val()
-        var current_instance_price = $(`#${current_region}-${current_instance_type}`)
+        var current_machine_type = $("#id_machine_type").val()
+        var current_instance_price = $(`#${current_region}-${current_machine_type}`)
         $("div.instance-costs").hide()
         current_instance_price.show()
     };
 
     function change_gpu_shown_pricing() {
         var current_gpu_accelerator = $("#id_gpu_accelerator").val()
         // var current_region = $("#id_region").val()
@@ -29,24 +29,24 @@
             $("#gpu_accelerator_costs").show()
             $(`#${current_region}-${current_gpu_accelerator}`).show()
         };
     };
 
     function change_data_storage_costs_shown_pricing() {
         // var current_region = $("#id_region").val()
-        var current_data_amount = $("#id_persistent_disk").val()
+        var current_data_amount = $("#id_disk_size").val()
         $("div.data-storage-costs").hide()
         $(`div[id*=${current_region}-Persistent]`).show()
         $("#data_total_cost span").text((parseInt(current_data_amount) * current_data_price.attr("data-cost")).toFixed(2))
     }
 
-    $("#id_instance_type, #id_region, #id_gpu_accelerator").on("change", function() {
+    $("#id_machine_type, #id_region, #id_gpu_accelerator").on("change", function() {
         // var current_region = $("#id_region").val()
-        var current_instance_type = $("#id_instance_type").val()
-        var current_instance_price = $(`#${current_region}-${current_instance_type}`).attr("data-cost")
+        var current_machine_type = $("#id_machine_type").val()
+        var current_instance_price = $(`#${current_region}-${current_machine_type}`).attr("data-cost")
         var current_gpu_accelerator = $("#id_gpu_accelerator").val()
         var current_gpu_accelerator_price = $(`#${current_region}-${current_gpu_accelerator}`).attr("data-cost")
         var instance_total_cost = parseFloat(current_instance_price) + parseFloat(current_gpu_accelerator_price)
 
         if ($("#id_gpu_accelerator").val()) {
             $("#instance_total_cost span").text(instance_total_cost.toFixed(2))
         } else {
@@ -56,20 +56,20 @@
 
     $("#id_region").on("change", function() {
         change_instance_shown_pricing();
         change_gpu_shown_pricing();
         change_data_storage_costs_shown_pricing();
     });
 
-    $("#id_instance_type").on("change", function() {
+    $("#id_machine_type").on("change", function() {
         change_instance_shown_pricing();
     });
 
     $("#id_gpu_accelerator").on("change", function() {
         change_gpu_shown_pricing();
     });
 
-    $("#id_persistent_disk").on("change", function() {
+    $("#id_disk_size").on("change", function() {
         change_data_storage_costs_shown_pricing();
     });
 
 });
```

### Comparing `hdn-research-environment-2.2.0/environment/tasks.py` & `hdn-research-environment-2.3.0/environment/tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-from typing import Iterable
 from datetime import timedelta
+from typing import Iterable
 
 from background_task import background
-from django.contrib.auth import get_user_model
 from django.apps import apps
+from django.contrib.auth import get_user_model
 from django.db import transaction
 from django.utils import timezone
 
+from environment.mailers import send_environment_access_expired
+from environment.models import BillingAccountSharingInvite
 from environment.services import (
-    get_environment_project_pairs_with_expired_access,
-    stop_running_environment,
     delete_environment,
+    get_environment_project_pairs_with_expired_access,
     share_billing_account,
+    stop_running_environment,
 )
-from environment.mailers import send_environment_access_expired
-from environment.models import BillingAccountSharingInvite
-
 
 User = get_user_model()
 
 Event = apps.get_model("events", "Event")
 
 
 def _expired_environment_termination_schedule():
@@ -49,15 +48,18 @@
     user = User.objects.select_related("cloud_identity").get(pk=user_id)
 
     expired_pairs = get_environment_project_pairs_with_expired_access(user)
     environments, projects = zip(*expired_pairs)
     for environment in environments:
         if environment.is_running:
             stop_running_environment(
-                user, environment.id, environment.region, environment.workspace_name
+                workbench_type=environment.type,
+                workbench_resource_id=environment.instance_name,
+                user_email=user.cloud_identity.email,
+                workspace_project_id=environment.workspace_name,
             )
     send_environment_access_expired(user, projects)
     if len(environments) > 0:
         environment_ids = [environment.id for environment in environments]
         terminate_environments_if_access_still_expired(
             user_id,
             environment_ids,
@@ -67,12 +69,21 @@
 
 @background
 def terminate_environments_if_access_still_expired(
     user_id: int, previously_stopped_environment_ids: Iterable[str]
 ):
     user = User.objects.get(pk=user_id)
     expired_pairs = get_environment_project_pairs_with_expired_access(user)
-    for environment, _ in expired_pairs:
+    for environment, project in expired_pairs:
         if environment.id in previously_stopped_environment_ids:
             delete_environment(
-                user, environment.id, environment.region, environment.workspace_name
+                user_email=user.cloud_identity.email,
+                dataset_identifier=environment.dataset_identifier,
+                workspace_project_id=environment.workspace_name,
+                region=environment.region.value,
+                bucket_name=project.project_file_root(),
+                machine_type=environment.machine_type,
+                workbench_type=environment.type.value,
+                disk_size=environment.disk_size,
+                gpu_accelerator_type=environment.gpu_accelerator_type,
+                workbench_resource_id=environment.gcp_identifier,
             )
```

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-2.3.0/environment/templates/environment/_available_environments_list.html`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                             {{ workspace.gcp_project_id }}
                         </h6>
                         <small>
                             <span class="d-inline font-weight-bold" style="padding-top: 0.375rem;">
                                 Billing Account:
                             </span>
                             <span class="d-inline font-weight-normal">
-                                {{ workspace.billing_name }}
+                                {{ workspace.gcp_billing_id }}
                             </span>
                         </small>
                     </div>
                     {% workspace_destroy_modal_button workspace=workspace environments_project_workflow_triplets=environments_project_workflow_triplets %}
                 </div>
             </div>
 
@@ -79,15 +79,16 @@
                                         <a href="{% url 'published_project' project.slug project.version %}" target="_blank">
                                             {{ project }}
                                         </a>
                                     </div>
                                     <div class="col-md-3">
                                         <small>
                                             <i>Environment type:</i> {{ environment.type.value|capfirst }}<br>
-                                            <i>Instance type:</i> {{ environment.instance_type.value }}<br>
+                                            <i>CPU:</i> {{ environment.cpu }}<br>
+                                            <i>Memory:</i> {{ environment.memory }}<br>
                                             <i>Region:</i> {{ environment.region.value }}
                                         </small>
                                     </div>
                                     <div class="col-md-2">
                                         {% if workflows.exists %}
                                             {{ workflows.first.get_type_display }}
                                         {% else %}
```

#### html2text {}

```diff
@@ -13,24 +13,25 @@
 {{ heading }}">
 {% if workflow.type == 5 %} Creating Workspace... {% else %} Destroying {
 { workflow.workspace_name }}... {% endif %}
 Loading...
 {% endfor %} {% for workspace, environments_project_workflow_triplets in
 workspace_project_environment_workflow_triplets_dict.items %}
 * {{ workspace.gcp_project_id }} *
- Billing Account:   {{ workspace.billing_name }}
+ Billing Account:   {{ workspace.gcp_billing_id }}
 {% workspace_destroy_modal_button workspace=workspace
 environments_project_workflow_triplets=environments_project_workflow_triplets
 %}
 {% if environments_project_workflow_triplets|length %}
     * {% for environment, project, workflows in
       environments_project_workflow_triplets %}
     * {{_project_}}
       Environment type: {{ environment.type.value|capfirst }}
-      Instance type: {{ environment.instance_type.value }}
+      CPU: {{ environment.cpu }}
+      Memory: {{ environment.memory }}
       Region: {{ environment.region.value }}
       {% if workflows.exists %} {{ workflows.first.get_type_display }} {% else
       %} {{ environment.status.value|capfirst }} {% endif %}
       {% if workflows.exists %}
       Loading...
       {% elif environment.is_running or environment.is_paused %} {% if
       environment.is_running %} Open {% environment_modal_button
```

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-2.3.0/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/_billing_accounts_list.html` & `hdn-research-environment-2.3.0/environment/templates/environment/_billing_accounts_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/_environment_tabs.html` & `hdn-research-environment-2.3.0/environment/templates/environment/_environment_tabs.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-2.3.0/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-2.3.0/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/create_workspace.html` & `hdn-research-environment-2.3.0/environment/templates/environment/create_workspace.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-2.3.0/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/manage_billing_account.html` & `hdn-research-environment-2.3.0/environment/templates/environment/manage_billing_account.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/manage_shared_billing_invitation.html` & `hdn-research-environment-2.3.0/environment/templates/environment/manage_shared_billing_invitation.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templates/environment/research_environments.html` & `hdn-research-environment-2.3.0/environment/templates/environment/research_environments.html`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         let data = request_data;
         if (button_type === "update") {
             const instance = $("#form-select option:selected").val();
             if (instance === "") return;
 
             data = JSON.parse(data);
-            data["instance_type"] = instance;
+            data["machine_type"] = instance;
             data = JSON.stringify(data);
         }
         fetch(url, {
             method: http_method,
             body: data,
             credentials: "same-origin",
             headers: {
```

### Comparing `hdn-research-environment-2.2.0/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-2.3.0/environment/templates/tag/environment_modal_button.html`

 * *Files 12% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         <button type="button" class="close" data-dismiss="modal" aria-label="Close">
           <span aria-hidden="true">&times;</span>
         </button>
       </div>
       <div class="modal-body">
         {% if instances_dict != None %}
             <select class="form-select" id="form-select" size="5" aria-label="size 5 select example">
-              {% for instance_type, instance_specification in instances_dict.items %}
-                <option value="{{ instance_type.value }}">{{ instance_specification }}</option>
+              {% for machine_type, instance_specification in instances_dict.items %}
+                <option value="{{ machine_type.value }}">{{ instance_specification }}</option>
               {% endfor %}
             </select>
         {% else %}
             <p>{{ modal_body }}</p>
         {% endif %}
       </div>
       <div class="modal-footer">
         <button type="button" class="btn btn-secondary inside-modal-button" data-dismiss="modal">Close</button>
-        {% environment_action_button button_type=action_button_type environment=environment project=project %}
+        {% environment_action_button button_type=action_button_type environment=environment %}
       </div>
     </div>
   </div>
 </div>
```

### Comparing `hdn-research-environment-2.2.0/environment/templates/tag/workspace_destroy_modal_button.html` & `hdn-research-environment-2.3.0/environment/templates/tag/workspace_destroy_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/templatetags/action_buttons.py` & `hdn-research-environment-2.3.0/environment/templatetags/action_buttons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 from typing import Iterable, Tuple
 
 from django import template
+from django.apps import apps
 from django.urls import reverse
-from django.db.models import Model
 
+from environment.constants import MACHINE_TYPE_SPECIFICATION
 from environment.entities import ResearchEnvironment, ResearchWorkspace
-from environment.constants import INSTANCE_TYPE_SPECIFICATION
 from environment.models import Workflow
 
-
-PublishedProject = Model
+PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 register = template.Library()
 
 
 button_types = {
     "pause": {
@@ -28,15 +27,15 @@
         "http_method": "PATCH",
         "url_name": "start_stopped_environment",
         "button_class": "btn btn-primary m-1",
     },
     "update": {
         "button_text": "Save Instance",
         "http_method": "PATCH",
-        "url_name": "change_environment_instance_type",
+        "url_name": "change_environment_machine_type",
         "button_class": "btn btn-primary",
     },
     "destroy": {
         "button_text": "Destroy",
         "http_method": "DELETE",
         "url_name": "delete_environment",
         "button_class": "btn btn-danger m-1",
@@ -82,35 +81,33 @@
     result_data = {
         "environment": environment,
         "project": project,
         "button_text": data["button_text"],
         "button_class": data["button_class"],
         "modal_title": data["modal_title"],
         "modal_body": data["modal_body"],
-        "modal_id": f"{data['action_button_type']}-{environment.id}",
+        "modal_id": f"{data['action_button_type']}-{environment.gcp_identifier}",
         "action_button_type": data["action_button_type"],
     }
     if button_type == "modal_instance":
-        result_data["instances_dict"] = INSTANCE_TYPE_SPECIFICATION
+        result_data["instances_dict"] = MACHINE_TYPE_SPECIFICATION
 
     return result_data
 
 
 @register.inclusion_tag("tag/environment_action_button.html")
 def environment_action_button(
     environment: ResearchEnvironment,
-    project: PublishedProject,
     button_type: str,
 ) -> dict:
     data = button_types[button_type]
     request_data = {
-        "workbench_id": environment.id,
-        "project_id": project.pk,
-        "region": environment.region.value,
         "gcp_project_id": environment.workspace_name,
+        "instance_name": environment.gcp_identifier,
+        "environment_type": environment.type.value,
     }
 
     result_data = {
         "button_class": data["button_class"],
         "button_text": data["button_text"],
         "button_type": button_type,
         "url": reverse(data["url_name"]),
@@ -123,16 +120,19 @@
 @register.inclusion_tag("tag/workspace_destroy_modal_button.html")
 def workspace_destroy_modal_button(
     workspace: ResearchWorkspace,
     environments_project_workflow_triplets: Iterable[
         Tuple[ResearchEnvironment, PublishedProject, Iterable[Workflow]]
     ],
 ) -> dict:
-    print(environments_project_workflow_triplets)
-    request_data = {"gcp_project_id": workspace.gcp_project_id}
+    request_data = {
+        "gcp_project_id": workspace.gcp_project_id,
+        "region": workspace.region.value,
+        "billing_account_id": workspace.gcp_billing_id,
+    }
     result_data = {
         "workspace": workspace,
         "modal_id": f"workspace-delete-{workspace.gcp_project_id}",
         "button_type": "workspace_delete",
         "request_url": reverse("delete_workspace"),
         "request_method": "DELETE",
         "request_data": json.dumps(request_data),
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/helpers.py` & `hdn-research-environment-2.3.0/environment/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib.auth import get_user_model
 
-from environment.models import CloudIdentity, BillingSetup
+from environment.models import BillingSetup, CloudIdentity
 
 User = get_user_model()
 
 
 def create_user_without_cloud_identity(
     username: str = "foo", email: str = "bar", password: str = "baz"
 ) -> User:
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/mocks.py` & `hdn-research-environment-2.3.0/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_decorators.py` & `hdn-research-environment-2.3.0/environment/tests/test_decorators.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest import skipIf
 from unittest.mock import Mock
 
+from django.conf import settings
 from django.test import TestCase
 from django.urls import reverse
-from django.conf import settings
 
 from environment.decorators import (
     cloud_identity_required,
-    require_PATCH,
     require_DELETE,
+    require_PATCH,
 )
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_services.py` & `hdn-research-environment-2.3.0/environment/tests/test_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 from unittest import skipIf
-from unittest.mock import patch, MagicMock
+from unittest.mock import MagicMock, patch
 
+from django.apps import apps
 from django.conf import settings
-from django.test import TestCase
 from django.contrib.auth import get_user_model
-from django.apps import apps
+from django.test import TestCase
 
-from environment.services import (
-    create_cloud_identity,
-    create_research_environment,
-    stop_running_environment,
-    start_stopped_environment,
-    change_environment_instance_type,
-    delete_environment,
-    verify_billing_and_create_workspace,
-    get_environments_with_projects,
+from environment.entities import (
+    EnvironmentStatus,
+    InstanceType,
+    Region,
+    ResearchEnvironment,
 )
 from environment.exceptions import (
-    IdentityProvisioningFailed,
-    EnvironmentCreationFailed,
-    StopEnvironmentFailed,
-    StartEnvironmentFailed,
+    BillingVerificationFailed,
     ChangeEnvironmentInstanceTypeFailed,
     DeleteEnvironmentFailed,
-    BillingVerificationFailed,
+    EnvironmentCreationFailed,
     GetAvailableEnvironmentsFailed,
+    IdentityProvisioningFailed,
+    StartEnvironmentFailed,
+    StopEnvironmentFailed,
 )
-from environment.entities import (
-    Region,
-    InstanceType,
-    EnvironmentStatus,
-    ResearchEnvironment,
+from environment.services import (
+    change_environment_machine_type,
+    create_cloud_identity,
+    create_research_environment,
+    delete_environment,
+    get_environments_with_projects,
+    start_stopped_environment,
+    stop_running_environment,
+    verify_billing_and_create_workspace,
 )
-from environment.tests.mocks import get_workspace_list_json
 from environment.tests.helpers import (
-    create_user_without_cloud_identity,
     create_user_with_cloud_identity,
+    create_user_without_cloud_identity,
 )
-
+from environment.tests.mocks import get_workspace_list_json
 
 PublishedProject = apps.get_model("project", "PublishedProject")
 
 
 User = get_user_model()
 
 
@@ -180,36 +179,36 @@
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
 class ChangeEnvironmentInstanceTypeTestCase(TestCase):
     def setUp(self):
         self.user = create_user_with_cloud_identity()
 
-    @patch("environment.api.change_workbench_instance_type")
-    def test_raises_if_request_fails(self, mock_change_workbench_instance_type):
-        mock_change_workbench_instance_type.return_value.ok = False
+    @patch("environment.api.change_workbench_machine_type")
+    def test_raises_if_request_fails(self, mock_change_workbench_machine_type):
+        mock_change_workbench_machine_type.return_value.ok = False
         self.assertRaises(
             ChangeEnvironmentInstanceTypeFailed,
-            change_environment_instance_type,
+            change_environment_machine_type,
             self.user,
             "workbench_id",
             Region.AUSTRALIA_SOUTHEAST,
             InstanceType.N1_STANDARD_2,
         )
 
-    @patch("environment.api.change_workbench_instance_type")
-    def test_raises_if_request_succeeds(self, mock_change_workbench_instance_type):
-        mock_change_workbench_instance_type.return_value.ok = True
-        result = change_environment_instance_type(
+    @patch("environment.api.change_workbench_machine_type")
+    def test_raises_if_request_succeeds(self, mock_change_workbench_machine_type):
+        mock_change_workbench_machine_type.return_value.ok = True
+        result = change_environment_machine_type(
             self.user,
             "workbench_id",
             Region.AUSTRALIA_SOUTHEAST,
             InstanceType.N1_STANDARD_2,
         )
-        self.assertEqual(result, mock_change_workbench_instance_type.return_value)
+        self.assertEqual(result, mock_change_workbench_machine_type.return_value)
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
 class DeleteEnvironmentTestCase(TestCase):
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_signals.py` & `hdn-research-environment-2.3.0/environment/tests/test_signals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from datetime import timedelta, datetime
+from datetime import datetime, timedelta
 from unittest import skipIf
 from unittest.mock import patch
 
-
-from django.test import TestCase
 from django.conf import settings
+from django.test import TestCase
 from django.utils import timezone
 
-from environment.signals import User, DataAccessRequest, Training, Event
+from environment.signals import DataAccessRequest, Event, Training, User
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
 class UserSignalsTestCase(TestCase):
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_utilities.py` & `hdn-research-environment-2.3.0/environment/tests/test_utilities.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unittest import skipIf
 
-from django.test import TestCase
 from django.conf import settings
+from django.test import TestCase
 
 from environment.tests.helpers import (
     create_user_with_cloud_identity,
     create_user_without_cloud_identity,
 )
 from environment.utilities import (
-    user_has_cloud_identity,
-    left_join_iterators,
     inner_join_iterators,
+    left_join_iterators,
+    user_has_cloud_identity,
 )
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_validators.py` & `hdn-research-environment-2.3.0/environment/tests/test_validators.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import skipIf
 
+from django.conf import settings
 from django.forms import ValidationError
 from django.test import TestCase
-from django.conf import settings
 
 from environment.validators import gcp_billing_account_id_validator
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
```

### Comparing `hdn-research-environment-2.2.0/environment/tests/test_views.py` & `hdn-research-environment-2.3.0/environment/tests/test_views.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from unittest import skipIf
 from unittest.mock import patch
 
+from django.conf import settings
 from django.test import TestCase
 from django.urls import reverse
-from django.conf import settings
 
+from environment.exceptions import BillingVerificationFailed
 from environment.tests.helpers import (
-    create_user_without_cloud_identity,
     create_user_with_cloud_identity,
+    create_user_without_cloud_identity,
 )
-from environment.exceptions import BillingVerificationFailed
 
 
 @skipIf(
     not settings.ENABLE_CLOUD_RESEARCH_ENVIRONMENTS,
     "Research environments are disabled",
 )
 class IdentityProvisioningTestCase(TestCase):
```

### Comparing `hdn-research-environment-2.2.0/environment/urls.py` & `hdn-research-environment-2.3.0/environment/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.urls import path
 
 from environment import views
 
-
 urlpatterns = [
     path("", views.research_environments, name="research_environments"),
     path(
         "billing/manage/<billing_account_id>",
         views.manage_billing_account,
         name="manage_billing_account",
     ),
@@ -33,16 +32,16 @@
     path(
         "environment/start",
         views.start_stopped_environment,
         name="start_stopped_environment",
     ),
     path(
         "environment/update",
-        views.change_environment_instance_type,
-        name="change_environment_instance_type",
+        views.change_environment_machine_type,
+        name="change_environment_machine_type",
     ),
     path("environment/delete", views.delete_environment, name="delete_environment"),
     path(
         "environment/create/<project_slug>/<project_version>",
         views.create_research_environment,
         name="create_research_environment",
     ),
```

### Comparing `hdn-research-environment-2.2.0/environment/utilities.py` & `hdn-research-environment-2.3.0/environment/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Iterator, Tuple, Optional, TypeVar, Callable
+from typing import Callable, Iterator, Optional, Tuple, TypeVar
 
 from django.db.models import Model
 
-
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
 User = Model
```

### Comparing `hdn-research-environment-2.2.0/environment/views.py` & `hdn-research-environment-2.3.0/environment/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-import json
 import concurrent
+import json
 
-from django.shortcuts import render, redirect
-from django.http import JsonResponse
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.db import transaction
-from django.views.decorators.http import require_http_methods, require_GET
+from django.http import Http404, JsonResponse
+from django.shortcuts import redirect, render
+from django.views.decorators.http import require_GET, require_http_methods
 from google.cloud.workflows.executions_v1beta.types.executions import Execution
 
-import environment.services as services
 import environment.constants as constants
-from environment.forms import (
-    CreateResearchEnvironmentForm,
-    CloudIdentityPasswordForm,
-    CreateWorkspaceForm,
-    ShareBillingAccountForm,
-)
+import environment.services as services
 from environment.decorators import (
     cloud_identity_required,
     require_DELETE,
     require_PATCH,
 )
-from environment.entities import Region, InstanceType
-from environment.utilities import (
-    user_has_cloud_identity,
+from environment.entities import InstanceType, Region
+from environment.forms import (
+    CloudIdentityPasswordForm,
+    CreateResearchEnvironmentForm,
+    CreateWorkspaceForm,
+    ShareBillingAccountForm,
 )
-from environment.models import Workflow, BillingAccountSharingInvite
+from environment.models import BillingAccountSharingInvite, Workflow
+from environment.utilities import user_has_cloud_identity
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 def identity_provisioning(request):
     if user_has_cloud_identity(request.user):
         return redirect("research_environments")
@@ -89,15 +87,14 @@
         projects_with_environments_being_created + environment_project_workflow_triplets
     )
 
     sorted_environments_project_workflow_triplets_dict = (
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating,
             workspaces_list,
-            billing_accounts_list,
         )
     )
 
     inprogress_workspaces = [
         workflow.workspace_name
         for workflow in workspace_workflows
         if workflow.workspace_name
@@ -110,14 +107,15 @@
 
     context = {
         "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
         "workspace_project_environment_workflow_triplets_dict": triplets_without_inprogress_workspaces,
         "workspace_workflows": workspace_workflows,
         "billing_accounts_list": billing_accounts_list,
+        "machine_type_specification_dict": constants.MACHINE_TYPE_SPECIFICATION,
     }
 
     return render(
         request,
         "environment/research_environments.html",
         context,
     )
@@ -162,15 +160,14 @@
         projects_with_environments_being_created + environment_project_workflow_triplets
     )
 
     sorted_environments_project_workflow_triplets_dict = (
         services.sort_environments_per_workspace(
             environment_projects_pairs_with_creating,
             workspaces_list,
-            billing_accounts_list,
         )
     )
 
     inprogress_workspaces = [
         workflow.workspace_name
         for workflow in workspace_workflows
         if workflow.workspace_name
@@ -183,14 +180,15 @@
 
     context = {
         "available_project_environment_workflow_triplets": available_project_environment_workflow_triplets,
         "environment_project_workflow_triplets": environment_projects_pairs_with_creating,
         "workspace_project_environment_workflow_triplets_dict": triplets_without_inprogress_workspaces,
         "workspace_workflows": workspace_workflows,
         "billing_accounts_list": billing_accounts_list,
+        "machine_type_specification_dict": constants.MACHINE_TYPE_SPECIFICATION,
     }
 
     execution_resource_name = request.GET.get("execution_resource_name")
     if execution_resource_name:
         workflow = Workflow.objects.get(execution_resource_name=execution_resource_name)
         workflow_state_context = {
             "recent_workflow": workflow,
@@ -210,14 +208,20 @@
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
 def create_workspace(request):
     billing_accounts_list = services.get_billing_accounts_list(request.user)
+    if not billing_accounts_list:
+        messages.info(
+            request,
+            "You have to have access to at least one billing account in order to create a workspace. Visit the Billing tab for more information.",
+        )
+        return redirect("research_environments")
 
     if request.method == "POST":
         form = CreateWorkspaceForm(
             request.POST, billing_accounts_list=billing_accounts_list
         )
         if form.is_valid():
             services.create_workspace(
@@ -238,36 +242,44 @@
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
 def create_research_environment(request, project_slug, project_version):
     workspaces_list = services.get_workspaces_list(request.user)
+    if not workspaces_list:
+        messages.info(
+            request,
+            "You have to have at least one workspace in order to create a research environment. You can create one using the form below.",
+        )
+        return redirect("create_workspace")
+
     project = services.get_available_projects(request.user).get(
         slug=project_slug, version=project_version
     )
 
     if request.method == "POST":
         form = CreateResearchEnvironmentForm(
             request.POST, workspace_list=workspaces_list
         )
         if form.is_valid():
             cpu_usage = services.cpu_usage(
-                value=InstanceType(form.cleaned_data["instance_type"]).cpus(),
+                value=InstanceType(form.cleaned_data["machine_type"]).cpus(),
                 user=request.user,
             )
             if cpu_usage <= constants.MAX_CPU_USAGE:
                 services.create_research_environment(
                     user=request.user,
                     project=project,
-                    workspace_name=form.cleaned_data["workspace_id"],
-                    instance_type=form.cleaned_data["instance_type"],
-                    environment_type=form.cleaned_data["environment_type"],
-                    persistent_disk=form.cleaned_data.get("persistent_disk"),
-                    gpu_accelerator=form.cleaned_data.get("gpu_accelerator"),
+                    workspace_project_id=form.cleaned_data["workspace"].gcp_project_id,
+                    machine_type=form.cleaned_data["machine_type"],
+                    region=form.cleaned_data["workspace"].region.value,
+                    workbench_type=form.cleaned_data["environment_type"],
+                    disk_size=form.cleaned_data.get("disk_size"),
+                    gpu_accelerator_type=form.cleaned_data.get("gpu_accelerator"),
                 )
                 return redirect("research_environments")
             else:
                 messages.error(
                     request,
                     f"Quota exceeded - the specified configuration would use {cpu_usage} out of {constants.MAX_CPU_USAGE} CPUs",
                 )
@@ -285,15 +297,17 @@
 
 
 @require_http_methods(["GET", "POST"])
 @login_required
 @cloud_identity_required
 @transaction.atomic
 def manage_billing_account(request, billing_account_id):
-    # TODO: Check whether the user is the billing account's owner
+    if not services.is_billing_account_owner(request.user, billing_account_id):
+        raise Http404()
+
     owner = request.user
     billing_account_sharing_form = ShareBillingAccountForm()
 
     if request.method == "POST":
         form_action = request.POST["action"]
         if form_action == "share_account":
             billing_account_sharing_form = ShareBillingAccountForm(request.POST)
@@ -353,77 +367,75 @@
 
 @require_PATCH
 @login_required
 @cloud_identity_required
 def stop_running_environment(request):
     data = json.loads(request.body)
     services.stop_running_environment(
-        user=request.user,
-        project_id=data["project_id"],
-        workbench_id=data["workbench_id"],
-        region=Region(data["region"]),
-        gcp_project_id=data["gcp_project_id"],
+        workbench_type=data["environment_type"],
+        workbench_resource_id=data["instance_name"],
+        user_email=request.user.cloud_identity.email,
+        workspace_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
 def start_stopped_environment(request):
     data = json.loads(request.body)
     services.start_stopped_environment(
-        user=request.user,
-        project_id=data["project_id"],
-        workbench_id=data["workbench_id"],
-        region=Region(data["region"]),
-        gcp_project_id=data["gcp_project_id"],
+        user_email=request.user.cloud_identity.email,
+        workbench_type=data["environment_type"],
+        workbench_resource_id=data["instance_name"],
+        workspace_project_id=data["gcp_project_id"],
     )
     return JsonResponse({})
 
 
 @require_PATCH
 @login_required
 @cloud_identity_required
-def change_environment_instance_type(request):
+def change_environment_machine_type(request):
     data = json.loads(request.body)
-    services.change_environment_instance_type(
-        user=request.user,
-        project_id=data["project_id"],
-        workbench_id=data["workbench_id"],
-        region=Region(data["region"]),
-        new_instance_type=InstanceType(data["instance_type"]),
-        gcp_project_id=data["gcp_project_id"],
+    services.change_environment_machine_type(
+        user_email=request.user.cloud_identity.email,
+        workspace_project_id=data["gcp_project_id"],
+        machine_type=data["machine_type"],
+        workbench_type=data["environment_type"],
+        workbench_resource_id=data["instance_name"],
     )
     return JsonResponse({})
 
 
 @require_DELETE
 @login_required
 @cloud_identity_required
 def delete_environment(request):
     data = json.loads(request.body)
     services.delete_environment(
-        user=request.user,
-        project_id=data["project_id"],
-        workbench_id=data["workbench_id"],
-        region=Region(data["region"]),
-        gcp_project_id=data["gcp_project_id"],
+        user_email=request.user.cloud_identity.email,
+        workspace_project_id=data["gcp_project_id"],
+        workbench_type=data["environment_type"],
+        workbench_resource_id=data["instance_name"],
     )
     return JsonResponse({})
 
 
 @require_DELETE
 @login_required
 @cloud_identity_required
 def delete_workspace(request):
     data = json.loads(request.body)
     services.delete_workspace(
         user=request.user,
         gcp_project_id=data["gcp_project_id"],
+        billing_account_id=data["billing_account_id"],
+        region=data["region"],
     )
     return JsonResponse({})
 
 
 @require_GET
 @login_required
 @cloud_identity_required
```

### Comparing `hdn-research-environment-2.2.0/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-2.3.0/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: hdn-research-environment
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -19,7 +17,8 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
+License-File: LICENSE
```

### Comparing `hdn-research-environment-2.2.0/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-2.3.0/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,19 +19,15 @@
 environment/signals.py
 environment/tasks.py
 environment/urls.py
 environment/utilities.py
 environment/validators.py
 environment/views.py
 environment/api/__init__.py
-environment/api/v1/__init__.py
-environment/api/v1/auth.py
-environment/api/v1/decorators.py
-environment/api/v2/__init__.py
-environment/api/v2/decorators.py
+environment/api/decorators.py
 environment/migrations/0001_initial.py
 environment/migrations/0002_billingsetup.py
 environment/migrations/0003_cloudidentity_is_workspace_done.py
 environment/migrations/0004_auto_20220309_0330.py
 environment/migrations/0005_workflow.py
 environment/migrations/0006_delete_billingsetup.py
 environment/migrations/0007_billingaccountsharinginvite.py
@@ -42,14 +38,15 @@
 environment/static/environment/css/create_research_environment.css
 environment/static/environment/css/environment-base.css
 environment/static/environment/css/manage_billing_account.css
 environment/static/environment/js/cookie.js
 environment/static/environment/js/forms.js
 environment/static/environment/js/gpu_disabling.js
 environment/static/environment/js/pricing_change.js
+environment/templates/.DS_Store
 environment/templates/environment/_available_environments_list.html
 environment/templates/environment/_available_projects_list.html
 environment/templates/environment/_billing_accounts_list.html
 environment/templates/environment/_environment_tabs.html
 environment/templates/environment/base_environment_home.html
 environment/templates/environment/create_research_environment.html
 environment/templates/environment/create_workspace.html
@@ -60,14 +57,15 @@
 environment/templates/environment/email/billing_sharing_confirmation.html
 environment/templates/environment/email/environment_access_expired.html
 environment/templates/tag/environment_action_button.html
 environment/templates/tag/environment_modal_button.html
 environment/templates/tag/workspace_destroy_modal_button.html
 environment/templatetags/__init__.py
 environment/templatetags/action_buttons.py
+environment/templatetags/environment_templatetags.py
 environment/tests/__init__.py
 environment/tests/helpers.py
 environment/tests/mocks.py
 environment/tests/test_decorators.py
 environment/tests/test_services.py
 environment/tests/test_signals.py
 environment/tests/test_utilities.py
```

### Comparing `hdn-research-environment-2.2.0/setup.cfg` & `hdn-research-environment-2.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 2.2.0
+version = 2.3.0
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

