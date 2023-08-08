# Comparing `tmp/bw_matchbox-1.0.7.tar.gz` & `tmp/bw_matchbox-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-1.0.7.tar", last modified: Tue Aug  8 07:45:25 2023, max compression
+gzip compressed data, was "bw_matchbox-1.0.8.tar", last modified: Tue Aug  8 08:32:18 2023, max compression
```

## Comparing `bw_matchbox-1.0.7.tar` & `bw_matchbox-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.582140 bw_matchbox-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 07:45:25.582140 bw_matchbox-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.570140 bw_matchbox-1.0.7/bw_matchbox/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.570140 bw_matchbox-1.0.7/bw_matchbox/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.570140 bw_matchbox-1.0.7/bw_matchbox/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/common-modal.css
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/common.css
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/fixed-table.css
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/process-detail.css
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.570140 bw_matchbox-1.0.7/bw_matchbox/assets/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessDetail/
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/js/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/common/CommonHelpers.js
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/common/CommonModal.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.570140 bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.574140 bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.578140 bw_matchbox-1.0.7/bw_matchbox/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/common-modal.html
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.578140 bw_matchbox-1.0.7/bw_matchbox/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.578140 bw_matchbox-1.0.7/bw_matchbox/data/
--rw-r--r--   0 runner    (1001) docker     (123)   123246 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 runner    (1001) docker     (123)    93862 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 runner    (1001) docker     (123)   116072 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/data/dare.json
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24887 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/bw_matchbox/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:45:25.578140 bw_matchbox-1.0.7/bw_matchbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 07:45:25.000000 bw_matchbox-1.0.7/bw_matchbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 07:45:13.000000 bw_matchbox-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-08 07:45:25.582140 bw_matchbox-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:18.001817 bw_matchbox-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 08:32:18.001817 bw_matchbox-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.989817 bw_matchbox-1.0.8/bw_matchbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.985817 bw_matchbox-1.0.8/bw_matchbox/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.989817 bw_matchbox-1.0.8/bw_matchbox/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/process-detail.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.989817 bw_matchbox-1.0.8/bw_matchbox/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.985817 bw_matchbox-1.0.8/bw_matchbox/assets/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.989817 bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.989817 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessDetail/
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.993817 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.993817 bw_matchbox-1.0.8/bw_matchbox/assets/js/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.985817 bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.993817 bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.997817 bw_matchbox-1.0.8/bw_matchbox/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.997817 bw_matchbox-1.0.8/bw_matchbox/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:17.997817 bw_matchbox-1.0.8/bw_matchbox/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   123246 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 runner    (1001) docker     (123)    93862 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 runner    (1001) docker     (123)   116072 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/data/dare.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24887 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/bw_matchbox/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:32:18.001817 bw_matchbox-1.0.8/bw_matchbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 08:32:17.000000 bw_matchbox-1.0.8/bw_matchbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-08 08:32:04.000000 bw_matchbox-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-08 08:32:18.005817 bw_matchbox-1.0.8/setup.cfg
```

### Comparing `bw_matchbox-1.0.7/LICENSE` & `bw_matchbox-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/PKG-INFO` & `bw_matchbox-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.7/README.md` & `bw_matchbox-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/common-modal.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/common-modal.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/common.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/compare.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/compare.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/fixed-table.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/fixed-table.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/processes-list.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-1.0.8/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-1.0.8/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareProxyDialogModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessDetail/ProcessDetail.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -39,15 +39,14 @@
                 return new Promise((resolve, _reject) => {
                     const title = 'Waitlist this process';
                     const content = this.getMarkWaitlistDialogContent();
                     let isOpened = true;
                     CommonModal.setModalContentId('mark-waitlist-dialog-modal')
                         .setTitle(title)
                         .setModalWindowOptions({
-                            // fullWindowWidth: true, // UNUSED (Default behavior)
                             autoHeight: true,
                             width: 'md',
                         })
                         .setModalContentOptions({
                             scrollable: true,
                             padded: true,
                         })
@@ -57,40 +56,26 @@
                             if (isOpened) {
                                 isOpened = false;
                                 // Don't proceed the operation!
                                 resolve(false);
                             }
                         })
                         .showModal();
