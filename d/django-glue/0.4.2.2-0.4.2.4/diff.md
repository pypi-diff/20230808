# Comparing `tmp/django-glue-0.4.2.2.tar.gz` & `tmp/django-glue-0.4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.4.2.2.tar", last modified: Fri Aug  4 18:23:43 2023, max compression
+gzip compressed data, was "django-glue-0.4.2.4.tar", last modified: Tue Aug  8 18:15:54 2023, max compression
```

## Comparing `django-glue-0.4.2.2.tar` & `django-glue-0.4.2.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.976311 django-glue-0.4.2.4/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.976311 django-glue-0.4.2.4/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.976311 django-glue-0.4.2.4/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-08 18:15:54.000000 django-glue-0.4.2.4/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:54.980311 django-glue-0.4.2.4/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-08 18:15:44.000000 django-glue-0.4.2.4/tests/wsgi.py
```

### Comparing `django-glue-0.4.2.2/CHANGELOG.md` & `django-glue-0.4.2.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # Changelog for Django Glue
 
+## 0.4.2.4
+
+### Changes
+- Versions fix. 
+
+
+## 0.4.2.3
+
+### Changes
+- Improve field logic for many-to-many and one-to-one relationships. 
+
 ## 0.4.2.2
 
 ### Changes
 - Foreign Key fields now work with glue.
 - Move validation logic from Glue Request Handler to View.  
 
-
-
 ## 0.4.2.1
 
 ### Changes
 - Model default values now work with glue.
 
 ## 0.4.2
```

### Comparing `django-glue-0.4.2.2/LICENSE.md` & `django-glue-0.4.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/PKG-INFO` & `django-glue-0.4.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2.2
+Version: 0.4.2.4
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2.2/README.md` & `django-glue-0.4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/context_processors.py` & `django-glue-0.4.2.4/django_glue/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/core/decorators.py` & `django-glue-0.4.2.4/django_glue/core/decorators.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/data_classes.py` & `django-glue-0.4.2.4/django_glue/data_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,26 +40,32 @@
 
     def to_dict(self) -> dict:
         return asdict(self)
 
 
 @dataclass
 class GlueJsonData:
+    """
+        Used to provide a consistent structure for our glue objects.
+    """
     fields: Optional[dict] = None
     simple_fields: Optional[dict] = None
     method_return: Optional[Any] = None
     custom: Optional[dict] = None
 
     def to_dict(self):
         remove_none_value_field_from_data_class_object(self)
         return asdict(self)
 
 
 @dataclass
 class GlueJsonResponseData:
+    """
+        Consistent structure for our json responses.
+    """
     message_title: Optional[str] = None
     message_body: Optional[str] = None
     data: Optional[GlueJsonData] = None
     optional_message_data: Optional[dict] = None
     response_type: GlueJsonResponseType = GlueJsonResponseType.SUCCESS
     response_status: GlueJsonResponseStatus = GlueJsonResponseStatus.SUCCESS
```

### Comparing `django-glue-0.4.2.2/django_glue/enums.py` & `django-glue-0.4.2.4/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/glue.py` & `django-glue-0.4.2.4/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/handlers.py` & `django-glue-0.4.2.4/django_glue/handlers.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/middleware.py` & `django-glue-0.4.2.4/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/responses.py` & `django-glue-0.4.2.4/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/services/model_objects.py` & `django-glue-0.4.2.4/django_glue/services/model_objects.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/services/query_sets.py` & `django-glue-0.4.2.4/django_glue/services/query_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django_glue.utils import decode_query_set_from_str, generate_simple_field_dict, get_field_names_from_model, \
     check_valid_method_kwargs, type_set_method_kwargs, field_name_included
 
 
 class GlueQuerySetService(Service):
     def __init__(self, meta_data: GlueMetaData) -> None:
         self.meta_data = meta_data
+        # Query set is optional for lazy loading. Call load_query_set() before using it.
         self.query_set: Optional[QuerySet] = None
 
     def load_query_set(self):
         self.query_set = decode_query_set_from_str(self.meta_data.query_set_str)
 
     def process_get_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
         self.load_query_set()
```

### Comparing `django-glue-0.4.2.2/django_glue/services/services.py` & `django-glue-0.4.2.4/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/services/templates.py` & `django-glue-0.4.2.4/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/sessions.py` & `django-glue-0.4.2.4/django_glue/sessions.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_ajax.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,14 @@
 class GlueModelObject {
     constructor(glue_unique_name) {
         // Needs to be named glue_unique_name to avoid overriding the unique_name property
         this.glue_unique_name = glue_unique_name
 
         for (let key in window.glue_session_data['context'][glue_unique_name].fields) {
             this[key] = window.glue_session_data['context'][glue_unique_name].fields[key].value
-            console.log(key, this[key])
         }
 
         window.glue_keep_live.add_unique_name(glue_unique_name)
     }
 
     async create() {
         return await glue_ajax_request(
```

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_query_set.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_template.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_view.js` & `django-glue-0.4.2.4/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/templates/django_glue/django_glue.html` & `django-glue-0.4.2.4/django_glue/templates/django_glue/django_glue.html`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/templatetags/django_glue.py` & `django-glue-0.4.2.4/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue/utils.py` & `django-glue-0.4.2.4/django_glue/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                         field_value = json_model['pk']
                         field_attr = ''
                     else:
                         field_value = json_model['fields'][field.name]
                         field_attr = generate_field_attr_dict(field)
 
                     # Todo: Field name logic is duplicated
-                    if field.attname == 'foreign_key_id':
+                    if field.many_to_one or field.one_to_one:
                         field_name = field.name + '_id'
                     else:
                         field_name = field.name
 
                     fields_dict[field_name] = GlueModelFieldData(
                         type=field.get_internal_type(),
                         value=field_value,
@@ -95,15 +95,15 @@
 
 
 # Todo: Field name logic is duplicated
 def get_field_names_from_model(model) -> list:
     field_names = []
 
     for field in model._meta.fields:
-        if field.attname == 'foreign_key_id':
+        if field.many_to_one or field.one_to_one:
             field_names.append(field.name + '_id')
         else:
             field_names.append(field.name)
 
     return field_names
```

### Comparing `django-glue-0.4.2.2/django_glue/views.py` & `django-glue-0.4.2.4/django_glue/views.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.2.4/django_glue.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2.2
+Version: 0.4.2.4
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2.2/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.2.4/django_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/setup.py` & `django-glue-0.4.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/manage.py` & `django-glue-0.4.2.4/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/migrations/0001_initial.py` & `django-glue-0.4.2.4/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py` & `django-glue-0.4.2.4/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/models.py` & `django-glue-0.4.2.4/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/settings.py` & `django-glue-0.4.2.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/urls.py` & `django-glue-0.4.2.4/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/utils.py` & `django-glue-0.4.2.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.2/tests/views.py` & `django-glue-0.4.2.4/tests/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from tests.utils import generate_randomized_test_model, generate_big_test_model
 from django_glue.glue import add_glue
 
 
 def big_model_object_view(request):
     big_model = BigTestModel.objects.first()
     add_glue(request, 'big_model', big_model, 'delete', fields=('foreign_key',))
+    add_glue(request, 'big_model_query', BigTestModel.objects.all(), 'delete', fields=('foreign_key',))
+
     return TemplateResponse(request, template='page/big_model_object_page.html')
 
 
 class ModelObjectView(TemplateView):
     template_name = 'page/model_object_page.html'
 
     def get_context_data(self, **kwargs):
```

