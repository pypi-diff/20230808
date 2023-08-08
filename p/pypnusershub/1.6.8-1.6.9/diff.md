# Comparing `tmp/pypnusershub-1.6.8.tar.gz` & `tmp/pypnusershub-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypnusershub-1.6.8.tar", last modified: Mon Jun 26 14:39:58 2023, max compression
+gzip compressed data, was "pypnusershub-1.6.9.tar", last modified: Tue Aug  8 13:02:18 2023, max compression
```

## Comparing `pypnusershub-1.6.8.tar` & `pypnusershub-1.6.9.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/requirements-common.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/requirements-dependencies.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:39:58.839547 pypnusershub-1.6.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.827547 pypnusershub-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.831548 pypnusershub-1.6.8/src/pypnusershub/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/db/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/fixtures.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/models_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/db/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs-samples.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11397 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/routes_register.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.835548 pypnusershub-1.6.8/src/pypnusershub/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/test_utilisateurs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-26 14:39:44.000000 pypnusershub-1.6.8/src/pypnusershub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:39:58.831548 pypnusershub-1.6.8/src/pypnusershub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 14:39:58.000000 pypnusershub-1.6.8/src/pypnusershub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.213372 pypnusershub-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-08 13:02:18.213372 pypnusershub-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/requirements-common.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/requirements-dependencies.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:02:18.213372 pypnusershub-1.6.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1754 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.205372 pypnusershub-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.209372 pypnusershub-1.6.9/src/pypnusershub/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.209372 pypnusershub-1.6.9/src/pypnusershub/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/db/fixtures.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/db/models_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/db/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.209372 pypnusershub-1.6.9/src/pypnusershub/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.209372 pypnusershub-1.6.9/src/pypnusershub/migrations/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/data/utilisateurs-samples.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/data/utilisateurs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.213372 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11397 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/routes_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.213372 pypnusershub-1.6.9/src/pypnusershub/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/test_utilisateurs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-08-08 13:02:08.000000 pypnusershub-1.6.9/src/pypnusershub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:02:18.209372 pypnusershub-1.6.9/src/pypnusershub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-08 13:02:18.000000 pypnusershub-1.6.9/src/pypnusershub.egg-info/top_level.txt
```

### Comparing `pypnusershub-1.6.8/LICENSE` & `pypnusershub-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/PKG-INFO` & `pypnusershub-1.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.8/README.md` & `pypnusershub-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/setup.py` & `pypnusershub-1.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/__main__.py` & `pypnusershub-1.6.9/src/pypnusershub/__main__.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/db/fixtures.sql` & `pypnusershub-1.6.9/src/pypnusershub/db/fixtures.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/db/models.py` & `pypnusershub-1.6.9/src/pypnusershub/db/models.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/db/models_register.py` & `pypnusershub-1.6.9/src/pypnusershub/db/models_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/db/tools.py` & `pypnusershub-1.6.9/src/pypnusershub/db/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                     engine.execute(line)
             engine.execute("COMMIT")
 
 def encode_token(payload):
     expire = datetime.now() + timedelta(seconds=current_app.config['COOKIE_EXPIRATION'])
     header = {
         "alg": "HS256",
-        "exp": str(int(datetime.timestamp(expire))),
+        "exp": int(datetime.timestamp(expire)),
     }
     jwt = JsonWebToken(["HS256"])
     key = current_app.config['SECRET_KEY'].encode("UTF-8")
     return jwt.encode(header, payload, key)
 
 
 def decode_token(payload):
```

### Comparing `pypnusershub-1.6.8/src/pypnusershub/env.py` & `pypnusershub-1.6.9/src/pypnusershub/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs-samples.sql` & `pypnusershub-1.6.9/src/pypnusershub/migrations/data/utilisateurs-samples.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/data/utilisateurs.sql` & `pypnusershub-1.6.9/src/pypnusershub/migrations/data/utilisateurs.sql`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/env.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/env.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py` & `pypnusershub-1.6.9/src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/routes.py` & `pypnusershub-1.6.9/src/pypnusershub/routes.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/routes_register.py` & `pypnusershub-1.6.9/src/pypnusershub/routes_register.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/schemas.py` & `pypnusershub-1.6.9/src/pypnusershub/schemas.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/tests/conftest.py` & `pypnusershub-1.6.9/src/pypnusershub/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/tests/fixtures.py` & `pypnusershub-1.6.9/src/pypnusershub/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/tests/test_utilisateurs.py` & `pypnusershub-1.6.9/src/pypnusershub/tests/test_utilisateurs.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/tests/test_utils.py` & `pypnusershub-1.6.9/src/pypnusershub/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/tests/utils.py` & `pypnusershub-1.6.9/src/pypnusershub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub/utils.py` & `pypnusershub-1.6.9/src/pypnusershub/utils.py`

 * *Files identical despite different names*

### Comparing `pypnusershub-1.6.8/src/pypnusershub.egg-info/PKG-INFO` & `pypnusershub-1.6.9/src/pypnusershub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypnusershub
-Version: 1.6.8
+Version: 1.6.9
 Summary: Python lib to authenticate using PN's UsersHub
 Home-page: https://github.com/PnX-SI/UsersHub-authentification-module
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `pypnusershub-1.6.8/src/pypnusershub.egg-info/SOURCES.txt` & `pypnusershub-1.6.9/src/pypnusershub.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/pypnusershub/migrations/versions/10e87bc144cd_get_id_role_by_name.py
 src/pypnusershub/migrations/versions/112ccf1024ce_add_unique_constraint_on_t_roles_uuid.py
 src/pypnusershub/migrations/versions/5b334b77f5f5_fix_v_roleslist_forall_applications.py
 src/pypnusershub/migrations/versions/72f227e37bdf_utilisateurs_sample_data.py
 src/pypnusershub/migrations/versions/830cc8f4daef_add_additional_data_field_to_organism.py
 src/pypnusershub/migrations/versions/951b8270a1cf_add_unique_constraint_on_uuid_organisme.py
 src/pypnusershub/migrations/versions/__init__.py
+src/pypnusershub/migrations/versions/f4bf21ac6238_fix_temp_user_organism_size.py
 src/pypnusershub/migrations/versions/fa35dfe5ff27_create_utilisateurs_schema.py
 src/pypnusershub/tests/__init__.py
 src/pypnusershub/tests/conftest.py
 src/pypnusershub/tests/fixtures.py
 src/pypnusershub/tests/test_utilisateurs.py
 src/pypnusershub/tests/test_utils.py
 src/pypnusershub/tests/utils.py
```