-                    let comment = '';
-                    // let hasComment = false;
-                    const commentEl = document.getElementById('mark-waitlist-comment');
+                    // Store comment value...
                     const okButtonEl = document.getElementById('mark-waitlist-ok');
-                    commentEl.addEventListener('input', (event) => {
-                        const {
-                            target
-                        } = event;
-                        const {
-                            value
-                        } = target;
-                        comment = value;
-                        // const hasValue = !!value;
-                        // if (hasValue !== hasComment) {
-                        //   okButtonEl.classList.toggle('disabled', !hasValue);
-                        //   hasComment = hasValue;
-                        // }
-                    });
                     // TODO: Add handlers for modal actions
                     okButtonEl.addEventListener('click', () => {
                         if (isOpened) {
                             isOpened = false;
                             CommonModal.hideModal({
                                 dontNotify: true
                             });
                             // Success: proceed with comment text
+                            const commentEl = document.getElementById('mark-waitlist-comment');
+                            const comment = commentEl.value;
                             resolve({
                                 comment
                             });
                         }
                     });
                     document
                         .getElementById('mark-waitlist-cancel')
@@ -109,59 +94,41 @@
                 const {
                     sharedData
                 } = this;
                 const {
                     addAttributeUrl
                 } = sharedData;
                 const urlBase = addAttributeUrl;
-                // ?attr=match_type&value=1
+                // Eg: ?attr=match_type&value=1
                 const urlQuery1 = CommonHelpers.makeQuery({
                     attr: 'match_type',
                     value: 1
                 }, {
                     addQuestionSymbol: true
                 }, );
-                // ?attr=waitlist_comment&value=<comment text>
+                // Eg: ?attr=waitlist_comment&value=<comment text>
                 const urlQuery2 = CommonHelpers.makeQuery({
                     attr: 'waitlist_comment',
                     value: comment
                 }, {
                     addQuestionSymbol: true
                 }, );
                 const url1 = urlBase + urlQuery1;
                 const url2 = urlBase + urlQuery2;
