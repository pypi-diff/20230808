# Comparing `tmp/oarepo-vocabularies-2.0.7.tar.gz` & `tmp/oarepo-vocabularies-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-2.0.7.tar", last modified: Tue Jul  4 10:48:43 2023, max compression
+gzip compressed data, was "oarepo-vocabularies-2.0.8.tar", last modified: Fri Jul  7 08:08:19 2023, max compression
```

## Comparing `oarepo-vocabularies-2.0.7.tar` & `oarepo-vocabularies-2.0.8.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.999164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ext_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.999164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.999164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.999164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/templates/oarepo_ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/templates/oarepo_ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.003164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.007164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.overrides
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.variables
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.995164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileLanguages.sh
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 10:48:42.999164 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 10:48:42.000000 oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-04 10:48:43.011164 oarepo-vocabularies-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 10:44:58.000000 oarepo-vocabularies-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/templates/oarepo_ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/templates/oarepo_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.879567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-07 08:04:31.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.871567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.overrides
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/theme/elements/sample.variables
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.883567 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileLanguages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:08:19.875567 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-07 08:08:19.000000 oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-07 08:08:19.887567 oarepo-vocabularies-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 08:04:32.000000 oarepo-vocabularies-2.0.8/setup.py
```

### Comparing `oarepo-vocabularies-2.0.7/LICENSE` & `oarepo-vocabularies-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/MANIFEST.in` & `oarepo-vocabularies-2.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/PKG-INFO` & `oarepo-vocabularies-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.7
+Version: 2.0.8
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-2.0.7/README.md` & `oarepo-vocabularies-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/config.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ext.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,17 @@
                 app.config.setdefault(k, getattr(config, k))
         app.config.setdefault(
             "VOCABULARIES_FACET_CACHE_SIZE", config.VOCABULARIES_FACET_CACHE_SIZE
         )
         app.config.setdefault(
             "VOCABULARIES_FACET_CACHE_TTL", config.VOCABULARIES_FACET_CACHE_TTL
         )
+        app.config.setdefault(
+            "INVENIO_VOCABULARY_TYPE_METADATA", config.INVENIO_VOCABULARY_TYPE_METADATA
+        )
 
         if "OAREPO_PERMISSIONS_PRESETS" not in app.config:
             app.config["OAREPO_PERMISSIONS_PRESETS"] = {}
 
         for k in ext_config.OAREPO_VOCABULARIES_PERMISSIONS_PRESETS:
             if k not in app.config["OAREPO_PERMISSIONS_PRESETS"]:
                 app.config["OAREPO_PERMISSIONS_PRESETS"][
```

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/fixtures.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/models/ui.json` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/api.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/config.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/resources/records/ui.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/config.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/facets.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/schema.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/search.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/service.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/services/ui_schema.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/services/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/templates/oarepo_ui/components/000-vocabularies.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/translations/messages.pot` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/ext.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/components.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/config.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/resources/resource.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/main.html`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/sidebar.html`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/package.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/translations.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies/ui/theme/webpack.py` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.7
+Version: 2.0.8
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 Provides-Extra: devs
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo vocabularies
```

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo-vocabularies-2.0.8/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.7/setup.cfg` & `oarepo-vocabularies-2.0.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.7
+version = 2.0.8
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

