# Comparing `tmp/lamindb_setup-0.49.5.tar.gz` & `tmp/lamindb_setup-0.49.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.49.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.49.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.49.5.tar` & `lamindb_setup-0.49.6.tar`

### file list

```diff
@@ -1,107 +1,108 @@
--rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.5/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.5/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.5/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.5/README.md
--rw-r--r--   0        0        0    59839 2023-08-06 21:15:15.938006 lamindb_setup-0.49.5/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.5/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.5/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.5/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.5/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.5/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.5/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.5/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.5/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.5/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.5/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.5/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.5/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.5/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.5/docs/reference.md
--rw-r--r--   0        0        0      364 2023-08-06 21:14:34.989760 lamindb_setup-0.49.5/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.5/lamin-project.yaml
--rw-r--r--   0        0        0     2758 2023-08-06 21:14:50.504187 lamindb_setup-0.49.5/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5704 2023-07-31 17:31:23.899228 lamindb_setup-0.49.5/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2072 2023-08-06 21:14:34.990057 lamindb_setup-0.49.5/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      849 2023-08-06 21:14:34.990237 lamindb_setup-0.49.5/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2014 2023-08-06 21:14:34.990409 lamindb_setup-0.49.5/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.5/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.5/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7475 2023-08-06 21:14:34.990684 lamindb_setup-0.49.5/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6601 2023-08-06 21:14:34.990879 lamindb_setup-0.49.5/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1417 2023-08-06 21:14:34.991033 lamindb_setup-0.49.5/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1685 2023-08-06 21:14:34.991186 lamindb_setup-0.49.5/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      782 2023-08-06 21:14:34.991331 lamindb_setup-0.49.5/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.5/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2188 2023-08-06 21:14:34.991491 lamindb_setup-0.49.5/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.5/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.5/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.5/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3497 2023-08-06 21:14:34.991664 lamindb_setup-0.49.5/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.5/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.5/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5998 2023-08-06 21:14:34.991847 lamindb_setup-0.49.5/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.5/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10928 2023-08-06 21:14:34.992038 lamindb_setup-0.49.5/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.5/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0    11248 2023-08-06 21:14:34.992292 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.5/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9340 2023-08-06 21:14:34.992512 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2317 2023-08-06 21:14:34.992697 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.5/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.5/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2174 2023-08-06 21:14:34.992898 lamindb_setup-0.49.5/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4867 2023-08-05 09:44:28.020872 lamindb_setup-0.49.5/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2734 2023-07-31 17:31:23.900624 lamindb_setup-0.49.5/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.5/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.5/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.5/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    36103 2023-08-06 12:24:47.608810 lamindb_setup-0.49.5/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.5/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.5/lnschema-core/README.md
--rw-r--r--   0        0        0      508 2023-08-06 12:24:47.608958 lamindb_setup-0.49.5/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.5/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
--rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
--rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
--rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
--rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
--rw-r--r--   0        0        0     6285 2023-08-06 12:24:47.609237 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
--rw-r--r--   0        0        0     2985 2023-08-06 12:24:47.609326 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py
--rw-r--r--   0        0        0      393 2023-08-06 12:24:47.609390 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0014_rename_ref_field_featureset_registry.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.5/lnschema-core/lnschema_core/mocks.py
--rw-r--r--   0        0        0    71611 2023-08-06 12:24:47.609755 lamindb_setup-0.49.5/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.5/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.5/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.5/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.5/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.5/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.5/noxfile.py
--rw-r--r--   0        0        0     1168 2023-08-06 21:14:34.993101 lamindb_setup-0.49.5/pyproject.toml
--rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.5/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.5/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.5/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.5/tests/test_bionty.py
--rw-r--r--   0        0        0     4936 2023-08-03 09:23:05.337238 lamindb_setup-0.49.5/tests/test_init_instance.py
--rw-r--r--   0        0        0     2207 2023-07-25 01:43:24.442039 lamindb_setup-0.49.5/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.5/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-24 10:02:47.316450 lamindb_setup-0.49.5/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.5/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.5/tests/test_signup.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 lamindb_setup-0.49.5/PKG-INFO
+-rw-r--r--   0        0        0     4433 2023-08-07 22:58:01.301177 lamindb_setup-0.49.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.6/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.6/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.6/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.6/README.md
+-rw-r--r--   0        0        0    60597 2023-08-07 22:58:01.301509 lamindb_setup-0.49.6/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.6/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.6/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.6/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.6/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.6/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.6/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.6/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.6/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.6/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.6/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.6/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.6/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.6/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.6/docs/reference.md
+-rw-r--r--   0        0        0      364 2023-08-06 21:14:34.989760 lamindb_setup-0.49.6/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.6/lamin-project.yaml
+-rw-r--r--   0        0        0     2758 2023-08-07 22:58:01.301780 lamindb_setup-0.49.6/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5704 2023-07-31 17:31:23.899228 lamindb_setup-0.49.6/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2072 2023-08-06 21:14:34.990057 lamindb_setup-0.49.6/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      849 2023-08-06 21:14:34.990237 lamindb_setup-0.49.6/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2067 2023-08-07 19:15:49.889368 lamindb_setup-0.49.6/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.6/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.6/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7444 2023-08-07 19:49:45.826769 lamindb_setup-0.49.6/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6584 2023-08-07 19:49:45.826931 lamindb_setup-0.49.6/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1417 2023-08-07 19:15:49.889910 lamindb_setup-0.49.6/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1679 2023-08-07 19:49:45.827076 lamindb_setup-0.49.6/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      779 2023-08-07 19:49:45.827207 lamindb_setup-0.49.6/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.6/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2185 2023-08-07 19:49:45.827342 lamindb_setup-0.49.6/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.6/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.6/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.6/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3497 2023-08-07 19:15:49.890591 lamindb_setup-0.49.6/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.6/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.6/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     6004 2023-08-07 19:15:49.890785 lamindb_setup-0.49.6/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.6/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10931 2023-08-07 19:15:49.890946 lamindb_setup-0.49.6/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.6/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.6/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0    11248 2023-08-07 19:15:49.891129 lamindb_setup-0.49.6/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.6/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     5630 2023-08-07 19:15:49.891789 lamindb_setup-0.49.6/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9508 2023-08-07 22:58:01.302137 lamindb_setup-0.49.6/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.6/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.6/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2317 2023-08-07 19:15:49.892135 lamindb_setup-0.49.6/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.6/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.6/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2174 2023-08-06 21:14:34.992898 lamindb_setup-0.49.6/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5183 2023-08-07 19:15:49.892730 lamindb_setup-0.49.6/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2734 2023-07-31 17:31:23.900624 lamindb_setup-0.49.6/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.6/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.6/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.6/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.6/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.6/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    36103 2023-08-06 12:24:47.608810 lamindb_setup-0.49.6/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.6/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.6/lnschema-core/README.md
+-rw-r--r--   0        0        0      508 2023-08-06 12:24:47.608958 lamindb_setup-0.49.6/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.6/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
+-rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
+-rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
+-rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
+-rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
+-rw-r--r--   0        0        0     6285 2023-08-06 12:24:47.609237 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
+-rw-r--r--   0        0        0     2985 2023-08-06 12:24:47.609326 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py
+-rw-r--r--   0        0        0      393 2023-08-06 12:24:47.609390 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0014_rename_ref_field_featureset_registry.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.6/lnschema-core/lnschema_core/mocks.py
+-rw-r--r--   0        0        0    71611 2023-08-06 12:24:47.609755 lamindb_setup-0.49.6/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.6/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.6/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.6/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.6/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.6/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     2452 2023-08-07 22:58:01.302468 lamindb_setup-0.49.6/noxfile.py
+-rw-r--r--   0        0        0     1168 2023-08-06 21:14:34.993101 lamindb_setup-0.49.6/pyproject.toml
+-rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.6/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.6/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.6/tests/hub/test_storage.py
+-rw-r--r--   0        0        0      280 2023-08-07 22:58:01.302738 lamindb_setup-0.49.6/tests/test_load_persistent_instance.py
+-rw-r--r--   0        0        0       45 2023-08-07 22:58:01.302905 lamindb_setup-0.49.6/tests/unit/test_bionty.py
+-rw-r--r--   0        0        0     4936 2023-08-07 22:58:01.303040 lamindb_setup-0.49.6/tests/unit/test_init_instance.py
+-rw-r--r--   0        0        0     2207 2023-08-07 22:58:01.303164 lamindb_setup-0.49.6/tests/unit/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-08-07 22:58:01.303253 lamindb_setup-0.49.6/tests/unit/test_login.py
+-rw-r--r--   0        0        0      457 2023-08-07 22:58:01.303360 lamindb_setup-0.49.6/tests/unit/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-08-07 22:58:01.303464 lamindb_setup-0.49.6/tests/unit/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-08-07 22:58:01.303570 lamindb_setup-0.49.6/tests/unit/test_signup.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 lamindb_setup-0.49.6/PKG-INFO
```