-                // DEBUG: For the test time
-                // console.log('[ProcessDetail:doMarkWaitlist] start', {
-                //   comment,
-                //   userAction,
-                //   addAttributeUrl,
-                //   urlBase,
-                //   url1,
-                //   url2,
-                //   urlQuery1,
-                //   urlQuery2,
-                // });
                 // Call both requests at once...
                 const allPromises = [fetch(url1), fetch(url2)];
                 return Promise.all(allPromises).then((resList) => {
                     const errorsList = resList
                         .map((res) => {
                             if (!res.ok) {
                                 return new Error(`HTTP error ${res.status}`);
                             }
                         })
                         .filter(Boolean);
                     const hasErrors = !!errorsList.length;
-                    // DEBUG: For the test time
-                    console.log('[ProcessDetail:doMarkWaitlist] success', {
-                        hasErrors,
-                        resList,
-                        errorsList,
-                    });
-                    debugger;
                     if (!hasErrors) {
                         // All is ok...
                         button.innerText = 'Waitlisted';
                         button.classList.remove('button-primary');
                     } else {
                         // Some errors?
                         // eslint-disable-next-line no-console
```

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,17 @@
                  *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
                  *   unit, // ''
                  *   rowData,
                  * });
                  */
                 const matchUrl = '/match/' + id;
                 const matchButton = matched ?
-                    `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> ${match_type || 'EDIT'}</a>` :
+                    `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> ${
+              match_type || 'EDIT'
+            }</a>` :
                     `<a class="button button-primary" href="${
               matchUrl || ''
             }"><i class="fa-solid fa-circle-xmark"></i> ADD</a>`;
                 const content = `
           <tr>
             <td><div><a href="/process/${id || ''}">${name || ''}</a></div></td>
             <td><div>${location || ''}</div></td>
```

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/common/CommonModal.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/common/CommonModal.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-1.0.8/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/common-modal.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/common-modal.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/compare.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/header.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/header.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/index.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/index.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/match.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/process_detail.html`

 * *Files 8% similar despite different names*

```diff
@@ -23,34 +23,34 @@
         {% if ds.database == source %}
           <button onClick="ProcessDetail.markWaitlist(this)" style="vertical-align: middle" class="button-primary" id="mark-waitlist">Waitlist</button>
           {% if not ds.matched %}<button onClick="ProcessDetail.markMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-match">No match needed</button>
           {% if same_name_count %}<button onClick="ProcessDetail.markAllMatched(this)" style="vertical-align: middle" class="button-primary" id="manual-multi-match">Mark all matched</button>{% endif %}
           <a style="vertical-align: middle" id="match-button" class="button button-primary" href="{{ url_for('match', source=ds.id)}}">Match</a>{% elif ds.match_type == "1" %}<button id="match-button" style="vertical-align: middle">No match needed</button>{% else %}<button id="match-button" style="vertical-align: middle">Matched</button>{% endif %}
         {% endif %}
       </h1>
-      <ul>
-          <li>Database: {{ ds.database }}</li>
-          <li>Location: {{ ds.location }}</li>
-          <li>Unit: {{ ds.unit }}</li>
-          <li>ID: {{ ds.id }}</li>
-          <li>Production amount: {{ ds['production amount'] }}</li>
-          <li>Reference product: {{ ds['reference product'] }}</li>
-          <li>Authors: {{ authors }}</li>
-          <li>Comment: {{ds.comment }}</li>
+      <ul class="details-list">
+          <li><label>Database:</label> {{ ds.database }}</li>
+          <li><label>Location:</label> {{ ds.location }}</li>
+          <li><label>Unit:</label> {{ ds.unit }}</li>
+          <li><label>ID:</label> {{ ds.id }}</li>
+          <li><label>Production amount:</label> {{ ds['production amount'] }}</li>
+          <li><label>Reference product:</label> {{ ds['reference product'] }}</li>
+          <li><label>Authors:</label> {{ authors }}</li>
+          <li><label>Comment:</label> {{ds.comment }}</li>
           {% if same_name_count %}
-              <li>Datasets with same name: {{ same_name_count }}: {% for obj in same_name %}<a href="{{ url_for('process_detail', id=obj.id) }}">{% if obj.data.matched %}<i class="fa-solid fa-check"></i> {% endif %}{{obj.location}}</a> {% endfor %}</li>
+              <li><label>Datasets with same name:</label> {{ same_name_count }}: {% for obj in same_name %}<a href="{{ url_for('process_detail', id=obj.id) }}">{% if obj.data.matched %}<i class="fa-solid fa-check"></i> {% endif %}{{obj.location}}</a> {% endfor %}</li>
           {% endif %}
           {% if proxy_node %}
-              <li>Proxy: <a href="{{ url_for('process_detail', id=proxy_node.id) }}">{{ proxy_node }}</a></li>
+              <li><label>Proxy:</label> <a href="{{ url_for('process_detail', id=proxy_node.id) }}">{{ proxy_node }}</a></li>
           {% endif %}
           {% if reference_node %}
-              <li>Proxy for: <a href="{{ url_for('process_detail', id=reference_node.id) }}">{{ reference_node }}</a></li>
+              <li><label>Proxy for:</label> <a href="{{ url_for('process_detail', id=reference_node.id) }}">{{ reference_node }}</a></li>
           {% endif %}
           {% if match_type %}
-              <li>Match type: {{ match_type }}</li>
+              <li><label>Match type:</label> {{ match_type }}</li>
           {% endif %}
 
       </ul>
       <h2>Technosphere Inputs</h2>
       <table width="100%">
         <tr>
           <th>Amount</th>
```

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/project.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/search.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-1.0.8/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/bin/matchbox.py` & `bw_matchbox-1.0.8/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-1.0.8/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/data/dare.json` & `bw_matchbox-1.0.8/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/utils.py` & `bw_matchbox-1.0.8/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox/webapp.py` & `bw_matchbox-1.0.8/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-1.0.8/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 1.0.7
+Version: 1.0.8
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-1.0.7/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-1.0.8/bw_matchbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_matchbox-1.0.7/setup.cfg` & `bw_matchbox-1.0.8/setup.cfg`

 * *Files identical despite different names*

