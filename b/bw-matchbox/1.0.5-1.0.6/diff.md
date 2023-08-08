# Comparing `tmp/bw_matchbox-1.0.5.tar.gz` & `tmp/bw_matchbox-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-1.0.5.tar", last modified: Mon Aug  7 22:08:11 2023, max compression
+gzip compressed data, was "bw_matchbox-1.0.6.tar", last modified: Tue Aug  8 05:32:05 2023, max compression
```

## Comparing `bw_matchbox-1.0.5.tar` & `bw_matchbox-1.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.912459 bw_matchbox-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-07 22:08:11.912459 bw_matchbox-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.900459 bw_matchbox-1.0.5/bw_matchbox/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.900459 bw_matchbox-1.0.5/bw_matchbox/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/process-detail.css
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.900459 bw_matchbox-1.0.5/bw_matchbox/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessDetail/
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/js/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.900459 bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.904459 bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.908459 bw_matchbox-1.0.5/bw_matchbox/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.908459 bw_matchbox-1.0.5/bw_matchbox/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.908459 bw_matchbox-1.0.5/bw_matchbox/data/
--rw-r--r--   0 runner    (1001) docker     (123)   123246 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 runner    (1001) docker     (123)    93862 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 runner    (1001) docker     (123)   116072 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/data/dare.json
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24754 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/bw_matchbox/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 22:08:11.908459 bw_matchbox-1.0.5/bw_matchbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-07 22:08:11.000000 bw_matchbox-1.0.5/bw_matchbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-07 22:08:02.000000 bw_matchbox-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-07 22:08:11.912459 bw_matchbox-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.235072 bw_matchbox-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 05:32:05.235072 bw_matchbox-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.223071 bw_matchbox-1.0.6/bw_matchbox/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/process-detail.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.223071 bw_matchbox-1.0.6/bw_matchbox/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessDetail/
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.227072 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.231072 bw_matchbox-1.0.6/bw_matchbox/assets/js/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.223071 bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.231072 bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.231072 bw_matchbox-1.0.6/bw_matchbox/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.231072 bw_matchbox-1.0.6/bw_matchbox/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.231072 bw_matchbox-1.0.6/bw_matchbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   123246 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93862 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116072 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/data/dare.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24828 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/bw_matchbox/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 05:32:05.235072 bw_matchbox-1.0.6/bw_matchbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 05:32:05.000000 bw_matchbox-1.0.6/bw_matchbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 05:31:56.000000 bw_matchbox-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-08 05:32:05.235072 bw_matchbox-1.0.6/setup.cfg
```

### Comparing `bw_matchbox-1.0.5/LICENSE` & `bw_matchbox-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/PKG-INFO` & `bw_matchbox-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.5/README.md` & `bw_matchbox-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/common.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/compare.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-1.0.6/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-1.0.6/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-1.0.6/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/header.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/index.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/match.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/project.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/search.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-1.0.6/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/bin/matchbox.py` & `bw_matchbox-1.0.6/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-1.0.6/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/data/dare.json` & `bw_matchbox-1.0.6/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/bw_matchbox/utils.py` & `bw_matchbox-1.0.6/bw_matchbox/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     "2": "Direct match with near-identical data",
     "3": "Match with updated data",
     "4": "Match with updated data and adding source transport",
     "5": "Match with market and replace or remove transport",
     "6": "Match with market and replace or remove transport and loss factor",
     "7": "Equivalent datasets after modification",
     "8": "Replace aggregated with unit process",
+    "9": "Rescaled direct correspondence",
 }
 
 
 def get_match_types(output_dir: Path) -> dict:
     match_types_file = output_dir / "match_types.json"
     try:
         return json.load(open(match_types_file))
```

### Comparing `bw_matchbox-1.0.5/bw_matchbox/webapp.py` & `bw_matchbox-1.0.6/bw_matchbox/webapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,45 +372,42 @@
     "Direct match with near-identical data": "Near-identical data",
     "Match with updated data": "Updated data",
     "Match with updated data and adding source transport": "Updated data w/ src trans",
     "Match with market and replace or remove transport": "Market w/ diff trans",
     mwmarortalf: "Market w/ diff trans loss",
     "Equivalent datasets after modification": "Modifications",
     "Replace aggregated with unit process": "Replace aggregated",
+    "Rescaled direct correspondence": "Rescaled",
     "Unknown": "Unknown",
 }
 
 
 def get_match_type_for_source_process(node):
     if hasattr(node, "data"):
         if "match_type" in node.data:
-            return MATCH_TYPE_ABBREVIATIONS[
-                matchbox_app.config["mb_match_types"].get(
-                    node.data["match_type"], "Unknown"
-                )
-            ]
+            label = matchbox_app.config["mb_match_types"].get(
+                node.data["match_type"], "Unknown"
+            )
+            return MATCH_TYPE_ABBREVIATIONS.get(label, label)
         elif node.data.get("proxy_id"):
             mt = bd.get_node(id=node.data["proxy_id"]).get("match_type")
-            return MATCH_TYPE_ABBREVIATIONS[
-                matchbox_app.config["mb_match_types"].get(mt, "Unknown")
-            ]
+            label = matchbox_app.config["mb_match_types"].get(mt, "Unknown")
+            return MATCH_TYPE_ABBREVIATIONS.get(label, label)
         else:
             return "Unknown"
     elif "match_type" in node:
-        return MATCH_TYPE_ABBREVIATIONS[
-            matchbox_app.config["mb_match_types"].get(node["match_type"], "Unknown")
-        ]
+        label = matchbox_app.config["mb_match_types"].get(node["match_type"], "Unknown")
+        return MATCH_TYPE_ABBREVIATIONS.get(label, label)
     else:
         mt = bd.get_node(id=node["proxy_id"]).get("match_type")
         if not mt or mt == "0":
             return "Unknown"
         else:
-            return MATCH_TYPE_ABBREVIATIONS[
-                matchbox_app.config["mb_match_types"].get(mt, "Unknown")
-            ]
+            label = matchbox_app.config["mb_match_types"].get(mt, "Unknown")
+            return MATCH_TYPE_ABBREVIATIONS.get(label, label)
 
 
 # @matchbox_app.route("/match-status", methods=["GET"])
 # @auth.login_required
 # def match_status():
 #     crud = {}
 #     status = {}
```

### Comparing `bw_matchbox-1.0.5/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-1.0.6/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.5/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-1.0.6/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.5/setup.cfg` & `bw_matchbox-1.0.6/setup.cfg`

 * *Files identical despite different names*