### Comparing `lamindb_setup-0.49.5/.github/workflows/build.yml` & `lamindb_setup-0.49.6/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -18,54 +18,38 @@
         group:
           - "unit"
           - "docs"
         lamin_env:
           - "staging"
           - "prod"
     timeout-minutes: 20
-
     steps:
-      - name: Checkout main
-        uses: actions/checkout@v3
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           submodules: recursive
-      - name: Checkout lndocs
-        uses: actions/checkout@v3
-        with:
-          repository: laminlabs/lndocs
-          ssh-key: ${{ secrets.READ_LNDOCS }}
-          path: lndocs
-          ref: main
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip"
           cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
-      - name: Cache pre-commit
-        uses: actions/cache@v3
+      - uses: actions/cache@v3
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
-      - name: Cache postgres
-        id: cache-postgres
+      - id: cache-postgres
         uses: actions/cache@v3
         with:
           path: ~/postgres.tar
           key: cache-postgres-0
-      - name: Cache postgres miss
-        if: steps.cache-postgres.outputs.cache-hit != 'true'
+      - if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
-      - name: Cache postgres use
-        if: steps.cache-postgres.outputs.cache-hit == 'true'
+      - if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
-      - name: install Python deps
-        run: |
-          python -m pip install -U pip
-          pip install -U laminci
+      - run: pip install -U laminci
       - name: install apt-get deps
         run: |
           sudo apt-get -y install graphviz
           sudo apt-get install libpq-dev
       # - run: nox -s lint
       - uses: aws-actions/configure-aws-credentials@v2
         with:
@@ -74,40 +58,65 @@
           aws-region: eu-central-1
       # - uses: "google-github-actions/auth@v0"
       #   with:
       #     credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
       # - uses: "google-github-actions/setup-gcloud@v0"
       - run: nox -s "install(group='${{ matrix.group }}')"
       - run: nox -s "build(lamin_env='${{ matrix.lamin_env }}', group='${{ matrix.group }}')"
-        env:
-          SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
-          SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
-      - name: upload coverage
-        uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v2
         with:
           name: coverage--${{ matrix.group }}
           path: .coverage
-      - run: nox -s docs
-        if: ${{ matrix.group == 'docs' }}
-      - uses: codecov/codecov-action@v2
+      # docs from here
+      - uses: actions/checkout@v3
+        if: ${{ matrix.group == 'docs' && matrix.group == 'prod' }}
         with:
-          token: ${{ secrets.CODECOV_TOKEN }}
+          repository: laminlabs/lndocs
+          ssh-key: ${{ secrets.READ_LNDOCS }}
+          path: lndocs
+          ref: main
+      - run: nox -s docs
+        if: ${{ matrix.group == 'docs' && matrix.group == 'prod' }}
       - uses: nwtgck/actions-netlify@v1.2
-        if: ${{ matrix.group == 'docs' }}
+        if: ${{ matrix.group == 'docs' && matrix.group == 'prod' }}
         with:
           publish-dir: "_build/html"
           production-deploy: ${{ github.event_name == 'push' }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
           NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
 
+  # a test group for testing user access to public buckets without AWS credentials
+  noaws:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.9"]
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: recursive
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          cache: "pip"
+          cache-dependency-path: ".github/workflows/build.yml" # See dependencies below
+      - run: pip install -U laminci
+      - run: nox -s "install(group='noaws')"
+      - run: nox -s noaws
+      - uses: actions/upload-artifact@v2
+        with:
+          name: coverage--noaws
+          path: .coverage
+
   coverage:
-    needs: build
+    needs: [build, noaws]
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: 3.9
           cache: "pip"
```

### Comparing `lamindb_setup-0.49.5/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/.gitignore` & `lamindb_setup-0.49.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/.pre-commit-config.yaml` & `lamindb_setup-0.49.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/LICENSE` & `lamindb_setup-0.49.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/changelog.md` & `lamindb_setup-0.49.6/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+👷 Test configuration with no AWS access | [460](https://github.com/laminlabs/lamindb-setup/pull/460) | [falexwolf](https://github.com/falexwolf) | 2023-08-07 | 0.49.6
+👷 Simplify CI setup | [458](https://github.com/laminlabs/lamindb-setup/pull/458) | [falexwolf](https://github.com/falexwolf) | 2023-08-07 |
+🎨 Use logger.save | [459](https://github.com/laminlabs/lamindb-setup/pull/459) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-07 |
+🐛 Fix aws access with no credentials | [457](https://github.com/laminlabs/lamindb-setup/pull/457) | [Koncopd](https://github.com/Koncopd) | 2023-08-07 |
+🔊 Refactored logging msg | [456](https://github.com/laminlabs/lamindb-setup/pull/456) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-07 |
 ♻️ Replace `lamin_logger` with `lamin_utils` | [454](https://github.com/laminlabs/lamindb-setup/pull/454) | [falexwolf](https://github.com/falexwolf) | 2023-08-06 | 0.49.5
 🚚 Rename `ORM` to `Registry` | [453](https://github.com/laminlabs/lamindb-setup/pull/453) | [sunnyosun](https://github.com/sunnyosun) | 2023-08-05 |
 ⬇️ Upper bound external dependencies | [452](https://github.com/laminlabs/lamindb-setup/pull/452) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.49.4
 🎨 Add `.record` property to `StorageSettings` | [451](https://github.com/laminlabs/lamindb-setup/pull/451) | [falexwolf](https://github.com/falexwolf) | 2023-08-03 | 0.49.3
 ✅ Fix init-instance test for sqlite instance | [450](https://github.com/laminlabs/lamindb-setup/pull/450) | [bpenteado](https://github.com/bpenteado) | 2023-08-02 |
 🎨 Fix `init-instance` anti-patterns and expand tests | [449](https://github.com/laminlabs/lamindb-setup/pull/449) | [bpenteado](https://github.com/bpenteado) | 2023-08-01 |
 ✨ Propagate kwargs through synchronization functions | [448](https://github.com/laminlabs/lamindb-setup/pull/448) | [Koncopd](https://github.com/Koncopd) | 2023-07-31 | 0.49.2
```

### Comparing `lamindb_setup-0.49.5/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.49.6/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/faq/multi-session.ipynb` & `lamindb_setup-0.49.6/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.49.6/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.49.6/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.49.6/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.49.6/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.49.6/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.49.6/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/docs/guide/setup-user.md` & `lamindb_setup-0.49.6/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/__init__.py` & `lamindb_setup-0.49.6/lamindb_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.49.5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.49.6"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/__main__.py` & `lamindb_setup-0.49.6/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.49.6/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_close.py` & `lamindb_setup-0.49.6/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_delete.py` & `lamindb_setup-0.49.6/lamindb_setup/_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,42 +12,44 @@
 def delete(instance_name: str):
     """Delete an instance."""
     instance_identifier = f"{settings.user.handle}/{instance_name}"
     logger.info(f"deleting instance {instance_identifier}")
     settings_file = instance_settings_file(instance_name, settings.user.handle)
     if not settings_file.exists():
         logger.warning(
-            "Could not delete as instance settings do not exist locally. Did you"
-            " provide a wrong instance name? Could you try loading it?"
+            "could not delete as instance settings do not exist locally. did you"
+            " provide a wrong instance name? could you try loading it?"
         )
         return None
     isettings = load_instance_settings(settings_file)
 
     delete_settings(settings_file)
     if settings._instance_exists:
         if instance_identifier == settings.instance.identifier:
             close(mute=True)  # close() does further operations, unlocking...
             settings._instance_settings = None
     delete_cache(isettings.storage.cache_dir)
     if isettings.dialect == "sqlite":
         if isettings._sqlite_file.exists():
             isettings._sqlite_file.unlink()
-            logger.info("    deleted '.lndb' sqlite file")
+            logger.success("    deleted '.lndb' sqlite file")
         else:
-            logger.info("    '.lndb' sqlite file does not exist")
+            logger.warning("    '.lndb' sqlite file does not exist")
     if isettings.is_remote:
-        logger.info("    manually delete your remote instance on lamin.ai")
-    logger.info(f"    manually delete your stored data: {isettings.storage.root}")
+        logger.warning("    consider manually delete your remote instance on lamin.ai")
+    logger.warning(
+        f"    consider manually delete your stored data: {isettings.storage.root}"
+    )
 
 
 def delete_cache(cache_dir: Path):
     if cache_dir is not None and cache_dir.exists():
         shutil.rmtree(cache_dir)
-        logger.info("    instance cache deleted")
+        logger.success("    instance cache deleted")
 
 
 def delete_settings(settings_file: Path):
     if settings_file.exists():
         settings_file.unlink()
-        logger.info(f"    deleted instance settings file: {settings_file}")
+        logger.success(f"    deleted instance settings file: {settings_file}")
     else:
-        logger.info(f"    instance settings file doesn't exist: {settings_file}")
+        logger.warning(f"    instance settings file doesn't exist: {settings_file}")
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_docstrings.py` & `lamindb_setup-0.49.6/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_init_instance.py` & `lamindb_setup-0.49.6/lamindb_setup/_init_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             root=ssettings.root_as_str,
             type=ssettings.type,
             region=ssettings.region,
             created_by_id=settings.user.id,
         ),
     )
     if created:
-        logger.success(f"saved: {storage}")
+        logger.save(f"saved: {storage}")
 
 
 def register_user_and_storage(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     from django.db.utils import OperationalError
     from lnschema_core.models import User
 
@@ -45,18 +45,18 @@
             defaults=dict(
                 handle=usettings.handle,
                 name=usettings.name,
                 email=usettings.email,
             ),
         )
         if created:
-            logger.success(f"saved: {user}")
+            logger.save(f"saved: {user}")
         register_storage(isettings.storage)
     except OperationalError as error:
-        logger.warning(f"Instance seems not set up ({error})")
+        logger.warning(f"instance seems not set up ({error})")
 
 
 def reload_schema_modules(isettings: InstanceSettings):
     schema_names = ["core"] + list(isettings.schema)
     schema_module_names = [get_schema_module_name(n) for n in schema_names]
 
     for schema_module_name in schema_module_names:
@@ -167,17 +167,15 @@
             db=db,
             schema=schema,
         )
         if result == "instance-exists-already":
             pass  # everything is alright!
         elif isinstance(result, str):
             raise RuntimeError(f"Registering instance on hub failed:\n{result}")
-        logger.success(
-            f"registered instance on hub: https://lamin.ai/{owner}/{name_str}"
-        )
+        logger.save(f"registered instance on hub: https://lamin.ai/{owner}/{name_str}")
 
     if _test:
         isettings._persist()
         return None
 
     silence_loggers()
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_load_instance.py` & `lamindb_setup-0.49.6/lamindb_setup/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         settings_file = instance_settings_file(name, owner)
         if settings_file.exists():
             logger.info(f"found cached instance metadata: {settings_file}")
             isettings = load_instance_settings(settings_file)
         else:
             if _log_error_message:
                 raise RuntimeError(
-                    f"Instance {owner}/{name} neither loadable from hub nor local"
-                    " cache. Check whether instance exists and you have access:"
+                    f"instance {owner}/{name} neither loadable from hub nor local"
+                    " cache. check whether instance exists and you have access:"
                     f" https://lamin.ai/{owner}/{name}?tab=collaborators"
                 )
             return "instance-not-reachable"
 
     if storage is not None:
         update_isettings_with_storage(isettings, storage)
     if _test:
@@ -137,19 +137,19 @@
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
     ssettings = StorageSettings(storage)
     if ssettings.is_cloud:
         try:  # triggering ssettings.id makes a lookup in the storage table
-            logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
+            logger.success(f"loaded storage: {ssettings.id} / {ssettings.root_as_str}")
         except RuntimeError:
             raise RuntimeError(
-                "Storage not registered!\n"
-                "Load instance without the `storage` arg and register storage root: "
+                "storage not registered!\n"
+                "load instance without the `storage` arg and register storage root: "
                 f"`lamin set storage --storage {storage}`"
             )
     else:
         # local storage
         # assumption is you want to merely update the storage location
         isettings._storage = ssettings  # need this here already
     # update isettings in place
@@ -168,10 +168,8 @@
         raise RuntimeError(
             "You have several storage locations: Can't identify in which storage"
             " location the root column is to be updated!"
         )
     storage = storages[0]
     storage.root = isettings.storage.root_as_str
     storage.save()
-    logger.success(
-        f"Updated storage root {storage.id} to {isettings.storage.root_as_str}"
-    )
+    logger.save(f"updated storage root {storage.id} to {isettings.storage.root_as_str}")
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_migrate.py` & `lamindb_setup-0.49.6/lamindb_setup/_migrate.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,12 @@
         from django.core.management import call_command
 
         setup_django(settings.instance)
         try:
             call_command("makemigrations", check_changes=True)
         except SystemExit:
             logger.error(
-                "Migrations are not in sync with ORMs, please create a migration: lamin"
+                "migrations are not in sync with ORMs, please create a migration: lamin"
                 " migrate create"
             )
             return False
         return True
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_notebook.py` & `lamindb_setup-0.49.6/lamindb_setup/_notebook.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 
 def track(notebook_path: str, pypackage: Optional[str] = None):
     try:
         from nbproject.dev import initialize_metadata, read_notebook, write_notebook
         from nbproject.dev._initialize import nbproject_id
     except ImportError:
-        logger.warning("Install nbproject! pip install nbproject")
+        logger.warning("install nbproject! pip install nbproject")
         return None
 
     nb = read_notebook(notebook_path)
     if "nbproject" not in nb.metadata:
         if pypackage is not None:
             pypackage = [pp for pp in pypackage.split(",") if len(pp) > 0]  # type: ignore # noqa
         metadata = initialize_metadata(nb, pypackage=pypackage).dict()
         nb.metadata["nbproject"] = metadata
         write_notebook(nb, notebook_path)
-        logger.success("Attached metadata to notebook")
+        logger.save("attached metadata to notebook")
     else:
-        logger.info(f"The notebook {notebook_path} is already tracked")
+        logger.info(f"the notebook {notebook_path} is already tracked")
 
         updated = False
         response = input("Do you want to assign a new id or version? (y/n) ")
 
         if response != "y":
             return None
         response = input("Do you want to generate a new id? (y/n) ")
@@ -37,9 +37,9 @@
         )
         if response != "n":
             new_version = input("Please type the version: ")
             nb.metadata["nbproject"]["version"] = new_version
             updated = True
 
         if updated:
-            logger.success("Updated the notebook metadata.")
+            logger.save("updated the notebook metadata.")
             write_notebook(nb, notebook_path)
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_register_instance.py` & `lamindb_setup-0.49.6/lamindb_setup/_register_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,12 +12,12 @@
         owner=isettings.owner,
         name=isettings.name,
         storage=isettings.storage.root_as_str,
         db=isettings.db if isettings.dialect != "sqlite" else None,
         schema=isettings._schema_str,
     )
     if result == "instance-exists-already":
-        logger.info("Instance was already registered")
+        logger.info("instance was already registered")
     elif isinstance(result, str):
-        raise RuntimeError(f"Creating instance on hub failed:\n{result}")
+        raise RuntimeError(f"creating instance on hub failed:\n{result}")
     else:
-        logger.success(f"Instance registered: https://lamin.ai/{isettings.identifier}")
+        logger.save(f"instance registered: https://lamin.ai/{isettings.identifier}")
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_schema.py` & `lamindb_setup-0.49.6/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_set.py` & `lamindb_setup-0.49.6/lamindb_setup/_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         >>>     profile="some_profile", # fsspec arg
         >>>     cache_regions=True # fsspec arg for s3
         >>> )
         """
         from .dev._hub_utils import get_storage_region
 
         if settings.instance.dialect == "sqlite":
-            logger.error("Can't set storage for sqlite instances.")
+            logger.error("can't set storage for sqlite instances.")
             return "set-storage-failed"
 
         new_isettings = InstanceSettings(
             owner=settings.instance.owner,
             name=settings.instance.name,
             storage_root=root,
             storage_region=get_storage_region(root),
@@ -52,14 +52,14 @@
         # if settings.instance.is_remote:
         #     add_storage_hub(
         #         root, account_handle=settings.instance.owner  # type: ignore
         #     )
 
         settings.storage._set_fs_kwargs(**fs_kwargs)
 
-        logger.success(f"Set storage {root}")
+        logger.save(f"set storage {root}")
 
 
 @deprecated("lamindb_setup.set.storage()")
 def set_storage(storage: Union[str, Path, UPath]):
     """Deprecated in favor of `set.storage`."""
     set.storage(storage)
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_settings.py` & `lamindb_setup-0.49.6/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_setup_user.py` & `lamindb_setup-0.49.6/lamindb_setup/_setup_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 def signup(email: str) -> Union[str, None]:
     """Sign up user."""
     from .dev._hub_core import sign_up_hub
 
     response = sign_up_hub(email)
     if response == "handle-exists":  # handle already exists
-        logger.error("The handle already exists: please choose a different one")
+        logger.error("the handle already exists: please choose a different one")
         return "handle-exists"
     if response == "user-exists":  # user already exists
-        logger.error("User already exists! Please login instead: `lamin login`")
+        logger.error("user already exists! please login instead: `lamin login`")
         return "user-exists"
     user_settings = load_or_create_user_settings()
     user_settings.email = email
     save_user_settings(user_settings)
     user_settings.password = response
     save_user_settings(user_settings)
     return None  # user needs to confirm email now
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.49.6/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     @classmethod
     def unlock(cls):
         pass
 
 
 class Locker:
     def __init__(self, user_id: str, storage_root: Union[UPath, Path], name: str):
-        logger.debug(f"Init cloud sqlite locker: {user_id}, {storage_root}, {name}.")
+        logger.debug(f"init cloud sqlite locker: {user_id}, {storage_root}, {name}.")
 
         self._counter = 0
 
         self.user = user_id
         self.name = name
 
         self.root = storage_root
@@ -72,15 +72,15 @@
                 if not self.fs.exists(user_path):
                     continue
                 if self.mapper[user_endpoint] == b"0":
                     continue
                 period = (datetime.now() - self.modified(user_path)).total_seconds()
                 if period > EXPIRATION_TIME:
                     logger.info(
-                        f"The lock of the user {user} seems to be stale, clearing"
+                        f"the lock of the user {user} seems to be stale, clearing"
                         f" {endpoint}."
                     )
                     self.mapper[user_endpoint] = b"0"
 
         self._has_lock = None
         self._locked_by = None
 
@@ -98,15 +98,15 @@
         # assume in utc if the time zone is not specified
         if mtime.tzinfo is None:
             mtime = mtime.replace(tzinfo=timezone.utc)
         return mtime.astimezone().replace(tzinfo=None)
 
     def _msg_on_counter(self, user):
         if self._counter == MAX_MSG_COUNTER:
-            logger.info(f"Competing for the lock with the user {user}.")
+            logger.warning(f"competing for the lock with the user {user}.")
 
         if self._counter <= MAX_MSG_COUNTER:
             self._counter += 1
 
     def _lock_unsafe(self):
         if self._has_lock:
             return None
@@ -136,15 +136,15 @@
             if c_number == 0:
                 continue
 
             if (number > c_number) or (number == c_number and self.priority > i):
                 self._has_lock = False
                 self._locked_by = user
                 self.mapper[f"numbers/{self.user}"] = b"0"
-                logger.info(f"The instance is already locked by the user {user}.")
+                logger.warning(f"the instance is already locked by the user {user}.")
                 return None
 
     def lock(self):
         try:
             self._lock_unsafe()
         except BaseException as e:
             self.unlock()
@@ -159,15 +159,15 @@
 
     def _clear(self):
         self.mapper[f"entering/{self.user}"] = b"0"
 
     @property
     def has_lock(self):
         if self._has_lock is None:
-            logger.info("The lock has not been initialized, trying to obtain the lock.")
+            logger.info("the lock has not been initialized, trying to obtain the lock.")
             self.lock()
 
         return self._has_lock
 
 
 _locker: Optional[Locker] = None
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_django.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_django.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         ]
     # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
             except Exception as e:
-                logger.warning(f"Failed to execute: {stmt} because of {e}")
+                logger.warning(f"failed to execute: {stmt} because of {e}")
     logger.success("created legacy migration preparations")
     return True
 
 
 def insert_legacy_data(isettings: InstanceSettings):
     import sqlalchemy as sa
 
@@ -138,15 +138,15 @@
     # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
                 logger.success(stmt)
             except Exception as e:
-                logger.warning(f"Failed to execute: {stmt} because of {e}")
+                logger.warning(f"failed to execute: {stmt} because of {e}")
 
 
 def setup_django(
     isettings: InstanceSettings,
     deploy_migrations: bool = False,
     create_migrations: bool = False,
     init: bool = False,
@@ -210,10 +210,10 @@
                     " deploy\n\nOtherwise, please install an earlier version of  your"
                     " custom schema module\n\nIn case you haven't yet migrated to"
                     " Django, please FIRST upgrade to lamindb 0.41.2 before deploying"
                     " this migration and consider reaching out to Lamin\n"
                 )
         else:
             if deploy_migrations:
-                logger.info("Database already up-to-date with migrations!")
+                logger.success("database already up-to-date with migrations!")
         global IS_SETUP
         IS_SETUP = True
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_hub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,25 +307,25 @@
                 "password": password,
                 "options": {"redirect_to": f"{get_lamin_site_base_url()}/signup"},
             }
         )
     except Exception as exception:  # this is bad, but I don't find APIError right now
         logger.error(exception)
         logger.error(
-            "Could not login. Probably your password is wrong or you didn't complete"
+            "could not login. probably your password is wrong or you didn't complete"
             " signup."
         )
         return "could-not-login"
     data = hub.table("account").select("*").eq("id", auth_response.user.id).execute()
     if len(data.data) > 0:  # user is completely registered
         user_id = data.data[0]["lnid"]
         user_handle = data.data[0]["handle"]
         user_name = data.data[0]["name"]
         if handle is not None and handle != user_handle:
             logger.warning(
-                f"Using account handle {user_handle} (cached handle was {handle})"
+                f"using account handle {user_handle} (cached handle was {handle})"
             )
     else:  # user did not complete signup as usermeta has no matching row
-        logger.error("Complete signup on your account page.")
+        logger.error("complete signup on your account page.")
         return "complete-signup"
     hub.auth.sign_out()
     return user_id, user_handle, user_name, auth_response.session.access_token
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_hub_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,26 +68,54 @@
 
 
 def get_storage_region(storage_root: Union[str, Path, UPath]) -> Optional[str]:
     storage_root_str = str(storage_root)
     storage_region = None
 
     if storage_root_str.startswith("s3://"):
-        import botocore.session
+        import botocore.session as session
+        from botocore.config import Config
+        from botocore.exceptions import ClientError, NoCredentialsError
+
+        bucket = storage_root_str.replace("s3://", "")
+
+        s3_session = session.get_session()
+
+        s3_client = s3_session.create_client("s3")
+        try:
+            response = s3_client.head_bucket(Bucket=bucket)
+            exc = None
+        except Exception as e:
+            response = None
+            exc = e
+
+        if isinstance(exc, NoCredentialsError):
+            s3_client = s3_session.create_client(
+                "s3", config=Config(signature_version=session.UNSIGNED)
+            )
+            try:
+                response = s3_client.head_bucket(Bucket=bucket)
+                exc = None
+            except Exception as e:
+                response = None
+                exc = e
+
+        if isinstance(exc, ClientError):
+            response = exc.response
+
+        if response is not None:
+            storage_region = (
+                response["ResponseMetadata"]
+                .get("HTTPHeaders", {})
+                .get("x-amz-bucket-region")
+            )
+            return storage_region
 
-        response = (
-            botocore.session.get_session()
-            .create_client("s3")
-            .get_bucket_location(Bucket=storage_root_str.replace("s3://", ""))
-        )
-        # returns `None` for us-east-1
-        # returns a string like "eu-central-1" etc. for all other regions
-        storage_region = response["LocationConstraint"]
-        if storage_region is None:
-            storage_region = "us-east-1"
+        if exc is not None:
+            raise exc
 
     return storage_region
 
 
 def validate_storage_root_arg(storage_root: str) -> None:
     if storage_root.endswith("/"):
         raise ValueError("Pass settings.storage.root_as_str rather than path")
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_settings_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,29 +96,29 @@
     def _sqlite_file_local(self) -> Path:
         """Local SQLite file."""
         return self.storage.cloud_to_local_no_update(self._sqlite_file)
 
     def _update_cloud_sqlite_file(self) -> None:
         """Upload the local sqlite file to the cloud file."""
         if self._is_cloud_sqlite:
-            logger.warning("Updating & unlocking cloud SQLite")
+            logger.warning("updating & unlocking cloud SQLite")
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.upload_from(cache_file)  # type: ignore
             cloud_mtime = sqlite_file.modified.timestamp()  # type: ignore
             # this seems to work even if there is an open connection
             # to the cache file
             os.utime(cache_file, times=(cloud_mtime, cloud_mtime))
             self._cloud_sqlite_locker.unlock()
 
     def _update_local_sqlite_file(self) -> None:
         """Download the cloud sqlite file if it is newer than local."""
         if self._is_cloud_sqlite:
             logger.warning(
-                "Updating local SQLite & locking cloud SQLite (sync back & unlock:"
+                "updating local SQLite & locking cloud SQLite (sync back & unlock:"
                 " lamin close)"
             )
             sqlite_file = self._sqlite_file
             cache_file = self.storage.cloud_to_local_no_update(sqlite_file)
             sqlite_file.synchronize(cache_file)  # type: ignore
             self._cloud_sqlite_locker.lock()
 
@@ -164,15 +164,19 @@
 
     @property
     def _cloud_sqlite_locker(self):
         # avoid circular import
         from ._cloud_sqlite_locker import empty_locker, get_locker
 
         if self._is_cloud_sqlite:
-            return get_locker(self)
+            try:
+                return get_locker(self)
+            except PermissionError:
+                logger.warning("read-only access - did not access locker")
+                return empty_locker
         else:
             return empty_locker
 
     @property
     def storage(self) -> StorageSettings:
         """Low-level access to storage location."""
         return self._storage
@@ -217,16 +221,16 @@
 
     def _is_db_setup(self, mute: bool = False) -> Tuple[bool, str]:
         """Is the database available and initialized as LaminDB?"""
         if not self._is_db_reachable(mute=mute):
             if self.dialect == "sqlite":
                 return (
                     False,
-                    f"SQLite file {self._sqlite_file} does not exist! It should be in"
-                    f" the storage root: {self.storage.root}",
+                    f"SQLite file {self._sqlite_file} does not exist! It should be"
+                    f" in the storage root: {self.storage.root}",
                 )
             else:
                 return False, f"Connection {self.db} not reachable"
 
         # in order to proceed with the next check, we need the local sqlite
         self._update_local_sqlite_file()
 
@@ -258,10 +262,10 @@
             import sqlalchemy as sa
 
             engine = sa.create_engine(self.db)
             try:
                 engine.connect()
             except Exception:
                 if not mute:
-                    logger.warning(f"Connection {self.db} not reachable")
+                    logger.warning(f"connection {self.db} not reachable")
                 return False
         return True
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_settings_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
     settings_dir = Path.home() / ".lamin"
     settings_dir.mkdir(parents=True, exist_ok=True)
     # deal with legacy settings directory
     legacy_dir = settings_dir.with_name(".lndb")
     if legacy_dir.exists():
         if not settings_dir.exists():
             legacy_dir.rename(settings_dir)
-            logger.info(f"Renamed legacy settings dir {legacy_dir} to {settings_dir}")
+            logger.info(f"renamed legacy settings dir {legacy_dir} to {settings_dir}")
         else:
             for path in legacy_dir.glob("*"):
                 shutil.copy(path, settings_dir)
             logger.info(
-                f"Copied content of legacy settings dir {legacy_dir} to {settings_dir}."
-                f" You can delete {legacy_dir}!"
+                f"copied content of legacy settings dir {legacy_dir} to {settings_dir}."
+                f" you can delete {legacy_dir}!"
             )
     return settings_dir
 
 
 # user_config_dir in appdirs is weird on MacOS!
 # hence, let's take home/.lndb
 settings_dir = get_settings_dir()
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 from appdirs import AppDirs
+from botocore.exceptions import NoCredentialsError
+from lamin_utils import logger
 
 from .upath import UPath
 
 DIRS = AppDirs("lamindb", "laminlabs")
 
 
 class StorageSettings:
@@ -32,14 +34,19 @@
         self._record: Optional[Any] = None
 
     @staticmethod
     def _str_to_path(storage: str) -> Union[Path, UPath]:
         if storage.startswith("s3://"):
             # for new buckets there could be problems if the region is not specified
             storage_root = UPath(storage, cache_regions=True)
+            try:
+                storage_root.stat()
+            except NoCredentialsError:
+                logger.warning("did not find aws credentials, using anonymous")
+                storage_root = UPath(storage_root, anon=True)
         elif storage.startswith("gs://"):
             storage_root = UPath(storage)
         else:  # local path
             os.makedirs(storage, exist_ok=True)  # resolve fails for nonexisting dir
             storage_root = Path(storage).resolve()
         return storage_root
```

### Comparing `lamindb_setup-0.49.5/lamindb_setup/dev/upath.py` & `lamindb_setup-0.49.6/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.49.6/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.6/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/.gitignore` & `lamindb_setup-0.49.6/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.49.6/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.49.6/lnschema-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/LICENSE` & `lamindb_setup-0.49.6/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/migrations/0013_remove_feature_labels_orm_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.49.6/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/lnschema-core/pyproject.toml` & `lamindb_setup-0.49.6/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/noxfile.py` & `lamindb_setup-0.49.6/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 def lint(session: nox.Session) -> None:
     run_pre_commit(session)
 
 
 @nox.session
 @nox.parametrize(
     "group",
-    ["unit", "docs"],
+    ["unit", "docs", "noaws"],
 )
 def install(session: nox.Session, group: str) -> None:
-    session.run(*"pip install git+https://github.com/laminlabs/bionty".split())
-    session.run(
-        *"pip install --no-deps git+https://github.com/laminlabs/lnschema-bionty"
-        .split()
-    )
-    # install lnschema-core from sub-module
-    session.run(*"pip install --no-deps ./lnschema-core".split())
-    # install lamindb-setup without deps
-    session.run(*"pip install .[aws,dev]".split())
+    if group != "noaws":
+        session.run(*"pip install git+https://github.com/laminlabs/bionty".split())
+        session.run(
+            *"pip install --no-deps git+https://github.com/laminlabs/lnschema-bionty"
+            .split()
+        )
+        # install lnschema-core from sub-module
+        session.run(*"pip install --no-deps ./lnschema-core".split())
+        # install lamindb-setup without deps
+        session.run(*"pip install .[aws,dev]".split())
+    else:
+        session.run(*"pip install .[aws,dev]".split())
 
 
 @nox.session
 @nox.parametrize(
     "group",
     ["unit", "docs"],
 )
@@ -39,15 +42,15 @@
 def build(session: nox.Session, group: str, lamin_env: str):
     env = {"LAMIN_ENV": lamin_env}
     login_testuser1(session, env=env)
     login_testuser2(session, env=env)
     coverage_args = "--cov=lamindb_setup --cov-append --cov-report=term-missing"  # noqa
     if group.startswith("unit"):
         session.run(
-            *f"pytest -s {coverage_args} ./tests --ignore tests/hub".split(),
+            *f"pytest -s {coverage_args} ./tests/unit".split(),
             env=env,
         )
     elif group.startswith("docs"):
         session.run(*f"pytest -s {coverage_args} ./docs".split(), env=env)
 
 
 @nox.session
@@ -64,7 +67,16 @@
             env=env,
         )
     login_testuser1(session, env=env)
     session.run(*"lamin init --storage ./docsbuild".split(), env=env)
     if lamin_env != "staging":
         build_docs(session)
         upload_docs_artifact()
+
+
+@nox.session
+def noaws(session: nox.Session):
+    login_testuser1(session)
+    coverage_args = "--cov=lamindb_setup --cov-append --cov-report=term-missing"  # noqa
+    session.run(
+        *f"pytest -s {coverage_args} ./tests/test_load_persistent_instance.py".split()
+    )
```

### Comparing `lamindb_setup-0.49.5/pyproject.toml` & `lamindb_setup-0.49.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/tests/hub/test_instance.py` & `lamindb_setup-0.49.6/tests/hub/test_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/tests/hub/test_storage.py` & `lamindb_setup-0.49.6/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/tests/test_init_instance.py` & `lamindb_setup-0.49.6/tests/unit/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/tests/test_load_instance.py` & `lamindb_setup-0.49.6/tests/unit/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.5/PKG-INFO` & `lamindb_setup-0.49.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.49.5
+Version: 0.49.6
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django<5.0.0
 Requires-Dist: dj_database_url<3.0.0
```

